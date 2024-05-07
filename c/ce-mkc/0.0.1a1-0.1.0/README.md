# Comparing `tmp/ce_mkc-0.0.1a1.tar.gz` & `tmp/ce_mkc-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ce_mkc-0.0.1a1.tar", max compression
+gzip compressed data, was "ce_mkc-0.1.0.tar", max compression
```

## Comparing `ce_mkc-0.0.1a1.tar` & `ce_mkc-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,4 @@
--rw-r--r--   0        0        0    15263 2024-03-20 07:03:50.879186 ce_mkc-0.0.1a1/README.md
--rw-r--r--   0        0        0       20 2024-05-07 07:55:29.423704 ce_mkc-0.0.1a1/ce_mkc/__init__.py
--rw-r--r--   0        0        0      158 2024-05-07 09:09:28.156513 ce_mkc-0.0.1a1/ce_mkc/__main__.py
--rw-r--r--   0        0        0    24232 2024-05-07 09:11:32.066174 ce_mkc-0.0.1a1/ce_mkc/ce_mkc.py
--rw-r--r--   0        0        0      547 2024-03-20 07:03:50.886613 ce_mkc-0.0.1a1/ce_mkc/templates/akhq/akhq.template
--rw-r--r--   0        0        0     5286 2024-03-20 07:03:50.886893 ce_mkc-0.0.1a1/ce_mkc/templates/docker-compose.template
--rw-r--r--   0        0        0     4397 2024-03-20 07:03:50.887211 ce_mkc-0.0.1a1/ce_mkc/templates/docker-compose.template.reference
--rw-r--r--   0        0        0     1803 2024-03-20 07:03:50.887704 ce_mkc-0.0.1a1/ce_mkc/templates/kafka/kafka.template
--rw-r--r--   0        0        0      313 2024-03-20 07:03:50.888064 ce_mkc-0.0.1a1/ce_mkc/templates/kafka/zookeeper.template
--rw-r--r--   0        0        0     2251 2024-03-20 07:03:50.888532 ce_mkc-0.0.1a1/ce_mkc/templates/kafkaconnect/kafkaconnect.template
--rw-r--r--   0        0        0      112 2024-03-20 07:03:50.888816 ce_mkc-0.0.1a1/ce_mkc/templates/mongod/mongod.conf.template
--rw-r--r--   0        0        0      372 2024-03-20 07:03:50.889009 ce_mkc-0.0.1a1/ce_mkc/templates/mongod/mongod.template
--rw-r--r--   0        0        0      335 2024-03-20 07:03:50.889354 ce_mkc-0.0.1a1/ce_mkc/templates/schemaregistry/schemaregistry.template
--rw-r--r--   0        0        0      597 2024-05-07 10:15:58.917499 ce_mkc-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0    16090 1970-01-01 00:00:00.000000 ce_mkc-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0    15263 2024-03-20 07:03:50.879186 ce_mkc-0.1.0/README.md
+-rw-r--r--   0        0        0    24186 2024-03-20 07:03:50.886024 ce_mkc-0.1.0/ce_mkc.py
+-rw-r--r--   0        0        0      595 2024-05-06 13:09:49.902413 ce_mkc-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    16090 1970-01-01 00:00:00.000000 ce_mkc-0.1.0/PKG-INFO
```

### Comparing `ce_mkc-0.0.1a1/README.md` & `ce_mkc-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ce_mkc-0.0.1a1/ce_mkc/ce_mkc.py` & `ce_mkc-0.1.0/ce_mkc.py`

 * *Files 0% similar despite different names*

```diff
@@ -641,22 +641,19 @@
 
 def _configureLogger(logLevel):
     format = '%(message)s'
     if logLevel != 'INFO':
         format = '%(levelname)s: %(message)s'
     logging.basicConfig(format=format, level=logLevel.upper())
 
-def main2():
+def main():
     args = setupArgs()
     _configureLogger(args.logLevel.upper())
     createAndDeployStack(args)
 
-def main():
-    print("hello, world 2")
-
-# if __name__ == "__main__":
-#     main()
+if __name__ == "__main__":
+    main()
 
 
 # TODO
 # Get schema registry to work
 # Get the data gen connector to work
```

### Comparing `ce_mkc-0.0.1a1/pyproject.toml` & `ce_mkc-0.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "ce-mkc"
-version = "0.0.1-a1"
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

### Comparing `ce_mkc-0.0.1a1/PKG-INFO` & `ce_mkc-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ce-mkc
-Version: 0.0.1a1
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

