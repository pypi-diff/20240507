# Comparing `tmp/gym_xarm-0.1.0.tar.gz` & `tmp/gym_xarm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym_xarm-0.1.0.tar", max compression
+gzip compressed data, was "gym_xarm-0.1.1.tar", max compression
```

## Comparing `gym_xarm-0.1.0.tar` & `gym_xarm-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    12597 2024-04-02 08:59:54.731564 gym_xarm-0.1.0/LICENSE
--rw-r--r--   0        0        0     3133 2024-05-03 13:43:39.142927 gym_xarm-0.1.0/README.md
--rw-r--r--   0        0        0      193 2024-04-07 16:59:39.111767 gym_xarm-0.1.0/gym_xarm/__init__.py
--rw-r--r--   0        0        0     1333 2024-04-07 16:59:39.111767 gym_xarm-0.1.0/gym_xarm/tasks/__init__.py
--rw-r--r--   0        0        0     2744 2024-04-22 15:00:16.508341 gym_xarm-0.1.0/gym_xarm/tasks/assets/lift.xml
--rw-r--r--   0        0        0  1211434 2024-04-02 08:59:54.747564 gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/base_link.stl
--rw-r--r--   0        0        0     3284 2024-04-02 08:59:54.747564 gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/block_inner.stl
--rw-r--r--   0        0        0     3284 2024-04-02 08:59:54.747564 gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/block_inner2.stl
--rw-r--r--   0        0        0     6284 2024-04-02 08:59:54.747564 gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/block_outer.stl
--rw-r--r--   0        0        0   242684 2024-04-02 08:59:54.751564 gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/left_finger.stl
--rw-r--r--   0        0        0   366284 2024-04-02 08:59:54.751564 gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/left_inner_knuckle.stl
--rw-r--r--   0        0        0    22284 2024-04-02 08:59:54.751564 gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/left_outer_knuckle.stl
--rw-r--r--   0        0        0   184184 2024-04-02 08:59:54.755564 gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/link1.stl
--rw-r--r--   0        0        0   225584 2024-04-02 08:59:54.755564 gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/link2.stl
--rw-r--r--   0        0        0   237084 2024-04-02 08:59:54.759564 gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/link3.stl
--rw-r--r--   0        0        0   243684 2024-04-02 08:59:54.759564 gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/link4.stl
--rw-r--r--   0        0        0   229084 2024-04-02 08:59:54.759564 gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/link5.stl
--rw-r--r--   0        0        0   399384 2024-04-02 08:59:54.763564 gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/link6.stl
--rw-r--r--   0        0        0   231684 2024-04-02 08:59:54.763564 gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/link7.stl
--rw-r--r--   0        0        0  2106184 2024-04-02 08:59:54.771565 gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/link_base.stl
--rw-r--r--   0        0        0   242684 2024-04-02 08:59:54.775565 gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/right_finger.stl
--rw-r--r--   0        0        0   366284 2024-04-02 08:59:54.775565 gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/right_inner_knuckle.stl
--rw-r--r--   0        0        0    22284 2024-04-02 08:59:54.775565 gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/right_outer_knuckle.stl
--rw-r--r--   0        0        0     4348 2024-04-02 08:59:54.775565 gym_xarm-0.1.0/gym_xarm/tasks/assets/peg_in_box.xml
--rw-r--r--   0        0        0     2856 2024-04-02 08:59:54.775565 gym_xarm-0.1.0/gym_xarm/tasks/assets/push.xml
--rw-r--r--   0        0        0     2470 2024-04-02 08:59:54.775565 gym_xarm-0.1.0/gym_xarm/tasks/assets/reach.xml
--rw-r--r--   0        0        0     2758 2024-04-02 08:59:54.775565 gym_xarm-0.1.0/gym_xarm/tasks/assets/shared.xml
--rw-r--r--   0        0        0     9756 2024-04-02 08:59:54.775565 gym_xarm-0.1.0/gym_xarm/tasks/assets/xarm.xml
--rw-r--r--   0        0        0    12989 2024-05-03 13:43:17.090266 gym_xarm-0.1.0/gym_xarm/tasks/base.py
--rw-r--r--   0        0        0     3259 2024-05-03 13:43:17.090266 gym_xarm-0.1.0/gym_xarm/tasks/lift.py
--rw-r--r--   0        0        0     1995 2024-05-03 13:43:17.090266 gym_xarm-0.1.0/gym_xarm/tasks/mocap.py
--rw-r--r--   0        0        0     3142 2024-04-07 16:59:39.111767 gym_xarm-0.1.0/gym_xarm/tasks/peg_in_box.py
--rw-r--r--   0        0        0     2858 2024-04-07 16:59:39.111767 gym_xarm-0.1.0/gym_xarm/tasks/push.py
--rw-r--r--   0        0        0     1668 2024-04-07 16:59:39.111767 gym_xarm-0.1.0/gym_xarm/tasks/reach.py
--rw-r--r--   0        0        0     1751 2024-05-03 13:43:39.146927 gym_xarm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4272 1970-01-01 00:00:00.000000 gym_xarm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    12597 2024-04-06 12:56:20.411050 gym_xarm-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3133 2024-05-07 08:40:10.121778 gym_xarm-0.1.1/README.md
+-rw-r--r--   0        0        0      193 2024-04-07 12:48:54.241761 gym_xarm-0.1.1/gym_xarm/__init__.py
+-rw-r--r--   0        0        0     1333 2024-04-07 12:48:54.241925 gym_xarm-0.1.1/gym_xarm/tasks/__init__.py
+-rw-r--r--   0        0        0     2744 2024-04-06 12:56:20.411649 gym_xarm-0.1.1/gym_xarm/tasks/assets/lift.xml
+-rw-r--r--   0        0        0  1211434 2024-04-06 12:56:20.414517 gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/base_link.stl
+-rw-r--r--   0        0        0     3284 2024-04-06 12:56:20.414664 gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/block_inner.stl
+-rw-r--r--   0        0        0     3284 2024-04-06 12:56:20.414746 gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/block_inner2.stl
+-rw-r--r--   0        0        0     6284 2024-04-06 12:56:20.414907 gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/block_outer.stl
+-rw-r--r--   0        0        0   242684 2024-04-06 12:56:20.415389 gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/left_finger.stl
+-rw-r--r--   0        0        0   366284 2024-04-06 12:56:20.416150 gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/left_inner_knuckle.stl
+-rw-r--r--   0        0        0    22284 2024-04-06 12:56:20.416299 gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/left_outer_knuckle.stl
+-rw-r--r--   0        0        0   184184 2024-04-06 12:56:20.416832 gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/link1.stl
+-rw-r--r--   0        0        0   225584 2024-04-06 12:56:20.417478 gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/link2.stl
+-rw-r--r--   0        0        0   237084 2024-04-06 12:56:20.418147 gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/link3.stl
+-rw-r--r--   0        0        0   243684 2024-04-06 12:56:20.418806 gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/link4.stl
+-rw-r--r--   0        0        0   229084 2024-04-06 12:56:20.419444 gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/link5.stl
+-rw-r--r--   0        0        0   399384 2024-04-06 12:56:20.420512 gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/link6.stl
+-rw-r--r--   0        0        0   231684 2024-04-06 12:56:20.421691 gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/link7.stl
+-rw-r--r--   0        0        0  2106184 2024-04-06 12:56:20.426092 gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/link_base.stl
+-rw-r--r--   0        0        0   242684 2024-04-06 12:56:20.427138 gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/right_finger.stl
+-rw-r--r--   0        0        0   366284 2024-04-06 12:56:20.427771 gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/right_inner_knuckle.stl
+-rw-r--r--   0        0        0    22284 2024-04-06 12:56:20.431114 gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/right_outer_knuckle.stl
+-rw-r--r--   0        0        0     4348 2024-04-06 12:56:20.431261 gym_xarm-0.1.1/gym_xarm/tasks/assets/peg_in_box.xml
+-rw-r--r--   0        0        0     2856 2024-04-06 12:56:20.431333 gym_xarm-0.1.1/gym_xarm/tasks/assets/push.xml
+-rw-r--r--   0        0        0     2470 2024-04-06 12:56:20.431401 gym_xarm-0.1.1/gym_xarm/tasks/assets/reach.xml
+-rw-r--r--   0        0        0     2758 2024-04-06 12:56:20.431468 gym_xarm-0.1.1/gym_xarm/tasks/assets/shared.xml
+-rw-r--r--   0        0        0     9756 2024-04-06 12:56:20.431568 gym_xarm-0.1.1/gym_xarm/tasks/assets/xarm.xml
+-rw-r--r--   0        0        0    12989 2024-04-28 14:20:38.451194 gym_xarm-0.1.1/gym_xarm/tasks/base.py
+-rw-r--r--   0        0        0     3259 2024-04-28 14:22:19.568111 gym_xarm-0.1.1/gym_xarm/tasks/lift.py
+-rw-r--r--   0        0        0     1995 2024-04-28 13:59:21.512355 gym_xarm-0.1.1/gym_xarm/tasks/mocap.py
+-rw-r--r--   0        0        0     3142 2024-04-07 12:48:54.242592 gym_xarm-0.1.1/gym_xarm/tasks/peg_in_box.py
+-rw-r--r--   0        0        0     2858 2024-04-07 12:48:54.242720 gym_xarm-0.1.1/gym_xarm/tasks/push.py
+-rw-r--r--   0        0        0     1668 2024-04-07 12:48:54.242858 gym_xarm-0.1.1/gym_xarm/tasks/reach.py
+-rw-r--r--   0        0        0     1757 2024-05-07 08:47:49.970795 gym_xarm-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4229 1970-01-01 00:00:00.000000 gym_xarm-0.1.1/PKG-INFO
```

### Comparing `gym_xarm-0.1.0/LICENSE` & `gym_xarm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/README.md` & `gym_xarm-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/__init__.py` & `gym_xarm-0.1.1/gym_xarm/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/assets/lift.xml` & `gym_xarm-0.1.1/gym_xarm/tasks/assets/lift.xml`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/base_link.stl` & `gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/base_link.stl`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/block_inner.stl` & `gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/block_inner.stl`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/block_inner2.stl` & `gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/block_inner2.stl`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/block_outer.stl` & `gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/block_outer.stl`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/left_finger.stl` & `gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/left_finger.stl`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/left_inner_knuckle.stl` & `gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/left_inner_knuckle.stl`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/left_outer_knuckle.stl` & `gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/left_outer_knuckle.stl`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/link1.stl` & `gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/link1.stl`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/link2.stl` & `gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/link2.stl`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/link3.stl` & `gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/link3.stl`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/link4.stl` & `gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/link4.stl`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/link5.stl` & `gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/link5.stl`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/link6.stl` & `gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/link6.stl`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/link7.stl` & `gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/link7.stl`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/link_base.stl` & `gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/link_base.stl`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/right_finger.stl` & `gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/right_finger.stl`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/right_inner_knuckle.stl` & `gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/right_inner_knuckle.stl`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/assets/mesh/right_outer_knuckle.stl` & `gym_xarm-0.1.1/gym_xarm/tasks/assets/mesh/right_outer_knuckle.stl`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/assets/peg_in_box.xml` & `gym_xarm-0.1.1/gym_xarm/tasks/assets/peg_in_box.xml`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/assets/push.xml` & `gym_xarm-0.1.1/gym_xarm/tasks/assets/push.xml`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/assets/reach.xml` & `gym_xarm-0.1.1/gym_xarm/tasks/assets/reach.xml`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/assets/shared.xml` & `gym_xarm-0.1.1/gym_xarm/tasks/assets/shared.xml`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/assets/xarm.xml` & `gym_xarm-0.1.1/gym_xarm/tasks/assets/xarm.xml`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/base.py` & `gym_xarm-0.1.1/gym_xarm/tasks/base.py`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/lift.py` & `gym_xarm-0.1.1/gym_xarm/tasks/lift.py`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/mocap.py` & `gym_xarm-0.1.1/gym_xarm/tasks/mocap.py`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/peg_in_box.py` & `gym_xarm-0.1.1/gym_xarm/tasks/peg_in_box.py`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/push.py` & `gym_xarm-0.1.1/gym_xarm/tasks/push.py`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/gym_xarm/tasks/reach.py` & `gym_xarm-0.1.1/gym_xarm/tasks/reach.py`

 * *Files identical despite different names*

### Comparing `gym_xarm-0.1.0/pyproject.toml` & `gym_xarm-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gym-xarm"
-version = "0.1.0"
+version = "0.1.1"
 description = "A gym environment for xArm"
 authors = [
     "Rémi Cadène <re.cadene@gmail.com>",
     "Quentin Gallouédec <quentin.gallouedec@ec-lyon.fr>",
     "Alexander Soare <alexander.soare159@gmail.com>",
     "Simon Alibert <alibert.sim@gmail.com>",
 ]
@@ -20,20 +20,20 @@
 ]
 packages = [{include = "gym_xarm"}]
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 mujoco = "^2.3.7"
-gymnasium = "^0.29.1"
-gymnasium-robotics = "^1.2.4"
-pre-commit = {version = "^3.7.0", optional = true}
-debugpy = {version = "^1.8.1", optional = true}
-pytest = {version = "^8.1.0", optional = true}
-pytest-cov = {version = "^5.0.0", optional = true}
+gymnasium = ">=0.29.1"
+gymnasium-robotics = ">=1.2.4"
+pre-commit = {version = ">=3.7.0", optional = true}
+debugpy = {version = ">=1.8.1", optional = true}
+pytest = {version = ">=8.1.0", optional = true}
+pytest-cov = {version = ">=5.0.0", optional = true}
 
 
 [tool.poetry.extras]
 dev = ["pre-commit", "debugpy"]
 test = ["pytest", "pytest-cov"]
```

### Comparing `gym_xarm-0.1.0/PKG-INFO` & `gym_xarm-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-xarm
-Version: 0.1.0
+Version: 0.1.1
 Summary: A gym environment for xArm
 License: Apache-2.0
 Keywords: robotics,deep,reinforcement,learning,xarm,environment,gym,gymnasium,mujoco
 Author: Rémi Cadène
 Author-email: re.cadene@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -13,21 +13,21 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Build Tools
 Provides-Extra: dev
 Provides-Extra: test
-Requires-Dist: debugpy (>=1.8.1,<2.0.0) ; extra == "dev"
-Requires-Dist: gymnasium (>=0.29.1,<0.30.0)
-Requires-Dist: gymnasium-robotics (>=1.2.4,<2.0.0)
+Requires-Dist: debugpy (>=1.8.1) ; extra == "dev"
+Requires-Dist: gymnasium (>=0.29.1)
+Requires-Dist: gymnasium-robotics (>=1.2.4)
 Requires-Dist: mujoco (>=2.3.7,<3.0.0)
-Requires-Dist: pre-commit (>=3.7.0,<4.0.0) ; extra == "dev"
-Requires-Dist: pytest (>=8.1.0,<9.0.0) ; extra == "test"
-Requires-Dist: pytest-cov (>=5.0.0,<6.0.0) ; extra == "test"
+Requires-Dist: pre-commit (>=3.7.0) ; extra == "dev"
+Requires-Dist: pytest (>=8.1.0) ; extra == "test"
+Requires-Dist: pytest-cov (>=5.0.0) ; extra == "test"
 Description-Content-Type: text/markdown
 
 # gym-xarm
 
 A gym environment for xArm
 
 <td><img src="http://remicadene.com/assets/gif/simxarm_tdmpc.gif" width="50%" alt="TDMPC policy on xArm env"/></td>
```

