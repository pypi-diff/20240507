# Comparing `tmp/mrkutil-1.3.1.tar.gz` & `tmp/mrkutil-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrkutil-1.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mrkutil-1.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mrkutil-1.3.1.tar` & `mrkutil-1.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       91 2024-04-10 18:38:36.896155 mrkutil-1.3.1/.flake8
--rw-r--r--   0        0        0     1800 2024-04-10 13:44:48.196615 mrkutil-1.3.1/.gitignore
--rw-r--r--   0        0        0      366 2024-04-10 18:38:32.560123 mrkutil-1.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11358 2024-04-10 13:44:48.196615 mrkutil-1.3.1/LICENSE
--rw-r--r--   0        0        0     3057 2024-04-11 06:14:47.021960 mrkutil-1.3.1/README.md
--rw-r--r--   0        0        0      113 2024-04-24 14:32:41.045641 mrkutil-1.3.1/mrkutil/__init__.py
--rw-r--r--   0        0        0       72 2024-04-10 13:44:48.196615 mrkutil-1.3.1/mrkutil/base/__init__.py
--rw-r--r--   0        0        0     1748 2024-04-10 19:00:33.746768 mrkutil-1.3.1/mrkutil/base/base_handler.py
--rw-r--r--   0        0        0       60 2024-04-10 18:50:04.170994 mrkutil-1.3.1/mrkutil/cache/__init__.py
--rw-r--r--   0        0        0     2406 2024-04-10 19:02:46.268056 mrkutil-1.3.1/mrkutil/cache/base_redis.py
--rw-r--r--   0        0        0      262 2024-04-24 12:44:29.700772 mrkutil-1.3.1/mrkutil/communication/__init__.py
--rw-r--r--   0        0        0     1462 2024-04-24 11:50:42.829911 mrkutil-1.3.1/mrkutil/communication/call_service.py
--rw-r--r--   0        0        0     3162 2024-04-24 14:31:17.548693 mrkutil-1.3.1/mrkutil/communication/listen.py
--rw-r--r--   0        0        0     1375 2024-04-24 12:37:29.267696 mrkutil-1.3.1/mrkutil/communication/trigger_service.py
--rw-r--r--   0        0        0      154 2024-04-10 13:44:48.196615 mrkutil-1.3.1/mrkutil/logging/__init__.py
--rw-r--r--   0        0        0     2681 2024-04-10 19:05:36.249709 mrkutil-1.3.1/mrkutil/logging/logging_config.py
--rw-r--r--   0        0        0     1831 2024-04-10 19:05:53.713880 mrkutil-1.3.1/mrkutil/logging/logging_formatter.py
--rw-r--r--   0        0        0      143 2024-04-10 13:44:48.196615 mrkutil-1.3.1/mrkutil/pagination/__init__.py
--rw-r--r--   0        0        0      805 2024-04-10 19:06:55.098484 mrkutil-1.3.1/mrkutil/pagination/dependency.py
--rw-r--r--   0        0        0     1692 2024-04-10 19:12:12.205642 mrkutil-1.3.1/mrkutil/pagination/mongoengine.py
--rw-r--r--   0        0        0     2552 2024-04-10 19:12:07.341593 mrkutil-1.3.1/mrkutil/pagination/sqlalchemy.py
--rw-r--r--   0        0        0       77 2024-04-10 18:53:14.101683 mrkutil-1.3.1/mrkutil/responses/__init__.py
--rw-r--r--   0        0        0     3225 2024-04-12 08:51:40.055110 mrkutil-1.3.1/mrkutil/responses/response_helper.py
--rw-r--r--   0        0        0      256 2024-04-10 18:53:21.969785 mrkutil-1.3.1/mrkutil/utilities.py
--rw-r--r--   0        0        0      822 2024-04-24 12:36:34.647032 mrkutil-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     3853 1970-01-01 00:00:00.000000 mrkutil-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0       91 2024-04-10 18:38:36.896155 mrkutil-1.3.2/.flake8
+-rw-r--r--   0        0        0     1800 2024-04-10 13:44:48.196615 mrkutil-1.3.2/.gitignore
+-rw-r--r--   0        0        0      366 2024-04-10 18:38:32.560123 mrkutil-1.3.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11358 2024-04-10 13:44:48.196615 mrkutil-1.3.2/LICENSE
+-rw-r--r--   0        0        0     3057 2024-04-11 06:14:47.021960 mrkutil-1.3.2/README.md
+-rw-r--r--   0        0        0      113 2024-05-07 05:01:38.840510 mrkutil-1.3.2/mrkutil/__init__.py
+-rw-r--r--   0        0        0       72 2024-04-10 13:44:48.196615 mrkutil-1.3.2/mrkutil/base/__init__.py
+-rw-r--r--   0        0        0     1748 2024-04-10 19:00:33.746768 mrkutil-1.3.2/mrkutil/base/base_handler.py
+-rw-r--r--   0        0        0       94 2024-04-29 09:23:03.607864 mrkutil-1.3.2/mrkutil/cache/__init__.py
+-rw-r--r--   0        0        0     5259 2024-05-07 05:00:46.228086 mrkutil-1.3.2/mrkutil/cache/base_redis.py
+-rw-r--r--   0        0        0      262 2024-04-24 12:44:29.700772 mrkutil-1.3.2/mrkutil/communication/__init__.py
+-rw-r--r--   0        0        0     1462 2024-04-24 11:50:42.829911 mrkutil-1.3.2/mrkutil/communication/call_service.py
+-rw-r--r--   0        0        0     3162 2024-04-24 14:31:17.548693 mrkutil-1.3.2/mrkutil/communication/listen.py
+-rw-r--r--   0        0        0     1375 2024-04-24 12:37:29.267696 mrkutil-1.3.2/mrkutil/communication/trigger_service.py
+-rw-r--r--   0        0        0      154 2024-04-10 13:44:48.196615 mrkutil-1.3.2/mrkutil/logging/__init__.py
+-rw-r--r--   0        0        0     2681 2024-04-10 19:05:36.249709 mrkutil-1.3.2/mrkutil/logging/logging_config.py
+-rw-r--r--   0        0        0     1831 2024-04-10 19:05:53.713880 mrkutil-1.3.2/mrkutil/logging/logging_formatter.py
+-rw-r--r--   0        0        0      143 2024-04-10 13:44:48.196615 mrkutil-1.3.2/mrkutil/pagination/__init__.py
+-rw-r--r--   0        0        0      805 2024-04-10 19:06:55.098484 mrkutil-1.3.2/mrkutil/pagination/dependency.py
+-rw-r--r--   0        0        0     1692 2024-04-10 19:12:12.205642 mrkutil-1.3.2/mrkutil/pagination/mongoengine.py
+-rw-r--r--   0        0        0     2552 2024-04-10 19:12:07.341593 mrkutil-1.3.2/mrkutil/pagination/sqlalchemy.py
+-rw-r--r--   0        0        0       77 2024-04-10 18:53:14.101683 mrkutil-1.3.2/mrkutil/responses/__init__.py
+-rw-r--r--   0        0        0     3225 2024-04-12 08:51:40.055110 mrkutil-1.3.2/mrkutil/responses/response_helper.py
+-rw-r--r--   0        0        0      256 2024-04-10 18:53:21.969785 mrkutil-1.3.2/mrkutil/utilities.py
+-rw-r--r--   0        0        0      822 2024-04-24 12:36:34.647032 mrkutil-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3853 1970-01-01 00:00:00.000000 mrkutil-1.3.2/PKG-INFO
```

### Comparing `mrkutil-1.3.1/.gitignore` & `mrkutil-1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.1/LICENSE` & `mrkutil-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.1/README.md` & `mrkutil-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.1/mrkutil/base/base_handler.py` & `mrkutil-1.3.2/mrkutil/base/base_handler.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.1/mrkutil/communication/call_service.py` & `mrkutil-1.3.2/mrkutil/communication/call_service.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.1/mrkutil/communication/listen.py` & `mrkutil-1.3.2/mrkutil/communication/listen.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.1/mrkutil/communication/trigger_service.py` & `mrkutil-1.3.2/mrkutil/communication/trigger_service.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.1/mrkutil/logging/logging_config.py` & `mrkutil-1.3.2/mrkutil/logging/logging_config.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.1/mrkutil/logging/logging_formatter.py` & `mrkutil-1.3.2/mrkutil/logging/logging_formatter.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.1/mrkutil/pagination/dependency.py` & `mrkutil-1.3.2/mrkutil/pagination/dependency.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.1/mrkutil/pagination/mongoengine.py` & `mrkutil-1.3.2/mrkutil/pagination/mongoengine.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.1/mrkutil/pagination/sqlalchemy.py` & `mrkutil-1.3.2/mrkutil/pagination/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.1/mrkutil/responses/response_helper.py` & `mrkutil-1.3.2/mrkutil/responses/response_helper.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.1/pyproject.toml` & `mrkutil-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.1/PKG-INFO` & `mrkutil-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrkutil
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python package containing common functions for python service based architecture.
 Author-email: Nebojsa Mrkic <mrkic.nebojsa@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: RabbitMQPubSub>=1.1.1
 Requires-Dist: redis>=4.3 ; extra == "extras"
 Requires-Dist: sqlalchemy>=1.4 ; extra == "extras"
```

