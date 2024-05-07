# Comparing `tmp/cmoonvision-0.2.0.tar.gz` & `tmp/cmoonvision-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmoonvision-0.2.0.tar", max compression
+gzip compressed data, was "cmoonvision-0.2.1.tar", max compression
```

## Comparing `cmoonvision-0.2.0.tar` & `cmoonvision-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0        0 2024-04-26 13:48:25.163207 cmoonvision-0.2.0/README.md
--rw-r--r--   0        0        0     5219 2024-04-27 16:03:55.383760 cmoonvision-0.2.0/cmoonvision/CmoonVision.py
--rw-r--r--   0        0        0      201 2024-04-28 02:52:22.565891 cmoonvision-0.2.0/cmoonvision/__init__.py
--rw-r--r--   0        0        0    12733 2024-04-28 04:04:59.359664 cmoonvision-0.2.0/cmoonvision/cmoon_utils.py
--rw-r--r--   0        0        0      431 2024-04-28 04:16:01.994742 cmoonvision-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 cmoonvision-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0        0 2024-04-26 13:48:25.163207 cmoonvision-0.2.1/README.md
+-rwxr-xr-x   0        0        0     5219 2024-04-27 16:03:55.383759 cmoonvision-0.2.1/cmoonvision/CmoonVision.py
+-rwxr-xr-x   0        0        0      201 2024-04-28 02:52:22.565891 cmoonvision-0.2.1/cmoonvision/__init__.py
+-rwxr-xr-x   0        0        0    12733 2024-04-28 04:04:59.359664 cmoonvision-0.2.1/cmoonvision/cmoon_utils.py
+-rwxr-xr-x   0        0        0     2777 2024-05-07 12:41:24.357203 cmoonvision-0.2.1/cmoonvision/cmoonvision_example.py
+-rwxr-xr-x   0        0        0      433 2024-05-07 13:07:00.503906 cmoonvision-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      546 1970-01-01 00:00:00.000000 cmoonvision-0.2.1/PKG-INFO
```

### Comparing `cmoonvision-0.2.0/cmoonvision/CmoonVision.py` & `cmoonvision-0.2.1/cmoonvision/CmoonVision.py`

 * *Files identical despite different names*

### Comparing `cmoonvision-0.2.0/cmoonvision/cmoon_utils.py` & `cmoonvision-0.2.1/cmoonvision/cmoon_utils.py`

 * *Files identical despite different names*

### Comparing `cmoonvision-0.2.0/PKG-INFO` & `cmoonvision-0.2.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: cmoonvision
-Version: 0.2.0
+Version: 0.2.1
 Summary: CmoonVision based on YoloV8
 License: AGPL-3.0
 Author: cmoon
 Author-email: cmoon@mail.ustc.edu.cn
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: ultralytics (>=8.2.2,<9.0.0)
+Requires-Dist: ultralytics (==8.2.8)
 Description-Content-Type: text/markdown
```

