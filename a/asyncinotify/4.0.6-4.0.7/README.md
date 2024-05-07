# Comparing `tmp/asyncinotify-4.0.6.tar.gz` & `tmp/asyncinotify-4.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncinotify-4.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "asyncinotify-4.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `asyncinotify-4.0.6.tar` & `asyncinotify-4.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1355 2024-01-15 17:50:42.126394 asyncinotify-4.0.6/.gitignore
--rw-r--r--   0        0        0     1346 2024-01-15 17:50:42.126394 asyncinotify-4.0.6/.gitlab-ci.yml
--rw-r--r--   0        0        0      121 2024-01-15 17:50:42.126394 asyncinotify-4.0.6/CHANGELOG.md
--rw-r--r--   0        0        0        0 2024-01-15 17:50:42.148394 asyncinotify-4.0.6/CONTRIBUTING.md
--rw-r--r--   0        0        0    16726 2024-01-15 17:50:42.126394 asyncinotify-4.0.6/LICENSE
--rw-r--r--   0        0        0     3747 2024-01-15 17:50:42.126394 asyncinotify-4.0.6/README.rst
--rw-r--r--   0        0        0      634 2024-01-15 17:50:42.126394 asyncinotify-4.0.6/docs/Makefile
--rw-r--r--   0        0        0       68 2024-01-15 17:50:42.126394 asyncinotify-4.0.6/docs/asyncinotify.rst
--rw-r--r--   0        0        0     2299 2024-01-15 17:50:42.126394 asyncinotify-4.0.6/docs/conf.py
--rw-r--r--   0        0        0     1571 2024-01-15 17:50:42.126394 asyncinotify-4.0.6/docs/index.rst
--rw-r--r--   0        0        0      795 2024-01-15 17:50:42.126394 asyncinotify-4.0.6/docs/make.bat
--rw-r--r--   0        0        0       40 2024-01-15 17:50:42.126394 asyncinotify-4.0.6/docs/requirements.txt
--rw-r--r--   0        0        0     4275 2024-01-15 17:50:42.126394 asyncinotify-4.0.6/examples/recursivewatch.py
--rw-r--r--   0        0        0     1081 2024-01-15 17:50:42.126394 asyncinotify-4.0.6/pyproject.toml
--rw-r--r--   0        0        0    23254 2024-01-15 17:50:42.127394 asyncinotify-4.0.6/src/asyncinotify/__init__.py
--rw-r--r--   0        0        0     1385 2024-01-15 17:50:42.127394 asyncinotify-4.0.6/src/asyncinotify/_ffi.py
--rw-r--r--   0        0        0        0 2024-01-15 17:50:42.148394 asyncinotify-4.0.6/src/asyncinotify/py.typed
--rwxr-xr-x   0        0        0    17482 2024-01-15 17:50:42.127394 asyncinotify-4.0.6/test.py
--rw-r--r--   0        0        0     4706 1970-01-01 00:00:00.000000 asyncinotify-4.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1355 2020-11-16 23:10:18.120975 asyncinotify-4.0.7/.gitignore
+-rw-r--r--   0        0        0     1346 2024-05-07 14:56:04.303562 asyncinotify-4.0.7/.gitlab-ci.yml
+-rw-r--r--   0        0        0      121 2020-11-16 23:10:18.120975 asyncinotify-4.0.7/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-11-16 23:10:18.120975 asyncinotify-4.0.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0    16726 2024-05-07 14:56:04.303562 asyncinotify-4.0.7/LICENSE
+-rw-r--r--   0        0        0     3747 2024-05-07 14:56:04.303562 asyncinotify-4.0.7/README.rst
+-rw-r--r--   0        0        0      634 2020-11-16 23:10:18.120975 asyncinotify-4.0.7/docs/Makefile
+-rw-r--r--   0        0        0       68 2020-11-18 20:39:20.954406 asyncinotify-4.0.7/docs/asyncinotify.rst
+-rw-r--r--   0        0        0     2299 2023-02-07 05:16:03.049588 asyncinotify-4.0.7/docs/conf.py
+-rw-r--r--   0        0        0     1571 2024-05-07 14:56:04.304562 asyncinotify-4.0.7/docs/index.rst
+-rw-r--r--   0        0        0      795 2020-11-16 23:10:18.185975 asyncinotify-4.0.7/docs/make.bat
+-rw-r--r--   0        0        0       40 2023-01-17 00:42:46.707537 asyncinotify-4.0.7/docs/requirements.txt
+-rw-r--r--   0        0        0     4275 2021-01-05 03:59:12.048279 asyncinotify-4.0.7/examples/recursivewatch.py
+-rw-r--r--   0        0        0     1081 2024-05-07 14:56:26.356216 asyncinotify-4.0.7/pyproject.toml
+-rw-r--r--   0        0        0    23254 2024-05-07 14:56:04.304562 asyncinotify-4.0.7/src/asyncinotify/__init__.py
+-rw-r--r--   0        0        0     1385 2023-02-07 05:19:32.137870 asyncinotify-4.0.7/src/asyncinotify/_ffi.py
+-rw-r--r--   0        0        0        0 2022-06-02 17:02:28.469706 asyncinotify-4.0.7/src/asyncinotify/py.typed
+-rwxr-xr-x   0        0        0    17482 2024-05-07 14:56:04.304562 asyncinotify-4.0.7/test.py
+-rw-r--r--   0        0        0     4706 1970-01-01 00:00:00.000000 asyncinotify-4.0.7/PKG-INFO
```

### Comparing `asyncinotify-4.0.6/.gitignore` & `asyncinotify-4.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `asyncinotify-4.0.6/.gitlab-ci.yml` & `asyncinotify-4.0.7/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `asyncinotify-4.0.6/LICENSE` & `asyncinotify-4.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncinotify-4.0.6/README.rst` & `asyncinotify-4.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `asyncinotify-4.0.6/docs/Makefile` & `asyncinotify-4.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `asyncinotify-4.0.6/docs/conf.py` & `asyncinotify-4.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `asyncinotify-4.0.6/docs/index.rst` & `asyncinotify-4.0.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `asyncinotify-4.0.6/docs/make.bat` & `asyncinotify-4.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `asyncinotify-4.0.6/examples/recursivewatch.py` & `asyncinotify-4.0.7/examples/recursivewatch.py`

 * *Files identical despite different names*

### Comparing `asyncinotify-4.0.6/pyproject.toml` & `asyncinotify-4.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = 'asyncinotify'
 description = 'A simple optionally-async python inotify library, focused on simplicity of use and operation, and leveraging modern Python features'
-version = '4.0.6'
+version = '4.0.7'
 readme = 'README.rst'
 requires-python = '>= 3.6, < 4'
 license = {text = 'MPL-2.0'}
 keywords = [
     'async',
     'inotify',
 ]
@@ -23,13 +23,13 @@
 ]
 
 [[project.authors]]
 name = "Taylor C. Richberger"
 email = "tcr@absolute-performance.com"
 
 [project.urls]
-repository  = 'https://github.com/absperf/asyncinotify/'
+repository  = 'https://github.com/ProCern/asyncinotify/'
 documentation = 'https://asyncinotify.readthedocs.io/'
 
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.2,<4", 'wheel']
```

### Comparing `asyncinotify-4.0.6/src/asyncinotify/__init__.py` & `asyncinotify-4.0.7/src/asyncinotify/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncinotify-4.0.6/src/asyncinotify/_ffi.py` & `asyncinotify-4.0.7/src/asyncinotify/_ffi.py`

 * *Files identical despite different names*

### Comparing `asyncinotify-4.0.6/test.py` & `asyncinotify-4.0.7/test.py`

 * *Files identical despite different names*

### Comparing `asyncinotify-4.0.6/PKG-INFO` & `asyncinotify-4.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncinotify
-Version: 4.0.6
+Version: 4.0.7
 Summary: A simple optionally-async python inotify library, focused on simplicity of use and operation, and leveraging modern Python features
 Keywords: async,inotify
 Author-email: "Taylor C. Richberger" <tcr@absolute-performance.com>
 Requires-Python: >= 3.6, < 4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 6 - Mature
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: AsyncIO
 Project-URL: documentation, https://asyncinotify.readthedocs.io/
-Project-URL: repository, https://github.com/absperf/asyncinotify/
+Project-URL: repository, https://github.com/ProCern/asyncinotify/
 
 asyncinotify
 ============
 
 An async python inotify package.  Kept as simple and easy-to-understand as
 possible, while still being flexible and powerful.  This is built on no external
 dependencies, and works through ctypes in a very obvious fashion.
```

