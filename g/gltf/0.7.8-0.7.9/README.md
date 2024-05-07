# Comparing `tmp/gltf-0.7.8.tar.gz` & `tmp/gltf-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gltf-0.7.8.tar", last modified: Wed May 19 04:34:10 2021, max compression
+gzip compressed data, was "dist/gltf-0.7.9.tar", last modified: Wed May 19 05:01:33 2021, max compression
```

## Comparing `gltf-0.7.8.tar` & `gltf-0.7.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 trey      (1000) trey      (1000)        0 2021-05-19 04:34:10.137837 gltf-0.7.8/
--rw-rw-r--   0 trey      (1000) trey      (1000)      633 2021-05-19 04:34:10.137837 gltf-0.7.8/PKG-INFO
--rw-r--r--   0 trey      (1000) trey      (1000)      299 2021-05-07 16:35:18.000000 gltf-0.7.8/README.md
-drwxrwxr-x   0 trey      (1000) trey      (1000)        0 2021-05-19 04:34:10.133837 gltf-0.7.8/bin/
--rw-r--r--   0 trey      (1000) trey      (1000)      474 2019-11-07 20:34:24.000000 gltf-0.7.8/bin/gltf-op
-drwxrwxr-x   0 trey      (1000) trey      (1000)        0 2021-05-19 04:34:10.137837 gltf-0.7.8/gltf/
--rw-rw-r--   0 trey      (1000) trey      (1000)      498 2021-02-10 23:18:00.000000 gltf-0.7.8/gltf/__init__.py
--rw-r--r--   0 trey      (1000) trey      (1000)     6150 2020-07-31 18:38:00.000000 gltf-0.7.8/gltf/animations.py
--rw-r--r--   0 trey      (1000) trey      (1000)    11549 2021-05-12 16:27:20.000000 gltf-0.7.8/gltf/buffers.py
--rw-r--r--   0 trey      (1000) trey      (1000)    20220 2021-05-12 16:31:39.000000 gltf-0.7.8/gltf/gltf.py
--rw-r--r--   0 trey      (1000) trey      (1000)    26614 2021-05-02 16:18:11.000000 gltf-0.7.8/gltf/materials.py
--rw-rw-r--   0 trey      (1000) trey      (1000)    24221 2021-04-28 23:59:10.000000 gltf-0.7.8/gltf/nodes.py
--rw-rw-r--   0 trey      (1000) trey      (1000)    30741 2021-05-19 03:11:38.000000 gltf-0.7.8/gltf/ops.py
--rw-r--r--   0 trey      (1000) trey      (1000)      901 2019-09-26 21:50:12.000000 gltf-0.7.8/gltf/utils.py
-drwxrwxr-x   0 trey      (1000) trey      (1000)        0 2021-05-19 04:34:10.137837 gltf-0.7.8/gltf.egg-info/
--rw-r--r--   0 trey      (1000) trey      (1000)      633 2021-05-19 04:34:10.000000 gltf-0.7.8/gltf.egg-info/PKG-INFO
--rw-r--r--   0 trey      (1000) trey      (1000)      319 2021-05-19 04:34:10.000000 gltf-0.7.8/gltf.egg-info/SOURCES.txt
--rw-r--r--   0 trey      (1000) trey      (1000)        1 2021-05-19 04:34:10.000000 gltf-0.7.8/gltf.egg-info/dependency_links.txt
--rw-r--r--   0 trey      (1000) trey      (1000)        1 2019-09-26 21:50:31.000000 gltf-0.7.8/gltf.egg-info/not-zip-safe
--rw-r--r--   0 trey      (1000) trey      (1000)       35 2021-05-19 04:34:10.000000 gltf-0.7.8/gltf.egg-info/requires.txt
--rw-r--r--   0 trey      (1000) trey      (1000)        5 2021-05-19 04:34:10.000000 gltf-0.7.8/gltf.egg-info/top_level.txt
--rw-rw-r--   0 trey      (1000) trey      (1000)       38 2021-05-19 04:34:10.137837 gltf-0.7.8/setup.cfg
--rw-r--r--   0 trey      (1000) trey      (1000)      925 2021-05-19 04:33:46.000000 gltf-0.7.8/setup.py
+drwxrwxr-x   0 trey      (1000) trey      (1000)        0 2021-05-19 05:01:33.497520 gltf-0.7.9/
+-rw-rw-r--   0 trey      (1000) trey      (1000)      633 2021-05-19 05:01:33.497520 gltf-0.7.9/PKG-INFO
+-rw-r--r--   0 trey      (1000) trey      (1000)      299 2021-05-07 16:35:18.000000 gltf-0.7.9/README.md
+drwxrwxr-x   0 trey      (1000) trey      (1000)        0 2021-05-19 05:01:33.493520 gltf-0.7.9/bin/
+-rw-r--r--   0 trey      (1000) trey      (1000)      474 2019-11-07 20:34:24.000000 gltf-0.7.9/bin/gltf-op
+drwxrwxr-x   0 trey      (1000) trey      (1000)        0 2021-05-19 05:01:33.493520 gltf-0.7.9/gltf/
+-rw-rw-r--   0 trey      (1000) trey      (1000)      498 2021-02-10 23:18:00.000000 gltf-0.7.9/gltf/__init__.py
+-rw-r--r--   0 trey      (1000) trey      (1000)     6150 2020-07-31 18:38:00.000000 gltf-0.7.9/gltf/animations.py
+-rw-r--r--   0 trey      (1000) trey      (1000)    11549 2021-05-12 16:27:20.000000 gltf-0.7.9/gltf/buffers.py
+-rw-r--r--   0 trey      (1000) trey      (1000)    20220 2021-05-12 16:31:39.000000 gltf-0.7.9/gltf/gltf.py
+-rw-r--r--   0 trey      (1000) trey      (1000)    26614 2021-05-02 16:18:11.000000 gltf-0.7.9/gltf/materials.py
+-rw-rw-r--   0 trey      (1000) trey      (1000)    24257 2021-05-19 05:01:13.000000 gltf-0.7.9/gltf/nodes.py
+-rw-rw-r--   0 trey      (1000) trey      (1000)    30741 2021-05-19 03:11:38.000000 gltf-0.7.9/gltf/ops.py
+-rw-r--r--   0 trey      (1000) trey      (1000)      901 2019-09-26 21:50:12.000000 gltf-0.7.9/gltf/utils.py
+drwxrwxr-x   0 trey      (1000) trey      (1000)        0 2021-05-19 05:01:33.497520 gltf-0.7.9/gltf.egg-info/
+-rw-r--r--   0 trey      (1000) trey      (1000)      633 2021-05-19 05:01:33.000000 gltf-0.7.9/gltf.egg-info/PKG-INFO
+-rw-r--r--   0 trey      (1000) trey      (1000)      319 2021-05-19 05:01:33.000000 gltf-0.7.9/gltf.egg-info/SOURCES.txt
+-rw-r--r--   0 trey      (1000) trey      (1000)        1 2021-05-19 05:01:33.000000 gltf-0.7.9/gltf.egg-info/dependency_links.txt
+-rw-r--r--   0 trey      (1000) trey      (1000)        1 2019-09-26 21:50:31.000000 gltf-0.7.9/gltf.egg-info/not-zip-safe
+-rw-r--r--   0 trey      (1000) trey      (1000)       35 2021-05-19 05:01:33.000000 gltf-0.7.9/gltf.egg-info/requires.txt
+-rw-r--r--   0 trey      (1000) trey      (1000)        5 2021-05-19 05:01:33.000000 gltf-0.7.9/gltf.egg-info/top_level.txt
+-rw-rw-r--   0 trey      (1000) trey      (1000)       38 2021-05-19 05:01:33.497520 gltf-0.7.9/setup.cfg
+-rw-r--r--   0 trey      (1000) trey      (1000)      925 2021-05-19 05:01:29.000000 gltf-0.7.9/setup.py
```

### Comparing `gltf-0.7.8/PKG-INFO` & `gltf-0.7.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: gltf
-Version: 0.7.8
+Version: 0.7.9
 Summary: Load, modify, and save GLTF files.
 Home-page: https://gitlab.com/seekxr/py-gltf
 Author: Trey Nelson
 Author-email: trey@seekxr.com
 License: Public Domain
 Description: GLTF provides the ability to load, modify, and save GLTF/GLB files.
```

### Comparing `gltf-0.7.8/gltf/animations.py` & `gltf-0.7.9/gltf/animations.py`

 * *Files identical despite different names*

### Comparing `gltf-0.7.8/gltf/buffers.py` & `gltf-0.7.9/gltf/buffers.py`

 * *Files identical despite different names*

### Comparing `gltf-0.7.8/gltf/gltf.py` & `gltf-0.7.9/gltf/gltf.py`

 * *Files identical despite different names*

### Comparing `gltf-0.7.8/gltf/materials.py` & `gltf-0.7.9/gltf/materials.py`

 * *Files identical despite different names*

### Comparing `gltf-0.7.8/gltf/nodes.py` & `gltf-0.7.9/gltf/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -330,19 +330,19 @@
             self.texcoords = texcoords if texcoords is not None else []
             self.colors = colors if colors is not None else []
             self.joints = joints if joints is not None else []
             self.weights = weights if weights is not None else []
 
     def render(self, gltf):
         attributes = {}
-        if self.positions and self.positions.count:
+        if self.positions is not None and self.positions.count:
             attributes['POSITION'] = gltf.index('accessors', self.positions)
-        if self.normals and self.normals.count:
+        if self.normals is not None and self.normals.count:
             attributes['NORMAL'] = gltf.index('accessors', self.normals)
-        if self.tangents and self.tangents.count:
+        if self.tangents is not None and self.tangents.count:
             attributes['TANGENT'] = gltf.index('accessors', self.tangents)
         for i, texcoords in enumerate(self.texcoords):
             attributes['TEXCOORD_' + str(i)] = gltf.index('accessors', texcoords)
         for i, colors in enumerate(self.colors):
             attributes['COLOR_' + str(i)] = gltf.index('accessors', colors)
         for i, joints in enumerate(self.joints):
             attributes['JOINTS_' + str(i)] = gltf.index('accessors', joints)
```

### Comparing `gltf-0.7.8/gltf/ops.py` & `gltf-0.7.9/gltf/ops.py`

 * *Files identical despite different names*

### Comparing `gltf-0.7.8/gltf/utils.py` & `gltf-0.7.9/gltf/utils.py`

 * *Files identical despite different names*

### Comparing `gltf-0.7.8/gltf.egg-info/PKG-INFO` & `gltf-0.7.9/gltf.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: gltf
-Version: 0.7.8
+Version: 0.7.9
 Summary: Load, modify, and save GLTF files.
 Home-page: https://gitlab.com/seekxr/py-gltf
 Author: Trey Nelson
 Author-email: trey@seekxr.com
 License: Public Domain
 Description: GLTF provides the ability to load, modify, and save GLTF/GLB files.
```

### Comparing `gltf-0.7.8/setup.py` & `gltf-0.7.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
-VERSION = '0.7.8'
+VERSION = '0.7.9'
 
 DESCRIPTION = """GLTF provides the ability to load, modify, and save GLTF/GLB files.
 
 [GLTF](https://www.khronos.org/gltf/) is an open 3D model standard by the Khronos Group.
 """
 
 DEPENDENCIES = ['numpy', 'pyquaternion', 'pillow', 'requests']
```

