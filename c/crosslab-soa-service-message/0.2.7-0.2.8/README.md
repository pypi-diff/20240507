# Comparing `tmp/crosslab_soa_service_message-0.2.7.tar.gz` & `tmp/crosslab_soa_service_message-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_soa_service_message-0.2.7.tar", last modified: Fri Apr  5 09:17:53 2024, max compression
+gzip compressed data, was "crosslab_soa_service_message-0.2.8.tar", last modified: Tue May  7 16:59:50 2024, max compression
```

## Comparing `crosslab_soa_service_message-0.2.7.tar` & `crosslab_soa_service_message-0.2.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:53.146779 crosslab_soa_service_message-0.2.7/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      405 2024-04-05 09:17:53.146779 crosslab_soa_service_message-0.2.7/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-11-08 12:05:41.000000 crosslab_soa_service_message-0.2.7/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)      580 2024-04-05 09:17:53.146779 crosslab_soa_service_message-0.2.7/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)       37 2023-11-08 12:05:41.000000 crosslab_soa_service_message-0.2.7/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:53.146779 crosslab_soa_service_message-0.2.7/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:53.146779 crosslab_soa_service_message-0.2.7/src/crosslab/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:53.146779 crosslab_soa_service_message-0.2.7/src/crosslab/soa_services/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:53.146779 crosslab_soa_service_message-0.2.7/src/crosslab/soa_services/message/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      213 2023-11-08 12:05:41.000000 crosslab_soa_service_message-0.2.7/src/crosslab/soa_services/message/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2618 2023-11-08 12:05:41.000000 crosslab_soa_service_message-0.2.7/src/crosslab/soa_services/message/message_service.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      232 2023-11-08 12:05:41.000000 crosslab_soa_service_message-0.2.7/src/crosslab/soa_services/message/messages.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:41.000000 crosslab_soa_service_message-0.2.7/src/crosslab/soa_services/message/py.typed
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:53.146779 crosslab_soa_service_message-0.2.7/src/crosslab_soa_service_message.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      405 2024-04-05 09:17:53.000000 crosslab_soa_service_message-0.2.7/src/crosslab_soa_service_message.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      523 2024-04-05 09:17:53.000000 crosslab_soa_service_message-0.2.7/src/crosslab_soa_service_message.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-04-05 09:17:53.000000 crosslab_soa_service_message-0.2.7/src/crosslab_soa_service_message.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       25 2024-04-05 09:17:53.000000 crosslab_soa_service_message-0.2.7/src/crosslab_soa_service_message.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2024-04-05 09:17:53.000000 crosslab_soa_service_message-0.2.7/src/crosslab_soa_service_message.egg-info/top_level.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:53.146779 crosslab_soa_service_message-0.2.7/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      916 2023-11-08 12:05:41.000000 crosslab_soa_service_message-0.2.7/tests/test_standard.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 16:59:50.368217 crosslab_soa_service_message-0.2.8/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      405 2024-05-07 16:59:50.368217 crosslab_soa_service_message-0.2.8/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-11-08 12:05:41.000000 crosslab_soa_service_message-0.2.8/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      580 2024-05-07 16:59:50.368217 crosslab_soa_service_message-0.2.8/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       37 2023-11-08 12:05:41.000000 crosslab_soa_service_message-0.2.8/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 16:59:50.368217 crosslab_soa_service_message-0.2.8/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 16:59:50.368217 crosslab_soa_service_message-0.2.8/src/crosslab/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 16:59:50.368217 crosslab_soa_service_message-0.2.8/src/crosslab/soa_services/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 16:59:50.368217 crosslab_soa_service_message-0.2.8/src/crosslab/soa_services/message/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      213 2023-11-08 12:05:41.000000 crosslab_soa_service_message-0.2.8/src/crosslab/soa_services/message/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2618 2023-11-08 12:05:41.000000 crosslab_soa_service_message-0.2.8/src/crosslab/soa_services/message/message_service.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      232 2023-11-08 12:05:41.000000 crosslab_soa_service_message-0.2.8/src/crosslab/soa_services/message/messages.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:41.000000 crosslab_soa_service_message-0.2.8/src/crosslab/soa_services/message/py.typed
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 16:59:50.368217 crosslab_soa_service_message-0.2.8/src/crosslab_soa_service_message.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      405 2024-05-07 16:59:50.000000 crosslab_soa_service_message-0.2.8/src/crosslab_soa_service_message.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      523 2024-05-07 16:59:50.000000 crosslab_soa_service_message-0.2.8/src/crosslab_soa_service_message.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-05-07 16:59:50.000000 crosslab_soa_service_message-0.2.8/src/crosslab_soa_service_message.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       25 2024-05-07 16:59:50.000000 crosslab_soa_service_message-0.2.8/src/crosslab_soa_service_message.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2024-05-07 16:59:50.000000 crosslab_soa_service_message-0.2.8/src/crosslab_soa_service_message.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 16:59:50.368217 crosslab_soa_service_message-0.2.8/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      916 2023-11-08 12:05:41.000000 crosslab_soa_service_message-0.2.8/tests/test_standard.py
```

### Comparing `crosslab_soa_service_message-0.2.7/setup.cfg` & `crosslab_soa_service_message-0.2.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_soa_service_message
-version = 0.2.7
+version = 0.2.8
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab SOA message Service.
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
 	Operating System :: OS Independent
```

### Comparing `crosslab_soa_service_message-0.2.7/src/crosslab/soa_services/message/message_service.py` & `crosslab_soa_service_message-0.2.8/src/crosslab/soa_services/message/message_service.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_message-0.2.7/src/crosslab_soa_service_message.egg-info/SOURCES.txt` & `crosslab_soa_service_message-0.2.8/src/crosslab_soa_service_message.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_message-0.2.7/tests/test_standard.py` & `crosslab_soa_service_message-0.2.8/tests/test_standard.py`

 * *Files identical despite different names*

