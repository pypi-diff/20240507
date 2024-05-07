# Comparing `tmp/dsw-config-4.5.0.tar.gz` & `tmp/dsw_config-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsw-config-4.5.0.tar", last modified: Tue Apr  2 10:28:56 2024, max compression
+gzip compressed data, was "dsw_config-4.6.0.tar", last modified: Tue May  7 07:12:48 2024, max compression
```

## Comparing `dsw-config-4.5.0.tar` & `dsw_config-4.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:28:56.862576 dsw-config-4.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-04-02 10:28:52.000000 dsw-config-4.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-02 10:28:56.862576 dsw-config-4.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-02 10:28:52.000000 dsw-config-4.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:28:56.858576 dsw-config-4.5.0/dsw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:28:56.862576 dsw-config-4.5.0/dsw/config/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-02 10:28:52.000000 dsw-config-4.5.0/dsw/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-02 10:28:56.000000 dsw-config-4.5.0/dsw/config/build_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     8472 2024-04-02 10:28:52.000000 dsw-config-4.5.0/dsw/config/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-02 10:28:52.000000 dsw-config-4.5.0/dsw/config/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-04-02 10:28:52.000000 dsw-config-4.5.0/dsw/config/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-02 10:28:52.000000 dsw-config-4.5.0/dsw/config/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-02 10:28:52.000000 dsw-config-4.5.0/dsw/config/sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:28:56.862576 dsw-config-4.5.0/dsw_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-02 10:28:56.000000 dsw-config-4.5.0/dsw_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-02 10:28:56.000000 dsw-config-4.5.0/dsw_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:28:56.000000 dsw-config-4.5.0/dsw_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:28:56.000000 dsw-config-4.5.0/dsw_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 10:28:56.000000 dsw-config-4.5.0/dsw_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 10:28:56.000000 dsw-config-4.5.0/dsw_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-02 10:28:52.000000 dsw-config-4.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:28:56.862576 dsw-config-4.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:28:52.000000 dsw-config-4.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:48.889741 dsw_config-4.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-07 07:12:44.000000 dsw_config-4.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-07 07:12:48.889741 dsw_config-4.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-07 07:12:44.000000 dsw_config-4.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:48.885741 dsw_config-4.6.0/dsw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:48.889741 dsw_config-4.6.0/dsw/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-07 07:12:44.000000 dsw_config-4.6.0/dsw/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 07:12:48.000000 dsw_config-4.6.0/dsw/config/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8472 2024-05-07 07:12:44.000000 dsw_config-4.6.0/dsw/config/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-07 07:12:44.000000 dsw_config-4.6.0/dsw/config/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-05-07 07:12:44.000000 dsw_config-4.6.0/dsw/config/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-07 07:12:44.000000 dsw_config-4.6.0/dsw/config/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-07 07:12:44.000000 dsw_config-4.6.0/dsw/config/sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:48.889741 dsw_config-4.6.0/dsw_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-07 07:12:48.000000 dsw_config-4.6.0/dsw_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-07 07:12:48.000000 dsw_config-4.6.0/dsw_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:12:48.000000 dsw_config-4.6.0/dsw_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:12:48.000000 dsw_config-4.6.0/dsw_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 07:12:48.000000 dsw_config-4.6.0/dsw_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-07 07:12:48.000000 dsw_config-4.6.0/dsw_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-07 07:12:44.000000 dsw_config-4.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:12:48.889741 dsw_config-4.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:12:44.000000 dsw_config-4.6.0/setup.py
```

### Comparing `dsw-config-4.5.0/LICENSE` & `dsw_config-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsw-config-4.5.0/PKG-INFO` & `dsw_config-4.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-config
-Version: 4.5.0
+Version: 4.6.0
 Summary: Library for DSW config manipulation
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,config,yaml,parser
```

### Comparing `dsw-config-4.5.0/README.md` & `dsw_config-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dsw-config-4.5.0/dsw/config/keys.py` & `dsw_config-4.6.0/dsw/config/keys.py`

 * *Files identical despite different names*

### Comparing `dsw-config-4.5.0/dsw/config/logging.py` & `dsw_config-4.6.0/dsw/config/logging.py`

 * *Files identical despite different names*

### Comparing `dsw-config-4.5.0/dsw/config/model.py` & `dsw_config-4.6.0/dsw/config/model.py`

 * *Files identical despite different names*

### Comparing `dsw-config-4.5.0/dsw/config/parser.py` & `dsw_config-4.6.0/dsw/config/parser.py`

 * *Files identical despite different names*

### Comparing `dsw-config-4.5.0/dsw/config/sentry.py` & `dsw_config-4.6.0/dsw/config/sentry.py`

 * *Files identical despite different names*

### Comparing `dsw-config-4.5.0/dsw_config.egg-info/PKG-INFO` & `dsw_config-4.6.0/dsw_config.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-config
-Version: 4.5.0
+Version: 4.6.0
 Summary: Library for DSW config manipulation
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,config,yaml,parser
```

### Comparing `dsw-config-4.5.0/pyproject.toml` & `dsw_config-4.6.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'dsw-config'
-version = "4.5.0"
+version = "4.6.0"
 description = 'Library for DSW config manipulation'
 readme = 'README.md'
 keywords = ['dsw', 'config', 'yaml', 'parser']
 license = { text = 'Apache License 2.0' }
 authors = [
     { name = 'Marek Suchánek', email = 'marek.suchanek@ds-wizard.org' }
 ]
```

