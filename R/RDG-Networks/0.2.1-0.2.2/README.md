# Comparing `tmp/RDG-Networks-0.2.1.tar.gz` & `tmp/RDG-Networks-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RDG-Networks-0.2.1.tar", last modified: Mon May  6 18:45:02 2024, max compression
+gzip compressed data, was "RDG-Networks-0.2.2.tar", last modified: Mon May  6 19:47:16 2024, max compression
```

## Comparing `RDG-Networks-0.2.1.tar` & `RDG-Networks-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-06 18:45:02.212053 RDG-Networks-0.2.1/
--rw-r--r--   0 5746604    (501) staff       (20)     1066 2023-12-16 13:43:14.000000 RDG-Networks-0.2.1/LICENSE.txt
--rw-r--r--   0 5746604    (501) staff       (20)     1896 2024-05-06 18:45:02.211866 RDG-Networks-0.2.1/PKG-INFO
-drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-06 18:45:02.210615 RDG-Networks-0.2.1/RDG_Networks.egg-info/
--rw-r--r--   0 5746604    (501) staff       (20)     1896 2024-05-06 18:45:02.000000 RDG-Networks-0.2.1/RDG_Networks.egg-info/PKG-INFO
--rw-r--r--   0 5746604    (501) staff       (20)      527 2024-05-06 18:45:02.000000 RDG-Networks-0.2.1/RDG_Networks.egg-info/SOURCES.txt
--rw-r--r--   0 5746604    (501) staff       (20)        1 2024-05-06 18:45:02.000000 RDG-Networks-0.2.1/RDG_Networks.egg-info/dependency_links.txt
--rw-r--r--   0 5746604    (501) staff       (20)      350 2024-05-06 18:45:02.000000 RDG-Networks-0.2.1/RDG_Networks.egg-info/entry_points.txt
--rw-r--r--   0 5746604    (501) staff       (20)       36 2024-05-06 18:45:02.000000 RDG-Networks-0.2.1/RDG_Networks.egg-info/requires.txt
--rw-r--r--   0 5746604    (501) staff       (20)       13 2024-05-06 18:45:02.000000 RDG-Networks-0.2.1/RDG_Networks.egg-info/top_level.txt
-drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-06 18:45:02.211654 RDG-Networks-0.2.1/RDG_networks/
--rw-r--r--   0 5746604    (501) staff       (20)     7977 2024-03-04 14:31:37.000000 RDG-Networks-0.2.1/RDG_networks/Classes.py
--rw-r--r--   0 5746604    (501) staff       (20)      661 2024-05-06 18:35:06.000000 RDG-Networks-0.2.1/RDG_networks/__init__.py
--rw-r--r--   0 5746604    (501) staff       (20)      984 2024-03-04 14:31:54.000000 RDG-Networks-0.2.1/RDG_networks/draw_segments.py
--rw-r--r--   0 5746604    (501) staff       (20)     1127 2024-03-04 14:31:51.000000 RDG-Networks-0.2.1/RDG_networks/generate_line_network.py
--rw-r--r--   0 5746604    (501) staff       (20)     9004 2024-05-06 18:31:39.000000 RDG-Networks-0.2.1/RDG_networks/generate_line_segments.py
--rw-r--r--   0 5746604    (501) staff       (20)     7318 2024-05-06 18:44:46.000000 RDG-Networks-0.2.1/RDG_networks/generate_line_segments_dynamic.py
--rw-r--r--   0 5746604    (501) staff       (20)     2797 2024-03-04 14:52:33.000000 RDG-Networks-0.2.1/RDG_networks/get_intersection_segments.py
--rw-r--r--   0 5746604    (501) staff       (20)     1605 2024-03-01 14:53:20.000000 RDG-Networks-0.2.1/RDG_networks/sample_in_polygon.py
--rw-r--r--   0 5746604    (501) staff       (20)     1392 2024-05-06 18:33:00.000000 RDG-Networks-0.2.1/README.md
--rw-r--r--   0 5746604    (501) staff       (20)       38 2024-05-06 18:45:02.212099 RDG-Networks-0.2.1/setup.cfg
--rw-r--r--   0 5746604    (501) staff       (20)     1117 2024-05-06 18:44:43.000000 RDG-Networks-0.2.1/setup.py
+drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-06 19:47:16.351930 RDG-Networks-0.2.2/
+-rw-r--r--   0 5746604    (501) staff       (20)     1066 2023-12-16 13:43:14.000000 RDG-Networks-0.2.2/LICENSE.txt
+-rw-r--r--   0 5746604    (501) staff       (20)     1896 2024-05-06 19:47:16.351710 RDG-Networks-0.2.2/PKG-INFO
+drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-06 19:47:16.349671 RDG-Networks-0.2.2/RDG_Networks.egg-info/
+-rw-r--r--   0 5746604    (501) staff       (20)     1896 2024-05-06 19:47:16.000000 RDG-Networks-0.2.2/RDG_Networks.egg-info/PKG-INFO
+-rw-r--r--   0 5746604    (501) staff       (20)      527 2024-05-06 19:47:16.000000 RDG-Networks-0.2.2/RDG_Networks.egg-info/SOURCES.txt
+-rw-r--r--   0 5746604    (501) staff       (20)        1 2024-05-06 19:47:16.000000 RDG-Networks-0.2.2/RDG_Networks.egg-info/dependency_links.txt
+-rw-r--r--   0 5746604    (501) staff       (20)      350 2024-05-06 19:47:16.000000 RDG-Networks-0.2.2/RDG_Networks.egg-info/entry_points.txt
+-rw-r--r--   0 5746604    (501) staff       (20)       36 2024-05-06 19:47:16.000000 RDG-Networks-0.2.2/RDG_Networks.egg-info/requires.txt
+-rw-r--r--   0 5746604    (501) staff       (20)       13 2024-05-06 19:47:16.000000 RDG-Networks-0.2.2/RDG_Networks.egg-info/top_level.txt
+drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-06 19:47:16.351292 RDG-Networks-0.2.2/RDG_networks/
+-rw-r--r--   0 5746604    (501) staff       (20)     7977 2024-03-04 14:31:37.000000 RDG-Networks-0.2.2/RDG_networks/Classes.py
+-rw-r--r--   0 5746604    (501) staff       (20)      661 2024-05-06 18:35:06.000000 RDG-Networks-0.2.2/RDG_networks/__init__.py
+-rw-r--r--   0 5746604    (501) staff       (20)      984 2024-03-04 14:31:54.000000 RDG-Networks-0.2.2/RDG_networks/draw_segments.py
+-rw-r--r--   0 5746604    (501) staff       (20)     1127 2024-03-04 14:31:51.000000 RDG-Networks-0.2.2/RDG_networks/generate_line_network.py
+-rw-r--r--   0 5746604    (501) staff       (20)     9004 2024-05-06 18:31:39.000000 RDG-Networks-0.2.2/RDG_networks/generate_line_segments.py
+-rw-r--r--   0 5746604    (501) staff       (20)     7438 2024-05-06 19:46:48.000000 RDG-Networks-0.2.2/RDG_networks/generate_line_segments_dynamic.py
+-rw-r--r--   0 5746604    (501) staff       (20)     2797 2024-03-04 14:52:33.000000 RDG-Networks-0.2.2/RDG_networks/get_intersection_segments.py
+-rw-r--r--   0 5746604    (501) staff       (20)     1605 2024-03-01 14:53:20.000000 RDG-Networks-0.2.2/RDG_networks/sample_in_polygon.py
+-rw-r--r--   0 5746604    (501) staff       (20)     1392 2024-05-06 18:33:00.000000 RDG-Networks-0.2.2/README.md
+-rw-r--r--   0 5746604    (501) staff       (20)       38 2024-05-06 19:47:16.351976 RDG-Networks-0.2.2/setup.cfg
+-rw-r--r--   0 5746604    (501) staff       (20)     1117 2024-05-06 19:47:10.000000 RDG-Networks-0.2.2/setup.py
```

### Comparing `RDG-Networks-0.2.1/LICENSE.txt` & `RDG-Networks-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.1/PKG-INFO` & `RDG-Networks-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RDG-Networks
-Version: 0.2.1
+Version: 0.2.2
 Summary: Most of the code from the RDG Networks project
 Home-page: https://github.com/NiekMooij/RDG_networks
 Author: Niek Mooij
 Author-email: mooij.niek@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `RDG-Networks-0.2.1/RDG_Networks.egg-info/PKG-INFO` & `RDG-Networks-0.2.2/RDG_Networks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RDG-Networks
-Version: 0.2.1
+Version: 0.2.2
 Summary: Most of the code from the RDG Networks project
 Home-page: https://github.com/NiekMooij/RDG_networks
 Author: Niek Mooij
 Author-email: mooij.niek@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `RDG-Networks-0.2.1/RDG_Networks.egg-info/SOURCES.txt` & `RDG-Networks-0.2.2/RDG_Networks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.1/RDG_networks/Classes.py` & `RDG-Networks-0.2.2/RDG_networks/Classes.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.1/RDG_networks/__init__.py` & `RDG-Networks-0.2.2/RDG_networks/__init__.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.1/RDG_networks/draw_segments.py` & `RDG-Networks-0.2.2/RDG_networks/draw_segments.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.1/RDG_networks/generate_line_network.py` & `RDG-Networks-0.2.2/RDG_networks/generate_line_network.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.1/RDG_networks/generate_line_segments.py` & `RDG-Networks-0.2.2/RDG_networks/generate_line_segments.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.1/RDG_networks/generate_line_segments_dynamic.py` & `RDG-Networks-0.2.2/RDG_networks/generate_line_segments_dynamic.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,14 +100,17 @@
         List[Dict[str, Any]]: The updated list of lines after handling intersections.
     """
     for index1, j1 in enumerate(lines):
         for index2, j2 in enumerate(lines):
             if j1['id'][:-2] == j2['id'][:-2] or index2 < index1:
                 continue
                 
+            if j1['growth_status'] == False and j2['growth_status'] == False:
+                continue
+                
             line1 = LineString([j1['start'], j1['end']])
             line2 = LineString([j2['start'], j2['end']])
 
             intersection_pt = line1.intersection(line2)
 
             if not intersection_pt.is_empty:
                 d1 = np.linalg.norm(np.array(j1['start']) - np.array([intersection_pt.x, intersection_pt.y]))
```

### Comparing `RDG-Networks-0.2.1/RDG_networks/get_intersection_segments.py` & `RDG-Networks-0.2.2/RDG_networks/get_intersection_segments.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.1/RDG_networks/sample_in_polygon.py` & `RDG-Networks-0.2.2/RDG_networks/sample_in_polygon.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.1/README.md` & `RDG-Networks-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.1/setup.py` & `RDG-Networks-0.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RDG-Networks',
-    version='0.2.1',
+    version='0.2.2',
     author='Niek Mooij',
     author_email='mooij.niek@gmail.com',
     description='Most of the code from the RDG Networks project',
     long_description=open('README.md').read(),
     url='https://github.com/NiekMooij/RDG_networks',
     classifiers=[
             'Programming Language :: Python :: 3',
```

