# Comparing `tmp/spacetrack-1.2.0.tar.gz` & `tmp/spacetrack-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacetrack-1.2.0.tar", last modified: Sat Nov 25 19:36:35 2023, max compression
+gzip compressed data, was "spacetrack-1.3.0.tar", last modified: Tue May  7 14:49:04 2024, max compression
```

## Comparing `spacetrack-1.2.0.tar` & `spacetrack-1.3.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 19:36:35.536206 spacetrack-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2023-11-25 19:36:20.000000 spacetrack-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2023-11-25 19:36:20.000000 spacetrack-1.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      211 2023-11-25 19:36:20.000000 spacetrack-1.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2023-11-25 19:36:20.000000 spacetrack-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2023-11-25 19:36:20.000000 spacetrack-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2023-11-25 19:36:35.536206 spacetrack-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2023-11-25 19:36:20.000000 spacetrack-1.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-11-25 19:36:20.000000 spacetrack-1.2.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 19:36:35.532206 spacetrack-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     9641 2023-11-25 19:36:20.000000 spacetrack-1.2.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2023-11-25 19:36:20.000000 spacetrack-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2023-11-25 19:36:20.000000 spacetrack-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      458 2023-11-25 19:36:20.000000 spacetrack-1.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-11-25 19:36:20.000000 spacetrack-1.2.0/docs/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 19:36:35.532206 spacetrack-1.2.0/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-11-25 19:36:20.000000 spacetrack-1.2.0/docs/modules/aio.rst
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-11-25 19:36:20.000000 spacetrack-1.2.0/docs/modules/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-11-25 19:36:20.000000 spacetrack-1.2.0/docs/modules/operators.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2023-11-25 19:36:20.000000 spacetrack-1.2.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2023-11-25 19:36:20.000000 spacetrack-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-25 19:36:35.536206 spacetrack-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 19:36:35.532206 spacetrack-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 19:36:35.532206 spacetrack-1.2.0/src/spacetrack/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2023-11-25 19:36:20.000000 spacetrack-1.2.0/src/spacetrack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8210 2023-11-25 19:36:20.000000 spacetrack-1.2.0/src/spacetrack/aio.py
--rw-r--r--   0 runner    (1001) docker     (127)    30170 2023-11-25 19:36:20.000000 spacetrack-1.2.0/src/spacetrack/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2023-11-25 19:36:20.000000 spacetrack-1.2.0/src/spacetrack/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 19:36:35.536206 spacetrack-1.2.0/src/spacetrack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2023-11-25 19:36:35.000000 spacetrack-1.2.0/src/spacetrack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      695 2023-11-25 19:36:35.000000 spacetrack-1.2.0/src/spacetrack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-25 19:36:35.000000 spacetrack-1.2.0/src/spacetrack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-11-25 19:36:35.000000 spacetrack-1.2.0/src/spacetrack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-25 19:36:35.000000 spacetrack-1.2.0/src/spacetrack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 19:36:35.536206 spacetrack-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-25 19:36:20.000000 spacetrack-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2023-11-25 19:36:20.000000 spacetrack-1.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2023-11-25 19:36:20.000000 spacetrack-1.2.0/tests/test_aio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-11-25 19:36:20.000000 spacetrack-1.2.0/tests/test_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    17288 2023-11-25 19:36:20.000000 spacetrack-1.2.0/tests/test_spacetrack.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-11-25 19:36:20.000000 spacetrack-1.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:49:04.556464 spacetrack-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-07 14:48:53.000000 spacetrack-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-07 14:48:53.000000 spacetrack-1.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-07 14:48:53.000000 spacetrack-1.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-07 14:48:53.000000 spacetrack-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-07 14:48:53.000000 spacetrack-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-07 14:49:04.556464 spacetrack-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-07 14:48:53.000000 spacetrack-1.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-07 14:48:53.000000 spacetrack-1.3.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:49:04.552464 spacetrack-1.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     9844 2024-05-07 14:48:53.000000 spacetrack-1.3.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-07 14:48:53.000000 spacetrack-1.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-07 14:48:53.000000 spacetrack-1.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-07 14:48:53.000000 spacetrack-1.3.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-07 14:48:53.000000 spacetrack-1.3.0/docs/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:49:04.552464 spacetrack-1.3.0/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-07 14:48:53.000000 spacetrack-1.3.0/docs/modules/aio.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-07 14:48:53.000000 spacetrack-1.3.0/docs/modules/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-07 14:48:53.000000 spacetrack-1.3.0/docs/modules/operators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-05-07 14:48:53.000000 spacetrack-1.3.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-07 14:48:53.000000 spacetrack-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:49:04.556464 spacetrack-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:49:04.552464 spacetrack-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:49:04.556464 spacetrack-1.3.0/src/spacetrack/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-07 14:48:53.000000 spacetrack-1.3.0/src/spacetrack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-05-07 14:48:53.000000 spacetrack-1.3.0/src/spacetrack/aio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30170 2024-05-07 14:48:53.000000 spacetrack-1.3.0/src/spacetrack/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-07 14:48:53.000000 spacetrack-1.3.0/src/spacetrack/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:49:04.556464 spacetrack-1.3.0/src/spacetrack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-07 14:49:04.000000 spacetrack-1.3.0/src/spacetrack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-07 14:49:04.000000 spacetrack-1.3.0/src/spacetrack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:49:04.000000 spacetrack-1.3.0/src/spacetrack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-07 14:49:04.000000 spacetrack-1.3.0/src/spacetrack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 14:49:04.000000 spacetrack-1.3.0/src/spacetrack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:49:04.556464 spacetrack-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:48:53.000000 spacetrack-1.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-07 14:48:53.000000 spacetrack-1.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-07 14:48:53.000000 spacetrack-1.3.0/tests/test_aio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-07 14:48:53.000000 spacetrack-1.3.0/tests/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-05-07 14:48:53.000000 spacetrack-1.3.0/tests/test_spacetrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-07 14:48:53.000000 spacetrack-1.3.0/tox.ini
```

### Comparing `spacetrack-1.2.0/.pre-commit-config.yaml` & `spacetrack-1.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spacetrack-1.2.0/LICENSE.txt` & `spacetrack-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spacetrack-1.2.0/PKG-INFO` & `spacetrack-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacetrack
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python client for space-track.org
 Author-email: Frazer McLean <frazer@frazermclean.co.uk>
 License: MIT
 Project-URL: Repository, https://github.com/python-astrodynamics/spacetrack
 Project-URL: Documentation, https://spacetrack.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `spacetrack-1.2.0/README.rst` & `spacetrack-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `spacetrack-1.2.0/docs/changelog.rst` & `spacetrack-1.3.0/docs/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,37 @@
 ==========
 
 Unreleased_
 -----------
 
 N/A
 
+1.3.0_ - 2024-05-07
+-------------------
+
+Added
+~~~~~
+
+- Timezone-aware datetimes are supported in request predicates.
+
 1.2.0_ - 2023-11-25
 -------------------
 
 Added
 ~~~~~
 
 - ``additional_rate_limit`` argument to
   :class:`~spacetrack.base.SpaceTrackClient`.
 
 Fixed
 ~~~~~
 
 - Since version 1.0, the value passed to ``SpaceTrackClient.callback``, if set,
-  is from :func:`time.monotonic` but the documentation was not updated to reflect
-  this.
+  is from :func:`time.monotonic` but the documentation was not updated to
+  reflect this.
 
 1.1.0_ - 2023-10-15
 -------------------
 
 Added
 ~~~~~
 
@@ -323,15 +331,16 @@
 -  ``Predicate`` class now has a ``default`` attribute.
 
 0.9.0_ - 2016-01-28
 -------------------
 
 First release.
 
-.. _Unreleased: https://github.com/python-astrodynamics/spacetrack/compare/1.2.0...HEAD
+.. _Unreleased: https://github.com/python-astrodynamics/spacetrack/compare/1.3.0...HEAD
+.. _1.3.0: https://github.com/python-astrodynamics/spacetrack/compare/1.2.0...1.3.0
 .. _1.2.0: https://github.com/python-astrodynamics/spacetrack/compare/1.1.0...1.2.0
 .. _1.1.0: https://github.com/python-astrodynamics/spacetrack/compare/1.0.1...1.1.0
 .. _1.0.1: https://github.com/python-astrodynamics/spacetrack/compare/1.0.0...1.0.1
 .. _1.0.0: https://github.com/python-astrodynamics/spacetrack/compare/0.16.0...1.0.0
 .. _0.16.0: https://github.com/python-astrodynamics/spacetrack/compare/0.15.0...0.16.0
 .. _0.15.0: https://github.com/python-astrodynamics/spacetrack/compare/0.14.0...0.15.0
 .. _0.14.0: https://github.com/python-astrodynamics/spacetrack/compare/0.13.7...0.14.0
```

### Comparing `spacetrack-1.2.0/docs/conf.py` & `spacetrack-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spacetrack-1.2.0/docs/index.rst` & `spacetrack-1.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `spacetrack-1.2.0/docs/usage.rst` & `spacetrack-1.3.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `spacetrack-1.2.0/pyproject.toml` & `spacetrack-1.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spacetrack"
-version = "1.2.0"
+version = "1.3.0"
 description = "Python client for space-track.org"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 authors = [
     { name = "Frazer McLean", email = "frazer@frazermclean.co.uk" },
 ]
```

### Comparing `spacetrack-1.2.0/src/spacetrack/aio.py` & `spacetrack-1.3.0/src/spacetrack/aio.py`

 * *Files identical despite different names*

### Comparing `spacetrack-1.2.0/src/spacetrack/base.py` & `spacetrack-1.3.0/src/spacetrack/base.py`

 * *Files identical despite different names*

### Comparing `spacetrack-1.2.0/src/spacetrack/operators.py` & `spacetrack-1.3.0/src/spacetrack/operators.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,16 @@
     - ``None`` -> ``'null-val'``
     """
     if isinstance(value, bool):
         return str(value).lower()
     elif isinstance(value, Sequence) and not isinstance(value, str):
         return ",".join(_stringify_predicate_value(x) for x in value)
     elif isinstance(value, datetime.datetime):
+        if value.tzinfo is not None:
+            value = value.astimezone(datetime.timezone.utc).replace(tzinfo=None)
         return value.isoformat(sep=" ")
     elif isinstance(value, datetime.date):
         return value.isoformat()
     elif value is None:
         return "null-val"
     else:
         return str(value)
```

### Comparing `spacetrack-1.2.0/src/spacetrack.egg-info/PKG-INFO` & `spacetrack-1.3.0/src/spacetrack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacetrack
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python client for space-track.org
 Author-email: Frazer McLean <frazer@frazermclean.co.uk>
 License: MIT
 Project-URL: Repository, https://github.com/python-astrodynamics/spacetrack
 Project-URL: Documentation, https://spacetrack.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `spacetrack-1.2.0/src/spacetrack.egg-info/SOURCES.txt` & `spacetrack-1.3.0/src/spacetrack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spacetrack-1.2.0/tests/conftest.py` & `spacetrack-1.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spacetrack-1.2.0/tests/test_aio.py` & `spacetrack-1.3.0/tests/test_aio.py`

 * *Files identical despite different names*

### Comparing `spacetrack-1.2.0/tests/test_operators.py` & `spacetrack-1.3.0/tests/test_operators.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 stringify_data = [
     (True, "true"),
     (False, "false"),
     ([1, 2], "1,2"),
     (["a", "b"], "a,b"),
     ((dt.date(2001, 2, 3), dt.date(2004, 5, 6)), "2001-02-03,2004-05-06"),
     (dt.datetime(2001, 2, 3, 4, 5, 6), "2001-02-03 04:05:06"),
+    (dt.datetime(2001, 2, 3, tzinfo=dt.timezone.utc), "2001-02-03 00:00:00"),
     (dt.date(2001, 2, 3), "2001-02-03"),
     (None, "null-val"),
 ]
 
 
 @pytest.mark.parametrize("value, expected", stringify_data)
 def test_stringify_predicate_value(value, expected):
```

### Comparing `spacetrack-1.2.0/tests/test_spacetrack.py` & `spacetrack-1.3.0/tests/test_spacetrack.py`

 * *Files identical despite different names*

### Comparing `spacetrack-1.2.0/tox.ini` & `spacetrack-1.3.0/tox.ini`

 * *Files identical despite different names*

