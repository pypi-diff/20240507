# Comparing `tmp/galaxy_auth-24.0.1.tar.gz` & `tmp/galaxy_auth-24.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy_auth-24.0.1.tar", last modified: Thu May  2 13:48:55 2024, max compression
+gzip compressed data, was "galaxy_auth-24.0.2.tar", last modified: Tue May  7 14:34:01 2024, max compression
```

## Comparing `galaxy_auth-24.0.1.tar` & `galaxy_auth-24.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:55.085936 galaxy_auth-24.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-02 13:48:55.085936 galaxy_auth-24.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:55.081936 galaxy_auth-24.0.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:55.081936 galaxy_auth-24.0.1/galaxy/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/galaxy/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:55.085936 galaxy_auth-24.0.1/galaxy/auth/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/galaxy/auth/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/galaxy/auth/providers/alwaysreject.py
--rw-r--r--   0 runner    (1001) docker     (127)    18512 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/galaxy/auth/providers/ldap_ad.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/galaxy/auth/providers/localdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/galaxy/auth/providers/pam_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/galaxy/auth/util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:55.085936 galaxy_auth-24.0.1/galaxy_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-02 13:48:55.000000 galaxy_auth-24.0.1/galaxy_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-02 13:48:55.000000 galaxy_auth-24.0.1/galaxy_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:48:55.000000 galaxy_auth-24.0.1/galaxy_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-02 13:48:55.000000 galaxy_auth-24.0.1/galaxy_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:48:55.000000 galaxy_auth-24.0.1/galaxy_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-02 13:48:55.085936 galaxy_auth-24.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:01.212763 galaxy_auth-24.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-07 14:31:50.000000 galaxy_auth-24.0.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-07 14:31:49.000000 galaxy_auth-24.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 14:31:50.000000 galaxy_auth-24.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-07 14:34:01.212763 galaxy_auth-24.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-07 14:31:50.000000 galaxy_auth-24.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 14:31:50.000000 galaxy_auth-24.0.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:01.208763 galaxy_auth-24.0.2/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-07 14:31:50.000000 galaxy_auth-24.0.2/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:01.208763 galaxy_auth-24.0.2/galaxy/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-05-07 14:31:50.000000 galaxy_auth-24.0.2/galaxy/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:01.208763 galaxy_auth-24.0.2/galaxy/auth/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-07 14:31:50.000000 galaxy_auth-24.0.2/galaxy/auth/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-07 14:31:50.000000 galaxy_auth-24.0.2/galaxy/auth/providers/alwaysreject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18512 2024-05-07 14:31:50.000000 galaxy_auth-24.0.2/galaxy/auth/providers/ldap_ad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-07 14:31:50.000000 galaxy_auth-24.0.2/galaxy/auth/providers/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-05-07 14:31:50.000000 galaxy_auth-24.0.2/galaxy/auth/providers/pam_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-07 14:31:50.000000 galaxy_auth-24.0.2/galaxy/auth/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:31:50.000000 galaxy_auth-24.0.2/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:01.212763 galaxy_auth-24.0.2/galaxy_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-07 14:34:01.000000 galaxy_auth-24.0.2/galaxy_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-07 14:34:01.000000 galaxy_auth-24.0.2/galaxy_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:34:01.000000 galaxy_auth-24.0.2/galaxy_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-07 14:34:01.000000 galaxy_auth-24.0.2/galaxy_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 14:34:01.000000 galaxy_auth-24.0.2/galaxy_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 14:31:50.000000 galaxy_auth-24.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-07 14:34:01.212763 galaxy_auth-24.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 14:31:50.000000 galaxy_auth-24.0.2/test-requirements.txt
```

### Comparing `galaxy_auth-24.0.1/HISTORY.rst` & `galaxy_auth-24.0.2/HISTORY.rst`

 * *Files 8% similar despite different names*

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
 
 No recorded changes since last release
 
 -------------------
 24.0.0 (2024-04-02)
```

### Comparing `galaxy_auth-24.0.1/LICENSE` & `galaxy_auth-24.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy_auth-24.0.1/PKG-INFO` & `galaxy_auth-24.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-auth
-Version: 24.0.1
+Version: 24.0.2
 Summary: Galaxy auth framework and implementations
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,14 +45,20 @@
 
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
 
 No recorded changes since last release
 
 -------------------
 24.0.0 (2024-04-02)
```

### Comparing `galaxy_auth-24.0.1/galaxy/auth/__init__.py` & `galaxy_auth-24.0.2/galaxy/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy_auth-24.0.1/galaxy/auth/providers/__init__.py` & `galaxy_auth-24.0.2/galaxy/auth/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy_auth-24.0.1/galaxy/auth/providers/alwaysreject.py` & `galaxy_auth-24.0.2/galaxy/auth/providers/alwaysreject.py`

 * *Files identical despite different names*

### Comparing `galaxy_auth-24.0.1/galaxy/auth/providers/ldap_ad.py` & `galaxy_auth-24.0.2/galaxy/auth/providers/ldap_ad.py`

 * *Files identical despite different names*

### Comparing `galaxy_auth-24.0.1/galaxy/auth/providers/localdb.py` & `galaxy_auth-24.0.2/galaxy/auth/providers/localdb.py`

 * *Files identical despite different names*

### Comparing `galaxy_auth-24.0.1/galaxy/auth/providers/pam_auth.py` & `galaxy_auth-24.0.2/galaxy/auth/providers/pam_auth.py`

 * *Files identical despite different names*

### Comparing `galaxy_auth-24.0.1/galaxy/auth/util.py` & `galaxy_auth-24.0.2/galaxy/auth/util.py`

 * *Files identical despite different names*

### Comparing `galaxy_auth-24.0.1/galaxy_auth.egg-info/PKG-INFO` & `galaxy_auth-24.0.2/galaxy_auth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-auth
-Version: 24.0.1
+Version: 24.0.2
 Summary: Galaxy auth framework and implementations
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,14 +45,20 @@
 
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
 
 No recorded changes since last release
 
 -------------------
 24.0.0 (2024-04-02)
```

### Comparing `galaxy_auth-24.0.1/galaxy_auth.egg-info/SOURCES.txt` & `galaxy_auth-24.0.2/galaxy_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy_auth-24.0.1/setup.cfg` & `galaxy_auth-24.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-auth
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.1
+version = 24.0.2
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-data
 	galaxy-util
 packages = find:
```

