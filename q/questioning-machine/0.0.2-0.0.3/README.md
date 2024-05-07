# Comparing `tmp/questioning_machine-0.0.2.tar.gz` & `tmp/questioning_machine-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questioning_machine-0.0.2.tar", last modified: Tue May  7 11:17:47 2024, max compression
+gzip compressed data, was "questioning_machine-0.0.3.tar", last modified: Tue May  7 18:38:44 2024, max compression
```

## Comparing `questioning_machine-0.0.2.tar` & `questioning_machine-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-07 11:17:47.281155 questioning_machine-0.0.2/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2024-05-07 11:04:57.000000 questioning_machine-0.0.2/LICENSE
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2024-05-07 11:11:20.000000 questioning_machine-0.0.2/MANIFEST.in
--rw-r--r--   0 alxfed    (1001) alxfed    (1001)      779 2024-05-07 11:17:47.281155 questioning_machine-0.0.2/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      156 2024-05-07 11:11:20.000000 questioning_machine-0.0.2/README.md
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      760 2024-05-07 11:15:42.000000 questioning_machine-0.0.2/pyproject.toml
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2024-05-07 11:17:47.281155 questioning_machine-0.0.2/setup.cfg
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-07 11:17:47.281155 questioning_machine-0.0.2/src/
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-07 11:17:47.281155 questioning_machine-0.0.2/src/questioning_machine/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      879 2024-05-07 11:11:20.000000 questioning_machine-0.0.2/src/questioning_machine/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1868 2024-05-07 11:04:57.000000 questioning_machine-0.0.2/src/questioning_machine/githf.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       70 2024-05-07 11:11:20.000000 questioning_machine-0.0.2/src/questioning_machine/machina.yaml
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-07 11:17:47.281155 questioning_machine-0.0.2/src/questioning_machine.egg-info/
--rw-r--r--   0 alxfed    (1001) alxfed    (1001)      779 2024-05-07 11:17:47.000000 questioning_machine-0.0.2/src/questioning_machine.egg-info/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      384 2024-05-07 11:17:47.000000 questioning_machine-0.0.2/src/questioning_machine.egg-info/SOURCES.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2024-05-07 11:17:47.000000 questioning_machine-0.0.2/src/questioning_machine.egg-info/dependency_links.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       30 2024-05-07 11:17:47.000000 questioning_machine-0.0.2/src/questioning_machine.egg-info/requires.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       20 2024-05-07 11:17:47.000000 questioning_machine-0.0.2/src/questioning_machine.egg-info/top_level.txt
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-07 18:38:44.636453 questioning_machine-0.0.3/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2024-05-07 11:04:57.000000 questioning_machine-0.0.3/LICENSE
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2024-05-07 11:11:20.000000 questioning_machine-0.0.3/MANIFEST.in
+-rw-r--r--   0 alxfed    (1001) alxfed    (1001)      781 2024-05-07 18:38:44.636453 questioning_machine-0.0.3/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      158 2024-05-07 11:18:57.000000 questioning_machine-0.0.3/README.md
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      760 2024-05-07 18:37:47.000000 questioning_machine-0.0.3/pyproject.toml
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2024-05-07 18:38:44.636453 questioning_machine-0.0.3/setup.cfg
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-07 18:38:44.612453 questioning_machine-0.0.3/src/
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-07 18:38:44.632453 questioning_machine-0.0.3/src/questioning_machine/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      879 2024-05-07 18:37:47.000000 questioning_machine-0.0.3/src/questioning_machine/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1868 2024-05-07 11:04:57.000000 questioning_machine-0.0.3/src/questioning_machine/githf.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       70 2024-05-07 11:11:20.000000 questioning_machine-0.0.3/src/questioning_machine/machina.yaml
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-07 18:38:44.636453 questioning_machine-0.0.3/src/questioning_machine.egg-info/
+-rw-r--r--   0 alxfed    (1001) alxfed    (1001)      781 2024-05-07 18:38:44.000000 questioning_machine-0.0.3/src/questioning_machine.egg-info/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      384 2024-05-07 18:38:44.000000 questioning_machine-0.0.3/src/questioning_machine.egg-info/SOURCES.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2024-05-07 18:38:44.000000 questioning_machine-0.0.3/src/questioning_machine.egg-info/dependency_links.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       30 2024-05-07 18:38:44.000000 questioning_machine-0.0.3/src/questioning_machine.egg-info/requires.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       20 2024-05-07 18:38:44.000000 questioning_machine-0.0.3/src/questioning_machine.egg-info/top_level.txt
```

### Comparing `questioning_machine-0.0.2/LICENSE` & `questioning_machine-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `questioning_machine-0.0.2/PKG-INFO` & `questioning_machine-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: questioning-machine
-Version: 0.0.2
+Version: 0.0.3
 Summary: Machine that asks questions.
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/questioning-machine/questioning-machine
 Project-URL: Bug Tracker, https://github.com/questioning-machine/questioning-machine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyGithub>=2.3.0
 Requires-Dist: PyYAML>=6.0.1
 
 # Questioning Machine
-Explanation of the Machine
+Machine that asks questions.
 <pre>
   pip install questioning-machine
 </pre>
 Then:
 ```Python
   # Python
   import questioning_machine
```

### Comparing `questioning_machine-0.0.2/pyproject.toml` & `questioning_machine-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "questioning-machine"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     {name="Alexander Fedotov", email="alex.fedotov@aol.com"},
 ]
 description = "Machine that asks questions."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers=[
```

### Comparing `questioning_machine-0.0.2/src/questioning_machine/__init__.py` & `questioning_machine-0.0.3/src/questioning_machine/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     MACHINE_YAML = githf.read_file(repository=gh, file_path='machina.yaml')
 
 except Exception as e:
     machina_path = os.path.join(os.path.dirname(__file__), 'machina.yaml')
     with open(machina_path, 'r') as yaml_file:
         MACHINE_YAML = yaml_file.read()
 
-NAME_OF_THE_MACHINE = yaml.load(MACHINE_YAML, Loader=yaml.FullLoader)
+QUESTIONING_MACHINE = yaml.load(MACHINE_YAML, Loader=yaml.FullLoader)
```

### Comparing `questioning_machine-0.0.2/src/questioning_machine/githf.py` & `questioning_machine-0.0.3/src/questioning_machine/githf.py`

 * *Files identical despite different names*

### Comparing `questioning_machine-0.0.2/src/questioning_machine.egg-info/PKG-INFO` & `questioning_machine-0.0.3/src/questioning_machine.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: questioning-machine
-Version: 0.0.2
+Version: 0.0.3
 Summary: Machine that asks questions.
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/questioning-machine/questioning-machine
 Project-URL: Bug Tracker, https://github.com/questioning-machine/questioning-machine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyGithub>=2.3.0
 Requires-Dist: PyYAML>=6.0.1
 
 # Questioning Machine
-Explanation of the Machine
+Machine that asks questions.
 <pre>
   pip install questioning-machine
 </pre>
 Then:
 ```Python
   # Python
   import questioning_machine
```

