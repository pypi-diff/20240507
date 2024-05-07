# Comparing `tmp/bk-notice-sdk-1.3.1.tar.gz` & `tmp/bk-notice-sdk-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bk-notice-sdk-1.3.1.tar", last modified: Mon Mar 11 08:48:11 2024, max compression
+gzip compressed data, was "dist/bk-notice-sdk-1.3.2.tar", last modified: Tue May  7 03:37:24 2024, max compression
```

## Comparing `bk-notice-sdk-1.3.1.tar` & `bk-notice-sdk-1.3.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:48:11.000000 bk-notice-sdk-1.3.1/
--rw-r--r--   0 root         (0) root         (0)     1069 2024-03-11 08:44:57.000000 bk-notice-sdk-1.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       31 2024-03-11 08:44:57.000000 bk-notice-sdk-1.3.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     3425 2024-03-11 08:48:11.000000 bk-notice-sdk-1.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      130 2024-03-11 08:44:57.000000 bk-notice-sdk-1.3.1/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:48:11.000000 bk-notice-sdk-1.3.1/bk_notice_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)       20 2024-03-11 08:48:11.000000 bk-notice-sdk-1.3.1/bk_notice_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-11 08:48:11.000000 bk-notice-sdk-1.3.1/bk_notice_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     3425 2024-03-11 08:48:11.000000 bk-notice-sdk-1.3.1/bk_notice_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       32 2024-03-11 08:48:11.000000 bk-notice-sdk-1.3.1/bk_notice_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      621 2024-03-11 08:48:11.000000 bk-notice-sdk-1.3.1/bk_notice_sdk.egg-info/SOURCES.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:48:11.000000 bk-notice-sdk-1.3.1/bk_notice_sdk/
--rw-r--r--   0 root         (0) root         (0)     1606 2024-03-11 08:44:57.000000 bk-notice-sdk-1.3.1/bk_notice_sdk/views.py
--rw-r--r--   0 root         (0) root         (0)      166 2024-03-11 08:44:57.000000 bk-notice-sdk-1.3.1/bk_notice_sdk/urls.py
--rw-r--r--   0 root         (0) root         (0)      872 2024-03-11 08:44:57.000000 bk-notice-sdk-1.3.1/bk_notice_sdk/apps.py
--rw-r--r--   0 root         (0) root         (0)     2935 2024-03-11 08:44:57.000000 bk-notice-sdk-1.3.1/bk_notice_sdk/utils.py
--rw-r--r--   0 root         (0) root         (0)     1447 2024-03-11 08:44:57.000000 bk-notice-sdk-1.3.1/bk_notice_sdk/config.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-11 08:44:57.000000 bk-notice-sdk-1.3.1/bk_notice_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:48:11.000000 bk-notice-sdk-1.3.1/bk_notice_sdk/management/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-11 08:44:57.000000 bk-notice-sdk-1.3.1/bk_notice_sdk/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:48:11.000000 bk-notice-sdk-1.3.1/bk_notice_sdk/management/commands/
--rw-r--r--   0 root         (0) root         (0)     1592 2024-03-11 08:44:57.000000 bk-notice-sdk-1.3.1/bk_notice_sdk/management/commands/register_application.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-11 08:44:57.000000 bk-notice-sdk-1.3.1/bk_notice_sdk/management/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:48:11.000000 bk-notice-sdk-1.3.1/bkapi/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-11 08:44:57.000000 bk-notice-sdk-1.3.1/bkapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 08:48:11.000000 bk-notice-sdk-1.3.1/bkapi/bk_notice/
--rw-r--r--   0 root         (0) root         (0)      467 2024-03-11 08:44:57.000000 bk-notice-sdk-1.3.1/bkapi/bk_notice/shortcuts.py
--rw-r--r--   0 root         (0) root         (0)       61 2024-03-11 08:44:57.000000 bk-notice-sdk-1.3.1/bkapi/bk_notice/__init__.py
--rw-r--r--   0 root         (0) root         (0)      852 2024-03-11 08:44:57.000000 bk-notice-sdk-1.3.1/bkapi/bk_notice/client.py
--rw-r--r--   0 root         (0) root         (0)     2541 2024-03-11 08:44:57.000000 bk-notice-sdk-1.3.1/README.md
--rw-r--r--   0 root         (0) root         (0)      902 2024-03-11 08:44:57.000000 bk-notice-sdk-1.3.1/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-11 08:48:11.000000 bk-notice-sdk-1.3.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:37:24.000000 bk-notice-sdk-1.3.2/
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 03:37:24.000000 bk-notice-sdk-1.3.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:37:24.000000 bk-notice-sdk-1.3.2/bk_notice_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       32 2024-05-07 03:37:24.000000 bk-notice-sdk-1.3.2/bk_notice_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      621 2024-05-07 03:37:24.000000 bk-notice-sdk-1.3.2/bk_notice_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-07 03:37:24.000000 bk-notice-sdk-1.3.2/bk_notice_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3425 2024-05-07 03:37:24.000000 bk-notice-sdk-1.3.2/bk_notice_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 03:37:24.000000 bk-notice-sdk-1.3.2/bk_notice_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-07 03:35:09.000000 bk-notice-sdk-1.3.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     2541 2024-05-07 03:35:09.000000 bk-notice-sdk-1.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:37:24.000000 bk-notice-sdk-1.3.2/bkapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:35:09.000000 bk-notice-sdk-1.3.2/bkapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:37:24.000000 bk-notice-sdk-1.3.2/bkapi/bk_notice/
+-rw-r--r--   0 root         (0) root         (0)      467 2024-05-07 03:35:09.000000 bk-notice-sdk-1.3.2/bkapi/bk_notice/shortcuts.py
+-rw-r--r--   0 root         (0) root         (0)       61 2024-05-07 03:35:09.000000 bk-notice-sdk-1.3.2/bkapi/bk_notice/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      852 2024-05-07 03:35:09.000000 bk-notice-sdk-1.3.2/bkapi/bk_notice/client.py
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-05-07 03:35:09.000000 bk-notice-sdk-1.3.2/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:37:24.000000 bk-notice-sdk-1.3.2/bk_notice_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:37:24.000000 bk-notice-sdk-1.3.2/bk_notice_sdk/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:37:24.000000 bk-notice-sdk-1.3.2/bk_notice_sdk/management/commands/
+-rw-r--r--   0 root         (0) root         (0)     1592 2024-05-07 03:35:09.000000 bk-notice-sdk-1.3.2/bk_notice_sdk/management/commands/register_application.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:35:09.000000 bk-notice-sdk-1.3.2/bk_notice_sdk/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:35:09.000000 bk-notice-sdk-1.3.2/bk_notice_sdk/management/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      794 2024-05-07 03:35:09.000000 bk-notice-sdk-1.3.2/bk_notice_sdk/views.py
+-rw-r--r--   0 root         (0) root         (0)     2935 2024-05-07 03:35:09.000000 bk-notice-sdk-1.3.2/bk_notice_sdk/utils.py
+-rw-r--r--   0 root         (0) root         (0)      872 2024-05-07 03:35:09.000000 bk-notice-sdk-1.3.2/bk_notice_sdk/apps.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2024-05-07 03:35:09.000000 bk-notice-sdk-1.3.2/bk_notice_sdk/config.py
+-rw-r--r--   0 root         (0) root         (0)      169 2024-05-07 03:35:09.000000 bk-notice-sdk-1.3.2/bk_notice_sdk/urls.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:35:09.000000 bk-notice-sdk-1.3.2/bk_notice_sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      130 2024-05-07 03:35:09.000000 bk-notice-sdk-1.3.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3425 2024-05-07 03:37:24.000000 bk-notice-sdk-1.3.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      902 2024-05-07 03:35:09.000000 bk-notice-sdk-1.3.2/setup.py
```

### Comparing `bk-notice-sdk-1.3.1/LICENSE` & `bk-notice-sdk-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bk-notice-sdk-1.3.1/PKG-INFO` & `bk-notice-sdk-1.3.2/bk_notice_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bk-notice-sdk
-Version: 1.3.1
+Version: 1.3.2
 Summary: A project for fetching and displaying announcement notifications.
 Home-page: UNKNOWN
 Author: blueking
 Author-email: blueking@tencent.com
 License: UNKNOWN
 Description: # bk-notice-sdk
```

### Comparing `bk-notice-sdk-1.3.1/bk_notice_sdk.egg-info/PKG-INFO` & `bk-notice-sdk-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bk-notice-sdk
-Version: 1.3.1
+Version: 1.3.2
 Summary: A project for fetching and displaying announcement notifications.
 Home-page: UNKNOWN
 Author: blueking
 Author-email: blueking@tencent.com
 License: UNKNOWN
 Description: # bk-notice-sdk
```

### Comparing `bk-notice-sdk-1.3.1/bk_notice_sdk.egg-info/SOURCES.txt` & `bk-notice-sdk-1.3.2/bk_notice_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bk-notice-sdk-1.3.1/bk_notice_sdk/apps.py` & `bk-notice-sdk-1.3.2/bk_notice_sdk/apps.py`

 * *Files identical despite different names*

### Comparing `bk-notice-sdk-1.3.1/bk_notice_sdk/utils.py` & `bk-notice-sdk-1.3.2/bk_notice_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `bk-notice-sdk-1.3.1/bk_notice_sdk/config.py` & `bk-notice-sdk-1.3.2/bk_notice_sdk/config.py`

 * *Files identical despite different names*

### Comparing `bk-notice-sdk-1.3.1/bk_notice_sdk/management/commands/register_application.py` & `bk-notice-sdk-1.3.2/bk_notice_sdk/management/commands/register_application.py`

 * *Files identical despite different names*

### Comparing `bk-notice-sdk-1.3.1/bkapi/bk_notice/client.py` & `bk-notice-sdk-1.3.2/bkapi/bk_notice/client.py`

 * *Files identical despite different names*

### Comparing `bk-notice-sdk-1.3.1/README.md` & `bk-notice-sdk-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `bk-notice-sdk-1.3.1/setup.py` & `bk-notice-sdk-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     requirements = f.read().splitlines()
 
 with open(os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf-8") as readme:
     README = readme.read()
 
 setup(
     name="bk-notice-sdk",  # 项目名称
-    version="1.3.1",  # 项目版本
+    version="1.3.2",  # 项目版本
     description="A project for fetching and displaying announcement notifications.",  # 项目的简短描述
     packages=find_packages(),  # 包含项目中的所有包
     author="blueking",
     author_email="blueking@tencent.com",
     # url
     include_package_data=True,  # 包含非代码文件（如模板、静态文件等）
     long_description=README,  # 项目的详细描述，从 README.md 文件获取
```

