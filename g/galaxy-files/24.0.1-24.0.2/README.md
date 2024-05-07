# Comparing `tmp/galaxy_files-24.0.1.tar.gz` & `tmp/galaxy_files-24.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy_files-24.0.1.tar", last modified: Thu May  2 13:47:21 2024, max compression
+gzip compressed data, was "galaxy_files-24.0.2.tar", last modified: Tue May  7 14:32:26 2024, max compression
```

## Comparing `galaxy_files-24.0.1.tar` & `galaxy_files-24.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:21.893414 galaxy_files-24.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-05-02 13:47:21.893414 galaxy_files-24.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:21.889414 galaxy_files-24.0.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:21.889414 galaxy_files-24.0.1/galaxy/files/
--rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:21.893414 galaxy_files-24.0.1/galaxy/files/sources/
--rw-r--r--   0 runner    (1001) docker     (127)    18971 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/_pyfilesystem2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7971 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/_rdm.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/anvil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/base64.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/basespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/drs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/galaxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/googlecloudstorage.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/googledrive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/http.py
--rw-r--r--   0 runner    (1001) docker     (127)    15242 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/invenio.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/onedata.py
--rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/posix.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/s3fs.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/sources/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:21.893414 galaxy_files-24.0.1/galaxy/files/unittest_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/unittest_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/files/uris.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:21.893414 galaxy_files-24.0.1/galaxy_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-05-02 13:47:21.000000 galaxy_files-24.0.1/galaxy_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-02 13:47:21.000000 galaxy_files-24.0.1/galaxy_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:47:21.000000 galaxy_files-24.0.1/galaxy_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 13:47:21.000000 galaxy_files-24.0.1/galaxy_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:47:21.000000 galaxy_files-24.0.1/galaxy_files.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-02 13:47:21.893414 galaxy_files-24.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 13:46:45.000000 galaxy_files-24.0.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:26.497372 galaxy_files-24.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-07 14:31:49.000000 galaxy_files-24.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-05-07 14:32:26.493372 galaxy_files-24.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:26.489372 galaxy_files-24.0.2/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:26.489372 galaxy_files-24.0.2/galaxy/files/
+-rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/galaxy/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:26.493372 galaxy_files-24.0.2/galaxy/files/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)    18971 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/galaxy/files/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/galaxy/files/sources/_pyfilesystem2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7971 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/galaxy/files/sources/_rdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/galaxy/files/sources/anvil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/galaxy/files/sources/base64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/galaxy/files/sources/basespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/galaxy/files/sources/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/galaxy/files/sources/drs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/galaxy/files/sources/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/galaxy/files/sources/galaxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/galaxy/files/sources/googlecloudstorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/galaxy/files/sources/googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/galaxy/files/sources/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15242 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/galaxy/files/sources/invenio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/galaxy/files/sources/onedata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/galaxy/files/sources/posix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/galaxy/files/sources/s3fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/galaxy/files/sources/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/galaxy/files/sources/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:26.493372 galaxy_files-24.0.2/galaxy/files/unittest_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/galaxy/files/unittest_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/galaxy/files/uris.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:26.493372 galaxy_files-24.0.2/galaxy_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-05-07 14:32:26.000000 galaxy_files-24.0.2/galaxy_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-07 14:32:26.000000 galaxy_files-24.0.2/galaxy_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:32:26.000000 galaxy_files-24.0.2/galaxy_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:32:26.000000 galaxy_files-24.0.2/galaxy_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 14:32:26.000000 galaxy_files-24.0.2/galaxy_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-07 14:32:26.497372 galaxy_files-24.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-07 14:31:50.000000 galaxy_files-24.0.2/test-requirements.txt
```

### Comparing `galaxy_files-24.0.1/HISTORY.rst` & `galaxy_files-24.0.2/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.2 (2024-05-07)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 24.0.1 (2024-05-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy_files-24.0.1/LICENSE.txt` & `galaxy_files-24.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `galaxy_files-24.0.1/PKG-INFO` & `galaxy_files-24.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-files
-Version: 24.0.1
+Version: 24.0.2
 Summary: Galaxy file source framework and default plugins
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -46,14 +46,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.2 (2024-05-07)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 24.0.1 (2024-05-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy_files-24.0.1/galaxy/files/__init__.py` & `galaxy_files-24.0.2/galaxy/files/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy_files-24.0.1/galaxy/files/sources/__init__.py` & `galaxy_files-24.0.2/galaxy/files/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy_files-24.0.1/galaxy/files/sources/_pyfilesystem2.py` & `galaxy_files-24.0.2/galaxy/files/sources/_pyfilesystem2.py`

 * *Files identical despite different names*

### Comparing `galaxy_files-24.0.1/galaxy/files/sources/_rdm.py` & `galaxy_files-24.0.2/galaxy/files/sources/_rdm.py`

 * *Files identical despite different names*

### Comparing `galaxy_files-24.0.1/galaxy/files/sources/anvil.py` & `galaxy_files-24.0.2/galaxy/files/sources/anvil.py`

 * *Files identical despite different names*

### Comparing `galaxy_files-24.0.1/galaxy/files/sources/base64.py` & `galaxy_files-24.0.2/galaxy/files/sources/base64.py`

 * *Files identical despite different names*

### Comparing `galaxy_files-24.0.1/galaxy/files/sources/basespace.py` & `galaxy_files-24.0.2/galaxy/files/sources/basespace.py`

 * *Files identical despite different names*

### Comparing `galaxy_files-24.0.1/galaxy/files/sources/dropbox.py` & `galaxy_files-24.0.2/galaxy/files/sources/dropbox.py`

 * *Files identical despite different names*

### Comparing `galaxy_files-24.0.1/galaxy/files/sources/drs.py` & `galaxy_files-24.0.2/galaxy/files/sources/drs.py`

 * *Files identical despite different names*

### Comparing `galaxy_files-24.0.1/galaxy/files/sources/ftp.py` & `galaxy_files-24.0.2/galaxy/files/sources/ftp.py`

 * *Files identical despite different names*

### Comparing `galaxy_files-24.0.1/galaxy/files/sources/galaxy.py` & `galaxy_files-24.0.2/galaxy/files/sources/galaxy.py`

 * *Files identical despite different names*

### Comparing `galaxy_files-24.0.1/galaxy/files/sources/googlecloudstorage.py` & `galaxy_files-24.0.2/galaxy/files/sources/googlecloudstorage.py`

 * *Files identical despite different names*

### Comparing `galaxy_files-24.0.1/galaxy/files/sources/googledrive.py` & `galaxy_files-24.0.2/galaxy/files/sources/googledrive.py`

 * *Files identical despite different names*

### Comparing `galaxy_files-24.0.1/galaxy/files/sources/http.py` & `galaxy_files-24.0.2/galaxy/files/sources/http.py`

 * *Files identical despite different names*

### Comparing `galaxy_files-24.0.1/galaxy/files/sources/invenio.py` & `galaxy_files-24.0.2/galaxy/files/sources/invenio.py`

 * *Files identical despite different names*

### Comparing `galaxy_files-24.0.1/galaxy/files/sources/onedata.py` & `galaxy_files-24.0.2/galaxy/files/sources/onedata.py`

 * *Files identical despite different names*

### Comparing `galaxy_files-24.0.1/galaxy/files/sources/posix.py` & `galaxy_files-24.0.2/galaxy/files/sources/posix.py`

 * *Files identical despite different names*

### Comparing `galaxy_files-24.0.1/galaxy/files/sources/s3fs.py` & `galaxy_files-24.0.2/galaxy/files/sources/s3fs.py`

 * *Files identical despite different names*

### Comparing `galaxy_files-24.0.1/galaxy/files/sources/ssh.py` & `galaxy_files-24.0.2/galaxy/files/sources/ssh.py`

 * *Files identical despite different names*

### Comparing `galaxy_files-24.0.1/galaxy/files/sources/webdav.py` & `galaxy_files-24.0.2/galaxy/files/sources/webdav.py`

 * *Files identical despite different names*

### Comparing `galaxy_files-24.0.1/galaxy/files/unittest_utils/__init__.py` & `galaxy_files-24.0.2/galaxy/files/unittest_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy_files-24.0.1/galaxy/files/uris.py` & `galaxy_files-24.0.2/galaxy/files/uris.py`

 * *Files identical despite different names*

### Comparing `galaxy_files-24.0.1/galaxy_files.egg-info/PKG-INFO` & `galaxy_files-24.0.2/galaxy_files.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-files
-Version: 24.0.1
+Version: 24.0.2
 Summary: Galaxy file source framework and default plugins
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -46,14 +46,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.2 (2024-05-07)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 24.0.1 (2024-05-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy_files-24.0.1/galaxy_files.egg-info/SOURCES.txt` & `galaxy_files-24.0.2/galaxy_files.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy_files-24.0.1/setup.cfg` & `galaxy_files-24.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-files
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.1
+version = 24.0.2
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util
 	fs
 	isal
```

