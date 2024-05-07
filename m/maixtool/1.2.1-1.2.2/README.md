# Comparing `tmp/maixtool-1.2.1.tar.gz` & `tmp/maixtool-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maixtool-1.2.1.tar", last modified: Fri Mar 15 11:20:23 2024, max compression
+gzip compressed data, was "maixtool-1.2.2.tar", last modified: Tue May  7 07:20:29 2024, max compression
```

## Comparing `maixtool-1.2.1.tar` & `maixtool-1.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2024-03-15 11:20:23.792528 maixtool-1.2.1/
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      577 2023-12-19 08:02:52.000000 maixtool-1.2.1/LICENSE
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      831 2024-03-15 11:20:23.792528 maixtool-1.2.1/PKG-INFO
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      135 2023-12-19 08:02:52.000000 maixtool-1.2.1/README.md
-drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2024-03-15 11:20:23.792528 maixtool-1.2.1/maixtool/
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)       32 2023-12-19 08:02:52.000000 maixtool-1.2.1/maixtool/__init__.py
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      202 2023-12-19 08:02:52.000000 maixtool-1.2.1/maixtool/__main__.py
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)     2797 2024-03-15 10:11:37.000000 maixtool-1.2.1/maixtool/app_deploy.py
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)     6420 2024-02-22 11:20:00.000000 maixtool-1.2.1/maixtool/app_release.py
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)     1383 2023-12-20 13:44:38.000000 maixtool-1.2.1/maixtool/maixcdk.py
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      784 2023-12-19 08:02:52.000000 maixtool-1.2.1/maixtool/maixtool.py
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)       25 2024-03-15 10:13:16.000000 maixtool-1.2.1/maixtool/version.py
-drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2024-03-15 11:20:23.792528 maixtool-1.2.1/maixtool.egg-info/
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      831 2024-03-15 11:20:23.000000 maixtool-1.2.1/maixtool.egg-info/PKG-INFO
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      370 2024-03-15 11:20:23.000000 maixtool-1.2.1/maixtool.egg-info/SOURCES.txt
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)        1 2024-03-15 11:20:23.000000 maixtool-1.2.1/maixtool.egg-info/dependency_links.txt
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)       94 2024-03-15 11:20:23.000000 maixtool-1.2.1/maixtool.egg-info/entry_points.txt
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)       37 2024-03-15 11:20:23.000000 maixtool-1.2.1/maixtool.egg-info/requires.txt
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)        9 2024-03-15 11:20:23.000000 maixtool-1.2.1/maixtool.egg-info/top_level.txt
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)       38 2024-03-15 11:20:23.792528 maixtool-1.2.1/setup.cfg
--rw-rw-r--   0 neucrack  (1000) neucrack  (1000)     4198 2023-12-19 08:02:52.000000 maixtool-1.2.1/setup.py
+drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2024-05-07 07:20:29.262474 maixtool-1.2.2/
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      577 2023-12-19 08:02:52.000000 maixtool-1.2.2/LICENSE
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      831 2024-05-07 07:20:29.262474 maixtool-1.2.2/PKG-INFO
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      135 2023-12-19 08:02:52.000000 maixtool-1.2.2/README.md
+drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2024-05-07 07:20:29.262474 maixtool-1.2.2/maixtool/
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)       32 2023-12-19 08:02:52.000000 maixtool-1.2.2/maixtool/__init__.py
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      202 2023-12-19 08:02:52.000000 maixtool-1.2.2/maixtool/__main__.py
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)     2797 2024-03-15 11:20:42.000000 maixtool-1.2.2/maixtool/app_deploy.py
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)     6420 2024-02-22 11:20:00.000000 maixtool-1.2.2/maixtool/app_release.py
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)     1498 2024-05-07 07:20:10.000000 maixtool-1.2.2/maixtool/maixcdk.py
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      784 2023-12-19 08:02:52.000000 maixtool-1.2.2/maixtool/maixtool.py
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)       25 2024-05-07 07:20:16.000000 maixtool-1.2.2/maixtool/version.py
+drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2024-05-07 07:20:29.262474 maixtool-1.2.2/maixtool.egg-info/
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      831 2024-05-07 07:20:29.000000 maixtool-1.2.2/maixtool.egg-info/PKG-INFO
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)      370 2024-05-07 07:20:29.000000 maixtool-1.2.2/maixtool.egg-info/SOURCES.txt
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)        1 2024-05-07 07:20:29.000000 maixtool-1.2.2/maixtool.egg-info/dependency_links.txt
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)       94 2024-05-07 07:20:29.000000 maixtool-1.2.2/maixtool.egg-info/entry_points.txt
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)       37 2024-05-07 07:20:29.000000 maixtool-1.2.2/maixtool.egg-info/requires.txt
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)        9 2024-05-07 07:20:29.000000 maixtool-1.2.2/maixtool.egg-info/top_level.txt
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)       38 2024-05-07 07:20:29.262474 maixtool-1.2.2/setup.cfg
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)     4198 2023-12-19 08:02:52.000000 maixtool-1.2.2/setup.py
```

### Comparing `maixtool-1.2.1/LICENSE` & `maixtool-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `maixtool-1.2.1/PKG-INFO` & `maixtool-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maixtool
-Version: 1.2.1
+Version: 1.2.2
 Summary: Tools for Maix series development
 Home-page: https://github.com/Sipeed/MaixCDK
 Author: Sipeed
 Author-email: support@sipeed.com
 License: Apache 2.0
 Keywords: Maix MaixCDK MaixPy maixtool
 Platform: UNKNOWN
```

### Comparing `maixtool-1.2.1/maixtool/app_deploy.py` & `maixtool-1.2.2/maixtool/app_deploy.py`

 * *Files identical despite different names*

### Comparing `maixtool-1.2.1/maixtool/app_release.py` & `maixtool-1.2.2/maixtool/app_release.py`

 * *Files identical despite different names*

### Comparing `maixtool-1.2.1/maixtool/maixcdk.py` & `maixtool-1.2.2/maixtool/maixcdk.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,28 +11,33 @@
 
 def get_sdk_path():
     sdk_path = None
     sdk_env_name = "MAIXCDK_PATH"
 
     # 1. get SDK absolute path from MAIXCDK_PATH env
     try:
-        if os.environ[sdk_env_name] and os.path.exists(os.environ[sdk_env_name]):
+        if os.environ[sdk_env_name]:
             sdk_path = os.environ[sdk_env_name]
     except Exception:
         pass
 
     # 2. check if in MaixCDK repo, higher priority
     path = os.path.abspath("../../")
     if os.path.exists(path+"/tools/cmake/project.py"):
         sdk_path = path
 
     # 3. check if MaixCDK path valid
-    if not sdk_path or not os.path.exists(sdk_path):
+    if not sdk_path:
         print("")
-        print("Error: can not find MaixCDK, please set MAIXCDK_PATH env to MaixCDK directory")
+        print("Error: can not find MaixCDK, please set MAIXCDK_PATH env to MaixCDK directory by `export MAIXCDK_PATH=xxxxx`")
+        print("")
+        sys.exit(1)
+    if not os.path.exists(sdk_path):
+        print("")
+        print(f"Error: MaixCDK set to {sdk_path}, but not exists!")
         print("")
         sys.exit(1)
     return os.path.abspath(sdk_path)
 
 def exec_project_py():
     # 1. get MaixCDK path
     sdk_path = get_sdk_path()
```

### Comparing `maixtool-1.2.1/maixtool/maixtool.py` & `maixtool-1.2.2/maixtool/maixtool.py`

 * *Files identical despite different names*

### Comparing `maixtool-1.2.1/maixtool.egg-info/PKG-INFO` & `maixtool-1.2.2/maixtool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maixtool
-Version: 1.2.1
+Version: 1.2.2
 Summary: Tools for Maix series development
 Home-page: https://github.com/Sipeed/MaixCDK
 Author: Sipeed
 Author-email: support@sipeed.com
 License: Apache 2.0
 Keywords: Maix MaixCDK MaixPy maixtool
 Platform: UNKNOWN
```

### Comparing `maixtool-1.2.1/setup.py` & `maixtool-1.2.2/setup.py`

 * *Files identical despite different names*

