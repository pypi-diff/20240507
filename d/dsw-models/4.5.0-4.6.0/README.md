# Comparing `tmp/dsw-models-4.5.0.tar.gz` & `tmp/dsw_models-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsw-models-4.5.0.tar", last modified: Tue Apr  2 10:29:04 2024, max compression
+gzip compressed data, was "dsw_models-4.6.0.tar", last modified: Tue May  7 07:12:47 2024, max compression
```

## Comparing `dsw-models-4.5.0.tar` & `dsw_models-4.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:29:04.526499 dsw-models-4.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-04-02 10:28:59.000000 dsw-models-4.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-02 10:29:04.526499 dsw-models-4.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-02 10:28:59.000000 dsw-models-4.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:29:04.522499 dsw-models-4.5.0/dsw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:29:04.522499 dsw-models-4.5.0/dsw/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 10:28:59.000000 dsw-models-4.5.0/dsw/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-02 10:29:04.000000 dsw-models-4.5.0/dsw/models/build_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-02 10:28:59.000000 dsw-models-4.5.0/dsw/models/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:29:04.526499 dsw-models-4.5.0/dsw/models/km/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 10:28:59.000000 dsw-models-4.5.0/dsw/models/km/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    90509 2024-04-02 10:28:59.000000 dsw-models-4.5.0/dsw/models/km/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-02 10:28:59.000000 dsw-models-4.5.0/dsw/models/km/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:29:04.526499 dsw-models-4.5.0/dsw_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-02 10:29:04.000000 dsw-models-4.5.0/dsw_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-02 10:29:04.000000 dsw-models-4.5.0/dsw_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:29:04.000000 dsw-models-4.5.0/dsw_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:29:04.000000 dsw-models-4.5.0/dsw_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 10:29:04.000000 dsw-models-4.5.0/dsw_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-02 10:28:59.000000 dsw-models-4.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:29:04.526499 dsw-models-4.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:28:59.000000 dsw-models-4.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:47.726654 dsw_models-4.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-07 07:12:43.000000 dsw_models-4.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-07 07:12:47.726654 dsw_models-4.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-07 07:12:43.000000 dsw_models-4.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:47.722654 dsw_models-4.6.0/dsw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:47.722654 dsw_models-4.6.0/dsw/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:43.000000 dsw_models-4.6.0/dsw/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 07:12:47.000000 dsw_models-4.6.0/dsw/models/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-07 07:12:43.000000 dsw_models-4.6.0/dsw/models/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:47.722654 dsw_models-4.6.0/dsw/models/km/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:43.000000 dsw_models-4.6.0/dsw/models/km/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90509 2024-05-07 07:12:43.000000 dsw_models-4.6.0/dsw/models/km/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-07 07:12:43.000000 dsw_models-4.6.0/dsw/models/km/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:47.726654 dsw_models-4.6.0/dsw_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-07 07:12:47.000000 dsw_models-4.6.0/dsw_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-07 07:12:47.000000 dsw_models-4.6.0/dsw_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:12:47.000000 dsw_models-4.6.0/dsw_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:12:47.000000 dsw_models-4.6.0/dsw_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-07 07:12:47.000000 dsw_models-4.6.0/dsw_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-07 07:12:43.000000 dsw_models-4.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:12:47.726654 dsw_models-4.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:12:43.000000 dsw_models-4.6.0/setup.py
```

### Comparing `dsw-models-4.5.0/LICENSE` & `dsw_models-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsw-models-4.5.0/PKG-INFO` & `dsw_models-4.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-models
-Version: 4.5.0
+Version: 4.6.0
 Summary: Library with DSW models and basic IO operations
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,config,yaml,parser
```

### Comparing `dsw-models-4.5.0/README.md` & `dsw_models-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dsw-models-4.5.0/dsw/models/km/events.py` & `dsw_models-4.6.0/dsw/models/km/events.py`

 * *Files identical despite different names*

### Comparing `dsw-models-4.5.0/dsw/models/km/package.py` & `dsw_models-4.6.0/dsw/models/km/package.py`

 * *Files identical despite different names*

### Comparing `dsw-models-4.5.0/dsw_models.egg-info/PKG-INFO` & `dsw_models-4.6.0/dsw_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-models
-Version: 4.5.0
+Version: 4.6.0
 Summary: Library with DSW models and basic IO operations
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,config,yaml,parser
```

### Comparing `dsw-models-4.5.0/pyproject.toml` & `dsw_models-4.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'dsw-models'
-version = "4.5.0"
+version = "4.6.0"
 description = 'Library with DSW models and basic IO operations'
 readme = 'README.md'
 keywords = ['dsw', 'config', 'yaml', 'parser']
 license = { text = 'Apache License 2.0' }
 authors = [
     { name = 'Marek Suchánek', email = 'marek.suchanek@ds-wizard.org' }
 ]
```

