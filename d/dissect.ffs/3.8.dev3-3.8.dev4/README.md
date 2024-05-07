# Comparing `tmp/dissect.ffs-3.8.dev3.tar.gz` & `tmp/dissect.ffs-3.8.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.ffs-3.8.dev3.tar", last modified: Thu Mar 28 17:22:05 2024, max compression
+gzip compressed data, was "dissect.ffs-3.8.dev4.tar", last modified: Thu Apr 11 11:56:50 2024, max compression
```

## Comparing `dissect.ffs-3.8.dev3.tar` & `dissect.ffs-3.8.dev4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:05.743808 dissect.ffs-3.8.dev3/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-28 17:21:51.000000 dissect.ffs-3.8.dev3/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-28 17:21:51.000000 dissect.ffs-3.8.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-28 17:21:51.000000 dissect.ffs-3.8.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-03-28 17:22:05.743808 dissect.ffs-3.8.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-28 17:21:51.000000 dissect.ffs-3.8.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:05.735808 dissect.ffs-3.8.dev3/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:05.739808 dissect.ffs-3.8.dev3/dissect/ffs/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-28 17:21:51.000000 dissect.ffs-3.8.dev3/dissect/ffs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-03-28 17:21:51.000000 dissect.ffs-3.8.dev3/dissect/ffs/c_ffs.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-28 17:21:51.000000 dissect.ffs-3.8.dev3/dissect/ffs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13006 2024-03-28 17:21:51.000000 dissect.ffs-3.8.dev3/dissect/ffs/ffs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:05.743808 dissect.ffs-3.8.dev3/dissect.ffs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-03-28 17:22:05.000000 dissect.ffs-3.8.dev3/dissect.ffs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-28 17:22:05.000000 dissect.ffs-3.8.dev3/dissect.ffs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:22:05.000000 dissect.ffs-3.8.dev3/dissect.ffs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 17:22:05.000000 dissect.ffs-3.8.dev3/dissect.ffs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-28 17:22:05.000000 dissect.ffs-3.8.dev3/dissect.ffs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-03-28 17:22:00.000000 dissect.ffs-3.8.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 17:22:05.743808 dissect.ffs-3.8.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:05.739808 dissect.ffs-3.8.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:51.000000 dissect.ffs-3.8.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-28 17:21:51.000000 dissect.ffs-3.8.dev3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:05.739808 dissect.ffs-3.8.dev3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    14565 2024-03-28 17:21:51.000000 dissect.ffs-3.8.dev3/tests/data/ffs.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    16364 2024-03-28 17:21:51.000000 dissect.ffs-3.8.dev3/tests/data/ffs_symlink_test1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    16084 2024-03-28 17:21:51.000000 dissect.ffs-3.8.dev3/tests/data/ffs_symlink_test2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    16113 2024-03-28 17:21:51.000000 dissect.ffs-3.8.dev3/tests/data/ffs_symlink_test3.bin.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:05.743808 dissect.ffs-3.8.dev3/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-28 17:21:51.000000 dissect.ffs-3.8.dev3/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-28 17:21:51.000000 dissect.ffs-3.8.dev3/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-28 17:21:51.000000 dissect.ffs-3.8.dev3/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-03-28 17:21:51.000000 dissect.ffs-3.8.dev3/tests/test_ffs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-28 17:21:51.000000 dissect.ffs-3.8.dev3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:50.272657 dissect.ffs-3.8.dev4/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-11 11:56:41.000000 dissect.ffs-3.8.dev4/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-11 11:56:41.000000 dissect.ffs-3.8.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 11:56:41.000000 dissect.ffs-3.8.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-11 11:56:50.272657 dissect.ffs-3.8.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-11 11:56:41.000000 dissect.ffs-3.8.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:50.268657 dissect.ffs-3.8.dev4/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:50.272657 dissect.ffs-3.8.dev4/dissect/ffs/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-11 11:56:41.000000 dissect.ffs-3.8.dev4/dissect/ffs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-04-11 11:56:41.000000 dissect.ffs-3.8.dev4/dissect/ffs/c_ffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-11 11:56:41.000000 dissect.ffs-3.8.dev4/dissect/ffs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13006 2024-04-11 11:56:41.000000 dissect.ffs-3.8.dev4/dissect/ffs/ffs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:50.272657 dissect.ffs-3.8.dev4/dissect.ffs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-11 11:56:50.000000 dissect.ffs-3.8.dev4/dissect.ffs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-11 11:56:50.000000 dissect.ffs-3.8.dev4/dissect.ffs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 11:56:50.000000 dissect.ffs-3.8.dev4/dissect.ffs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 11:56:50.000000 dissect.ffs-3.8.dev4/dissect.ffs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 11:56:50.000000 dissect.ffs-3.8.dev4/dissect.ffs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-11 11:56:45.000000 dissect.ffs-3.8.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 11:56:50.272657 dissect.ffs-3.8.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:50.272657 dissect.ffs-3.8.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:41.000000 dissect.ffs-3.8.dev4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-11 11:56:41.000000 dissect.ffs-3.8.dev4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:50.272657 dissect.ffs-3.8.dev4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    14565 2024-04-11 11:56:41.000000 dissect.ffs-3.8.dev4/tests/data/ffs.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    16364 2024-04-11 11:56:41.000000 dissect.ffs-3.8.dev4/tests/data/ffs_symlink_test1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    16084 2024-04-11 11:56:41.000000 dissect.ffs-3.8.dev4/tests/data/ffs_symlink_test2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    16113 2024-04-11 11:56:41.000000 dissect.ffs-3.8.dev4/tests/data/ffs_symlink_test3.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:50.272657 dissect.ffs-3.8.dev4/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-11 11:56:41.000000 dissect.ffs-3.8.dev4/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-11 11:56:41.000000 dissect.ffs-3.8.dev4/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 11:56:41.000000 dissect.ffs-3.8.dev4/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-11 11:56:41.000000 dissect.ffs-3.8.dev4/tests/test_ffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-11 11:56:41.000000 dissect.ffs-3.8.dev4/tox.ini
```

### Comparing `dissect.ffs-3.8.dev3/LICENSE` & `dissect.ffs-3.8.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.8.dev3/PKG-INFO` & `dissect.ffs-3.8.dev4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.ffs
-Version: 3.8.dev3
+Version: 3.8.dev4
 Summary: A Dissect module implementing a parser for the FFS file system, commonly used by BSD operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ffs
 Project-URL: repository, https://github.com/fox-it/dissect.ffs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.ffs-3.8.dev3/README.md` & `dissect.ffs-3.8.dev4/README.md`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.8.dev3/dissect/ffs/c_ffs.py` & `dissect.ffs-3.8.dev4/dissect/ffs/c_ffs.py`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.8.dev3/dissect/ffs/ffs.py` & `dissect.ffs-3.8.dev4/dissect/ffs/ffs.py`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.8.dev3/dissect.ffs.egg-info/PKG-INFO` & `dissect.ffs-3.8.dev4/dissect.ffs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.ffs
-Version: 3.8.dev3
+Version: 3.8.dev4
 Summary: A Dissect module implementing a parser for the FFS file system, commonly used by BSD operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ffs
 Project-URL: repository, https://github.com/fox-it/dissect.ffs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.ffs-3.8.dev3/dissect.ffs.egg-info/SOURCES.txt` & `dissect.ffs-3.8.dev4/dissect.ffs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.8.dev3/pyproject.toml` & `dissect.ffs-3.8.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.8.dev3/tests/data/ffs.bin.gz` & `dissect.ffs-3.8.dev4/tests/data/ffs.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.8.dev3/tests/data/ffs_symlink_test1.bin.gz` & `dissect.ffs-3.8.dev4/tests/data/ffs_symlink_test1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.8.dev3/tests/data/ffs_symlink_test2.bin.gz` & `dissect.ffs-3.8.dev4/tests/data/ffs_symlink_test2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.8.dev3/tests/data/ffs_symlink_test3.bin.gz` & `dissect.ffs-3.8.dev4/tests/data/ffs_symlink_test3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.8.dev3/tests/docs/Makefile` & `dissect.ffs-3.8.dev4/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.8.dev3/tests/docs/conf.py` & `dissect.ffs-3.8.dev4/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.8.dev3/tests/test_ffs.py` & `dissect.ffs-3.8.dev4/tests/test_ffs.py`

 * *Files identical despite different names*

### Comparing `dissect.ffs-3.8.dev3/tox.ini` & `dissect.ffs-3.8.dev4/tox.ini`

 * *Files identical despite different names*

