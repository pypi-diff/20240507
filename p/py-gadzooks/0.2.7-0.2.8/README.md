# Comparing `tmp/py_gadzooks-0.2.7.tar.gz` & `tmp/py_gadzooks-0.2.8.tar.gz`

## Comparing `py_gadzooks-0.2.7.tar` & `py_gadzooks-0.2.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 py_gadzooks-0.2.7/gadzooks/__init__.py
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 py_gadzooks-0.2.7/gadzooks/build_docs.py
--rw-r--r--   0        0        0     7882 2020-02-02 00:00:00.000000 py_gadzooks-0.2.7/gadzooks/check_version.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 py_gadzooks-0.2.7/gadzooks/loc_summarize.py
--rwxr-xr-x   0        0        0     1385 2020-02-02 00:00:00.000000 py_gadzooks-0.2.7/gadzooks/main.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 py_gadzooks-0.2.7/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 py_gadzooks-0.2.7/LICENSE
--rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 py_gadzooks-0.2.7/README.md
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 py_gadzooks-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 py_gadzooks-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 py_gadzooks-0.2.8/gadzooks/__init__.py
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 py_gadzooks-0.2.8/gadzooks/build_docs.py
+-rw-r--r--   0        0        0     7882 2020-02-02 00:00:00.000000 py_gadzooks-0.2.8/gadzooks/check_version.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 py_gadzooks-0.2.8/gadzooks/loc_summarize.py
+-rwxr-xr-x   0        0        0     1385 2020-02-02 00:00:00.000000 py_gadzooks-0.2.8/gadzooks/main.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 py_gadzooks-0.2.8/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 py_gadzooks-0.2.8/LICENSE
+-rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 py_gadzooks-0.2.8/README.md
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 py_gadzooks-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 py_gadzooks-0.2.8/PKG-INFO
```

### Comparing `py_gadzooks-0.2.7/gadzooks/__init__.py` & `py_gadzooks-0.2.8/gadzooks/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from argparse import ArgumentParser, Namespace
 import sys
 from typing import ClassVar, Optional
 
 
-__version__ = '0.2.7'
+__version__ = '0.2.8'
 
 
 def error(msg: str) -> None:
     """Prints an error message and exits the program with return code 1."""
     print(f'ERROR: {msg}', file=sys.stderr)
     sys.exit(1)
 
 def warning(msg: str) -> None:
     """Prints a warning message."""
-    print(f'WARNING: {msg}', file=sys.stderr)
+    print(f'\033[1;33mWARNING: {msg}\x1b[0m', file=sys.stderr)
 
 
 class Subcommand:
     """Configures a subcommand for the main executable."""
 
     @classmethod
     def configure_parser(cls, parser: ArgumentParser) -> None:
```

### Comparing `py_gadzooks-0.2.7/gadzooks/build_docs.py` & `py_gadzooks-0.2.8/gadzooks/build_docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import binascii
 from collections.abc import Sequence
 import hashlib
 from pathlib import Path
 import subprocess
 from typing import Optional
 
-from gadzooks import Subcommand, error
+from gadzooks import Subcommand, error, warning
 
 
 def xor_bytes(hashes: list[bytes]) -> bytes:
     """Computes the XOR of a collection of byte strings of the same length."""
     assert len(hashes) > 0
     arr = [0 for _ in hashes[0]]
     for h in hashes:
@@ -65,16 +65,16 @@
                 prev_checksum = f.read().strip()
             if checksum == prev_checksum:
                 print(f'checksum matches {args.checksum_file} -- source docs are unchanged')
                 return
             msg = 'source docs have changed'
         else:
             msg = 'no checksum file found'
-        if args.check_only:
-            print(f'\033[1;33mWARNING: {msg}')
+        if msg and args.check_only:
+            warning(msg)
             return
         print(msg)
         msg = 'rebuilding docs...'
         if args.force:
             msg = 'force ' + msg
         print(msg)
         print(' '.join(extra_args))
```

### Comparing `py_gadzooks-0.2.7/gadzooks/check_version.py` & `py_gadzooks-0.2.8/gadzooks/check_version.py`

 * *Files identical despite different names*

### Comparing `py_gadzooks-0.2.7/gadzooks/loc_summarize.py` & `py_gadzooks-0.2.8/gadzooks/loc_summarize.py`

 * *Files identical despite different names*

### Comparing `py_gadzooks-0.2.7/gadzooks/main.py` & `py_gadzooks-0.2.8/gadzooks/main.py`

 * *Files identical despite different names*

### Comparing `py_gadzooks-0.2.7/LICENSE` & `py_gadzooks-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `py_gadzooks-0.2.7/README.md` & `py_gadzooks-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `py_gadzooks-0.2.7/pyproject.toml` & `py_gadzooks-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_gadzooks-0.2.7/PKG-INFO` & `py_gadzooks-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: py-gadzooks
-Version: 0.2.7
+Version: 0.2.8
 Summary: A collection of code maintenance tools for Python projects, intended to be used within git hooks.
 Project-URL: Documentation, https://github.com/jeremander/gadzooks#readme
 Project-URL: Issues, https://github.com/jeremander/gadzooks/issues
 Project-URL: Source, https://github.com/jeremander/gadzooks
 Author-email: Jeremy Silver <jeremys@nessiness.com>
 License-Expression: MIT
 License-File: LICENSE
```

