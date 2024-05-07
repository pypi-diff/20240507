# Comparing `tmp/ifcpatch-0.0.240418.tar.gz` & `tmp/ifcpatch-0.0.240507.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifcpatch-0.0.240418.tar", last modified: Thu Apr 18 00:56:55 2024, max compression
+gzip compressed data, was "ifcpatch-0.0.240507.tar", last modified: Tue May  7 13:37:59 2024, max compression
```

## Comparing `ifcpatch-0.0.240418.tar` & `ifcpatch-0.0.240507.tar`

### file list

```diff
@@ -1,19 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:56:55.727825 ifcpatch-0.0.240418/
--rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-04-18 00:56:51.000000 ifcpatch-0.0.240418/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-18 00:56:51.000000 ifcpatch-0.0.240418/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-18 00:56:55.727825 ifcpatch-0.0.240418/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:56:55.727825 ifcpatch-0.0.240418/ifcpatch/
--rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-04-18 00:56:51.000000 ifcpatch-0.0.240418/ifcpatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-18 00:56:51.000000 ifcpatch-0.0.240418/ifcpatch/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:56:55.727825 ifcpatch-0.0.240418/ifcpatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-18 00:56:55.000000 ifcpatch-0.0.240418/ifcpatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-18 00:56:55.000000 ifcpatch-0.0.240418/ifcpatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 00:56:55.000000 ifcpatch-0.0.240418/ifcpatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-18 00:56:55.000000 ifcpatch-0.0.240418/ifcpatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 00:56:55.000000 ifcpatch-0.0.240418/ifcpatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-18 00:56:53.000000 ifcpatch-0.0.240418/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 00:56:55.727825 ifcpatch-0.0.240418/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:56:55.727825 ifcpatch-0.0.240418/test/
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-18 00:56:51.000000 ifcpatch-0.0.240418/test/test_ExtractElements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-18 00:56:51.000000 ifcpatch-0.0.240418/test/test_MergeDuplicateTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-18 00:56:51.000000 ifcpatch-0.0.240418/test/test_RegenerateGlobalIds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:37:59.221688 ifcpatch-0.0.240507/
+-rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-07 13:37:59.221688 ifcpatch-0.0.240507/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:37:59.213688 ifcpatch-0.0.240507/ifcpatch/
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:37:59.217688 ifcpatch-0.0.240507/ifcpatch/recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/ConvertLengthUnit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/ConvertNestToAggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/ConvertPropertiesToQuantities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/DowngradeIndexedPolyCurve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/ExtractElements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/ExtractPropertiesToSQLite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/FixArchiCADToRevitDoorSwings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/FixArchiCADToRevitSpaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/FixRevitClassificationCodeTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/FixRevitTINs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20738 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/Ifc2Sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/MergeDuplicateTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/MergeProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/Migrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/OffsetObjectPlacements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/OffsetStoreyElevations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/Optimise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9104 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/PurgeData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/RecycleNonRootedElements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/RegenerateGlobalIds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/RemoveRevitUniformatClassification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/RemoveSiteRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/ResetAbsoluteCoordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/ResetSpatialElementLocations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/SetRefElevation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/SetWorldCoordinateSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/SplitByBuildingStorey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/TessellateElements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/ifcpatch/recipes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:37:59.221688 ifcpatch-0.0.240507/ifcpatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-07 13:37:59.000000 ifcpatch-0.0.240507/ifcpatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-07 13:37:59.000000 ifcpatch-0.0.240507/ifcpatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:37:59.000000 ifcpatch-0.0.240507/ifcpatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 13:37:59.000000 ifcpatch-0.0.240507/ifcpatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 13:37:59.000000 ifcpatch-0.0.240507/ifcpatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-07 13:37:57.000000 ifcpatch-0.0.240507/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 13:37:59.221688 ifcpatch-0.0.240507/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:37:59.221688 ifcpatch-0.0.240507/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/test/test_ConvertLengthUnit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/test/test_ExtractElements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/test/test_MergeDuplicateTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/test/test_MergeProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-07 13:37:55.000000 ifcpatch-0.0.240507/test/test_RegenerateGlobalIds.py
```

### Comparing `ifcpatch-0.0.240418/COPYING` & `ifcpatch-0.0.240507/COPYING`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240418/COPYING.LESSER` & `ifcpatch-0.0.240507/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240418/PKG-INFO` & `ifcpatch-0.0.240507/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifcpatch
-Version: 0.0.240418
+Version: 0.0.240507
 Summary: IFC patching utility
 Author-email: Dion Moult <dion@thinkmoult.com>
 Project-URL: Homepage, http://ifcopenshell.org
 Project-URL: Documentation, https://docs.ifcopenshell.org
 Project-URL: Issues, https://github.com/IfcOpenShell/IfcOpenShell/issues
 Keywords: IFC,BIM
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ifcpatch-0.0.240418/ifcpatch/__init__.py` & `ifcpatch-0.0.240507/ifcpatch/__init__.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240418/ifcpatch/__main__.py` & `ifcpatch-0.0.240507/ifcpatch/__main__.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240418/ifcpatch.egg-info/PKG-INFO` & `ifcpatch-0.0.240507/ifcpatch.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifcpatch
-Version: 0.0.240418
+Version: 0.0.240507
 Summary: IFC patching utility
 Author-email: Dion Moult <dion@thinkmoult.com>
 Project-URL: Homepage, http://ifcopenshell.org
 Project-URL: Documentation, https://docs.ifcopenshell.org
 Project-URL: Issues, https://github.com/IfcOpenShell/IfcOpenShell/issues
 Keywords: IFC,BIM
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ifcpatch-0.0.240418/pyproject.toml` & `ifcpatch-0.0.240507/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ifcpatch"
-version = "0.0.240418"
+version = "0.0.240507"
 authors = [
   { name="Dion Moult", email="dion@thinkmoult.com" },
 ]
 description = "IFC patching utility"
 readme = "README.md"
 keywords = ["IFC", "BIM"]
 classifiers = [
@@ -19,9 +19,9 @@
 
 [project.urls]
 Homepage = "http://ifcopenshell.org"
 Documentation = "https://docs.ifcopenshell.org"
 Issues = "https://github.com/IfcOpenShell/IfcOpenShell/issues"
 
 [tool.setuptools.packages.find]
-include = ["ifcpatch"]
+include = ["ifcpatch*"]
 exclude = ["test*"]
```

### Comparing `ifcpatch-0.0.240418/test/test_ExtractElements.py` & `ifcpatch-0.0.240507/test/test_ExtractElements.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240418/test/test_MergeDuplicateTypes.py` & `ifcpatch-0.0.240507/test/test_MergeDuplicateTypes.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240418/test/test_RegenerateGlobalIds.py` & `ifcpatch-0.0.240507/test/test_RegenerateGlobalIds.py`

 * *Files identical despite different names*

