# Comparing `tmp/g3visu-0.1.1.tar.gz` & `tmp/g3visu-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g3visu-0.1.1.tar", last modified: Mon Apr 29 17:54:31 2024, max compression
+gzip compressed data, was "g3visu-0.1.2.tar", last modified: Tue May  7 07:07:38 2024, max compression
```

## Comparing `g3visu-0.1.1.tar` & `g3visu-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 17:54:31.990063 g3visu-0.1.1/
--rw-rw-rw-   0        0        0     1091 2023-06-02 14:34:32.000000 g3visu-0.1.1/LICENCE
--rw-rw-rw-   0        0        0     1759 2024-04-29 17:54:31.988045 g3visu-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      403 2024-04-29 17:51:24.000000 g3visu-0.1.1/README.md
--rw-rw-rw-   0        0        0     1397 2024-04-29 17:53:48.000000 g3visu-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-29 17:54:31.991060 g3visu-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-29 17:54:31.847777 g3visu-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 17:54:31.878388 g3visu-0.1.1/src/g3visu/
--rw-rw-rw-   0        0        0      289 2024-04-17 21:37:30.000000 g3visu-0.1.1/src/g3visu/__init__.py
--rw-rw-rw-   0        0        0     5593 2024-04-18 07:47:45.000000 g3visu-0.1.1/src/g3visu/_cli.py
-drwxrwxrwx   0        0        0        0 2024-04-29 17:54:31.922981 g3visu-0.1.1/src/g3visu/meta/
--rw-rw-rw-   0        0        0       99 2024-04-09 13:05:34.000000 g3visu-0.1.1/src/g3visu/meta/__init__.py
--rw-rw-rw-   0        0        0     3591 2024-04-17 22:37:48.000000 g3visu-0.1.1/src/g3visu/meta/_meta.py
-drwxrwxrwx   0        0        0        0 2024-04-29 17:54:31.940120 g3visu-0.1.1/src/g3visu/site/
--rw-rw-rw-   0        0        0      120 2024-04-17 22:23:28.000000 g3visu-0.1.1/src/g3visu/site/__init__.py
--rw-rw-rw-   0        0        0    22701 2024-04-25 14:02:06.000000 g3visu-0.1.1/src/g3visu/site/_site_svg.py
--rw-rw-rw-   0        0        0    11402 2024-04-09 13:09:55.000000 g3visu-0.1.1/src/g3visu/site/_table.py
-drwxrwxrwx   0        0        0        0 2024-04-29 17:54:31.969863 g3visu-0.1.1/src/g3visu/typeinfo/
--rw-rw-rw-   0        0        0      411 2024-04-10 09:28:19.000000 g3visu-0.1.1/src/g3visu/typeinfo/__init__.py
--rw-rw-rw-   0        0        0     1310 2024-02-23 16:36:17.000000 g3visu-0.1.1/src/g3visu/typeinfo/_list_operations.py
--rw-rw-rw-   0        0        0    19489 2024-04-25 14:06:22.000000 g3visu-0.1.1/src/g3visu/typeinfo/_typeinfo.py
--rw-rw-rw-   0        0        0        0 2023-11-08 22:15:47.000000 g3visu-0.1.1/src/g3visu/typeinfo/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-29 17:54:31.976740 g3visu-0.1.1/src/g3visu/utils/
--rw-rw-rw-   0        0        0      308 2024-04-09 15:49:09.000000 g3visu-0.1.1/src/g3visu/utils/__init__.py
--rw-rw-rw-   0        0        0     7709 2024-04-29 17:44:55.000000 g3visu-0.1.1/src/g3visu/utils/_download_from_sites.py
-drwxrwxrwx   0        0        0        0 2024-04-29 17:54:31.981053 g3visu-0.1.1/src/g3visu.egg-info/
--rw-rw-rw-   0        0        0     1759 2024-04-29 17:54:31.000000 g3visu-0.1.1/src/g3visu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      620 2024-04-29 17:54:31.000000 g3visu-0.1.1/src/g3visu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 17:54:31.000000 g3visu-0.1.1/src/g3visu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-29 17:54:31.000000 g3visu-0.1.1/src/g3visu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      143 2024-04-29 17:54:31.000000 g3visu-0.1.1/src/g3visu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-29 17:54:31.000000 g3visu-0.1.1/src/g3visu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 07:07:38.173924 g3visu-0.1.2/
+-rw-rw-rw-   0        0        0     1091 2024-04-29 14:15:00.000000 g3visu-0.1.2/LICENCE
+-rw-rw-rw-   0        0        0     1759 2024-05-07 07:07:38.173924 g3visu-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2024-04-30 08:21:52.000000 g3visu-0.1.2/README.md
+-rw-rw-rw-   0        0        0     1397 2024-05-07 06:44:33.000000 g3visu-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-07 07:07:38.173924 g3visu-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-07 07:07:38.104242 g3visu-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 07:07:38.112355 g3visu-0.1.2/src/g3visu/
+-rw-rw-rw-   0        0        0      289 2024-04-29 14:15:00.000000 g3visu-0.1.2/src/g3visu/__init__.py
+-rw-rw-rw-   0        0        0     5593 2024-04-30 12:55:51.000000 g3visu-0.1.2/src/g3visu/_cli.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:07:38.142653 g3visu-0.1.2/src/g3visu/meta/
+-rw-rw-rw-   0        0        0       99 2024-04-29 14:15:00.000000 g3visu-0.1.2/src/g3visu/meta/__init__.py
+-rw-rw-rw-   0        0        0     3591 2024-04-29 14:15:00.000000 g3visu-0.1.2/src/g3visu/meta/_meta.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:07:38.142653 g3visu-0.1.2/src/g3visu/site/
+-rw-rw-rw-   0        0        0      120 2024-04-29 14:15:00.000000 g3visu-0.1.2/src/g3visu/site/__init__.py
+-rw-rw-rw-   0        0        0    22979 2024-05-06 19:35:19.000000 g3visu-0.1.2/src/g3visu/site/_site_svg.py
+-rw-rw-rw-   0        0        0    11402 2024-04-29 14:15:00.000000 g3visu-0.1.2/src/g3visu/site/_table.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:07:38.158298 g3visu-0.1.2/src/g3visu/typeinfo/
+-rw-rw-rw-   0        0        0      411 2024-04-29 14:15:00.000000 g3visu-0.1.2/src/g3visu/typeinfo/__init__.py
+-rw-rw-rw-   0        0        0     1310 2024-04-30 12:56:03.000000 g3visu-0.1.2/src/g3visu/typeinfo/_list_operations.py
+-rw-rw-rw-   0        0        0    19489 2024-04-30 12:56:11.000000 g3visu-0.1.2/src/g3visu/typeinfo/_typeinfo.py
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:15:00.000000 g3visu-0.1.2/src/g3visu/typeinfo/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-07 07:07:38.158298 g3visu-0.1.2/src/g3visu/utils/
+-rw-rw-rw-   0        0        0      308 2024-04-29 14:15:00.000000 g3visu-0.1.2/src/g3visu/utils/__init__.py
+-rw-rw-rw-   0        0        0     7709 2024-04-30 08:21:52.000000 g3visu-0.1.2/src/g3visu/utils/_download_from_sites.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:07:38.158298 g3visu-0.1.2/src/g3visu.egg-info/
+-rw-rw-rw-   0        0        0     1759 2024-05-07 07:07:38.000000 g3visu-0.1.2/src/g3visu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      620 2024-05-07 07:07:38.000000 g3visu-0.1.2/src/g3visu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 07:07:38.000000 g3visu-0.1.2/src/g3visu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-07 07:07:38.000000 g3visu-0.1.2/src/g3visu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      143 2024-05-07 07:07:38.000000 g3visu-0.1.2/src/g3visu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-07 07:07:38.000000 g3visu-0.1.2/src/g3visu.egg-info/top_level.txt
```

### Comparing `g3visu-0.1.1/LICENCE` & `g3visu-0.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `g3visu-0.1.1/PKG-INFO` & `g3visu-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g3visu
-Version: 0.1.1
+Version: 0.1.2
 Summary: System G3 Visualization files' parsers and generators
 Author: Elektroline a.s.
 Project-URL: Homepage, https://gitlab.elektroline.cz/plc/systemg3-py/SystemG3Visu.git
 Keywords: Elektroline,System G3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
```

### Comparing `g3visu-0.1.1/pyproject.toml` & `g3visu-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "g3visu"
-version = "0.1.1"
+version = "0.1.2"
 description = "System G3 Visualization files' parsers and generators"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
   { name = "Elektroline a.s." },
 ]
 classifiers = [
```

### Comparing `g3visu-0.1.1/src/g3visu/_cli.py` & `g3visu-0.1.2/src/g3visu/_cli.py`

 * *Files identical despite different names*

### Comparing `g3visu-0.1.1/src/g3visu/meta/_meta.py` & `g3visu-0.1.2/src/g3visu/meta/_meta.py`

 * *Files identical despite different names*

### Comparing `g3visu-0.1.1/src/g3visu/site/_site_svg.py` & `g3visu-0.1.2/src/g3visu/site/_site_svg.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,14 +403,18 @@
         if type_name == 'Gate_G3':
             self._add_gate(
                 name,
                 shv_path,
                 column_names=kwargs['column_names'],
                 row_count=kwargs['row_count']
                 )
+        elif type_name == 'Vetra_G3':
+            self._add_requestor(
+                type_name, name, shv_path, row_names=kwargs['row_names']
+                )
         elif type_name == 'Heating_G3':
             self._add_heating(
                 name,
                 shv_path,
                 row_names=kwargs['row_names']
                 )
         elif kwargs.get('is_requestor_loop', False):
@@ -546,14 +550,16 @@
         if shv_type == 'Gate_G3':
             return {
                 'column_names': type_variant[0],
                 'row_count': type_variant[1]
             }
         if shv_type == 'Heating_G3':
             return {'row_names': type_variant}
+        if shv_type == 'Vetra_G3':
+            return {'row_names': type_variant, 'is_requestor_loop': False}
         if is_requestor_loop(element):
             return {'row_names': type_variant, 'is_requestor_loop': True}
         return {}
 
     def update(self) -> None:
         """Update the site SVG file from the system config data."""
         logger.info('Adding elements to site.svg')
```

### Comparing `g3visu-0.1.1/src/g3visu/site/_table.py` & `g3visu-0.1.2/src/g3visu/site/_table.py`

 * *Files identical despite different names*

### Comparing `g3visu-0.1.1/src/g3visu/typeinfo/_list_operations.py` & `g3visu-0.1.2/src/g3visu/typeinfo/_list_operations.py`

 * *Files identical despite different names*

### Comparing `g3visu-0.1.1/src/g3visu/typeinfo/_typeinfo.py` & `g3visu-0.1.2/src/g3visu/typeinfo/_typeinfo.py`

 * *Files identical despite different names*

### Comparing `g3visu-0.1.1/src/g3visu/utils/_download_from_sites.py` & `g3visu-0.1.2/src/g3visu/utils/_download_from_sites.py`

 * *Files identical despite different names*

### Comparing `g3visu-0.1.1/src/g3visu.egg-info/PKG-INFO` & `g3visu-0.1.2/src/g3visu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g3visu
-Version: 0.1.1
+Version: 0.1.2
 Summary: System G3 Visualization files' parsers and generators
 Author: Elektroline a.s.
 Project-URL: Homepage, https://gitlab.elektroline.cz/plc/systemg3-py/SystemG3Visu.git
 Keywords: Elektroline,System G3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
```

### Comparing `g3visu-0.1.1/src/g3visu.egg-info/SOURCES.txt` & `g3visu-0.1.2/src/g3visu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

