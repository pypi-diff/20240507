# Comparing `tmp/ftrack_framework_core-2.2.0.tar.gz` & `tmp/ftrack_framework_core-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftrack_framework_core-2.2.0.tar", max compression
+gzip compressed data, was "ftrack_framework_core-2.2.1.tar", max compression
```

## Comparing `ftrack_framework_core-2.2.0.tar` & `ftrack_framework_core-2.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    10176 2024-05-02 08:07:31.883972 ftrack_framework_core-2.2.0/LICENSE.txt
--rw-r--r--   0        0        0      177 2024-05-02 08:07:31.883972 ftrack_framework_core-2.2.0/README.md
--rw-r--r--   0        0        0     1196 2024-05-02 08:07:31.883972 ftrack_framework_core-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      566 2024-05-02 08:07:31.883972 ftrack_framework_core-2.2.0/source/ftrack_framework_core/__init__.py
--rw-r--r--   0        0        0     6749 2024-05-02 08:07:31.883972 ftrack_framework_core-2.2.0/source/ftrack_framework_core/asset/__init__.py
--rw-r--r--   0        0        0     7568 2024-05-02 08:07:31.883972 ftrack_framework_core-2.2.0/source/ftrack_framework_core/asset/asset_info.py
--rw-r--r--   0        0        0     4130 2024-05-02 08:07:31.883972 ftrack_framework_core-2.2.0/source/ftrack_framework_core/asset/dcc_object.py
--rw-r--r--   0        0        0    17702 2024-05-02 08:07:31.883972 ftrack_framework_core-2.2.0/source/ftrack_framework_core/client/__init__.py
--rw-r--r--   0        0        0     8631 2024-05-02 08:07:31.883972 ftrack_framework_core-2.2.0/source/ftrack_framework_core/client/host_connection.py
--rw-r--r--   0        0        0     4603 2024-05-02 08:07:31.883972 ftrack_framework_core-2.2.0/source/ftrack_framework_core/configure_logging.py
--rw-r--r--   0        0        0     9330 2024-05-02 08:07:31.883972 ftrack_framework_core-2.2.0/source/ftrack_framework_core/engine/__init__.py
--rw-r--r--   0        0        0    17206 2024-05-02 08:07:31.883972 ftrack_framework_core-2.2.0/source/ftrack_framework_core/event/__init__.py
--rw-r--r--   0        0        0      162 2024-05-02 08:07:31.883972 ftrack_framework_core-2.2.0/source/ftrack_framework_core/exceptions/__init__.py
--rw-r--r--   0        0        0      277 2024-05-02 08:07:31.883972 ftrack_framework_core-2.2.0/source/ftrack_framework_core/exceptions/engine.py
--rw-r--r--   0        0        0     1501 2024-05-02 08:07:31.883972 ftrack_framework_core-2.2.0/source/ftrack_framework_core/exceptions/plugin.py
--rw-r--r--   0        0        0    12705 2024-05-02 08:07:31.883972 ftrack_framework_core-2.2.0/source/ftrack_framework_core/host/__init__.py
--rw-r--r--   0        0        0     8625 2024-05-02 08:07:31.883972 ftrack_framework_core-2.2.0/source/ftrack_framework_core/log/__init__.py
--rw-r--r--   0        0        0     1184 2024-05-02 08:07:31.883972 ftrack_framework_core-2.2.0/source/ftrack_framework_core/log/log_item.py
--rw-r--r--   0        0        0     1831 2024-05-02 08:07:31.883972 ftrack_framework_core-2.2.0/source/ftrack_framework_core/plugin/__init__.py
--rw-r--r--   0        0        0     1975 2024-05-02 08:07:31.883972 ftrack_framework_core-2.2.0/source/ftrack_framework_core/plugin/plugin_info.py
--rw-r--r--   0        0        0     7983 2024-05-02 08:07:31.883972 ftrack_framework_core-2.2.0/source/ftrack_framework_core/registry/__init__.py
--rw-r--r--   0        0        0     3437 2024-05-02 08:07:31.883972 ftrack_framework_core-2.2.0/source/ftrack_framework_core/widget/__init__.py
--rw-r--r--   0        0        0    17207 2024-05-02 08:07:31.883972 ftrack_framework_core-2.2.0/source/ftrack_framework_core/widget/dialog.py
--rw-r--r--   0        0        0     4475 2024-05-02 08:07:31.883972 ftrack_framework_core-2.2.0/source/ftrack_framework_core/widget/widget.py
--rw-r--r--   0        0        0     1268 1970-01-01 00:00:00.000000 ftrack_framework_core-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10176 2024-05-07 07:52:37.229764 ftrack_framework_core-2.2.1/LICENSE.txt
+-rw-r--r--   0        0        0      177 2024-05-07 07:52:37.229764 ftrack_framework_core-2.2.1/README.md
+-rw-r--r--   0        0        0     1196 2024-05-07 07:52:37.229764 ftrack_framework_core-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0      566 2024-05-07 07:52:37.229764 ftrack_framework_core-2.2.1/source/ftrack_framework_core/__init__.py
+-rw-r--r--   0        0        0     6749 2024-05-07 07:52:37.229764 ftrack_framework_core-2.2.1/source/ftrack_framework_core/asset/__init__.py
+-rw-r--r--   0        0        0     7568 2024-05-07 07:52:37.229764 ftrack_framework_core-2.2.1/source/ftrack_framework_core/asset/asset_info.py
+-rw-r--r--   0        0        0     4130 2024-05-07 07:52:37.229764 ftrack_framework_core-2.2.1/source/ftrack_framework_core/asset/dcc_object.py
+-rw-r--r--   0        0        0    17702 2024-05-07 07:52:37.229764 ftrack_framework_core-2.2.1/source/ftrack_framework_core/client/__init__.py
+-rw-r--r--   0        0        0     8631 2024-05-07 07:52:37.229764 ftrack_framework_core-2.2.1/source/ftrack_framework_core/client/host_connection.py
+-rw-r--r--   0        0        0     4603 2024-05-07 07:52:37.229764 ftrack_framework_core-2.2.1/source/ftrack_framework_core/configure_logging.py
+-rw-r--r--   0        0        0     9330 2024-05-07 07:52:37.229764 ftrack_framework_core-2.2.1/source/ftrack_framework_core/engine/__init__.py
+-rw-r--r--   0        0        0    17206 2024-05-07 07:52:37.229764 ftrack_framework_core-2.2.1/source/ftrack_framework_core/event/__init__.py
+-rw-r--r--   0        0        0      162 2024-05-07 07:52:37.229764 ftrack_framework_core-2.2.1/source/ftrack_framework_core/exceptions/__init__.py
+-rw-r--r--   0        0        0      277 2024-05-07 07:52:37.229764 ftrack_framework_core-2.2.1/source/ftrack_framework_core/exceptions/engine.py
+-rw-r--r--   0        0        0     1501 2024-05-07 07:52:37.229764 ftrack_framework_core-2.2.1/source/ftrack_framework_core/exceptions/plugin.py
+-rw-r--r--   0        0        0    12705 2024-05-07 07:52:37.229764 ftrack_framework_core-2.2.1/source/ftrack_framework_core/host/__init__.py
+-rw-r--r--   0        0        0     8625 2024-05-07 07:52:37.229764 ftrack_framework_core-2.2.1/source/ftrack_framework_core/log/__init__.py
+-rw-r--r--   0        0        0     1184 2024-05-07 07:52:37.229764 ftrack_framework_core-2.2.1/source/ftrack_framework_core/log/log_item.py
+-rw-r--r--   0        0        0     1831 2024-05-07 07:52:37.229764 ftrack_framework_core-2.2.1/source/ftrack_framework_core/plugin/__init__.py
+-rw-r--r--   0        0        0     1975 2024-05-07 07:52:37.229764 ftrack_framework_core-2.2.1/source/ftrack_framework_core/plugin/plugin_info.py
+-rw-r--r--   0        0        0     8014 2024-05-07 07:52:37.229764 ftrack_framework_core-2.2.1/source/ftrack_framework_core/registry/__init__.py
+-rw-r--r--   0        0        0     3437 2024-05-07 07:52:37.229764 ftrack_framework_core-2.2.1/source/ftrack_framework_core/widget/__init__.py
+-rw-r--r--   0        0        0    17207 2024-05-07 07:52:37.229764 ftrack_framework_core-2.2.1/source/ftrack_framework_core/widget/dialog.py
+-rw-r--r--   0        0        0     4475 2024-05-07 07:52:37.229764 ftrack_framework_core-2.2.1/source/ftrack_framework_core/widget/widget.py
+-rw-r--r--   0        0        0     1268 1970-01-01 00:00:00.000000 ftrack_framework_core-2.2.1/PKG-INFO
```

### Comparing `ftrack_framework_core-2.2.0/LICENSE.txt` & `ftrack_framework_core-2.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.2.0/pyproject.toml` & `ftrack_framework_core-2.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ftrack-framework-core"
-version = "2.2.0"
+version = "2.2.1"
 description='ftrack Framework Core library'
 authors = ["ftrack Integrations Team <integrations@backlight.co>"]
 readme = "README.md"
 packages = [{include = "ftrack_framework_core", from = "source"}]
 license = "Apache-2.0"
 homepage = "https://ftrack.com"
 repository = "https://github.com/ftrackhq/integrations/tree/main/libs/framework-core"
```

### Comparing `ftrack_framework_core-2.2.0/source/ftrack_framework_core/__init__.py` & `ftrack_framework_core-2.2.1/source/ftrack_framework_core/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.2.0/source/ftrack_framework_core/asset/__init__.py` & `ftrack_framework_core-2.2.1/source/ftrack_framework_core/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.2.0/source/ftrack_framework_core/asset/asset_info.py` & `ftrack_framework_core-2.2.1/source/ftrack_framework_core/asset/asset_info.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.2.0/source/ftrack_framework_core/asset/dcc_object.py` & `ftrack_framework_core-2.2.1/source/ftrack_framework_core/asset/dcc_object.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.2.0/source/ftrack_framework_core/client/__init__.py` & `ftrack_framework_core-2.2.1/source/ftrack_framework_core/client/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.2.0/source/ftrack_framework_core/client/host_connection.py` & `ftrack_framework_core-2.2.1/source/ftrack_framework_core/client/host_connection.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.2.0/source/ftrack_framework_core/configure_logging.py` & `ftrack_framework_core-2.2.1/source/ftrack_framework_core/configure_logging.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.2.0/source/ftrack_framework_core/engine/__init__.py` & `ftrack_framework_core-2.2.1/source/ftrack_framework_core/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.2.0/source/ftrack_framework_core/event/__init__.py` & `ftrack_framework_core-2.2.1/source/ftrack_framework_core/event/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.2.0/source/ftrack_framework_core/exceptions/plugin.py` & `ftrack_framework_core-2.2.1/source/ftrack_framework_core/exceptions/plugin.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.2.0/source/ftrack_framework_core/host/__init__.py` & `ftrack_framework_core-2.2.1/source/ftrack_framework_core/host/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.2.0/source/ftrack_framework_core/log/__init__.py` & `ftrack_framework_core-2.2.1/source/ftrack_framework_core/log/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.2.0/source/ftrack_framework_core/log/log_item.py` & `ftrack_framework_core-2.2.1/source/ftrack_framework_core/log/log_item.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.2.0/source/ftrack_framework_core/plugin/__init__.py` & `ftrack_framework_core-2.2.1/source/ftrack_framework_core/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.2.0/source/ftrack_framework_core/plugin/plugin_info.py` & `ftrack_framework_core-2.2.1/source/ftrack_framework_core/plugin/plugin_info.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.2.0/source/ftrack_framework_core/registry/__init__.py` & `ftrack_framework_core-2.2.1/source/ftrack_framework_core/registry/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 
     # Register
     def scan_extensions(self, paths, extension_types=None):
         '''
         Scan framework extension modules from the given *paths*. If *extension_types*
         is given, only consider the given extension types.
         '''
+        unique_extensions = []
 
         discovered_extensions = []
         for path in reversed(paths):
             logging.debug(
                 f'Scanning {path} for {f"{extension_types} " if extension_types else ""}extensions'
             )
             dir_extensions = registry.get_extensions_from_directory(
```

### Comparing `ftrack_framework_core-2.2.0/source/ftrack_framework_core/widget/__init__.py` & `ftrack_framework_core-2.2.1/source/ftrack_framework_core/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.2.0/source/ftrack_framework_core/widget/dialog.py` & `ftrack_framework_core-2.2.1/source/ftrack_framework_core/widget/dialog.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.2.0/source/ftrack_framework_core/widget/widget.py` & `ftrack_framework_core-2.2.1/source/ftrack_framework_core/widget/widget.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.2.0/PKG-INFO` & `ftrack_framework_core-2.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftrack-framework-core
-Version: 2.2.0
+Version: 2.2.1
 Summary: ftrack Framework Core library
 Home-page: https://ftrack.com
 License: Apache-2.0
 Author: ftrack Integrations Team
 Author-email: integrations@backlight.co
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```

