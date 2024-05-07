# Comparing `tmp/ce_mkc-0.0.1a3.tar.gz` & `tmp/ce_mkc-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ce_mkc-0.0.1a3.tar", max compression
+gzip compressed data, was "ce_mkc-0.1.0.tar", max compression
```

## Comparing `ce_mkc-0.0.1a3.tar` & `ce_mkc-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,4 @@
--rw-r--r--   0        0        0    15263 2024-03-20 07:03:50.879186 ce_mkc-0.0.1a3/README.md
--rw-r--r--   0        0        0       31 2024-05-07 16:27:58.758864 ce_mkc-0.0.1a3/ce_mkc/__init__.py
--rw-r--r--   0        0        0      157 2024-05-07 16:29:20.775519 ce_mkc-0.0.1a3/ce_mkc/__main__.py
--rw-r--r--   0        0        0        0 2024-05-07 16:26:36.738532 ce_mkc-0.0.1a3/ce_mkc/main2/__init__.py
--rw-r--r--   0        0        0      157 2024-05-07 16:26:44.302520 ce_mkc-0.0.1a3/ce_mkc/main2/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    24249 2024-05-07 16:32:25.241250 ce_mkc-0.0.1a3/ce_mkc/main2/ce_mkc.py
--rw-r--r--   0        0        0        0 2024-05-07 15:13:57.333707 ce_mkc-0.0.1a3/ce_mkc/templates/__init__.py
--rw-r--r--   0        0        0      547 2024-03-20 07:03:50.886613 ce_mkc-0.0.1a3/ce_mkc/templates/akhq/akhq.template
--rw-r--r--   0        0        0     5286 2024-03-20 07:03:50.886893 ce_mkc-0.0.1a3/ce_mkc/templates/docker-compose.template
--rw-r--r--   0        0        0     4397 2024-03-20 07:03:50.887211 ce_mkc-0.0.1a3/ce_mkc/templates/docker-compose.template.reference
--rw-r--r--   0        0        0     1803 2024-03-20 07:03:50.887704 ce_mkc-0.0.1a3/ce_mkc/templates/kafka/kafka.template
--rw-r--r--   0        0        0      313 2024-03-20 07:03:50.888064 ce_mkc-0.0.1a3/ce_mkc/templates/kafka/zookeeper.template
--rw-r--r--   0        0        0     2251 2024-03-20 07:03:50.888532 ce_mkc-0.0.1a3/ce_mkc/templates/kafkaconnect/kafkaconnect.template
--rw-r--r--   0        0        0      112 2024-03-20 07:03:50.888816 ce_mkc-0.0.1a3/ce_mkc/templates/mongod/mongod.conf.template
--rw-r--r--   0        0        0      372 2024-03-20 07:03:50.889009 ce_mkc-0.0.1a3/ce_mkc/templates/mongod/mongod.template
--rw-r--r--   0        0        0      335 2024-03-20 07:03:50.889354 ce_mkc-0.0.1a3/ce_mkc/templates/schemaregistry/schemaregistry.template
--rw-r--r--   0        0        0      597 2024-05-07 10:52:34.993340 ce_mkc-0.0.1a3/pyproject.toml
--rw-r--r--   0        0        0    16090 1970-01-01 00:00:00.000000 ce_mkc-0.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0    15263 2024-03-20 07:03:50.879186 ce_mkc-0.1.0/README.md
+-rw-r--r--   0        0        0    24186 2024-03-20 07:03:50.886024 ce_mkc-0.1.0/ce_mkc.py
+-rw-r--r--   0        0        0      595 2024-05-06 13:09:49.902413 ce_mkc-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    16090 1970-01-01 00:00:00.000000 ce_mkc-0.1.0/PKG-INFO
```

### Comparing `ce_mkc-0.0.1a3/README.md` & `ce_mkc-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ce_mkc-0.0.1a3/ce_mkc/main2/ce_mkc.py` & `ce_mkc-0.1.0/ce_mkc.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,14 @@
 import time
 from pymongo import MongoClient
 from zipfile import ZipFile
 
 import docker
 import requests
 
-#import templates
-from importlib import resources as impresources
-import templates
-
 ########################################################################################################################
 # Constants
 ########################################################################################################################
 
 DEFAULT_CONFIG_DATA = {
         "zookeeperVersion" : "6.2.0",
         "kafkaVersion" : "6.2.0",
@@ -42,23 +38,20 @@
 CONTAINERS = [
     KAFKA_CONNECT_CONTAINER_NAME,
     SCHEMA_REGISTRY_CONTAINER_NAME,
     KAFKA_BROKER_CONTAINER_NAME,
     ZOOKEEPER_CONTAINER_NAME
 ]
 
-CONTAINER_TEMPLATE_PATH_AKHQ = "akhq/akhq.template"
-CONTAINER_TEMPLATE_PATH_KAFKA = "kafka/kafka.template"
-CONTAINER_TEMPLATE_PATH_ZOOKEEPER = "kafka/zookeeper.template"
-CONTAINER_TEMPLATE_PATH_MONGOD = "mongod/mongod.template"
-CONTAINER_TEMPLATE_PATH_KAFKA_CONNECT = "kafkaconnect/kafkaconnect.template"
-CONTAINER_TEMPLATE_PATH_SCHEMA_REGISTRY = "schemaregistry/schemaregistry.template"
-
-DOCKER_COMPOSE_TEMPLATE_PATH = "docker-compose.template"
-MONGODB_CONF_TEMPLATE_PATH = "mongod/mongod.conf.template"
+CONTAINER_TEMPLATE_PATH_AKHQ = "templates/akhq/akhq.template"
+CONTAINER_TEMPLATE_PATH_KAFKA = "templates/kafka/kafka.template"
+CONTAINER_TEMPLATE_PATH_ZOOKEEPER = "templates/kafka/zookeeper.template"
+CONTAINER_TEMPLATE_PATH_MONGOD = "templates/mongod/mongod.template"
+CONTAINER_TEMPLATE_PATH_KAFKA_CONNECT = "templates/kafkaconnect/kafkaconnect.template"
+CONTAINER_TEMPLATE_PATH_SCHEMA_REGISTRY = "templates/schemaregistry/schemaregistry.template"
 
 
 CONNECTOR_DOWNLOADS_PATH = "connector-downloads"
 MDB_KAFKA_CONNECTOR_VERSIONS = [
     "0.1",
     "0.2",
     "1.0.0",
@@ -112,29 +105,34 @@
     },
     "confluent-datagen-connector" : {
         "downloadURL" : "https://d1i4a15mxbxib1.cloudfront.net/api/plugins/confluentinc/kafka-connect-datagen/versions/{version}/confluentinc-kafka-connect-datagen-{version}.zip",
         "versions" : CONFLUENT_DATAGEN_CONNECTORS_VERSIONS
     }
 }
 
+
+DOCKER_COMPOSE_TEMPLATE_PATH = "templates/docker-compose.template"
+MONGODB_CONF_TEMPLATE_PATH = "templates/mongod/mongod.conf.template"
+
 MONGODB_CONN_STR = "localhost:27017"
 KAFKA_CONNECT_CONFIG_URL = "http://localhost:8083"
 SCHEMA_REGISTRY_CONFIG_URL = "http://localhost:8081"
 
 ########################################################################################################################
 # Helper Methods
 ########################################################################################################################
 
 def createMongoDBConfFromTemplate(config):
     """
     Create MongoDB Conf From Template
 
     :return:
     """
-    templateData = readTemplate(MONGODB_CONF_TEMPLATE_PATH)
+    with open(MONGODB_CONF_TEMPLATE_PATH, 'r') as f:
+        templateData = f.read()
 
     mongodbConfFile = templateData.format()
     logging.debug("Created docker-compose file data {}".format(mongodbConfFile))
 
     return mongodbConfFile
 
 def downloadConnectorJar(connectorName, downloadUrl, connectorVersion="latest", forceDownload=False):
@@ -224,16 +222,15 @@
 
 def readTemplate(templatePath):
     """
     Read Template
     :param templatePath:
     :return:
     """
-    inp_file = impresources.files(templates) / templatePath
-    with inp_file.open("rt") as f:
+    with open(templatePath, 'r') as f:
         templateData = f.read()
     return templateData
 
 
 def parseConfigFile(configFile, launchFullStack=False):
     """
     Parse Config File
@@ -645,20 +642,18 @@
 def _configureLogger(logLevel):
     format = '%(message)s'
     if logLevel != 'INFO':
         format = '%(levelname)s: %(message)s'
     logging.basicConfig(format=format, level=logLevel.upper())
 
 def main():
-    print(__name__)
-    
     args = setupArgs()
     _configureLogger(args.logLevel.upper())
     createAndDeployStack(args)
 
-# if __name__ == "__main__":
-#     main()
+if __name__ == "__main__":
+    main()
 
 
 # TODO
 # Get schema registry to work
 # Get the data gen connector to work
```

### Comparing `ce_mkc-0.0.1a3/pyproject.toml` & `ce_mkc-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "ce-mkc"
-version = "0.0.1-a3"
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

### Comparing `ce_mkc-0.0.1a3/PKG-INFO` & `ce_mkc-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ce-mkc
-Version: 0.0.1a3
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

