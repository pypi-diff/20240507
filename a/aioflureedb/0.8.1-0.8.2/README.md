# Comparing `tmp/aioflureedb-0.8.1.tar.gz` & `tmp/aioflureedb-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioflureedb-0.8.1.tar", last modified: Wed May 10 09:49:34 2023, max compression
+gzip compressed data, was "aioflureedb-0.8.2.tar", last modified: Tue May  7 12:54:32 2024, max compression
```

## Comparing `aioflureedb-0.8.1.tar` & `aioflureedb-0.8.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-10 09:49:34.343709 aioflureedb-0.8.1/
--rw-rw-r--   0 rob       (1000) rob       (1000)      774 2023-05-10 09:49:34.343709 aioflureedb-0.8.1/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)     1798 2023-03-30 05:22:33.000000 aioflureedb-0.8.1/README.md
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-10 09:49:34.343709 aioflureedb-0.8.1/aioflureedb/
--rw-r--r--   0 rob       (1000) rob       (1000)    74993 2023-05-10 09:46:00.000000 aioflureedb-0.8.1/aioflureedb/__init__.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     6874 2023-04-14 14:10:59.000000 aioflureedb-0.8.1/aioflureedb/__main__.py
--rw-r--r--   0 rob       (1000) rob       (1000)    25925 2023-04-14 14:07:21.000000 aioflureedb-0.8.1/aioflureedb/domain_api.py
--rw-r--r--   0 rob       (1000) rob       (1000)     7030 2023-04-14 14:06:52.000000 aioflureedb-0.8.1/aioflureedb/signing.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-10 09:49:34.343709 aioflureedb-0.8.1/aioflureedb.egg-info/
--rw-r--r--   0 rob       (1000) rob       (1000)      774 2023-05-10 09:49:33.000000 aioflureedb-0.8.1/aioflureedb.egg-info/PKG-INFO
--rw-r--r--   0 rob       (1000) rob       (1000)      289 2023-05-10 09:49:34.000000 aioflureedb-0.8.1/aioflureedb.egg-info/SOURCES.txt
--rw-r--r--   0 rob       (1000) rob       (1000)        1 2023-05-10 09:49:33.000000 aioflureedb-0.8.1/aioflureedb.egg-info/dependency_links.txt
--rw-r--r--   0 rob       (1000) rob       (1000)       66 2023-05-10 09:49:34.000000 aioflureedb-0.8.1/aioflureedb.egg-info/requires.txt
--rw-r--r--   0 rob       (1000) rob       (1000)       12 2023-05-10 09:49:34.000000 aioflureedb-0.8.1/aioflureedb.egg-info/top_level.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-10 09:49:34.343709 aioflureedb-0.8.1/setup.cfg
--rw-r--r--   0 rob       (1000) rob       (1000)     1148 2023-05-10 09:46:09.000000 aioflureedb-0.8.1/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2024-05-07 12:54:32.244363 aioflureedb-0.8.2/
+-rw-r--r--   0 rob       (1000) rob       (1000)      928 2024-05-07 12:54:32.244363 aioflureedb-0.8.2/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1798 2023-04-06 10:53:51.000000 aioflureedb-0.8.2/README.md
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2024-05-07 12:54:32.244363 aioflureedb-0.8.2/aioflureedb/
+-rw-rw-r--   0 rob       (1000) rob       (1000)    74993 2023-05-25 06:14:17.000000 aioflureedb-0.8.2/aioflureedb/__init__.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     6874 2023-04-20 06:26:42.000000 aioflureedb-0.8.2/aioflureedb/__main__.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    25925 2023-04-20 06:26:42.000000 aioflureedb-0.8.2/aioflureedb/domain_api.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     7151 2024-05-07 12:50:54.000000 aioflureedb-0.8.2/aioflureedb/signing.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2024-05-07 12:54:32.244363 aioflureedb-0.8.2/aioflureedb.egg-info/
+-rw-r--r--   0 rob       (1000) rob       (1000)      928 2024-05-07 12:54:32.000000 aioflureedb-0.8.2/aioflureedb.egg-info/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      289 2024-05-07 12:54:32.000000 aioflureedb-0.8.2/aioflureedb.egg-info/SOURCES.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2024-05-07 12:54:32.000000 aioflureedb-0.8.2/aioflureedb.egg-info/dependency_links.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       89 2024-05-07 12:54:32.000000 aioflureedb-0.8.2/aioflureedb.egg-info/requires.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       12 2024-05-07 12:54:32.000000 aioflureedb-0.8.2/aioflureedb.egg-info/top_level.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2024-05-07 12:54:32.244363 aioflureedb-0.8.2/setup.cfg
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1174 2024-05-07 12:51:43.000000 aioflureedb-0.8.2/setup.py
```

### Comparing `aioflureedb-0.8.1/PKG-INFO` & `aioflureedb-0.8.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: aioflureedb
-Version: 0.8.1
+Version: 0.8.2
 Summary: Asynchonous library for usage of the FlureeDB API
 Home-page: https://github.com/pibara/aioflureedb
 Author: Rob J Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: flureedb fluree flureeql sparql graphql
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Other Environment
+Requires-Dist: starkbank-ecdsa>=2.0.3
+Requires-Dist: python-mbedtls>=2.10.1
+Requires-Dist: aiohttp
+Requires-Dist: base58
 Provides-Extra: domainapi
+Requires-Dist: jsonata>=0.2.3; extra == "domainapi"
 
 An asynchonous client library for communicating with a FlureeDB server, making signed transactions and queries.
     
-
```

### Comparing `aioflureedb-0.8.1/README.md` & `aioflureedb-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `aioflureedb-0.8.1/aioflureedb/__init__.py` & `aioflureedb-0.8.2/aioflureedb/__init__.py`

 * *Files identical despite different names*

### Comparing `aioflureedb-0.8.1/aioflureedb/__main__.py` & `aioflureedb-0.8.2/aioflureedb/__main__.py`

 * *Files identical despite different names*

### Comparing `aioflureedb-0.8.1/aioflureedb/domain_api.py` & `aioflureedb-0.8.2/aioflureedb/domain_api.py`

 * *Files identical despite different names*

### Comparing `aioflureedb-0.8.1/aioflureedb/signing.py` & `aioflureedb-0.8.2/aioflureedb/signing.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 """Low level signing library for FlureeDB signatures"""
 import json
 from enum import Enum
 import random
 import time
 from time import mktime
 import base64
-import hashlib
 import unicodedata
 from email.utils import formatdate
 from datetime import datetime
 import base58
 from ellipticcurve import privateKey, ecdsa
+from mbedtls import hashlib
 
 
 def _to_hex(x):
     """Convert binary string x to a hex string
 
     Parameters
     ----------
@@ -71,15 +71,18 @@
     string
         Base58 encoded FlureeDB address
     """
     x = pubkey.point.x.to_bytes(32, byteorder='big')
     yred = (2 + pubkey.point.y % 2).to_bytes(1, byteorder='big')
     key = yred + x
     hash1 = hashlib.sha256()
-    hash2 = hashlib.new('ripemd160')
+    if 'ripemd160' in hashlib.algorithms_available:
+        hash2 = hashlib.new('ripemd160')
+    else:
+        hash2 = hashlib2.new('ripemd160')
     hash1.update(key)
     hash2.update(hash1.digest())
     core = _net_id_map[chain] + hash2.digest()
     hash3 = hashlib.sha256()
     hash4 = hashlib.sha256()
     hash3.update(core)
     hash4.update(hash3.digest())
```

### Comparing `aioflureedb-0.8.1/aioflureedb.egg-info/PKG-INFO` & `aioflureedb-0.8.2/aioflureedb.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: aioflureedb
-Version: 0.8.1
+Version: 0.8.2
 Summary: Asynchonous library for usage of the FlureeDB API
 Home-page: https://github.com/pibara/aioflureedb
 Author: Rob J Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: flureedb fluree flureeql sparql graphql
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Other Environment
+Requires-Dist: starkbank-ecdsa>=2.0.3
+Requires-Dist: python-mbedtls>=2.10.1
+Requires-Dist: aiohttp
+Requires-Dist: base58
 Provides-Extra: domainapi
+Requires-Dist: jsonata>=0.2.3; extra == "domainapi"
 
 An asynchonous client library for communicating with a FlureeDB server, making signed transactions and queries.
     
-
```

### Comparing `aioflureedb-0.8.1/setup.py` & `aioflureedb-0.8.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 from sys import platform
 here = path.abspath(path.dirname(__file__))
 
-requirements = ["starkbank-ecdsa>=2.0.3", "aiohttp", "base58"]
+requirements = ["starkbank-ecdsa>=2.0.3", "python-mbedtls>=2.10.1", "aiohttp", "base58"]
 
 setup(
     name='aioflureedb',
-    version='0.8.1',
+    version='0.8.2',
     description='Asynchonous library for usage of the FlureeDB API',
     long_description="""An asynchonous client library for communicating with a FlureeDB server, making signed transactions and queries.
     """,
     url='https://github.com/pibara/aioflureedb',
     author='Rob J Meijer',
     author_email='pibara@gmail.com',
     license='BSD',
```

