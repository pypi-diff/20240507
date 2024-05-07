# Comparing `tmp/expiringsqlitedict-7.0.2.tar.gz` & `tmp/expiringsqlitedict-7.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expiringsqlitedict-7.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "expiringsqlitedict-7.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `expiringsqlitedict-7.0.2.tar` & `expiringsqlitedict-7.0.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0      249 2023-01-17 17:32:50.440949 expiringsqlitedict-7.0.2/.gitignore
--rw-r--r--   0        0        0      271 2018-06-07 21:48:55.951133 expiringsqlitedict-7.0.2/.travis.yml
--rw-r--r--   0        0        0     1900 2022-07-01 21:27:31.727826 expiringsqlitedict-7.0.2/CHANGELOG.txt
--rw-r--r--   0        0        0    16727 2023-07-18 23:00:00.257716 expiringsqlitedict-7.0.2/LICENSE
--rw-r--r--   0        0        0       52 2021-10-13 21:06:48.260857 expiringsqlitedict-7.0.2/Makefile
--rw-r--r--   0        0        0     3702 2023-07-18 21:30:52.504076 expiringsqlitedict-7.0.2/README.md
--rwxr-xr-x   0        0        0      988 2023-04-29 13:08:50.374197 expiringsqlitedict-7.0.2/bench.py
--rw-r--r--   0        0        0      634 2023-01-17 00:40:43.681234 expiringsqlitedict-7.0.2/docs/Makefile
--rw-r--r--   0        0        0     2302 2023-01-17 00:42:16.953463 expiringsqlitedict-7.0.2/docs/conf.py
--rw-r--r--   0        0        0       87 2023-01-17 00:44:05.124729 expiringsqlitedict-7.0.2/docs/expiringsqlitedict.rst
--rw-r--r--   0        0        0      520 2023-01-17 00:47:24.429206 expiringsqlitedict-7.0.2/docs/index.rst
--rw-r--r--   0        0        0      800 2023-01-17 00:40:43.682233 expiringsqlitedict-7.0.2/docs/make.bat
--rw-r--r--   0        0        0       40 2023-01-17 00:43:04.237580 expiringsqlitedict-7.0.2/docs/requirements.txt
--rwxr-xr-x   0        0        0     2874 2023-11-03 15:15:57.363150 expiringsqlitedict-7.0.2/justfile
--rw-r--r--   0        0        0     1299 2023-11-03 15:14:36.264707 expiringsqlitedict-7.0.2/pyproject.toml
--rwxr-xr-x   0        0        0    23434 2023-11-03 15:14:21.875453 expiringsqlitedict-7.0.2/src/expiringsqlitedict/__init__.py
--rw-r--r--   0        0        0        0 2023-01-17 00:39:05.082991 expiringsqlitedict-7.0.2/src/expiringsqlitedict/py.typed
--rwxr-xr-x   0        0        0    17983 2023-07-19 02:02:15.553877 expiringsqlitedict-7.0.2/test.py
--rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 expiringsqlitedict-7.0.2/PKG-INFO
+-rw-r--r--   0        0        0      249 2023-01-17 17:32:50.440949 expiringsqlitedict-7.0.4/.gitignore
+-rw-r--r--   0        0        0     1034 2024-05-07 15:05:36.603482 expiringsqlitedict-7.0.4/.readthedocs.yaml
+-rw-r--r--   0        0        0      271 2018-06-07 21:48:55.951133 expiringsqlitedict-7.0.4/.travis.yml
+-rw-r--r--   0        0        0     1900 2022-07-01 21:27:31.727826 expiringsqlitedict-7.0.4/CHANGELOG.txt
+-rw-r--r--   0        0        0    16727 2023-07-18 23:00:00.257716 expiringsqlitedict-7.0.4/LICENSE
+-rw-r--r--   0        0        0       52 2021-10-13 21:06:48.260857 expiringsqlitedict-7.0.4/Makefile
+-rw-r--r--   0        0        0     3702 2023-07-18 21:30:52.504076 expiringsqlitedict-7.0.4/README.md
+-rwxr-xr-x   0        0        0      988 2023-04-29 13:08:50.374197 expiringsqlitedict-7.0.4/bench.py
+-rw-r--r--   0        0        0      634 2023-01-17 00:40:43.681234 expiringsqlitedict-7.0.4/docs/Makefile
+-rw-r--r--   0        0        0     2302 2023-01-17 00:42:16.953463 expiringsqlitedict-7.0.4/docs/conf.py
+-rw-r--r--   0        0        0       87 2023-01-17 00:44:05.124729 expiringsqlitedict-7.0.4/docs/expiringsqlitedict.rst
+-rw-r--r--   0        0        0      520 2023-01-17 00:47:24.429206 expiringsqlitedict-7.0.4/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-01-17 00:40:43.682233 expiringsqlitedict-7.0.4/docs/make.bat
+-rw-r--r--   0        0        0       40 2023-01-17 00:43:04.237580 expiringsqlitedict-7.0.4/docs/requirements.txt
+-rwxr-xr-x   0        0        0     2874 2023-11-03 15:15:57.363150 expiringsqlitedict-7.0.4/justfile
+-rw-r--r--   0        0        0     1300 2024-05-07 15:08:27.287081 expiringsqlitedict-7.0.4/pyproject.toml
+-rwxr-xr-x   0        0        0    23434 2023-11-03 15:14:21.875453 expiringsqlitedict-7.0.4/src/expiringsqlitedict/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-17 00:39:05.082991 expiringsqlitedict-7.0.4/src/expiringsqlitedict/py.typed
+-rwxr-xr-x   0        0        0    17983 2023-07-19 02:02:15.553877 expiringsqlitedict-7.0.4/test.py
+-rw-r--r--   0        0        0     4928 1970-01-01 00:00:00.000000 expiringsqlitedict-7.0.4/PKG-INFO
```

### Comparing `expiringsqlitedict-7.0.2/CHANGELOG.txt` & `expiringsqlitedict-7.0.4/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-7.0.2/LICENSE` & `expiringsqlitedict-7.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-7.0.2/README.md` & `expiringsqlitedict-7.0.4/README.md`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-7.0.2/bench.py` & `expiringsqlitedict-7.0.4/bench.py`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-7.0.2/docs/Makefile` & `expiringsqlitedict-7.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-7.0.2/docs/conf.py` & `expiringsqlitedict-7.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-7.0.2/docs/index.rst` & `expiringsqlitedict-7.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-7.0.2/docs/make.bat` & `expiringsqlitedict-7.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-7.0.2/justfile` & `expiringsqlitedict-7.0.4/justfile`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-7.0.2/pyproject.toml` & `expiringsqlitedict-7.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = 'expiringsqlitedict'
 description = 'Persistent compressed expiring dict in Python, backed up by sqlite3 and json'
-version = '7.0.2'
+version = '7.0.4'
 readme = 'README.md'
 requires-python = '>= 3.6, < 4'
 license = { text = 'MPL 2.0' }
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
@@ -20,18 +20,18 @@
     'Topic :: Database :: Front-Ends',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Software Development :: Libraries',
 ]
 
 [[project.authors]]
 name = "Taylor C. Richberger"
-email = "tcr@absolute-performance.com"
+email = "taylor.richberger@procern.com"
 
 [project.urls]
-repository  = 'https://github.com/absperf/expiringsqlitedict'
+repository  = 'https://github.com/ProCern/expiringsqlitedict'
 documentation = 'https://expiringsqlitedict.readthedocs.io/'
 
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.2,<4", 'wheel']
 
 [project.optional-dependencies]
```

### Comparing `expiringsqlitedict-7.0.2/src/expiringsqlitedict/__init__.py` & `expiringsqlitedict-7.0.4/src/expiringsqlitedict/__init__.py`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-7.0.2/test.py` & `expiringsqlitedict-7.0.4/test.py`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-7.0.2/PKG-INFO` & `expiringsqlitedict-7.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: expiringsqlitedict
-Version: 7.0.2
+Version: 7.0.4
 Summary: Persistent compressed expiring dict in Python, backed up by sqlite3 and json
-Author-email: "Taylor C. Richberger" <tcr@absolute-performance.com>
+Author-email: "Taylor C. Richberger" <taylor.richberger@procern.com>
 Requires-Python: >= 3.6, < 4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: orjson ; extra == "test"
 Project-URL: documentation, https://expiringsqlitedict.readthedocs.io/
-Project-URL: repository, https://github.com/absperf/expiringsqlitedict
+Project-URL: repository, https://github.com/ProCern/expiringsqlitedict
 Provides-Extra: test
 
 # expiringsqlitedict -- expiring file-backed `dict`
 
 A lightweight wrapper around Python's sqlite3 database with a MutableMapping
 interface:
```

