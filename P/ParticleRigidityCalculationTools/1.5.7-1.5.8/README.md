# Comparing `tmp/particlerigiditycalculationtools-1.5.7.tar.gz` & `tmp/particlerigiditycalculationtools-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "particlerigiditycalculationtools-1.5.7.tar", last modified: Thu Apr 18 12:31:19 2024, max compression
+gzip compressed data, was "particlerigiditycalculationtools-1.5.8.tar", last modified: Mon May  6 22:27:01 2024, max compression
```

## Comparing `particlerigiditycalculationtools-1.5.7.tar` & `particlerigiditycalculationtools-1.5.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:19.650439 particlerigiditycalculationtools-1.5.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-18 12:31:14.000000 particlerigiditycalculationtools-1.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-18 12:31:19.650439 particlerigiditycalculationtools-1.5.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:19.650439 particlerigiditycalculationtools-1.5.7/ParticleRigidityCalculationTools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-18 12:31:19.000000 particlerigiditycalculationtools-1.5.7/ParticleRigidityCalculationTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-18 12:31:19.000000 particlerigiditycalculationtools-1.5.7/ParticleRigidityCalculationTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:31:19.000000 particlerigiditycalculationtools-1.5.7/ParticleRigidityCalculationTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 12:31:19.000000 particlerigiditycalculationtools-1.5.7/ParticleRigidityCalculationTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-18 12:31:19.000000 particlerigiditycalculationtools-1.5.7/ParticleRigidityCalculationTools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-04-18 12:31:14.000000 particlerigiditycalculationtools-1.5.7/ParticleRigidityCalculationTools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-04-18 12:31:14.000000 particlerigiditycalculationtools-1.5.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 12:31:19.650439 particlerigiditycalculationtools-1.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-18 12:31:14.000000 particlerigiditycalculationtools-1.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:27:01.831522 particlerigiditycalculationtools-1.5.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-06 22:26:56.000000 particlerigiditycalculationtools-1.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-05-06 22:27:01.831522 particlerigiditycalculationtools-1.5.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:27:01.831522 particlerigiditycalculationtools-1.5.8/ParticleRigidityCalculationTools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-05-06 22:27:01.000000 particlerigiditycalculationtools-1.5.8/ParticleRigidityCalculationTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-06 22:27:01.000000 particlerigiditycalculationtools-1.5.8/ParticleRigidityCalculationTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 22:27:01.000000 particlerigiditycalculationtools-1.5.8/ParticleRigidityCalculationTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-06 22:27:01.000000 particlerigiditycalculationtools-1.5.8/ParticleRigidityCalculationTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-06 22:27:01.000000 particlerigiditycalculationtools-1.5.8/ParticleRigidityCalculationTools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-05-06 22:26:56.000000 particlerigiditycalculationtools-1.5.8/ParticleRigidityCalculationTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-06 22:26:56.000000 particlerigiditycalculationtools-1.5.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 22:27:01.831522 particlerigiditycalculationtools-1.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-06 22:26:56.000000 particlerigiditycalculationtools-1.5.8/setup.py
```

### Comparing `particlerigiditycalculationtools-1.5.7/LICENSE` & `particlerigiditycalculationtools-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `particlerigiditycalculationtools-1.5.7/PKG-INFO` & `particlerigiditycalculationtools-1.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParticleRigidityCalculationTools
-Version: 1.5.7
+Version: 1.5.8
 Summary: Python library containing tools for dealing with conversions between particle energy and rigidity
 Home-page: https://github.com/ChrisSWDavis/ParticleRigidityCalculationTools
 Author: Chris S. W. Davis
 Author-email: ChrisSWDavis@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `particlerigiditycalculationtools-1.5.7/ParticleRigidityCalculationTools.egg-info/PKG-INFO` & `particlerigiditycalculationtools-1.5.8/ParticleRigidityCalculationTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParticleRigidityCalculationTools
-Version: 1.5.7
+Version: 1.5.8
 Summary: Python library containing tools for dealing with conversions between particle energy and rigidity
 Home-page: https://github.com/ChrisSWDavis/ParticleRigidityCalculationTools
 Author: Chris S. W. Davis
 Author-email: ChrisSWDavis@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `particlerigiditycalculationtools-1.5.7/ParticleRigidityCalculationTools.py` & `particlerigiditycalculationtools-1.5.8/ParticleRigidityCalculationTools.py`

 * *Files identical despite different names*

### Comparing `particlerigiditycalculationtools-1.5.7/README.md` & `particlerigiditycalculationtools-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `particlerigiditycalculationtools-1.5.7/setup.py` & `particlerigiditycalculationtools-1.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='ParticleRigidityCalculationTools',
     py_modules=["ParticleRigidityCalculationTools"],
-    version='1.5.7',
+    version='1.5.8',
     description='Python library containing tools for dealing with conversions between particle energy and rigidity',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Chris S. W. Davis',
     author_email='ChrisSWDavis@gmail.com',
     license='MIT',
     url='https://github.com/ChrisSWDavis/ParticleRigidityCalculationTools',
```

