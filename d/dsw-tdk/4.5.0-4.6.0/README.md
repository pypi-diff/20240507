# Comparing `tmp/dsw-tdk-4.5.0.tar.gz` & `tmp/dsw_tdk-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsw-tdk-4.5.0.tar", last modified: Tue Apr  2 10:29:22 2024, max compression
+gzip compressed data, was "dsw_tdk-4.6.0.tar", last modified: Tue May  7 07:12:54 2024, max compression
```

## Comparing `dsw-tdk-4.5.0.tar` & `dsw_tdk-4.6.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:29:22.289680 dsw-tdk-4.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-02 10:29:22.289680 dsw-tdk-4.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:29:22.277680 dsw-tdk-4.5.0/dsw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:29:22.281680 dsw-tdk-4.5.0/dsw/tdk/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14222 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-02 10:29:21.000000 dsw-tdk-4.5.0/dsw/tdk/build_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    21676 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)    25930 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    17235 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:29:22.285680 dsw-tdk-4.5.0/dsw/tdk/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/templates/LICENSE.j2
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/templates/README.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/templates/env.j2
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/templates/starter.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:29:22.285680 dsw-tdk-4.5.0/dsw_tdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-02 10:29:22.000000 dsw-tdk-4.5.0/dsw_tdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-02 10:29:22.000000 dsw-tdk-4.5.0/dsw_tdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:29:22.000000 dsw-tdk-4.5.0/dsw_tdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 10:29:22.000000 dsw-tdk-4.5.0/dsw_tdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:29:22.000000 dsw-tdk-4.5.0/dsw_tdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-02 10:29:22.000000 dsw-tdk-4.5.0/dsw_tdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 10:29:22.000000 dsw-tdk-4.5.0/dsw_tdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:29:22.289680 dsw-tdk-4.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:29:22.285680 dsw-tdk-4.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/tests/test_cmd_dot-env.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/tests/test_cmd_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/tests/test_cmd_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/tests/test_cmd_new.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/tests/test_cmd_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/tests/test_cmd_put.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/tests/test_cmd_unpackage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/tests/test_cmd_verify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:54.206779 dsw_tdk-4.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8693 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-07 07:12:54.206779 dsw_tdk-4.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:54.198779 dsw_tdk-4.6.0/dsw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:54.202779 dsw_tdk-4.6.0/dsw/tdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/dsw/tdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/dsw/tdk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14222 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/dsw/tdk/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 07:12:53.000000 dsw_tdk-4.6.0/dsw/tdk/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21676 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/dsw/tdk/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/dsw/tdk/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25930 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/dsw/tdk/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17235 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/dsw/tdk/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:54.202779 dsw_tdk-4.6.0/dsw/tdk/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/dsw/tdk/templates/LICENSE.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/dsw/tdk/templates/README.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/dsw/tdk/templates/env.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/dsw/tdk/templates/starter.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/dsw/tdk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/dsw/tdk/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:54.202779 dsw_tdk-4.6.0/dsw_tdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-07 07:12:54.000000 dsw_tdk-4.6.0/dsw_tdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-07 07:12:54.000000 dsw_tdk-4.6.0/dsw_tdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:12:54.000000 dsw_tdk-4.6.0/dsw_tdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 07:12:54.000000 dsw_tdk-4.6.0/dsw_tdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:12:54.000000 dsw_tdk-4.6.0/dsw_tdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-07 07:12:54.000000 dsw_tdk-4.6.0/dsw_tdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-07 07:12:54.000000 dsw_tdk-4.6.0/dsw_tdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:12:54.206779 dsw_tdk-4.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:54.202779 dsw_tdk-4.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/tests/test_cmd_dot-env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/tests/test_cmd_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/tests/test_cmd_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/tests/test_cmd_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/tests/test_cmd_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/tests/test_cmd_put.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/tests/test_cmd_unpackage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-07 07:12:46.000000 dsw_tdk-4.6.0/tests/test_cmd_verify.py
```

### Comparing `dsw-tdk-4.5.0/CHANGELOG.md` & `dsw_tdk-4.6.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 
+## [4.6.0]
+
+Released for version consistency with other DSW tools.
+
 ## [4.5.0]
 
 Released for version consistency with other DSW tools.
 
 ## [4.4.1]
 
 Released for version consistency with other DSW tools.
@@ -415,7 +419,8 @@
 [4.2.0]: /../../tree/v4.2.0
 [4.2.1]: /../../tree/v4.2.1
 [4.3.0]: /../../tree/v4.3.0
 [4.3.1]: /../../tree/v4.3.1
 [4.4.0]: /../../tree/v4.4.0
 [4.4.1]: /../../tree/v4.4.1
 [4.5.0]: /../../tree/v4.5.0
+[4.6.0]: /../../tree/v4.6.0
```

### Comparing `dsw-tdk-4.5.0/LICENSE` & `dsw_tdk-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.5.0/PKG-INFO` & `dsw_tdk-4.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-tdk
-Version: 4.5.0
+Version: 4.6.0
 Summary: Data Stewardship Wizard Template Development Toolkit
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: documents,dsw,jinja2,template,toolkit
```

### Comparing `dsw-tdk-4.5.0/README.md` & `dsw_tdk-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.5.0/dsw/tdk/api_client.py` & `dsw_tdk-4.6.0/dsw/tdk/api_client.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.5.0/dsw/tdk/cli.py` & `dsw_tdk-4.6.0/dsw/tdk/cli.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.5.0/dsw/tdk/consts.py` & `dsw_tdk-4.6.0/dsw/tdk/consts.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.5.0/dsw/tdk/core.py` & `dsw_tdk-4.6.0/dsw/tdk/core.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.5.0/dsw/tdk/model.py` & `dsw_tdk-4.6.0/dsw/tdk/model.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.5.0/dsw/tdk/utils.py` & `dsw_tdk-4.6.0/dsw/tdk/utils.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.5.0/dsw/tdk/validation.py` & `dsw_tdk-4.6.0/dsw/tdk/validation.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.5.0/dsw_tdk.egg-info/PKG-INFO` & `dsw_tdk-4.6.0/dsw_tdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-tdk
-Version: 4.5.0
+Version: 4.6.0
 Summary: Data Stewardship Wizard Template Development Toolkit
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: documents,dsw,jinja2,template,toolkit
```

### Comparing `dsw-tdk-4.5.0/dsw_tdk.egg-info/SOURCES.txt` & `dsw_tdk-4.6.0/dsw_tdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.5.0/pyproject.toml` & `dsw_tdk-4.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'dsw-tdk'
-version = "4.5.0"
+version = "4.6.0"
 description = 'Data Stewardship Wizard Template Development Toolkit'
 readme = 'README.md'
 keywords = ['documents', 'dsw', 'jinja2', 'template', 'toolkit']
 license = { text = 'Apache License 2.0' }
 authors = [
     { name = 'Marek Suchánek', email = 'marek.suchanek@ds-wizard.org' }
 ]
```

### Comparing `dsw-tdk-4.5.0/tests/test_basic.py` & `dsw_tdk-4.6.0/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.5.0/tests/test_cmd_dot-env.py` & `dsw_tdk-4.6.0/tests/test_cmd_dot-env.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.5.0/tests/test_cmd_get.py` & `dsw_tdk-4.6.0/tests/test_cmd_get.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.5.0/tests/test_cmd_list.py` & `dsw_tdk-4.6.0/tests/test_cmd_list.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.5.0/tests/test_cmd_new.py` & `dsw_tdk-4.6.0/tests/test_cmd_new.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.5.0/tests/test_cmd_package.py` & `dsw_tdk-4.6.0/tests/test_cmd_package.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.5.0/tests/test_cmd_put.py` & `dsw_tdk-4.6.0/tests/test_cmd_put.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.5.0/tests/test_cmd_unpackage.py` & `dsw_tdk-4.6.0/tests/test_cmd_unpackage.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.5.0/tests/test_cmd_verify.py` & `dsw_tdk-4.6.0/tests/test_cmd_verify.py`

 * *Files identical despite different names*

