# Comparing `tmp/pstk-0.0.1.tar.gz` & `tmp/pstk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pstk-0.0.1.tar", max compression
+gzip compressed data, was "pstk-0.0.2.tar", max compression
```

## Comparing `pstk-0.0.1.tar` & `pstk-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1466 2024-04-17 16:10:51.138101 pstk-0.0.1/LICENSE
--rw-r--r--   0        0        0      481 2024-04-17 16:10:51.138101 pstk-0.0.1/README.md
--rw-r--r--   0        0        0       30 2024-04-17 16:10:51.138101 pstk-0.0.1/pstk/__init__.py
--rw-r--r--   0        0        0     3616 2024-04-17 16:10:51.138101 pstk-0.0.1/pstk/main_cli.py
--rw-r--r--   0        0        0      393 2024-04-17 16:10:51.138101 pstk-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1068 1970-01-01 00:00:00.000000 pstk-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1466 2024-05-07 02:08:46.991077 pstk-0.0.2/LICENSE
+-rw-r--r--   0        0        0      481 2024-05-07 02:08:46.991077 pstk-0.0.2/README.md
+-rw-r--r--   0        0        0       30 2024-05-07 02:08:46.991077 pstk-0.0.2/pstk/__init__.py
+-rw-r--r--   0        0        0     4247 2024-05-07 02:08:46.991077 pstk-0.0.2/pstk/main_cli.py
+-rw-r--r--   0        0        0      393 2024-05-07 02:08:46.991077 pstk-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1068 1970-01-01 00:00:00.000000 pstk-0.0.2/PKG-INFO
```

### Comparing `pstk-0.0.1/LICENSE` & `pstk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pstk-0.0.1/pstk/main_cli.py` & `pstk-0.0.2/pstk/main_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,26 @@
 import argparse
 import psycopg2
 from pathlib import Path
 import re
 from dotenv import load_dotenv
 import os
+import subprocess
 import shutil
 
+def exec_sudo(*args):
+    val = subprocess.run(
+        ('sudo', *args),
+        # check=True,
+        capture_output=True,
+    )
+    # print(f'`{" ".join(args)}`: {val}')
+    if val.returncode != 0:
+        raise Exception(val)
+
 def main(
     root: Path,
     mode: str, # test | install
     host: str,
     port: int,
     replace: bool,
     extension: bool,
@@ -20,20 +31,19 @@
     **conn_args,
 ):
     load_dotenv(root / '.env')
     for key in {'dbname', 'user', 'password',}:
         if (value := os.getenv(f'POSTGRES_{key.upper()}')):
             conn_args[key] = value
 
+    conn_args['host'] = host
+    conn_args['port'] = port
+
     print(conn_args)
-    conn = psycopg2.connect(
-        host=host,
-        port=port,
-        **conn_args,
-    )
+    conn = psycopg2.connect(**conn_args)
 
     schema = root / schema_path
 
     if not schema.exists():
         raise FileNotFoundError(schema)
     
     schema_name_match = re.search(r'^create schema (\w+);', schema.read_text())
@@ -43,16 +53,26 @@
     schema_name = schema_name_match.group(1)
 
     tmp_path = Path('/tmp')
     files_path = root / 'files'
     if files_path.exists():
         for file_path in files_path.iterdir():
             tmp_file_path = tmp_path / file_path.name
+            # print(f'Copy {file_path} to {tmp_file_path}')
             shutil.copy(file_path, tmp_file_path)
-            tmp_file_path.chmod(700)
+            exec_sudo('chmod', '700', str(tmp_file_path))
+            exec_sudo('chown', 'postgres:postgres', str(tmp_file_path))
+            # tmp_file_path.chmod(700)
+
+    # os.system('ls -l /tmp')
+
+    if extension:
+        os.chdir(root)
+        print(f'Building extension {schema_name}.')
+        exec_sudo('make')
 
     with conn.cursor() as cur:
         if extension:
             print(f'Checking if extension {schema_name} exists.')
             cur.execute(
                 'SELECT EXISTS (SELECT 1 FROM pg_extension WHERE extname = %s)',
                 (schema_name,)
@@ -61,15 +81,15 @@
                 if replace:
                     print(f'Dropping extension {schema_name}.')
                     cur.execute(f'drop extension {schema_name} cascade')
                 else:
                     raise Exception(f'Extension {schema_name} already exists. Run with --replace to replace.')
 
             print(f'Installing binaries from extension {schema_name}.')
-            os.system('sudo make install')
+            exec_sudo('make', 'install')
 
             print(f'Creating extension {schema_name}.')
             cur.execute(f'create extension {schema_name}')
         else:
             print(f'Checking if schema {schema_name} exists.')
             cur.execute(
                 'SELECT EXISTS (SELECT 1 FROM information_schema.schemata WHERE schema_name = %s)',
@@ -99,12 +119,13 @@
     parser.add_argument('root', type=Path)
     parser.add_argument('mode', type=str)
     parser.add_argument('--dbname', default='postgres')
     parser.add_argument('--user', default='postgres')
     parser.add_argument('--password', default='postgres')
     parser.add_argument('--host', default='localhost')
     parser.add_argument('--port', type=int, default=5432)
+    parser.add_argument('--socket')
     parser.add_argument('--replace', action='store_true')
     parser.add_argument('--extension', action='store_true')
     parser.add_argument('--schema-path', default='schema.sql')
 
     main(**vars(parser.parse_args()))
```

### Comparing `pstk-0.0.1/PKG-INFO` & `pstk-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pstk
-Version: 0.0.1
+Version: 0.0.2
 Summary: A toolkit for developing Postgres schemas & extensions.
 Author: albaike
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

