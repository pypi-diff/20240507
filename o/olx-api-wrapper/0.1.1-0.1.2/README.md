# Comparing `tmp/olx-api-wrapper-0.1.1.tar.gz` & `tmp/olx-api-wrapper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olx-api-wrapper-0.1.1.tar", last modified: Tue May  7 07:11:07 2024, max compression
+gzip compressed data, was "olx-api-wrapper-0.1.2.tar", last modified: Tue May  7 09:43:26 2024, max compression
```

## Comparing `olx-api-wrapper-0.1.1.tar` & `olx-api-wrapper-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:07.413425 olx-api-wrapper-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-05-07 07:11:07.413425 olx-api-wrapper-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9382 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:07.413425 olx-api-wrapper-0.1.1/olx/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/advert_logo.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/advert_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/adverts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/categories_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/cities_districts.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/languages_currencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/olx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/paid_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/payments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/threads_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/user_business.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:07.413425 olx-api-wrapper-0.1.1/olx_api_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-05-07 07:11:07.000000 olx-api-wrapper-0.1.1/olx_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-07 07:11:07.000000 olx-api-wrapper-0.1.1/olx_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:11:07.000000 olx-api-wrapper-0.1.1/olx_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 07:11:07.000000 olx-api-wrapper-0.1.1/olx_api_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-07 07:11:07.000000 olx-api-wrapper-0.1.1/olx_api_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:11:07.413425 olx-api-wrapper-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:43:26.888237 olx-api-wrapper-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-07 09:43:16.000000 olx-api-wrapper-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-05-07 09:43:26.888237 olx-api-wrapper-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9382 2024-05-07 09:43:16.000000 olx-api-wrapper-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:43:26.884237 olx-api-wrapper-0.1.2/olx/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-07 09:43:16.000000 olx-api-wrapper-0.1.2/olx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-07 09:43:16.000000 olx-api-wrapper-0.1.2/olx/advert_logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-07 09:43:16.000000 olx-api-wrapper-0.1.2/olx/advert_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-07 09:43:16.000000 olx-api-wrapper-0.1.2/olx/adverts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-07 09:43:16.000000 olx-api-wrapper-0.1.2/olx/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-07 09:43:16.000000 olx-api-wrapper-0.1.2/olx/categories_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-07 09:43:16.000000 olx-api-wrapper-0.1.2/olx/cities_districts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-07 09:43:16.000000 olx-api-wrapper-0.1.2/olx/languages_currencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-07 09:43:16.000000 olx-api-wrapper-0.1.2/olx/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-05-07 09:43:16.000000 olx-api-wrapper-0.1.2/olx/olx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-07 09:43:16.000000 olx-api-wrapper-0.1.2/olx/paid_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-07 09:43:16.000000 olx-api-wrapper-0.1.2/olx/payments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-07 09:43:16.000000 olx-api-wrapper-0.1.2/olx/threads_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-07 09:43:16.000000 olx-api-wrapper-0.1.2/olx/user_business.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-07 09:43:16.000000 olx-api-wrapper-0.1.2/olx/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:43:26.888237 olx-api-wrapper-0.1.2/olx_api_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-05-07 09:43:26.000000 olx-api-wrapper-0.1.2/olx_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-07 09:43:26.000000 olx-api-wrapper-0.1.2/olx_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:43:26.000000 olx-api-wrapper-0.1.2/olx_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 09:43:26.000000 olx-api-wrapper-0.1.2/olx_api_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-07 09:43:26.000000 olx-api-wrapper-0.1.2/olx_api_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 09:43:26.888237 olx-api-wrapper-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-07 09:43:16.000000 olx-api-wrapper-0.1.2/setup.py
```

### Comparing `olx-api-wrapper-0.1.1/LICENSE` & `olx-api-wrapper-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.1.1/PKG-INFO` & `olx-api-wrapper-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olx-api-wrapper
-Version: 0.1.1
+Version: 0.1.2
 Summary: Unofficial Wrapper for OLX API
 Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: Paweł Stawikowski
 Author-email: pawikoski@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.1.1 Summary: Unofficial
+Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.1.2 Summary: Unofficial
 Wrapper for OLX API Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: PaweÅ Stawikowski Author-email: pawikoski@gmail.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
```

### Comparing `olx-api-wrapper-0.1.1/README.md` & `olx-api-wrapper-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.1.1/olx/advert_logo.py` & `olx-api-wrapper-0.1.2/olx/advert_logo.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.1.1/olx/advert_statistics.py` & `olx-api-wrapper-0.1.2/olx/advert_statistics.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.1.1/olx/adverts.py` & `olx-api-wrapper-0.1.2/olx/adverts.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.1.1/olx/auth.py` & `olx-api-wrapper-0.1.2/olx/auth.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.1.1/olx/categories_attributes.py` & `olx-api-wrapper-0.1.2/olx/categories_attributes.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.1.1/olx/cities_districts.py` & `olx-api-wrapper-0.1.2/olx/cities_districts.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.1.1/olx/languages_currencies.py` & `olx-api-wrapper-0.1.2/olx/languages_currencies.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.1.1/olx/models.py` & `olx-api-wrapper-0.1.2/olx/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 @dataclass
 class AuthenticatedUser:
     id: int
     email: str
     status: str
     name: str
-    phone: Optional[str]
+    phone: Optional[str | Number]
     phone_login: Optional[int]
     created_at: str
     last_login_at: str
     avatar: Optional[str]
     is_business: bool
```

### Comparing `olx-api-wrapper-0.1.1/olx/olx.py` & `olx-api-wrapper-0.1.2/olx/olx.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.1.1/olx/paid_features.py` & `olx-api-wrapper-0.1.2/olx/paid_features.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.1.1/olx/payments.py` & `olx-api-wrapper-0.1.2/olx/payments.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.1.1/olx/threads_messages.py` & `olx-api-wrapper-0.1.2/olx/threads_messages.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.1.1/olx/users.py` & `olx-api-wrapper-0.1.2/olx/users.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.1.1/olx_api_wrapper.egg-info/PKG-INFO` & `olx-api-wrapper-0.1.2/olx_api_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olx-api-wrapper
-Version: 0.1.1
+Version: 0.1.2
 Summary: Unofficial Wrapper for OLX API
 Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: Paweł Stawikowski
 Author-email: pawikoski@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.1.1 Summary: Unofficial
+Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.1.2 Summary: Unofficial
 Wrapper for OLX API Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: PaweÅ Stawikowski Author-email: pawikoski@gmail.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
```

