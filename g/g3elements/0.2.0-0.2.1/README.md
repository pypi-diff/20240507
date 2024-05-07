# Comparing `tmp/g3elements-0.2.0.tar.gz` & `tmp/g3elements-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g3elements-0.2.0.tar", last modified: Mon Apr 29 12:51:52 2024, max compression
+gzip compressed data, was "g3elements-0.2.1.tar", last modified: Tue May  7 07:05:28 2024, max compression
```

## Comparing `g3elements-0.2.0.tar` & `g3elements-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 12:51:52.226670 g3elements-0.2.0/
--rw-rw-rw-   0        0        0     1091 2023-06-02 14:34:32.000000 g3elements-0.2.0/LICENCE
--rw-rw-rw-   0        0        0     1124 2024-04-29 12:51:52.224668 g3elements-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       57 2023-07-26 10:08:43.000000 g3elements-0.2.0/README.md
--rw-rw-rw-   0        0        0     1331 2024-04-25 12:01:00.000000 g3elements-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-29 12:51:52.227667 g3elements-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-29 12:51:52.043685 g3elements-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 12:51:52.090665 g3elements-0.2.0/src/g3elements/
--rw-rw-rw-   0        0        0     3452 2024-04-24 19:57:47.000000 g3elements-0.2.0/src/g3elements/__init__.py
--rw-rw-rw-   0        0        0    56627 2024-04-24 19:55:40.000000 g3elements-0.2.0/src/g3elements/_elements.py
--rw-rw-rw-   0        0        0        0 2023-07-31 11:06:46.000000 g3elements-0.2.0/src/g3elements/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-29 12:51:52.193668 g3elements-0.2.0/src/g3elements/route_utils/
--rw-rw-rw-   0        0        0      424 2024-03-24 09:01:33.000000 g3elements-0.2.0/src/g3elements/route_utils/__init__.py
--rw-rw-rw-   0        0        0    47295 2024-04-02 13:14:25.000000 g3elements-0.2.0/src/g3elements/route_utils/_analyzer.py
--rw-rw-rw-   0        0        0    18088 2024-03-24 18:15:19.000000 g3elements-0.2.0/src/g3elements/route_utils/_manager.py
--rw-rw-rw-   0        0        0     3495 2024-03-23 17:23:25.000000 g3elements-0.2.0/src/g3elements/route_utils/_tram.py
-drwxrwxrwx   0        0        0        0 2024-04-29 12:51:52.221666 g3elements-0.2.0/src/g3elements.egg-info/
--rw-rw-rw-   0        0        0     1124 2024-04-29 12:51:51.000000 g3elements-0.2.0/src/g3elements.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2024-04-29 12:51:52.000000 g3elements-0.2.0/src/g3elements.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 12:51:51.000000 g3elements-0.2.0/src/g3elements.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-04-29 12:51:51.000000 g3elements-0.2.0/src/g3elements.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-29 12:51:51.000000 g3elements-0.2.0/src/g3elements.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 07:05:28.190700 g3elements-0.2.1/
+-rw-rw-rw-   0        0        0     1091 2024-05-06 12:36:41.000000 g3elements-0.2.1/LICENCE
+-rw-rw-rw-   0        0        0     1124 2024-05-07 07:05:28.190700 g3elements-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       57 2024-05-06 12:36:41.000000 g3elements-0.2.1/README.md
+-rw-rw-rw-   0        0        0     1331 2024-05-07 06:46:23.000000 g3elements-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-07 07:05:28.190700 g3elements-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-07 07:05:28.152458 g3elements-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 07:05:28.172591 g3elements-0.2.1/src/g3elements/
+-rw-rw-rw-   0        0        0     3452 2024-05-06 12:36:41.000000 g3elements-0.2.1/src/g3elements/__init__.py
+-rw-rw-rw-   0        0        0    56676 2024-05-06 18:46:14.000000 g3elements-0.2.1/src/g3elements/_elements.py
+-rw-rw-rw-   0        0        0        0 2024-05-06 12:36:41.000000 g3elements-0.2.1/src/g3elements/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-07 07:05:28.190700 g3elements-0.2.1/src/g3elements/route_utils/
+-rw-rw-rw-   0        0        0      424 2024-05-06 12:36:41.000000 g3elements-0.2.1/src/g3elements/route_utils/__init__.py
+-rw-rw-rw-   0        0        0    47295 2024-05-06 12:36:41.000000 g3elements-0.2.1/src/g3elements/route_utils/_analyzer.py
+-rw-rw-rw-   0        0        0    18088 2024-05-06 12:36:41.000000 g3elements-0.2.1/src/g3elements/route_utils/_manager.py
+-rw-rw-rw-   0        0        0     3495 2024-05-06 12:36:41.000000 g3elements-0.2.1/src/g3elements/route_utils/_tram.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:05:28.190700 g3elements-0.2.1/src/g3elements.egg-info/
+-rw-rw-rw-   0        0        0     1124 2024-05-07 07:05:28.000000 g3elements-0.2.1/src/g3elements.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2024-05-07 07:05:28.000000 g3elements-0.2.1/src/g3elements.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 07:05:28.000000 g3elements-0.2.1/src/g3elements.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-07 07:05:28.000000 g3elements-0.2.1/src/g3elements.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-07 07:05:28.000000 g3elements-0.2.1/src/g3elements.egg-info/top_level.txt
```

### Comparing `g3elements-0.2.0/LICENCE` & `g3elements-0.2.1/LICENCE`

 * *Files identical despite different names*

### Comparing `g3elements-0.2.0/PKG-INFO` & `g3elements-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g3elements
-Version: 0.2.0
+Version: 0.2.1
 Summary: G3 PLC system elements
 Author-email: Konstantin Mykhailov <kmykhailov@elektroline.cz>
 Project-URL: Homepage, https://gitlab.elektroline.cz/plc/systemg3-py/SystemG3Elements
 Keywords: Elektroline,System G3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
```

### Comparing `g3elements-0.2.0/pyproject.toml` & `g3elements-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "g3elements"
-version = "0.2.0"
+version = "0.2.1"
 description = "G3 PLC system elements"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
   { name = "Konstantin Mykhailov", email = "kmykhailov@elektroline.cz" },
 ]
 classifiers = [
```

### Comparing `g3elements-0.2.0/src/g3elements/__init__.py` & `g3elements-0.2.1/src/g3elements/__init__.py`

 * *Files identical despite different names*

### Comparing `g3elements-0.2.0/src/g3elements/_elements.py` & `g3elements-0.2.1/src/g3elements/_elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -467,15 +467,15 @@
     return isinstance(obj, CabinetMonitoringModule)
 
 
 class CabinetRFID(_CabinetChild):
     is_safety: Literal[False] = False
 
     def _shv_path_relative(self) -> str:
-        return ''
+        return f'devices/cabinet/{self.cabinet}/other/{self.name}'
 
 
 def is_rfid(obj: Any) -> TypeGuard[CabinetRFID]:
     return isinstance(obj, CabinetRFID)
 
 
 class CabinetUPS(_CabinetChild):
```

### Comparing `g3elements-0.2.0/src/g3elements/route_utils/_analyzer.py` & `g3elements-0.2.1/src/g3elements/route_utils/_analyzer.py`

 * *Files identical despite different names*

### Comparing `g3elements-0.2.0/src/g3elements/route_utils/_manager.py` & `g3elements-0.2.1/src/g3elements/route_utils/_manager.py`

 * *Files identical despite different names*

### Comparing `g3elements-0.2.0/src/g3elements/route_utils/_tram.py` & `g3elements-0.2.1/src/g3elements/route_utils/_tram.py`

 * *Files identical despite different names*

### Comparing `g3elements-0.2.0/src/g3elements.egg-info/PKG-INFO` & `g3elements-0.2.1/src/g3elements.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g3elements
-Version: 0.2.0
+Version: 0.2.1
 Summary: G3 PLC system elements
 Author-email: Konstantin Mykhailov <kmykhailov@elektroline.cz>
 Project-URL: Homepage, https://gitlab.elektroline.cz/plc/systemg3-py/SystemG3Elements
 Keywords: Elektroline,System G3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
```

