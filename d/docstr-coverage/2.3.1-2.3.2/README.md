# Comparing `tmp/docstr-coverage-2.3.1.tar.gz` & `tmp/docstr-coverage-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docstr-coverage-2.3.1.tar", last modified: Thu Feb 29 00:40:06 2024, max compression
+gzip compressed data, was "docstr-coverage-2.3.2.tar", last modified: Tue May  7 16:53:28 2024, max compression
```

## Comparing `docstr-coverage-2.3.1.tar` & `docstr-coverage-2.3.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2024-02-29 00:40:06.745587 docstr-coverage-2.3.1/
--rw-r--r--   0 Hunter     (501) staff       (20)     1075 2021-11-05 17:40:10.000000 docstr-coverage-2.3.1/LICENSE.txt
--rw-r--r--   0 Hunter     (501) staff       (20)      127 2021-11-05 17:40:10.000000 docstr-coverage-2.3.1/MANIFEST.in
--rw-r--r--   0 Hunter     (501) staff       (20)    10547 2024-02-29 00:40:06.745662 docstr-coverage-2.3.1/PKG-INFO
--rw-r--r--   0 Hunter     (501) staff       (20)     9228 2024-02-29 00:34:02.000000 docstr-coverage-2.3.1/README.md
-drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2024-02-29 00:40:06.743417 docstr-coverage-2.3.1/docstr_coverage/
--rw-r--r--   0 Hunter     (501) staff       (20)      552 2021-11-05 17:40:10.000000 docstr-coverage-2.3.1/docstr_coverage/__init__.py
--rw-r--r--   0 Hunter     (501) staff       (20)     3117 2024-02-29 00:31:11.000000 docstr-coverage-2.3.1/docstr_coverage/badge.py
--rw-r--r--   0 Hunter     (501) staff       (20)    14135 2023-04-13 20:04:25.000000 docstr-coverage-2.3.1/docstr_coverage/cli.py
--rw-r--r--   0 Hunter     (501) staff       (20)     2841 2021-11-05 17:40:10.000000 docstr-coverage-2.3.1/docstr_coverage/config_file.py
--rw-r--r--   0 Hunter     (501) staff       (20)    11206 2023-04-13 20:04:25.000000 docstr-coverage-2.3.1/docstr_coverage/coverage.py
--rw-r--r--   0 Hunter     (501) staff       (20)     2854 2021-11-05 17:40:10.000000 docstr-coverage-2.3.1/docstr_coverage/ignore_config.py
--rw-r--r--   0 Hunter     (501) staff       (20)     5564 2021-11-05 17:40:10.000000 docstr-coverage-2.3.1/docstr_coverage/printers.py
--rw-r--r--   0 Hunter     (501) staff       (20)    12005 2021-11-05 17:40:10.000000 docstr-coverage-2.3.1/docstr_coverage/result_collection.py
-drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2024-02-29 00:40:06.744354 docstr-coverage-2.3.1/docstr_coverage/templates/
--rw-r--r--   0 Hunter     (501) staff       (20)     1108 2021-11-05 17:40:10.000000 docstr-coverage-2.3.1/docstr_coverage/templates/flat.svg
--rw-r--r--   0 Hunter     (501) staff       (20)     5032 2023-04-13 20:04:25.000000 docstr-coverage-2.3.1/docstr_coverage/visitor.py
-drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2024-02-29 00:40:06.744246 docstr-coverage-2.3.1/docstr_coverage.egg-info/
--rw-r--r--   0 Hunter     (501) staff       (20)    10547 2024-02-29 00:40:06.000000 docstr-coverage-2.3.1/docstr_coverage.egg-info/PKG-INFO
--rw-r--r--   0 Hunter     (501) staff       (20)      867 2024-02-29 00:40:06.000000 docstr-coverage-2.3.1/docstr_coverage.egg-info/SOURCES.txt
--rw-r--r--   0 Hunter     (501) staff       (20)        1 2024-02-29 00:40:06.000000 docstr-coverage-2.3.1/docstr_coverage.egg-info/dependency_links.txt
--rw-r--r--   0 Hunter     (501) staff       (20)       65 2024-02-29 00:40:06.000000 docstr-coverage-2.3.1/docstr_coverage.egg-info/entry_points.txt
--rw-r--r--   0 Hunter     (501) staff       (20)        1 2021-11-07 22:18:00.000000 docstr-coverage-2.3.1/docstr_coverage.egg-info/not-zip-safe
--rw-r--r--   0 Hunter     (501) staff       (20)      164 2024-02-29 00:40:06.000000 docstr-coverage-2.3.1/docstr_coverage.egg-info/requires.txt
--rw-r--r--   0 Hunter     (501) staff       (20)       16 2024-02-29 00:40:06.000000 docstr-coverage-2.3.1/docstr_coverage.egg-info/top_level.txt
--rw-r--r--   0 Hunter     (501) staff       (20)      269 2021-11-05 17:40:10.000000 docstr-coverage-2.3.1/pyproject.toml
--rw-r--r--   0 Hunter     (501) staff       (20)      132 2024-02-29 00:40:06.745915 docstr-coverage-2.3.1/setup.cfg
--rw-r--r--   0 Hunter     (501) staff       (20)     2016 2024-02-29 00:34:39.000000 docstr-coverage-2.3.1/setup.py
-drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2024-02-29 00:40:06.741168 docstr-coverage-2.3.1/tests/
-drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2024-02-29 00:40:06.741207 docstr-coverage-2.3.1/tests/sample_files/
-drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2024-02-29 00:40:06.745427 docstr-coverage-2.3.1/tests/sample_files/badges/
--rw-r--r--   0 Hunter     (501) staff       (20)     1084 2021-11-05 17:40:10.000000 docstr-coverage-2.3.1/tests/sample_files/badges/0.svg
--rw-r--r--   0 Hunter     (501) staff       (20)     1085 2021-11-05 17:40:10.000000 docstr-coverage-2.3.1/tests/sample_files/badges/100.svg
--rw-r--r--   0 Hunter     (501) staff       (20)     1086 2021-11-05 17:40:10.000000 docstr-coverage-2.3.1/tests/sample_files/badges/12.svg
--rw-r--r--   0 Hunter     (501) staff       (20)     1086 2021-11-05 17:40:10.000000 docstr-coverage-2.3.1/tests/sample_files/badges/54.svg
--rw-r--r--   0 Hunter     (501) staff       (20)     1086 2021-11-05 17:40:10.000000 docstr-coverage-2.3.1/tests/sample_files/badges/71.svg
--rw-r--r--   0 Hunter     (501) staff       (20)     1086 2021-11-05 17:40:10.000000 docstr-coverage-2.3.1/tests/sample_files/badges/84.svg
--rw-r--r--   0 Hunter     (501) staff       (20)     1086 2021-11-05 17:40:10.000000 docstr-coverage-2.3.1/tests/sample_files/badges/94.svg
+drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2024-05-07 16:53:28.684152 docstr-coverage-2.3.2/
+-rw-r--r--   0 Hunter     (501) staff       (20)     1075 2021-11-05 17:40:10.000000 docstr-coverage-2.3.2/LICENSE.txt
+-rw-r--r--   0 Hunter     (501) staff       (20)      127 2021-11-05 17:40:10.000000 docstr-coverage-2.3.2/MANIFEST.in
+-rw-r--r--   0 Hunter     (501) staff       (20)    10547 2024-05-07 16:53:28.684219 docstr-coverage-2.3.2/PKG-INFO
+-rw-r--r--   0 Hunter     (501) staff       (20)     9228 2024-05-07 16:46:39.000000 docstr-coverage-2.3.2/README.md
+drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2024-05-07 16:53:28.682126 docstr-coverage-2.3.2/docstr_coverage/
+-rw-r--r--   0 Hunter     (501) staff       (20)      552 2021-11-05 17:40:10.000000 docstr-coverage-2.3.2/docstr_coverage/__init__.py
+-rw-r--r--   0 Hunter     (501) staff       (20)     3117 2024-02-29 00:31:11.000000 docstr-coverage-2.3.2/docstr_coverage/badge.py
+-rw-r--r--   0 Hunter     (501) staff       (20)    14135 2023-04-13 20:04:25.000000 docstr-coverage-2.3.2/docstr_coverage/cli.py
+-rw-r--r--   0 Hunter     (501) staff       (20)     2841 2021-11-05 17:40:10.000000 docstr-coverage-2.3.2/docstr_coverage/config_file.py
+-rw-r--r--   0 Hunter     (501) staff       (20)    11206 2023-04-13 20:04:25.000000 docstr-coverage-2.3.2/docstr_coverage/coverage.py
+-rw-r--r--   0 Hunter     (501) staff       (20)     2854 2021-11-05 17:40:10.000000 docstr-coverage-2.3.2/docstr_coverage/ignore_config.py
+-rw-r--r--   0 Hunter     (501) staff       (20)     5564 2021-11-05 17:40:10.000000 docstr-coverage-2.3.2/docstr_coverage/printers.py
+-rw-r--r--   0 Hunter     (501) staff       (20)    12005 2021-11-05 17:40:10.000000 docstr-coverage-2.3.2/docstr_coverage/result_collection.py
+drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2024-05-07 16:53:28.683137 docstr-coverage-2.3.2/docstr_coverage/templates/
+-rw-r--r--   0 Hunter     (501) staff       (20)     1108 2021-11-05 17:40:10.000000 docstr-coverage-2.3.2/docstr_coverage/templates/flat.svg
+-rw-r--r--   0 Hunter     (501) staff       (20)     5032 2023-04-13 20:04:25.000000 docstr-coverage-2.3.2/docstr_coverage/visitor.py
+drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2024-05-07 16:53:28.683028 docstr-coverage-2.3.2/docstr_coverage.egg-info/
+-rw-r--r--   0 Hunter     (501) staff       (20)    10547 2024-05-07 16:53:28.000000 docstr-coverage-2.3.2/docstr_coverage.egg-info/PKG-INFO
+-rw-r--r--   0 Hunter     (501) staff       (20)      867 2024-05-07 16:53:28.000000 docstr-coverage-2.3.2/docstr_coverage.egg-info/SOURCES.txt
+-rw-r--r--   0 Hunter     (501) staff       (20)        1 2024-05-07 16:53:28.000000 docstr-coverage-2.3.2/docstr_coverage.egg-info/dependency_links.txt
+-rw-r--r--   0 Hunter     (501) staff       (20)       65 2024-05-07 16:53:28.000000 docstr-coverage-2.3.2/docstr_coverage.egg-info/entry_points.txt
+-rw-r--r--   0 Hunter     (501) staff       (20)        1 2021-11-07 22:18:00.000000 docstr-coverage-2.3.2/docstr_coverage.egg-info/not-zip-safe
+-rw-r--r--   0 Hunter     (501) staff       (20)      156 2024-05-07 16:53:28.000000 docstr-coverage-2.3.2/docstr_coverage.egg-info/requires.txt
+-rw-r--r--   0 Hunter     (501) staff       (20)       16 2024-05-07 16:53:28.000000 docstr-coverage-2.3.2/docstr_coverage.egg-info/top_level.txt
+-rw-r--r--   0 Hunter     (501) staff       (20)      269 2021-11-05 17:40:10.000000 docstr-coverage-2.3.2/pyproject.toml
+-rw-r--r--   0 Hunter     (501) staff       (20)      132 2024-05-07 16:53:28.684483 docstr-coverage-2.3.2/setup.cfg
+-rw-r--r--   0 Hunter     (501) staff       (20)     2008 2024-05-07 16:46:39.000000 docstr-coverage-2.3.2/setup.py
+drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2024-05-07 16:53:28.679747 docstr-coverage-2.3.2/tests/
+drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2024-05-07 16:53:28.679787 docstr-coverage-2.3.2/tests/sample_files/
+drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2024-05-07 16:53:28.684031 docstr-coverage-2.3.2/tests/sample_files/badges/
+-rw-r--r--   0 Hunter     (501) staff       (20)     1084 2021-11-05 17:40:10.000000 docstr-coverage-2.3.2/tests/sample_files/badges/0.svg
+-rw-r--r--   0 Hunter     (501) staff       (20)     1085 2021-11-05 17:40:10.000000 docstr-coverage-2.3.2/tests/sample_files/badges/100.svg
+-rw-r--r--   0 Hunter     (501) staff       (20)     1086 2021-11-05 17:40:10.000000 docstr-coverage-2.3.2/tests/sample_files/badges/12.svg
+-rw-r--r--   0 Hunter     (501) staff       (20)     1086 2021-11-05 17:40:10.000000 docstr-coverage-2.3.2/tests/sample_files/badges/54.svg
+-rw-r--r--   0 Hunter     (501) staff       (20)     1086 2021-11-05 17:40:10.000000 docstr-coverage-2.3.2/tests/sample_files/badges/71.svg
+-rw-r--r--   0 Hunter     (501) staff       (20)     1086 2021-11-05 17:40:10.000000 docstr-coverage-2.3.2/tests/sample_files/badges/84.svg
+-rw-r--r--   0 Hunter     (501) staff       (20)     1086 2021-11-05 17:40:10.000000 docstr-coverage-2.3.2/tests/sample_files/badges/94.svg
```

### Comparing `docstr-coverage-2.3.1/LICENSE.txt` & `docstr-coverage-2.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.3.1/PKG-INFO` & `docstr-coverage-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docstr-coverage
-Version: 2.3.1
+Version: 2.3.2
 Summary: Utility for examining python source files to ensure proper documentation. Lists missing docstrings, and calculates overall docstring coverage percentage rating.
 Home-page: https://github.com/HunterMcGushion/docstr_coverage
 Author: Hunter McGushion
 Author-email: hunter@mcgushion.com
 License: MIT
 Keywords: docstring coverage documentation audit source code statistics report
 Platform: UNKNOWN
@@ -204,15 +204,15 @@
 and configuring the `paths` section of the [`.docstr.yaml` config](#config-file). 
  This is preferrable over [pre-commit args](https://pre-commit.com/#config-args), 
  as it facilitates the use of the same config in CI, pre-commit and manual runs.
 
 ```yaml
 repos:
   - repo: https://github.com/HunterMcGushion/docstr_coverage
-    rev: v2.3.1 # most recent docstr-coverage release or commit sha
+    rev: v2.3.2 # most recent docstr-coverage release or commit sha
     hooks:
       - id: docstr-coverage
         args: ["--verbose", "2"] # override the .docstr.yaml to see less output
 ```
 
 #### Package in Your Project
```

### Comparing `docstr-coverage-2.3.1/README.md` & `docstr-coverage-2.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
 and configuring the `paths` section of the [`.docstr.yaml` config](#config-file). 
  This is preferrable over [pre-commit args](https://pre-commit.com/#config-args), 
  as it facilitates the use of the same config in CI, pre-commit and manual runs.
 
 ```yaml
 repos:
   - repo: https://github.com/HunterMcGushion/docstr_coverage
-    rev: v2.3.1 # most recent docstr-coverage release or commit sha
+    rev: v2.3.2 # most recent docstr-coverage release or commit sha
     hooks:
       - id: docstr-coverage
         args: ["--verbose", "2"] # override the .docstr.yaml to see less output
 ```
 
 #### Package in Your Project
```

### Comparing `docstr-coverage-2.3.1/docstr_coverage/__init__.py` & `docstr-coverage-2.3.2/docstr_coverage/__init__.py`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.3.1/docstr_coverage/badge.py` & `docstr-coverage-2.3.2/docstr_coverage/badge.py`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.3.1/docstr_coverage/cli.py` & `docstr-coverage-2.3.2/docstr_coverage/cli.py`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.3.1/docstr_coverage/config_file.py` & `docstr-coverage-2.3.2/docstr_coverage/config_file.py`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.3.1/docstr_coverage/coverage.py` & `docstr-coverage-2.3.2/docstr_coverage/coverage.py`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.3.1/docstr_coverage/ignore_config.py` & `docstr-coverage-2.3.2/docstr_coverage/ignore_config.py`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.3.1/docstr_coverage/printers.py` & `docstr-coverage-2.3.2/docstr_coverage/printers.py`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.3.1/docstr_coverage/result_collection.py` & `docstr-coverage-2.3.2/docstr_coverage/result_collection.py`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.3.1/docstr_coverage/templates/flat.svg` & `docstr-coverage-2.3.2/docstr_coverage/templates/flat.svg`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.3.1/docstr_coverage/visitor.py` & `docstr-coverage-2.3.2/docstr_coverage/visitor.py`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.3.1/docstr_coverage.egg-info/PKG-INFO` & `docstr-coverage-2.3.2/docstr_coverage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docstr-coverage
-Version: 2.3.1
+Version: 2.3.2
 Summary: Utility for examining python source files to ensure proper documentation. Lists missing docstrings, and calculates overall docstring coverage percentage rating.
 Home-page: https://github.com/HunterMcGushion/docstr_coverage
 Author: Hunter McGushion
 Author-email: hunter@mcgushion.com
 License: MIT
 Keywords: docstring coverage documentation audit source code statistics report
 Platform: UNKNOWN
@@ -204,15 +204,15 @@
 and configuring the `paths` section of the [`.docstr.yaml` config](#config-file). 
  This is preferrable over [pre-commit args](https://pre-commit.com/#config-args), 
  as it facilitates the use of the same config in CI, pre-commit and manual runs.
 
 ```yaml
 repos:
   - repo: https://github.com/HunterMcGushion/docstr_coverage
-    rev: v2.3.1 # most recent docstr-coverage release or commit sha
+    rev: v2.3.2 # most recent docstr-coverage release or commit sha
     hooks:
       - id: docstr-coverage
         args: ["--verbose", "2"] # override the .docstr.yaml to see less output
 ```
 
 #### Package in Your Project
```

### Comparing `docstr-coverage-2.3.1/docstr_coverage.egg-info/SOURCES.txt` & `docstr-coverage-2.3.2/docstr_coverage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.3.1/setup.py` & `docstr-coverage-2.3.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 def readme():
     with open("README.md") as f:
         return f.read()
 
 
-MAJOR, MINOR, MICRO = 2, 3, 1
+MAJOR, MINOR, MICRO = 2, 3, 2
 __VERSION__ = "{}.{}.{}".format(MAJOR, MINOR, MICRO)
 
 setup(
     name="docstr-coverage",
     version=__VERSION__,
     description=(
         "Utility for examining python source files to ensure proper documentation. "
@@ -24,15 +24,15 @@
     author="Hunter McGushion",
     author_email="hunter@mcgushion.com",
     license="MIT",
     packages=["docstr_coverage"],
     install_requires=[
         "click",
         "PyYAML",
-        "tqdm==4.63.1",
+        "tqdm",
         "importlib_resources; python_version < '3.9'",
     ],
     extras_require={
         "lint": ["flake8==4.0.1", "black==22.3.0", "isort==5.10.1"],
         "test": ["pytest==6.2.5", "pytest-mock==3.4.0"],
     },
     include_package_data=True,
```

### Comparing `docstr-coverage-2.3.1/tests/sample_files/badges/0.svg` & `docstr-coverage-2.3.2/tests/sample_files/badges/0.svg`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.3.1/tests/sample_files/badges/100.svg` & `docstr-coverage-2.3.2/tests/sample_files/badges/100.svg`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.3.1/tests/sample_files/badges/12.svg` & `docstr-coverage-2.3.2/tests/sample_files/badges/12.svg`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.3.1/tests/sample_files/badges/54.svg` & `docstr-coverage-2.3.2/tests/sample_files/badges/54.svg`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.3.1/tests/sample_files/badges/71.svg` & `docstr-coverage-2.3.2/tests/sample_files/badges/71.svg`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.3.1/tests/sample_files/badges/84.svg` & `docstr-coverage-2.3.2/tests/sample_files/badges/84.svg`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.3.1/tests/sample_files/badges/94.svg` & `docstr-coverage-2.3.2/tests/sample_files/badges/94.svg`

 * *Files identical despite different names*

