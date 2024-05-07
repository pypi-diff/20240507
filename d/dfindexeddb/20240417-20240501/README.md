# Comparing `tmp/dfindexeddb-20240417.tar.gz` & `tmp/dfindexeddb-20240501.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfindexeddb-20240417.tar", last modified: Wed Apr 17 13:09:16 2024, max compression
+gzip compressed data, was "dfindexeddb-20240501.tar", last modified: Tue May  7 01:16:25 2024, max compression
```

## Comparing `dfindexeddb-20240417.tar` & `dfindexeddb-20240501.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:09:16.124606 dfindexeddb-20240417/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 13:09:07.000000 dfindexeddb-20240417/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-17 13:09:07.000000 dfindexeddb-20240417/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19935 2024-04-17 13:09:16.124606 dfindexeddb-20240417/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-04-17 13:09:07.000000 dfindexeddb-20240417/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:09:16.120607 dfindexeddb-20240417/dfindexeddb/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:09:16.120607 dfindexeddb-20240417/dfindexeddb/indexeddb/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/indexeddb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:09:16.124606 dfindexeddb-20240417/dfindexeddb/indexeddb/chromium/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/indexeddb/chromium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32122 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/indexeddb/chromium/blink.py
--rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/indexeddb/chromium/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    45079 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/indexeddb/chromium/record.py
--rw-r--r--   0 runner    (1001) docker     (127)    22102 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/indexeddb/chromium/v8.py
--rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/indexeddb/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:09:16.124606 dfindexeddb-20240417/dfindexeddb/indexeddb/firefox/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/indexeddb/firefox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:09:16.124606 dfindexeddb-20240417/dfindexeddb/indexeddb/safari/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/indexeddb/safari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/indexeddb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:09:16.124606 dfindexeddb-20240417/dfindexeddb/leveldb/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/leveldb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/leveldb/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/leveldb/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/leveldb/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/leveldb/ldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/leveldb/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/leveldb/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/leveldb/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-17 13:09:07.000000 dfindexeddb-20240417/dfindexeddb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:09:16.124606 dfindexeddb-20240417/dfindexeddb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19935 2024-04-17 13:09:16.000000 dfindexeddb-20240417/dfindexeddb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-17 13:09:16.000000 dfindexeddb-20240417/dfindexeddb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 13:09:16.000000 dfindexeddb-20240417/dfindexeddb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-17 13:09:16.000000 dfindexeddb-20240417/dfindexeddb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-17 13:09:16.000000 dfindexeddb-20240417/dfindexeddb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 13:09:16.000000 dfindexeddb-20240417/dfindexeddb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-17 13:09:07.000000 dfindexeddb-20240417/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 13:09:16.124606 dfindexeddb-20240417/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-17 13:09:07.000000 dfindexeddb-20240417/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:16:25.428833 dfindexeddb-20240501/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-07 01:16:19.000000 dfindexeddb-20240501/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-07 01:16:19.000000 dfindexeddb-20240501/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18496 2024-05-07 01:16:25.428833 dfindexeddb-20240501/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-05-07 01:16:19.000000 dfindexeddb-20240501/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:16:25.420833 dfindexeddb-20240501/dfindexeddb/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:16:25.424833 dfindexeddb-20240501/dfindexeddb/indexeddb/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:16:25.424833 dfindexeddb-20240501/dfindexeddb/indexeddb/chromium/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/chromium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32122 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/chromium/blink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/chromium/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47366 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/chromium/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22102 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/chromium/v8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:16:25.424833 dfindexeddb-20240501/dfindexeddb/indexeddb/firefox/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/firefox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:16:25.424833 dfindexeddb-20240501/dfindexeddb/indexeddb/safari/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/safari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/safari/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/safari/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21595 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/safari/webkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:16:25.424833 dfindexeddb-20240501/dfindexeddb/leveldb/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/leveldb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7982 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/leveldb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/leveldb/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/leveldb/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/leveldb/ldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/leveldb/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10747 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/leveldb/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/leveldb/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:16:25.424833 dfindexeddb-20240501/dfindexeddb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18496 2024-05-07 01:16:25.000000 dfindexeddb-20240501/dfindexeddb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-07 01:16:25.000000 dfindexeddb-20240501/dfindexeddb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:16:25.000000 dfindexeddb-20240501/dfindexeddb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-07 01:16:25.000000 dfindexeddb-20240501/dfindexeddb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 01:16:25.000000 dfindexeddb-20240501/dfindexeddb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 01:16:25.000000 dfindexeddb-20240501/dfindexeddb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-07 01:16:19.000000 dfindexeddb-20240501/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 01:16:25.428833 dfindexeddb-20240501/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-07 01:16:19.000000 dfindexeddb-20240501/setup.py
```

### Comparing `dfindexeddb-20240417/LICENSE` & `dfindexeddb-20240501/LICENSE`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240417/PKG-INFO` & `dfindexeddb-20240501/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfindexeddb
-Version: 20240417
+Version: 20240501
 Summary: dfindexeddb is an experimental Python tool for performing digital forensic analysis of IndexedDB and leveldb files.
 Author-email: Syd Pleno <sydp@google.com>
 Maintainer-email: dfIndexeddb Developers <dfindexeddb-dev@googlegroups.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -219,20 +219,20 @@
 License-File: AUTHORS
 Requires-Dist: python-snappy==0.6.1
 Requires-Dist: zstd==1.5.5.1
 
 # dfIndexeddb
 
 dfindexeddb is an experimental Python tool for performing digital forensic
-analysis of IndexedDB and leveldb files.
+analysis of IndexedDB and LevelDB files.
 
-It parses leveldb, IndexedDB and javascript structures from these files without
+It parses LevelDB, IndexedDB and JavaScript structures from these files without
 requiring native libraries.  (Note: only a subset of IndexedDB key types and
-Javascript types for Chromium-based browsers are currently supported.  Safari
-and Firefox are under development).
+JavaScript types for Safari and Chromium-based browsers are currently supported.
+Firefox is under development).
 
 The content of IndexedDB files is dependent on what a web application stores
 locally/offline using the web browser's
 [IndexedDB API](https://www.w3.org/TR/IndexedDB/).  Examples of content might
 include:
 * text from a text/source-code editor application,
 * emails and contact information from an e-mail application,
@@ -271,15 +271,15 @@
     $ python3 -m venv .venv
     $ source .venv/bin/activate
     $ pip install .
 ```
 
 ## Usage
 
-Two CLI tools for parsing IndexedDB/leveldb files are available after
+Two CLI tools for parsing IndexedDB/LevelDB files are available after
 installation:
 
 
 ### IndexedDB
 
 ```
 $ dfindexeddb -h
@@ -293,57 +293,50 @@
     ldb         Parse a ldb file as indexeddb.
     log         Parse a log file as indexeddb.
 
 options:
   -h, --help    show this help message and exit
 ```
 
-To parse Indexeddb records from a LevelDB folder, use the following command:
+#### Examples:
 
-```
-dfindexeddb db -h
-usage: dfindexeddb db [-h] -s SOURCE [--use_manifest] [-o {json,jsonl,repr}]
+To parse IndexedDB records from an sqlite file for Safari and output the
+results as JSON-L, use the following command:
 
-options:
-  -h, --help            show this help message and exit
-  -s SOURCE, --source SOURCE
-                        The source leveldb folder
-  --use_manifest        Use manifest file to determine active/recovered records.
-  -o {json,jsonl,repr}, --output {json,jsonl,repr}
-                        Output format. Default is json
+```
+dfindexeddb db -s SOURCE --format safari -o jsonl
 ```
 
-To parse Indexeddb records from a LevelDB ldb (.ldb) file, use the following 
-command:
+To parse IndexedDB records from a LevelDB folder for Chrome/Chromium, using the
+manifest file to determine recovered records and output as JSON, use the
+following command:
 
 ```
-dfindexeddb ldb -h
-usage: dfindexeddb ldb [-h] -s SOURCE [-o {json,jsonl,repr}]
+dfindexeddb db -s SOURCE --format chrome --use_manifest
+```
+
+To parse IndexedDB records from a LevelDB ldb (.ldb) file and output the
+results as JSON-L, use the following command:
 
-options:
-  -h, --help            show this help message and exit
-  -s SOURCE, --source SOURCE
-                        The source .ldb file.
-  -o {json,jsonl,repr}, --output {json,jsonl,repr}
-                        Output format. Default is json
+```
+dfindexeddb ldb -s SOURCE -o jsonl
 ```
 
-To parse Indexeddb records from a LevelDB log (.log) file, use the following 
-command:
+To parse IndexedDB records from a LevelDB log (.log) file and output the
+results as the Python printable representation, use the following command:
 
 ```
-dfindexeddb log -h
-usage: dfindexeddb log [-h] -s SOURCE [-o {json,jsonl,repr}]
+dfindexeddb log -s SOURCE -o repr
+```
 
-options:
-  -h, --help            show this help message and exit
-  -s SOURCE, --source SOURCE
-                        The source .log file.
-  -o {json,jsonl,repr}, --output {json,jsonl,repr}
-                        Output format. Default is json
+To parse a file as a Chrome/Chromium IndexedDB blink value and output the
+results as JSON:
+
+```
+dfindexeddb blink -s SOURCE
 ```
 
 ### LevelDB
 
 ```
 $ dfleveldb -h
 usage: dfleveldb [-h] {db,log,ldb,descriptor} ...
@@ -357,60 +350,40 @@
     ldb                 Parse a leveldb table (.ldb) file.
     descriptor          Parse a leveldb descriptor (MANIFEST) file.
 
 options:
   -h, --help            show this help message and exit
 ```
 
+#### Examples
+
 To parse records from a LevelDB folder, use the following command:
 
 ```
-dfindexeddb db -h
-usage: dfindexeddb db [-h] -s SOURCE [--use_manifest] [-o {json,jsonl,repr}]
-
-options:
-  -h, --help            show this help message and exit
-  -s SOURCE, --source SOURCE
-                        The source leveldb folder
-  --use_manifest        Use manifest file to determine active/recovered records.
-  -o {json,jsonl,repr}, --output {json,jsonl,repr}
-                        Output format. Default is json
+dfindexeddb db -s SOURCE
 ```
 
-To parse records from a LevelDB log (.log) file, use the following command:
+To parse blocks / physical records/ write batches / internal key records from a
+LevelDB log (.log) file, use the following command, specifying the type (block,
+physical_records, etc) via the `-t` option.  By default, internal key records are parsed:
 
 ```
-$ dfleveldb log  -s SOURCE [-o {json,jsonl,repr}] [-t {blocks,physical_records,write_batches,parsed_internal_key}]
-
-options:
-  -h, --help            show this help message and exit
-  -s SOURCE, --source SOURCE
-                        The source leveldb file
-  -o {json,jsonl,repr}, --output {json,jsonl,repr}
-                        Output format. Default is json
-  -t {blocks,physical_records,write_batches,parsed_internal_key}, --structure_type {blocks,physical_records,write_batches,parsed_internal_key}
-                        Parses the specified structure. Default is parsed_internal_key.
+$ dfleveldb log  -s SOURCE [-t {blocks,physical_records,write_batches,parsed_internal_key}]
 ```
 
-To parse records from a LevelDB table (.ldb) file, use the following command:
+To parse blocks / records from a LevelDB table (.ldb) file, use the following
+command, specifying the type (blocks, records) via the `-t` option.  By
+default, records are parsed:
 
 ```
-$ dfleveldb ldb -s SOURCE [-o {json,jsonl,repr}] [-t {blocks,records}]
-
-options:
-  -h, --help            show this help message and exit
-  -s SOURCE, --source SOURCE
-                        The source leveldb file
-  -o {json,jsonl,repr}, --output {json,jsonl,repr}
-                        Output format. Default is json
-  -t {blocks,records}, --structure_type {blocks,records}
-                        Parses the specified structure. Default is records.
+$ dfleveldb ldb -s SOURCE [-t {blocks,records}]
 ```
 
-To parse version edit records from a Descriptor (MANIFEST) file:
+To parse version edit records from a Descriptor (MANIFEST) file, use the
+following command:
 
 ```
 $ dfleveldb descriptor -s SOURCE [-o {json,jsonl,repr}] [-t {blocks,physical_records,versionedit} | -v]
 
 options:
   -h, --help            show this help message and exit
   -s SOURCE, --source SOURCE
```

### Comparing `dfindexeddb-20240417/dfindexeddb/__init__.py` & `dfindexeddb-20240501/dfindexeddb/__init__.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240417/dfindexeddb/errors.py` & `dfindexeddb-20240501/dfindexeddb/errors.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240417/dfindexeddb/indexeddb/__init__.py` & `dfindexeddb-20240501/dfindexeddb/indexeddb/__init__.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240417/dfindexeddb/indexeddb/chromium/__init__.py` & `dfindexeddb-20240501/dfindexeddb/indexeddb/chromium/__init__.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240417/dfindexeddb/indexeddb/chromium/blink.py` & `dfindexeddb-20240501/dfindexeddb/indexeddb/chromium/blink.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240417/dfindexeddb/indexeddb/chromium/definitions.py` & `dfindexeddb-20240501/dfindexeddb/indexeddb/chromium/definitions.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240417/dfindexeddb/indexeddb/chromium/record.py` & `dfindexeddb-20240501/dfindexeddb/indexeddb/chromium/record.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Parses Chromium IndexedDb structures."""
 from __future__ import annotations
 from dataclasses import dataclass, field
 from datetime import datetime
 import io
-from typing import Any, BinaryIO, Optional, Tuple, Type, TypeVar, Union
+import pathlib
+import sys
+import traceback
+from typing import Any, BinaryIO, Generator, Optional, Tuple, Type, TypeVar, \
+    Union
 
 from dfindexeddb import errors
 from dfindexeddb.indexeddb.chromium import blink
 from dfindexeddb.indexeddb.chromium import definitions
 from dfindexeddb.leveldb import record
 from dfindexeddb.leveldb import utils
 
@@ -452,15 +456,15 @@
     return decoder.DecodeVarint()[1]
 
   @classmethod
   def FromDecoder(
       cls, decoder: utils.LevelDBDecoder, key_prefix: KeyPrefix,
       base_offset: int = 0
   ) -> MaxDatabaseIdKey:
-    """Decodes the maximum databse key."""
+    """Decodes the maximum database key."""
     offset, key_type = decoder.DecodeUint8()
     if key_type != definitions.GlobalMetadataKeyType.MAX_DATABASE_ID:
       raise errors.ParserError('Not a MaxDatabaseIdKey')
     return cls(offset=base_offset + offset, key_prefix=key_prefix)
 
 
 @dataclass
@@ -1327,34 +1331,37 @@
 
 
 @dataclass
 class IndexedDBRecord:
   """An IndexedDB Record.
 
   Attributes:
+    path: the source file path
     offset: the offset of the record.
     key: the key of the record.
     value: the value of the record.
     sequence_number: if available, the sequence number of the record.
     type: the type of the record.
-    level: the leveldb level, None indicates the record came from a log file.
+    level: the leveldb level, if applicable, None can indicate the record
+        originated from a log file or the level could not be determined.
     recovered: True if the record is a recovered record.
   """
   path: str
   offset: int
   key: Any
   value: Any
   sequence_number: Optional[int]
   type: int
   level: Optional[int]
   recovered: Optional[bool]
 
   @classmethod
   def FromLevelDBRecord(
-      cls, db_record: record.LevelDBRecord
+      cls,
+      db_record: record.LevelDBRecord
   ) -> IndexedDBRecord:
     """Returns an IndexedDBRecord from a ParsedInternalKey."""
     idb_key = IndexedDbKey.FromBytes(
         db_record.record.key, base_offset=db_record.record.offset)
     idb_value = idb_key.ParseValue(db_record.record.value)
     return cls(
         path=db_record.path,
@@ -1362,7 +1369,78 @@
         key=idb_key,
         value=idb_value,
         sequence_number=db_record.record.sequence_number if hasattr(
             db_record.record, 'sequence_number') else None,
         type=db_record.record.record_type,
         level=db_record.level,
         recovered=db_record.recovered)
+
+  @classmethod
+  def FromFile(
+      cls,
+      file_path: pathlib.Path
+  ) -> Generator[IndexedDBRecord, None, None]:
+    """Yields IndexedDBRecords from a file."""
+    for db_record in record.LevelDBRecord.FromFile(file_path):
+      try:
+        yield cls.FromLevelDBRecord(db_record)
+      except(
+          errors.ParserError,
+          errors.DecoderError,
+          NotImplementedError) as err:
+        print((
+            'Error parsing Indexeddb record: '
+            f'{err} at offset {db_record.record.offset} in '
+            f'{db_record.path}'),
+            file=sys.stderr)
+        print(f'Traceback: {traceback.format_exc()}', file=sys.stderr)
+
+
+class FolderReader:
+  """A IndexedDB folder reader for Chrome/Chromium.
+
+  Attributes:
+    foldername (str): the source LevelDB folder.
+  """
+
+  def __init__(self, foldername: pathlib.Path):
+    """Initializes the FileReader.
+
+    Args:
+      foldername: the source IndexedDB folder.
+
+    Raises:
+      ValueError: if foldername is None or not a directory.
+    """
+    if not foldername or not foldername.is_dir():
+      raise ValueError(f'{foldername} is None or not a directory')
+    self.foldername = foldername
+
+  def GetRecords(
+      self,
+      use_manifest: bool = False
+  ) -> Generator[IndexedDBRecord, None, None]:
+    """Yield LevelDBRecords.
+
+    Args:
+      use_manifest: True to use the current manifest in the folder as a means to
+          find the active file set.
+
+    Yields:
+      IndexedDBRecord.
+    """
+    leveldb_folder_reader = record.FolderReader(self.foldername)
+    for leveldb_record in leveldb_folder_reader.GetRecords(
+        use_manifest=use_manifest):
+      try:
+        yield IndexedDBRecord.FromLevelDBRecord(
+            leveldb_record)
+      except(
+          errors.ParserError,
+          errors.DecoderError,
+          NotImplementedError) as err:
+        print((
+            'Error parsing Indexeddb record: '
+            f'{err} at offset {leveldb_record.record.offset} in '
+            f'{leveldb_record.path}'),
+            file=sys.stderr)
+        print(f'Traceback: {traceback.format_exc()}', file=sys.stderr)
```

### Comparing `dfindexeddb-20240417/dfindexeddb/indexeddb/chromium/v8.py` & `dfindexeddb-20240501/dfindexeddb/indexeddb/chromium/v8.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240417/dfindexeddb/indexeddb/cli.py` & `dfindexeddb-20240501/dfindexeddb/leveldb/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,163 +8,162 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""A CLI tool for dfindexeddb."""
+"""A CLI tool for leveldb files."""
 import argparse
 import dataclasses
-import enum
 from datetime import datetime
 import json
 import pathlib
-import sys
-import traceback
 
-from dfindexeddb import errors
 from dfindexeddb import version
-from dfindexeddb.leveldb import record as leveldb_record
-from dfindexeddb.indexeddb.chromium import record as chromium_record
-from dfindexeddb.indexeddb.chromium import v8
+from dfindexeddb.leveldb import descriptor
+from dfindexeddb.leveldb import ldb
+from dfindexeddb.leveldb import log
+from dfindexeddb.leveldb import record
 
 
 _VALID_PRINTABLE_CHARACTERS = (
     ' abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789' +
     '!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~.')
 
 
 class Encoder(json.JSONEncoder):
-  """A JSON encoder class for dfindexeddb fields."""
+  """A JSON encoder class for dfleveldb fields."""
+
   def default(self, o):
+    """Returns a serializable object for o."""
     if dataclasses.is_dataclass(o):
       o_dict = dataclasses.asdict(o)
       return o_dict
     if isinstance(o, bytes):
       out = []
       for x in o:
         if chr(x) not in _VALID_PRINTABLE_CHARACTERS:
           out.append(f'\\x{x:02X}')
         else:
           out.append(chr(x))
       return ''.join(out)
     if isinstance(o, datetime):
       return o.isoformat()
-    if isinstance(o, v8.Undefined):
-      return "<undefined>"
-    if isinstance(o, v8.Null):
-      return "<null>"
     if isinstance(o, set):
       return list(o)
-    if isinstance(o, v8.RegExp):
-      return str(o)
-    if isinstance(o, enum.Enum):
-      return o.name
     return json.JSONEncoder.default(self, o)
 
 
 def _Output(structure, output):
   """Helper method to output parsed structure to stdout."""
   if output == 'json':
     print(json.dumps(structure, indent=2, cls=Encoder))
   elif output == 'jsonl':
     print(json.dumps(structure, cls=Encoder))
   elif output == 'repr':
     print(structure)
 
 
 def DbCommand(args):
-  """The CLI for processing a directory as indexeddb."""
-  if args.use_manifest:
-    for db_record in leveldb_record.LevelDBRecord.FromManifest(args.source):
-      record = db_record.record
-      try:
-        idb_record = chromium_record.IndexedDBRecord.FromLevelDBRecord(
-            db_record)
-      except(
-          errors.ParserError,
-          errors.DecoderError,
-          NotImplementedError) as err:
-        print((
-            f'Error parsing Indexeddb record {record.__class__.__name__}: {err}'
-            f' at offset {record.offset} in {db_record.path}'), file=sys.stderr)
-        print(f'Traceback: {traceback.format_exc()}', file=sys.stderr)
-        continue
-      _Output(idb_record, output=args.output)
-  else:
-    for db_record in leveldb_record.LevelDBRecord.FromDir(args.source):
-      record = db_record.record
-      try:
-        idb_record = chromium_record.IndexedDBRecord.FromLevelDBRecord(
-            db_record)
-      except(
-          errors.ParserError,
-          errors.DecoderError,
-          NotImplementedError) as err:
-        print((
-            f'Error parsing Indexeddb record {record.__class__.__name__}: {err}'
-            f' at offset {record.offset} in {db_record.path}'), file=sys.stderr)
-        print(f'Traceback: {traceback.format_exc()}', file=sys.stderr)
-        continue
-      _Output(idb_record, output=args.output)
+  """The CLI for processing leveldb folders."""
+  for leveldb_record in record.FolderReader(
+      args.source).GetRecords(use_manifest=args.use_manifest):
+    _Output(leveldb_record, output=args.output)
 
 
 def LdbCommand(args):
-  """The CLI for processing a leveldb table (.ldb) file as indexeddb."""
-  for db_record in leveldb_record.LevelDBRecord.FromFile(args.source):
-    record = db_record.record
-    try:
-      idb_record = chromium_record.IndexedDBRecord.FromLevelDBRecord(
-          db_record)
-    except(
-        errors.ParserError,
-        errors.DecoderError,
-        NotImplementedError) as err:
-      print(
-          (f'Error parsing Indexeddb record {record.__class__.__name__}: {err} '
-           f'at offset {record.offset} in {db_record.path}'), file=sys.stderr)
-      print(f'Traceback: {traceback.format_exc()}', file=sys.stderr)
-      continue
-    _Output(idb_record, output=args.output)
+  """The CLI for processing ldb files."""
+  ldb_file = ldb.FileReader(args.source)
+
+  if args.structure_type == 'blocks':
+    # Prints block information.
+    for block in ldb_file.GetBlocks():
+      _Output(block, output=args.output)
+
+  elif args.structure_type == 'records' or not args.structure_type:
+    # Prints key value record information.
+    for key_value_record in ldb_file.GetKeyValueRecords():
+      _Output(key_value_record, output=args.output)
+
+  else:
+    print(f'{args.structure_type} is not supported for ldb files.')
 
 
 def LogCommand(args):
-  """The CLI for processing a leveldb log file as indexeddb."""
-  for db_record in leveldb_record.LevelDBRecord.FromFile(args.source):
-    record = db_record.record
-    try:
-      idb_record = chromium_record.IndexedDBRecord.FromLevelDBRecord(
-          db_record)
-    except(
-        errors.ParserError,
-        errors.DecoderError,
-        NotImplementedError) as err:
-      print(
-          (f'Error parsing Indexeddb record {record.__class__.__name__}: {err} '
-           f'at offset {record.offset} in {db_record.path}'), file=sys.stderr)
-      print(f'Traceback: {traceback.format_exc()}', file=sys.stderr)
-      continue
-    _Output(idb_record, output=args.output)
+  """The CLI for processing log files."""
+  log_file = log.FileReader(args.source)
+
+  if args.structure_type == 'blocks':
+    # Prints block information.
+    for block in log_file.GetBlocks():
+      _Output(block, output=args.output)
+
+  elif args.structure_type == 'physical_records':
+    # Prints log file physical record information.
+    for log_file_record in log_file.GetPhysicalRecords():
+      _Output(log_file_record, output=args.output)
+
+  elif args.structure_type == 'write_batches':
+    # Prints log file batch information.
+    for batch in log_file.GetWriteBatches():
+      _Output(batch, output=args.output)
+
+  elif (args.structure_type in ('parsed_internal_key', 'records')
+        or not args.structure_type):
+    # Prints key value record information.
+    for internal_key_record in log_file.GetParsedInternalKeys():
+      _Output(internal_key_record, output=args.output)
+
+  else:
+    print(f'{args.structure_type} is not supported for log files.')
+
 
+def DescriptorCommand(args):
+  """The CLI for processing descriptor (MANIFEST) files."""
+  manifest_file = descriptor.FileReader(args.source)
+
+  if args.version_history:
+    for levels in manifest_file.GetVersions():
+      _Output(levels, output=args.output)
+
+  elif args.structure_type == 'blocks':
+    # Prints block information.
+    for block in manifest_file.GetBlocks():
+      _Output(block, output=args.output)
+
+  elif args.structure_type == 'physical_records':
+    # Prints log file physical record information.
+    for log_file_record in manifest_file.GetPhysicalRecords():
+      _Output(log_file_record, output=args.output)
+
+  elif (args.structure_type == 'versionedit'
+        or not args.structure_type):
+    for version_edit in manifest_file.GetVersionEdits():
+      _Output(version_edit, output=args.output)
+
+  else:
+    print(f'{args.structure_type} is not supported for descriptor files.')
 
 def App():
-  """The CLI app entrypoint for dfindexeddb."""
+  """The CLI app entrypoint for parsing leveldb files."""
   parser = argparse.ArgumentParser(
-      prog='dfindexeddb',
-      description='A cli tool for parsing indexeddb files',
+      prog='dfleveldb',
+      description='A cli tool for parsing leveldb files',
       epilog=f'Version {version.GetVersion()}')
 
   subparsers = parser.add_subparsers()
 
   parser_db = subparsers.add_parser(
-      'db', help='Parse a directory as indexeddb.')
+      'db', help='Parse a directory as leveldb.')
   parser_db.add_argument(
-      '-s', '--source', required=True, type=pathlib.Path,
-      help='The source leveldb folder')
+      '-s', '--source',
+      required=True,
+      type=pathlib.Path,
+      help='The source leveldb directory')
   parser_db.add_argument(
       '--use_manifest',
       action='store_true',
       help='Use manifest file to determine active/deleted records.')
   parser_db.add_argument(
       '-o',
       '--output',
@@ -172,41 +171,95 @@
           'json',
           'jsonl',
           'repr'],
       default='json',
       help='Output format.  Default is json')
   parser_db.set_defaults(func=DbCommand)
 
+  parser_log = subparsers.add_parser(
+      'log', help='Parse a leveldb log file.')
+  parser_log.add_argument(
+      '-s', '--source',
+      required=True,
+      type=pathlib.Path,
+      help='The source leveldb file')
+  parser_log.add_argument(
+      '-o',
+      '--output',
+      choices=[
+          'json',
+          'jsonl',
+          'repr'],
+      default='json',
+      help='Output format.  Default is json')
+  parser_log.add_argument(
+      '-t',
+      '--structure_type',
+      choices=[
+          'blocks',
+          'physical_records',
+          'write_batches',
+          'parsed_internal_key'],
+      help='Parses the specified structure.  Default is parsed_internal_key.')
+  parser_log.set_defaults(func=LogCommand)
+
   parser_ldb = subparsers.add_parser(
-      'ldb', help='Parse a ldb file as indexeddb.')
+      'ldb', help='Parse a leveldb table (.ldb) file.')
   parser_ldb.add_argument(
-      '-s', '--source', required=True, type=pathlib.Path,
-      help='The source .ldb file.')
+      '-s', '--source',
+      required=True,
+      type=pathlib.Path,
+      help='The source leveldb file')
   parser_ldb.add_argument(
       '-o',
       '--output',
       choices=[
           'json',
           'jsonl',
           'repr'],
       default='json',
       help='Output format.  Default is json')
+  parser_ldb.add_argument(
+      '-t',
+      '--structure_type',
+      choices=[
+          'blocks',
+          'records'],
+      help='Parses the specified structure.  Default is records.')
   parser_ldb.set_defaults(func=LdbCommand)
 
-  parser_log = subparsers.add_parser(
-      'log', help='Parse a log file as indexeddb.')
-  parser_log.add_argument(
-      '-s', '--source', required=True, type=pathlib.Path,
-      help='The source .log file.')
-  parser_log.add_argument(
+  parser_descriptor = subparsers.add_parser(
+      'descriptor', help='Parse a leveldb descriptor (MANIFEST) file.')
+  parser_descriptor.add_argument(
+      '-s', '--source',
+      required=True,
+      type=pathlib.Path,
+      help='The source leveldb file')
+  parser_descriptor.add_argument(
       '-o',
       '--output',
       choices=[
           'json',
           'jsonl',
           'repr'],
       default='json',
       help='Output format.  Default is json')
-  parser_log.set_defaults(func=LogCommand)
+  db_group = parser_descriptor.add_mutually_exclusive_group()
+  db_group.add_argument(
+      '-t',
+      '--structure_type',
+      choices=[
+          'blocks', 'physical_records', 'versionedit'],
+      help='Parses the specified structure.  Default is versionedit.')
+  db_group.add_argument(
+      '-v',
+      '--version_history',
+      action='store_true',
+      help='Parses the leveldb version history.')
+  parser_descriptor.set_defaults(func=DescriptorCommand)
 
   args = parser.parse_args()
-  args.func(args)
+
+  if not hasattr(args, 'func'):
+    parser.print_usage()
+  else:
+    args.func(args)
```

### Comparing `dfindexeddb-20240417/dfindexeddb/indexeddb/firefox/__init__.py` & `dfindexeddb-20240501/dfindexeddb/indexeddb/firefox/__init__.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240417/dfindexeddb/indexeddb/safari/__init__.py` & `dfindexeddb-20240501/dfindexeddb/indexeddb/safari/__init__.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240417/dfindexeddb/leveldb/__init__.py` & `dfindexeddb-20240501/dfindexeddb/leveldb/__init__.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240417/dfindexeddb/leveldb/definitions.py` & `dfindexeddb-20240501/dfindexeddb/leveldb/definitions.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240417/dfindexeddb/leveldb/descriptor.py` & `dfindexeddb-20240501/dfindexeddb/leveldb/descriptor.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240417/dfindexeddb/leveldb/ldb.py` & `dfindexeddb-20240501/dfindexeddb/leveldb/ldb.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240417/dfindexeddb/leveldb/log.py` & `dfindexeddb-20240501/dfindexeddb/leveldb/log.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240417/dfindexeddb/leveldb/utils.py` & `dfindexeddb-20240501/dfindexeddb/leveldb/utils.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240417/dfindexeddb/utils.py` & `dfindexeddb-20240501/dfindexeddb/utils.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240417/dfindexeddb/version.py` & `dfindexeddb-20240501/dfindexeddb/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Version information for dfIndexeddb."""
 
 
-__version__ = "20240417"
+__version__ = "20240501"
 
 
 def GetVersion():
   """Returns the version information."""
   return __version__
```

### Comparing `dfindexeddb-20240417/dfindexeddb.egg-info/PKG-INFO` & `dfindexeddb-20240501/dfindexeddb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfindexeddb
-Version: 20240417
+Version: 20240501
 Summary: dfindexeddb is an experimental Python tool for performing digital forensic analysis of IndexedDB and leveldb files.
 Author-email: Syd Pleno <sydp@google.com>
 Maintainer-email: dfIndexeddb Developers <dfindexeddb-dev@googlegroups.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -219,20 +219,20 @@
 License-File: AUTHORS
 Requires-Dist: python-snappy==0.6.1
 Requires-Dist: zstd==1.5.5.1
 
 # dfIndexeddb
 
 dfindexeddb is an experimental Python tool for performing digital forensic
-analysis of IndexedDB and leveldb files.
+analysis of IndexedDB and LevelDB files.
 
-It parses leveldb, IndexedDB and javascript structures from these files without
+It parses LevelDB, IndexedDB and JavaScript structures from these files without
 requiring native libraries.  (Note: only a subset of IndexedDB key types and
-Javascript types for Chromium-based browsers are currently supported.  Safari
-and Firefox are under development).
+JavaScript types for Safari and Chromium-based browsers are currently supported.
+Firefox is under development).
 
 The content of IndexedDB files is dependent on what a web application stores
 locally/offline using the web browser's
 [IndexedDB API](https://www.w3.org/TR/IndexedDB/).  Examples of content might
 include:
 * text from a text/source-code editor application,
 * emails and contact information from an e-mail application,
@@ -271,15 +271,15 @@
     $ python3 -m venv .venv
     $ source .venv/bin/activate
     $ pip install .
 ```
 
 ## Usage
 
-Two CLI tools for parsing IndexedDB/leveldb files are available after
+Two CLI tools for parsing IndexedDB/LevelDB files are available after
 installation:
 
 
 ### IndexedDB
 
 ```
 $ dfindexeddb -h
@@ -293,57 +293,50 @@
     ldb         Parse a ldb file as indexeddb.
     log         Parse a log file as indexeddb.
 
 options:
   -h, --help    show this help message and exit
 ```
 
-To parse Indexeddb records from a LevelDB folder, use the following command:
+#### Examples:
 
-```
-dfindexeddb db -h
-usage: dfindexeddb db [-h] -s SOURCE [--use_manifest] [-o {json,jsonl,repr}]
+To parse IndexedDB records from an sqlite file for Safari and output the
+results as JSON-L, use the following command:
 
-options:
-  -h, --help            show this help message and exit
-  -s SOURCE, --source SOURCE
-                        The source leveldb folder
-  --use_manifest        Use manifest file to determine active/recovered records.
-  -o {json,jsonl,repr}, --output {json,jsonl,repr}
-                        Output format. Default is json
+```
+dfindexeddb db -s SOURCE --format safari -o jsonl
 ```
 
-To parse Indexeddb records from a LevelDB ldb (.ldb) file, use the following 
-command:
+To parse IndexedDB records from a LevelDB folder for Chrome/Chromium, using the
+manifest file to determine recovered records and output as JSON, use the
+following command:
 
 ```
-dfindexeddb ldb -h
-usage: dfindexeddb ldb [-h] -s SOURCE [-o {json,jsonl,repr}]
+dfindexeddb db -s SOURCE --format chrome --use_manifest
+```
+
+To parse IndexedDB records from a LevelDB ldb (.ldb) file and output the
+results as JSON-L, use the following command:
 
-options:
-  -h, --help            show this help message and exit
-  -s SOURCE, --source SOURCE
-                        The source .ldb file.
-  -o {json,jsonl,repr}, --output {json,jsonl,repr}
-                        Output format. Default is json
+```
+dfindexeddb ldb -s SOURCE -o jsonl
 ```
 
-To parse Indexeddb records from a LevelDB log (.log) file, use the following 
-command:
+To parse IndexedDB records from a LevelDB log (.log) file and output the
+results as the Python printable representation, use the following command:
 
 ```
-dfindexeddb log -h
-usage: dfindexeddb log [-h] -s SOURCE [-o {json,jsonl,repr}]
+dfindexeddb log -s SOURCE -o repr
+```
 
-options:
-  -h, --help            show this help message and exit
-  -s SOURCE, --source SOURCE
-                        The source .log file.
-  -o {json,jsonl,repr}, --output {json,jsonl,repr}
-                        Output format. Default is json
+To parse a file as a Chrome/Chromium IndexedDB blink value and output the
+results as JSON:
+
+```
+dfindexeddb blink -s SOURCE
 ```
 
 ### LevelDB
 
 ```
 $ dfleveldb -h
 usage: dfleveldb [-h] {db,log,ldb,descriptor} ...
@@ -357,60 +350,40 @@
     ldb                 Parse a leveldb table (.ldb) file.
     descriptor          Parse a leveldb descriptor (MANIFEST) file.
 
 options:
   -h, --help            show this help message and exit
 ```
 
+#### Examples
+
 To parse records from a LevelDB folder, use the following command:
 
 ```
-dfindexeddb db -h
-usage: dfindexeddb db [-h] -s SOURCE [--use_manifest] [-o {json,jsonl,repr}]
-
-options:
-  -h, --help            show this help message and exit
-  -s SOURCE, --source SOURCE
-                        The source leveldb folder
-  --use_manifest        Use manifest file to determine active/recovered records.
-  -o {json,jsonl,repr}, --output {json,jsonl,repr}
-                        Output format. Default is json
+dfindexeddb db -s SOURCE
 ```
 
-To parse records from a LevelDB log (.log) file, use the following command:
+To parse blocks / physical records/ write batches / internal key records from a
+LevelDB log (.log) file, use the following command, specifying the type (block,
+physical_records, etc) via the `-t` option.  By default, internal key records are parsed:
 
 ```
-$ dfleveldb log  -s SOURCE [-o {json,jsonl,repr}] [-t {blocks,physical_records,write_batches,parsed_internal_key}]
-
-options:
-  -h, --help            show this help message and exit
-  -s SOURCE, --source SOURCE
-                        The source leveldb file
-  -o {json,jsonl,repr}, --output {json,jsonl,repr}
-                        Output format. Default is json
-  -t {blocks,physical_records,write_batches,parsed_internal_key}, --structure_type {blocks,physical_records,write_batches,parsed_internal_key}
-                        Parses the specified structure. Default is parsed_internal_key.
+$ dfleveldb log  -s SOURCE [-t {blocks,physical_records,write_batches,parsed_internal_key}]
 ```
 
-To parse records from a LevelDB table (.ldb) file, use the following command:
+To parse blocks / records from a LevelDB table (.ldb) file, use the following
+command, specifying the type (blocks, records) via the `-t` option.  By
+default, records are parsed:
 
 ```
-$ dfleveldb ldb -s SOURCE [-o {json,jsonl,repr}] [-t {blocks,records}]
-
-options:
-  -h, --help            show this help message and exit
-  -s SOURCE, --source SOURCE
-                        The source leveldb file
-  -o {json,jsonl,repr}, --output {json,jsonl,repr}
-                        Output format. Default is json
-  -t {blocks,records}, --structure_type {blocks,records}
-                        Parses the specified structure. Default is records.
+$ dfleveldb ldb -s SOURCE [-t {blocks,records}]
 ```
 
-To parse version edit records from a Descriptor (MANIFEST) file:
+To parse version edit records from a Descriptor (MANIFEST) file, use the
+following command:
 
 ```
 $ dfleveldb descriptor -s SOURCE [-o {json,jsonl,repr}] [-t {blocks,physical_records,versionedit} | -v]
 
 options:
   -h, --help            show this help message and exit
   -s SOURCE, --source SOURCE
```

### Comparing `dfindexeddb-20240417/dfindexeddb.egg-info/SOURCES.txt` & `dfindexeddb-20240501/dfindexeddb.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 dfindexeddb/indexeddb/chromium/__init__.py
 dfindexeddb/indexeddb/chromium/blink.py
 dfindexeddb/indexeddb/chromium/definitions.py
 dfindexeddb/indexeddb/chromium/record.py
 dfindexeddb/indexeddb/chromium/v8.py
 dfindexeddb/indexeddb/firefox/__init__.py
 dfindexeddb/indexeddb/safari/__init__.py
+dfindexeddb/indexeddb/safari/definitions.py
+dfindexeddb/indexeddb/safari/record.py
+dfindexeddb/indexeddb/safari/webkit.py
 dfindexeddb/leveldb/__init__.py
 dfindexeddb/leveldb/cli.py
 dfindexeddb/leveldb/definitions.py
 dfindexeddb/leveldb/descriptor.py
 dfindexeddb/leveldb/ldb.py
 dfindexeddb/leveldb/log.py
 dfindexeddb/leveldb/record.py
```

### Comparing `dfindexeddb-20240417/pyproject.toml` & `dfindexeddb-20240501/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dfindexeddb"
-version = "20240417"
+version = "20240501"
 requires-python = ">=3.8"
 description = "dfindexeddb is an experimental Python tool for performing digital forensic analysis of IndexedDB and leveldb files."
 license = {file = "LICENSE"}
 authors = [{name = "Syd Pleno", email = "sydp@google.com"}]
 maintainers = [
   {name = "dfIndexeddb Developers", email = "dfindexeddb-dev@googlegroups.com"},
 ]
```

### Comparing `dfindexeddb-20240417/setup.py` & `dfindexeddb-20240501/setup.py`

 * *Files identical despite different names*

