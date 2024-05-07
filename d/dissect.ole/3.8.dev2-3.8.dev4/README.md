# Comparing `tmp/dissect.ole-3.8.dev2.tar.gz` & `tmp/dissect.ole-3.8.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.ole-3.8.dev2.tar", last modified: Thu Mar 21 10:16:52 2024, max compression
+gzip compressed data, was "dissect.ole-3.8.dev4.tar", last modified: Thu Apr 11 11:57:00 2024, max compression
```

## Comparing `dissect.ole-3.8.dev2.tar` & `dissect.ole-3.8.dev4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:16:52.560888 dissect.ole-3.8.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-21 10:16:42.000000 dissect.ole-3.8.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-21 10:16:42.000000 dissect.ole-3.8.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-21 10:16:42.000000 dissect.ole-3.8.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-03-21 10:16:52.560888 dissect.ole-3.8.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-03-21 10:16:42.000000 dissect.ole-3.8.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:16:52.556888 dissect.ole-3.8.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:16:52.556888 dissect.ole-3.8.dev2/dissect/ole/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-21 10:16:42.000000 dissect.ole-3.8.dev2/dissect/ole/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-03-21 10:16:42.000000 dissect.ole-3.8.dev2/dissect/ole/c_ole.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-21 10:16:42.000000 dissect.ole-3.8.dev2/dissect/ole/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9571 2024-03-21 10:16:42.000000 dissect.ole-3.8.dev2/dissect/ole/ole.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:16:52.560888 dissect.ole-3.8.dev2/dissect.ole.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-03-21 10:16:52.000000 dissect.ole-3.8.dev2/dissect.ole.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-21 10:16:52.000000 dissect.ole-3.8.dev2/dissect.ole.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 10:16:52.000000 dissect.ole-3.8.dev2/dissect.ole.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-21 10:16:52.000000 dissect.ole-3.8.dev2/dissect.ole.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-21 10:16:52.000000 dissect.ole-3.8.dev2/dissect.ole.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-03-21 10:16:47.000000 dissect.ole-3.8.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 10:16:52.560888 dissect.ole-3.8.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:16:52.556888 dissect.ole-3.8.dev2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:16:52.560888 dissect.ole-3.8.dev2/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-21 10:16:42.000000 dissect.ole-3.8.dev2/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-21 10:16:42.000000 dissect.ole-3.8.dev2/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-21 10:16:42.000000 dissect.ole-3.8.dev2/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-03-21 10:16:42.000000 dissect.ole-3.8.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:57:00.681986 dissect.ole-3.8.dev4/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-11 11:56:51.000000 dissect.ole-3.8.dev4/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-11 11:56:51.000000 dissect.ole-3.8.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 11:56:51.000000 dissect.ole-3.8.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-11 11:57:00.681986 dissect.ole-3.8.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-11 11:56:51.000000 dissect.ole-3.8.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:57:00.677986 dissect.ole-3.8.dev4/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:57:00.681986 dissect.ole-3.8.dev4/dissect/ole/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 11:56:51.000000 dissect.ole-3.8.dev4/dissect/ole/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-04-11 11:56:51.000000 dissect.ole-3.8.dev4/dissect/ole/c_ole.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-11 11:56:51.000000 dissect.ole-3.8.dev4/dissect/ole/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9571 2024-04-11 11:56:51.000000 dissect.ole-3.8.dev4/dissect/ole/ole.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:57:00.681986 dissect.ole-3.8.dev4/dissect.ole.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-11 11:57:00.000000 dissect.ole-3.8.dev4/dissect.ole.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-11 11:57:00.000000 dissect.ole-3.8.dev4/dissect.ole.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 11:57:00.000000 dissect.ole-3.8.dev4/dissect.ole.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 11:57:00.000000 dissect.ole-3.8.dev4/dissect.ole.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 11:57:00.000000 dissect.ole-3.8.dev4/dissect.ole.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-11 11:56:55.000000 dissect.ole-3.8.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 11:57:00.681986 dissect.ole-3.8.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:57:00.677986 dissect.ole-3.8.dev4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:57:00.681986 dissect.ole-3.8.dev4/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-11 11:56:51.000000 dissect.ole-3.8.dev4/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-11 11:56:51.000000 dissect.ole-3.8.dev4/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 11:56:51.000000 dissect.ole-3.8.dev4/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-11 11:56:51.000000 dissect.ole-3.8.dev4/tox.ini
```

### Comparing `dissect.ole-3.8.dev2/LICENSE` & `dissect.ole-3.8.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.ole-3.8.dev2/PKG-INFO` & `dissect.ole-3.8.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.ole
-Version: 3.8.dev2
+Version: 3.8.dev4
 Summary: A Dissect module implementing a parser for the Object Linking & Embedding (OLE) format, commonly used by document editors on Windows operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ole
 Project-URL: repository, https://github.com/fox-it/dissect.ole
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.ole-3.8.dev2/README.md` & `dissect.ole-3.8.dev4/README.md`

 * *Files identical despite different names*

### Comparing `dissect.ole-3.8.dev2/dissect/ole/c_ole.py` & `dissect.ole-3.8.dev4/dissect/ole/c_ole.py`

 * *Files identical despite different names*

### Comparing `dissect.ole-3.8.dev2/dissect/ole/ole.py` & `dissect.ole-3.8.dev4/dissect/ole/ole.py`

 * *Files identical despite different names*

### Comparing `dissect.ole-3.8.dev2/dissect.ole.egg-info/PKG-INFO` & `dissect.ole-3.8.dev4/dissect.ole.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.ole
-Version: 3.8.dev2
+Version: 3.8.dev4
 Summary: A Dissect module implementing a parser for the Object Linking & Embedding (OLE) format, commonly used by document editors on Windows operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ole
 Project-URL: repository, https://github.com/fox-it/dissect.ole
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.ole-3.8.dev2/pyproject.toml` & `dissect.ole-3.8.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.ole-3.8.dev2/tests/docs/Makefile` & `dissect.ole-3.8.dev4/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.ole-3.8.dev2/tests/docs/conf.py` & `dissect.ole-3.8.dev4/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.ole-3.8.dev2/tox.ini` & `dissect.ole-3.8.dev4/tox.ini`

 * *Files identical despite different names*

