# Comparing `tmp/laravel_queue-0.0.8.tar.gz` & `tmp/laravel_queue-0.0.9.tar.gz`

## Comparing `laravel_queue-0.0.8.tar` & `laravel_queue-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 laravel_queue-0.0.8/.github/workflows/build.yml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 laravel_queue-0.0.8/src/laravel_queue/__about__.py
--rw-r--r--   0        0        0     5532 2020-02-02 00:00:00.000000 laravel_queue-0.0.8/src/laravel_queue/__init__.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 laravel_queue-0.0.8/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 laravel_queue-0.0.8/LICENSE
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 laravel_queue-0.0.8/README.md
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 laravel_queue-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 laravel_queue-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 laravel_queue-0.0.9/.github/workflows/build.yml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 laravel_queue-0.0.9/src/laravel_queue/__about__.py
+-rw-r--r--   0        0        0     5532 2020-02-02 00:00:00.000000 laravel_queue-0.0.9/src/laravel_queue/__init__.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 laravel_queue-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 laravel_queue-0.0.9/LICENSE
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 laravel_queue-0.0.9/README.md
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 laravel_queue-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 laravel_queue-0.0.9/PKG-INFO
```

### Comparing `laravel_queue-0.0.8/.github/workflows/build.yml` & `laravel_queue-0.0.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `laravel_queue-0.0.8/src/laravel_queue/__init__.py` & `laravel_queue-0.0.9/src/laravel_queue/__init__.py`

 * *Files identical despite different names*

### Comparing `laravel_queue-0.0.8/LICENSE` & `laravel_queue-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `laravel_queue-0.0.8/README.md` & `laravel_queue-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `laravel_queue-0.0.8/pyproject.toml` & `laravel_queue-0.0.9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-
 dependencies = [
   "psycopg2",
   "phpserialize"
 ]
 
+[project.urls]
+Repository = "https://github.com/2ndnaturewater/python-laravel-queue"
+Issues = "https://github.com/2ndnaturewater/python-laravel-queue/issues"
+
 [tool.hatch.version]
 path = "src/laravel_queue/__about__.py"
```

### Comparing `laravel_queue-0.0.8/PKG-INFO` & `laravel_queue-0.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: laravel_queue
-Version: 0.0.8
+Version: 0.0.9
 Summary: Reads from a Laravel queue
+Project-URL: Repository, https://github.com/2ndnaturewater/python-laravel-queue
+Project-URL: Issues, https://github.com/2ndnaturewater/python-laravel-queue/issues
 Author-email: 2NDNATURE <info@2ndnaturewater.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: phpserialize
```

