# Comparing `tmp/accelbyte-py-sdk-all-0.4.0.tar.gz` & `tmp/accelbyte_py_sdk_all-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-all-0.4.0.tar", last modified: Tue Mar 26 05:45:59 2024, max compression
+gzip compressed data, was "accelbyte_py_sdk_all-0.5.0.tar", last modified: Tue May  7 06:31:33 2024, max compression
```

## Comparing `accelbyte-py-sdk-all-0.4.0.tar` & `accelbyte_py_sdk_all-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:45:59.218433 accelbyte-py-sdk-all-0.4.0/
--rw-r--r--   0 root         (0) root         (0)    43160 2024-03-26 05:45:59.218433 accelbyte-py-sdk-all-0.4.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    41507 2024-03-26 05:45:50.000000 accelbyte-py-sdk-all-0.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:45:59.218433 accelbyte-py-sdk-all-0.4.0/accelbyte_py_sdk_all.egg-info/
--rw-r--r--   0 root         (0) root         (0)    43160 2024-03-26 05:45:59.000000 accelbyte-py-sdk-all-0.4.0/accelbyte_py_sdk_all.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      243 2024-03-26 05:45:59.000000 accelbyte-py-sdk-all-0.4.0/accelbyte_py_sdk_all.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 05:45:59.000000 accelbyte-py-sdk-all-0.4.0/accelbyte_py_sdk_all.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1024 2024-03-26 05:45:59.000000 accelbyte-py-sdk-all-0.4.0/accelbyte_py_sdk_all.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 05:45:59.000000 accelbyte-py-sdk-all-0.4.0/accelbyte_py_sdk_all.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)     1552 2024-03-26 05:39:06.000000 accelbyte-py-sdk-all-0.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-26 05:45:59.218433 accelbyte-py-sdk-all-0.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:31:33.311907 accelbyte_py_sdk_all-0.5.0/
+-rw-r--r--   0 root         (0) root         (0)    43234 2024-05-07 06:31:33.311907 accelbyte_py_sdk_all-0.5.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    41526 2024-05-07 06:31:24.000000 accelbyte_py_sdk_all-0.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:31:33.311907 accelbyte_py_sdk_all-0.5.0/accelbyte_py_sdk_all.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    43234 2024-05-07 06:31:33.000000 accelbyte_py_sdk_all-0.5.0/accelbyte_py_sdk_all.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      243 2024-05-07 06:31:33.000000 accelbyte_py_sdk_all-0.5.0/accelbyte_py_sdk_all.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:31:33.000000 accelbyte_py_sdk_all-0.5.0/accelbyte_py_sdk_all.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1064 2024-05-07 06:31:33.000000 accelbyte_py_sdk_all-0.5.0/accelbyte_py_sdk_all.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:31:33.000000 accelbyte_py_sdk_all-0.5.0/accelbyte_py_sdk_all.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)     1599 2024-05-07 06:24:47.000000 accelbyte_py_sdk_all-0.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 06:31:33.311907 accelbyte_py_sdk_all-0.5.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-all-0.4.0/PKG-INFO` & `accelbyte_py_sdk_all-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-all
-Version: 0.4.0
+Version: 0.5.0
 Summary: AccelByte Python SDK - All
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 Requires-Dist: accelbyte-py-sdk-feat-auth
 Requires-Dist: accelbyte-py-sdk-feat-token-validation
 Requires-Dist: accelbyte-py-sdk-service-achievement
@@ -29,24 +29,25 @@
 Requires-Dist: accelbyte-py-sdk-service-matchmaking
 Requires-Dist: accelbyte-py-sdk-service-platform
 Requires-Dist: accelbyte-py-sdk-service-qosm
 Requires-Dist: accelbyte-py-sdk-service-reporting
 Requires-Dist: accelbyte-py-sdk-service-seasonpass
 Requires-Dist: accelbyte-py-sdk-service-session
 Requires-Dist: accelbyte-py-sdk-service-sessionbrowser
+Requires-Dist: accelbyte-py-sdk-service-sessionhistory
 Requires-Dist: accelbyte-py-sdk-service-social
 Requires-Dist: accelbyte-py-sdk-service-ugc
 
 # AccelByte Modular Python SDK
 
 > :warning: **This [accelbyte-python-modular-sdk](https://github.com/AccelByte/accelbyte-python-modular-sdk) 
 > is not to be confused with [accelbyte-python-sdk](https://github.com/AccelByte/accelbyte-python-sdk):** 
-> * The former (modular SDK) is planned to be the sucessor for the latter (monolithic SDK).
+> * The former (modular SDK) is **experimental** and is planned to be the sucessor for the latter (monolithic SDK).
 > * The modular SDK allows developers to include only the required modules in projects.
-> * If you are starting a new project, you may experiment with modular SDK.
+> * If you are starting a new project, you may try to use modular SDK.
 > * If you use monolithic SDK in an existing project, a migration path is available via compatibility layer in modular SDK.
 > * Both monolithic and modular SDK will be maintained for some time to give time for migration until monolithic SDK is deprecated in the future.
 
 A software development kit (SDK) for interacting with AccelByte Gaming Services (AGS) written in Python.
 
 This SDK was generated from AGS OpenAPI spec files included in the [spec](spec) directory.
```

### Comparing `accelbyte-py-sdk-all-0.4.0/README.md` & `accelbyte_py_sdk_all-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # AccelByte Modular Python SDK
 
 > :warning: **This [accelbyte-python-modular-sdk](https://github.com/AccelByte/accelbyte-python-modular-sdk) 
 > is not to be confused with [accelbyte-python-sdk](https://github.com/AccelByte/accelbyte-python-sdk):** 
-> * The former (modular SDK) is planned to be the sucessor for the latter (monolithic SDK).
+> * The former (modular SDK) is **experimental** and is planned to be the sucessor for the latter (monolithic SDK).
 > * The modular SDK allows developers to include only the required modules in projects.
-> * If you are starting a new project, you may experiment with modular SDK.
+> * If you are starting a new project, you may try to use modular SDK.
 > * If you use monolithic SDK in an existing project, a migration path is available via compatibility layer in modular SDK.
 > * Both monolithic and modular SDK will be maintained for some time to give time for migration until monolithic SDK is deprecated in the future.
 
 A software development kit (SDK) for interacting with AccelByte Gaming Services (AGS) written in Python.
 
 This SDK was generated from AGS OpenAPI spec files included in the [spec](spec) directory.
```

### Comparing `accelbyte-py-sdk-all-0.4.0/accelbyte_py_sdk_all.egg-info/PKG-INFO` & `accelbyte_py_sdk_all-0.5.0/accelbyte_py_sdk_all.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-all
-Version: 0.4.0
+Version: 0.5.0
 Summary: AccelByte Python SDK - All
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 Requires-Dist: accelbyte-py-sdk-feat-auth
 Requires-Dist: accelbyte-py-sdk-feat-token-validation
 Requires-Dist: accelbyte-py-sdk-service-achievement
@@ -29,24 +29,25 @@
 Requires-Dist: accelbyte-py-sdk-service-matchmaking
 Requires-Dist: accelbyte-py-sdk-service-platform
 Requires-Dist: accelbyte-py-sdk-service-qosm
 Requires-Dist: accelbyte-py-sdk-service-reporting
 Requires-Dist: accelbyte-py-sdk-service-seasonpass
 Requires-Dist: accelbyte-py-sdk-service-session
 Requires-Dist: accelbyte-py-sdk-service-sessionbrowser
+Requires-Dist: accelbyte-py-sdk-service-sessionhistory
 Requires-Dist: accelbyte-py-sdk-service-social
 Requires-Dist: accelbyte-py-sdk-service-ugc
 
 # AccelByte Modular Python SDK
 
 > :warning: **This [accelbyte-python-modular-sdk](https://github.com/AccelByte/accelbyte-python-modular-sdk) 
 > is not to be confused with [accelbyte-python-sdk](https://github.com/AccelByte/accelbyte-python-sdk):** 
-> * The former (modular SDK) is planned to be the sucessor for the latter (monolithic SDK).
+> * The former (modular SDK) is **experimental** and is planned to be the sucessor for the latter (monolithic SDK).
 > * The modular SDK allows developers to include only the required modules in projects.
-> * If you are starting a new project, you may experiment with modular SDK.
+> * If you are starting a new project, you may try to use modular SDK.
 > * If you use monolithic SDK in an existing project, a migration path is available via compatibility layer in modular SDK.
 > * Both monolithic and modular SDK will be maintained for some time to give time for migration until monolithic SDK is deprecated in the future.
 
 A software development kit (SDK) for interacting with AccelByte Gaming Services (AGS) written in Python.
 
 This SDK was generated from AGS OpenAPI spec files included in the [spec](spec) directory.
```

### Comparing `accelbyte-py-sdk-all-0.4.0/accelbyte_py_sdk_all.egg-info/requires.txt` & `accelbyte_py_sdk_all-0.5.0/accelbyte_py_sdk_all.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,9 +23,10 @@
 accelbyte-py-sdk-service-matchmaking
 accelbyte-py-sdk-service-platform
 accelbyte-py-sdk-service-qosm
 accelbyte-py-sdk-service-reporting
 accelbyte-py-sdk-service-seasonpass
 accelbyte-py-sdk-service-session
 accelbyte-py-sdk-service-sessionbrowser
+accelbyte-py-sdk-service-sessionhistory
 accelbyte-py-sdk-service-social
 accelbyte-py-sdk-service-ugc
```

### Comparing `accelbyte-py-sdk-all-0.4.0/pyproject.toml` & `accelbyte_py_sdk_all-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "accelbyte-py-sdk-all"
 readme = "README.md"
-version = "0.4.0"
+version = "0.5.0"
 description = "AccelByte Python SDK - All"
 requires-python = ">=3.9"
 dependencies = [
     "accelbyte-py-sdk-core",
     # Features
     "accelbyte-py-sdk-feat-auth",
     "accelbyte-py-sdk-feat-token-validation",
@@ -38,10 +38,11 @@
     "accelbyte-py-sdk-service-matchmaking",
     "accelbyte-py-sdk-service-platform",
     "accelbyte-py-sdk-service-qosm",
     "accelbyte-py-sdk-service-reporting",
     "accelbyte-py-sdk-service-seasonpass",
     "accelbyte-py-sdk-service-session",
     "accelbyte-py-sdk-service-sessionbrowser",
+    "accelbyte-py-sdk-service-sessionhistory",
     "accelbyte-py-sdk-service-social",
     "accelbyte-py-sdk-service-ugc",
 ]
```

