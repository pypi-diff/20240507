# Comparing `tmp/resc_vcs_scraper-3.1.0.tar.gz` & `tmp/resc_vcs_scraper-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_vcs_scraper-3.1.0.tar", last modified: Tue May  7 15:00:10 2024, max compression
+gzip compressed data, was "resc_vcs_scraper-4.0.0.tar", last modified: Mon Apr 22 20:30:35 2024, max compression
```

## Comparing `resc_vcs_scraper-3.1.0.tar` & `resc_vcs_scraper-4.0.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:10.528366 resc_vcs_scraper-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8456 2024-05-07 15:00:10.528366 resc_vcs_scraper-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8061 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-07 15:00:10.528366 resc_vcs_scraper-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:10.520366 resc_vcs_scraper-3.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:10.528366 resc_vcs_scraper-3.1.0/src/resc_vcs_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8456 2024-05-07 15:00:10.000000 resc_vcs_scraper-3.1.0/src/resc_vcs_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-07 15:00:10.000000 resc_vcs_scraper-3.1.0/src/resc_vcs_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 15:00:10.000000 resc_vcs_scraper-3.1.0/src/resc_vcs_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 15:00:10.000000 resc_vcs_scraper-3.1.0/src/resc_vcs_scraper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 15:00:10.000000 resc_vcs_scraper-3.1.0/src/resc_vcs_scraper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-07 15:00:10.000000 resc_vcs_scraper-3.1.0/src/resc_vcs_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 15:00:10.000000 resc_vcs_scraper-3.1.0/src/resc_vcs_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:10.524366 resc_vcs_scraper-3.1.0/src/vcs_scraper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/src/vcs_scraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/src/vcs_scraper/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/src/vcs_scraper/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/src/vcs_scraper/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/src/vcs_scraper/dict_remapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/src/vcs_scraper/environment_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/src/vcs_scraper/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:10.524366 resc_vcs_scraper-3.1.0/src/vcs_scraper/project_collector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/src/vcs_scraper/project_collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/src/vcs_scraper/project_collector/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:10.528366 resc_vcs_scraper-3.1.0/src/vcs_scraper/repository_collector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/src/vcs_scraper/repository_collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/src/vcs_scraper/repository_collector/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:10.528366 resc_vcs_scraper-3.1.0/src/vcs_scraper/static/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/src/vcs_scraper/static/logging.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:10.528366 resc_vcs_scraper-3.1.0/src/vcs_scraper/vcs_connectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/src/vcs_scraper/vcs_connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/src/vcs_scraper/vcs_connectors/azure_devops_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/src/vcs_scraper/vcs_connectors/azure_devops_data_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/src/vcs_scraper/vcs_connectors/bitbucket_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/src/vcs_scraper/vcs_connectors/bitbucket_data_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/src/vcs_scraper/vcs_connectors/github_public_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/src/vcs_scraper/vcs_connectors/vcs_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/src/vcs_scraper/vcs_connectors/vcs_connector_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-07 15:00:06.000000 resc_vcs_scraper-3.1.0/src/vcs_scraper/vcs_instances_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:30:35.580189 resc_vcs_scraper-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8456 2024-04-22 20:30:35.580189 resc_vcs_scraper-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8059 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-22 20:30:35.580189 resc_vcs_scraper-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:30:35.572189 resc_vcs_scraper-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:30:35.580189 resc_vcs_scraper-4.0.0/src/resc_vcs_scraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8456 2024-04-22 20:30:35.000000 resc_vcs_scraper-4.0.0/src/resc_vcs_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-22 20:30:35.000000 resc_vcs_scraper-4.0.0/src/resc_vcs_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 20:30:35.000000 resc_vcs_scraper-4.0.0/src/resc_vcs_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-22 20:30:35.000000 resc_vcs_scraper-4.0.0/src/resc_vcs_scraper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 20:30:35.000000 resc_vcs_scraper-4.0.0/src/resc_vcs_scraper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-22 20:30:35.000000 resc_vcs_scraper-4.0.0/src/resc_vcs_scraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 20:30:35.000000 resc_vcs_scraper-4.0.0/src/resc_vcs_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:30:35.576189 resc_vcs_scraper-4.0.0/src/vcs_scraper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/src/vcs_scraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/src/vcs_scraper/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/src/vcs_scraper/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/src/vcs_scraper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/src/vcs_scraper/dict_remapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/src/vcs_scraper/environment_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/src/vcs_scraper/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:30:35.576189 resc_vcs_scraper-4.0.0/src/vcs_scraper/project_collector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/src/vcs_scraper/project_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/src/vcs_scraper/project_collector/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:30:35.576189 resc_vcs_scraper-4.0.0/src/vcs_scraper/repository_collector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/src/vcs_scraper/repository_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/src/vcs_scraper/repository_collector/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:30:35.576189 resc_vcs_scraper-4.0.0/src/vcs_scraper/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/src/vcs_scraper/static/logging.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:30:35.576189 resc_vcs_scraper-4.0.0/src/vcs_scraper/vcs_connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/src/vcs_scraper/vcs_connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/src/vcs_scraper/vcs_connectors/azure_devops_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/src/vcs_scraper/vcs_connectors/azure_devops_data_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/src/vcs_scraper/vcs_connectors/bitbucket_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/src/vcs_scraper/vcs_connectors/bitbucket_data_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/src/vcs_scraper/vcs_connectors/github_public_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/src/vcs_scraper/vcs_connectors/vcs_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/src/vcs_scraper/vcs_connectors/vcs_connector_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-22 20:30:29.000000 resc_vcs_scraper-4.0.0/src/vcs_scraper/vcs_instances_parser.py
```

### Comparing `resc_vcs_scraper-3.1.0/LICENSE.md` & `resc_vcs_scraper-4.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-3.1.0/PKG-INFO` & `resc_vcs_scraper-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: resc_vcs_scraper
-Version: 3.1.0
+Version: 4.0.0
 Summary: Repository Scanner - Version Control System - Scraper
-Home-page: https://github.com/abnamro/resc-vcs-scraper
+Home-page: https://github.com/ABNAMRO/repository-scanner
 Download-URL: 
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: celery==5.3.1
@@ -48,15 +48,15 @@
 ## Getting started
 
 These instructions will help you to get a copy of the project up and running on your local machine for development and testing purposes.
 
 ### Prerequisites
 - [Git](https://git-scm.com/downloads)
 - [Docker Desktop](https://www.docker.com/products/docker-desktop/)
-- [Python 3.12.0](https://www.python.org/downloads/release/python-3120/)
+- [Python 3.9.0](https://www.python.org/downloads/release/python-390/)
 
 ### Run locally from source
 <details>
   <summary>Preview</summary>
   <b>Prerequisites:</b> RabbitMQ must be up and running locally.</br>
   If you have already deployed RESC through helm in Kubernetes, then rabbitmq is already running for you.</br> 
   Clone the repository, open the Git Bash terminal from /components/resc-vcs-scraper folder, and run below commands.
```

### Comparing `resc_vcs_scraper-3.1.0/README.md` & `resc_vcs_scraper-4.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 ## Getting started
 
 These instructions will help you to get a copy of the project up and running on your local machine for development and testing purposes.
 
 ### Prerequisites
 - [Git](https://git-scm.com/downloads)
 - [Docker Desktop](https://www.docker.com/products/docker-desktop/)
-- [Python 3.12.0](https://www.python.org/downloads/release/python-3120/)
+- [Python 3.9.0](https://www.python.org/downloads/release/python-390/)
 
 ### Run locally from source
 <details>
   <summary>Preview</summary>
   <b>Prerequisites:</b> RabbitMQ must be up and running locally.</br>
   If you have already deployed RESC through helm in Kubernetes, then rabbitmq is already running for you.</br> 
   Clone the repository, open the Git Bash terminal from /components/resc-vcs-scraper folder, and run below commands.
```

### Comparing `resc_vcs_scraper-3.1.0/setup.cfg` & `resc_vcs_scraper-4.0.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = resc_vcs_scraper
 description = Repository Scanner - Version Control System - Scraper
-version = 3.1.0
+version = 4.0.0
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
-url = https://github.com/abnamro/resc-vcs-scraper
+url = https://github.com/ABNAMRO/repository-scanner
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE.md
 requirements_files = file: requirements.txt
 
 [options]
```

### Comparing `resc_vcs_scraper-3.1.0/src/resc_vcs_scraper.egg-info/PKG-INFO` & `resc_vcs_scraper-4.0.0/src/resc_vcs_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: resc_vcs_scraper
-Version: 3.1.0
+Version: 4.0.0
 Summary: Repository Scanner - Version Control System - Scraper
-Home-page: https://github.com/abnamro/resc-vcs-scraper
+Home-page: https://github.com/ABNAMRO/repository-scanner
 Download-URL: 
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: celery==5.3.1
@@ -48,15 +48,15 @@
 ## Getting started
 
 These instructions will help you to get a copy of the project up and running on your local machine for development and testing purposes.
 
 ### Prerequisites
 - [Git](https://git-scm.com/downloads)
 - [Docker Desktop](https://www.docker.com/products/docker-desktop/)
-- [Python 3.12.0](https://www.python.org/downloads/release/python-3120/)
+- [Python 3.9.0](https://www.python.org/downloads/release/python-390/)
 
 ### Run locally from source
 <details>
   <summary>Preview</summary>
   <b>Prerequisites:</b> RabbitMQ must be up and running locally.</br>
   If you have already deployed RESC through helm in Kubernetes, then rabbitmq is already running for you.</br> 
   Clone the repository, open the Git Bash terminal from /components/resc-vcs-scraper folder, and run below commands.
```

### Comparing `resc_vcs_scraper-3.1.0/src/resc_vcs_scraper.egg-info/SOURCES.txt` & `resc_vcs_scraper-4.0.0/src/resc_vcs_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-3.1.0/src/vcs_scraper/common.py` & `resc_vcs_scraper-4.0.0/src/vcs_scraper/common.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-3.1.0/src/vcs_scraper/configuration.py` & `resc_vcs_scraper-4.0.0/src/vcs_scraper/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-3.1.0/src/vcs_scraper/dict_remapper.py` & `resc_vcs_scraper-4.0.0/src/vcs_scraper/dict_remapper.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-3.1.0/src/vcs_scraper/environment_wrapper.py` & `resc_vcs_scraper-4.0.0/src/vcs_scraper/environment_wrapper.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-3.1.0/src/vcs_scraper/model.py` & `resc_vcs_scraper-4.0.0/src/vcs_scraper/model.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-3.1.0/src/vcs_scraper/project_collector/common.py` & `resc_vcs_scraper-4.0.0/src/vcs_scraper/project_collector/common.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-3.1.0/src/vcs_scraper/repository_collector/common.py` & `resc_vcs_scraper-4.0.0/src/vcs_scraper/repository_collector/common.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-3.1.0/src/vcs_scraper/static/logging.ini` & `resc_vcs_scraper-4.0.0/src/vcs_scraper/static/logging.ini`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-3.1.0/src/vcs_scraper/vcs_connectors/azure_devops_connector.py` & `resc_vcs_scraper-4.0.0/src/vcs_scraper/vcs_connectors/azure_devops_connector.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-3.1.0/src/vcs_scraper/vcs_connectors/bitbucket_connector.py` & `resc_vcs_scraper-4.0.0/src/vcs_scraper/vcs_connectors/bitbucket_connector.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-3.1.0/src/vcs_scraper/vcs_connectors/github_public_connector.py` & `resc_vcs_scraper-4.0.0/src/vcs_scraper/vcs_connectors/github_public_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,24 +58,24 @@
 
     def get_repository_details(
         self, project_key: str, repository_name: str
     ) -> GithubRepository:
         repo_details = self.api_client.get_repo(f"{project_key}/{repository_name}")
         return repo_details
 
-    def get_latest_commit(self, project_key: str, repository_id: str) -> str | None:
-        latest_commit: str | None = None
+    def get_latest_commit(self, project_key: str, repository_id: str) -> str:
+        latest_commit = None
         self.api_client.per_page = 1
         commits = self.api_client.get_repo(
             f"{project_key}/{repository_id}"
         ).get_commits()
         if commits:
             latest_commit = commits[0].sha
         self.api_client.per_page = None
-        return latest_commit  
+        return latest_commit  # type: ignore[return-value]
 
     @staticmethod
     def export_repository(
         repository_information: GithubRepository,
         latest_commit: str,
         vcs_instance_name: str,
     ) -> Repository:
```

### Comparing `resc_vcs_scraper-3.1.0/src/vcs_scraper/vcs_connectors/vcs_connector.py` & `resc_vcs_scraper-4.0.0/src/vcs_scraper/vcs_connectors/vcs_connector.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-3.1.0/src/vcs_scraper/vcs_connectors/vcs_connector_factory.py` & `resc_vcs_scraper-4.0.0/src/vcs_scraper/vcs_connectors/vcs_connector_factory.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-3.1.0/src/vcs_scraper/vcs_instances_parser.py` & `resc_vcs_scraper-4.0.0/src/vcs_scraper/vcs_instances_parser.py`

 * *Files identical despite different names*

