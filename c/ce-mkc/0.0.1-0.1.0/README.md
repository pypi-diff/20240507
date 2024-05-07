# Comparing `tmp/ce_mkc-0.0.1.tar.gz` & `tmp/ce_mkc-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ce_mkc-0.0.1.tar", max compression
+gzip compressed data, was "ce_mkc-0.1.0.tar", max compression
```

## Comparing `ce_mkc-0.0.1.tar` & `ce_mkc-0.1.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    15263 2024-03-20 07:03:50.879186 ce_mkc-0.0.1/README.md
--rw-r--r--   0        0        0    24186 2024-03-20 07:03:50.886024 ce_mkc-0.0.1/ce_mkc.py
--rw-r--r--   0        0        0      594 2024-05-06 13:17:28.764672 ce_mkc-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    16088 1970-01-01 00:00:00.000000 ce_mkc-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    15263 2024-03-20 07:03:50.879186 ce_mkc-0.1.0/README.md
+-rw-r--r--   0        0        0    24186 2024-03-20 07:03:50.886024 ce_mkc-0.1.0/ce_mkc.py
+-rw-r--r--   0        0        0      595 2024-05-06 13:09:49.902413 ce_mkc-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    16090 1970-01-01 00:00:00.000000 ce_mkc-0.1.0/PKG-INFO
```

### Comparing `ce_mkc-0.0.1/README.md` & `ce_mkc-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ce_mkc-0.0.1/ce_mkc.py` & `ce_mkc-0.1.0/ce_mkc.py`

 * *Files identical despite different names*

### Comparing `ce_mkc-0.0.1/pyproject.toml` & `ce_mkc-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "ce-mkc"
-version = "0.0.1"
+version = "0.1.0"
 description = "A command line utility to set up Kafka, MongoDB, and MongoDB Kafka Connector environments."
 authors = ["Your Name <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "~3.9"
+python = "~3.10"
 certifi = "2023.7.22"
 charset-normalizer = "3.2.0"
 confluent-kafka = "2.2.0"
 dnspython = "2.3.0"
 docker = "6.1.3"
 idna = "3.4"
 packaging = "23.1"
```

### Comparing `ce_mkc-0.0.1/PKG-INFO` & `ce_mkc-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ce-mkc
-Version: 0.0.1
+Version: 0.1.0
 Summary: A command line utility to set up Kafka, MongoDB, and MongoDB Kafka Connector environments.
 License: MIT
 Author: Your Name
 Author-email: you@example.com
-Requires-Python: >=3.9,<3.10
+Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: certifi (==2023.7.22)
 Requires-Dist: charset-normalizer (==3.2.0)
 Requires-Dist: confluent-kafka (==2.2.0)
 Requires-Dist: dnspython (==2.3.0)
 Requires-Dist: docker (==6.1.3)
 Requires-Dist: idna (==3.4)
 Requires-Dist: packaging (==23.1)
```

