# Comparing `tmp/gym_aloha-0.1.0.tar.gz` & `tmp/gym_aloha-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym_aloha-0.1.0.tar", max compression
+gzip compressed data, was "gym_aloha-0.1.1.tar", max compression
```

## Comparing `gym_aloha-0.1.0.tar` & `gym_aloha-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    12582 2024-04-07 17:16:47.213194 gym_aloha-0.1.0/LICENSE
--rw-r--r--   0        0        0     4014 2024-05-03 13:40:16.306466 gym_aloha-0.1.0/README.md
--rw-r--r--   0        0        0      746 2024-04-07 17:26:55.922834 gym_aloha-0.1.0/gym_aloha/__init__.py
--rw-r--r--   0        0        0     3590 2024-04-07 16:57:12.996351 gym_aloha-0.1.0/gym_aloha/assets/bimanual_viperx_end_effector_insertion.xml
--rw-r--r--   0        0        0     2314 2024-04-07 16:57:12.996351 gym_aloha-0.1.0/gym_aloha/assets/bimanual_viperx_end_effector_transfer_cube.xml
--rw-r--r--   0        0        0     4262 2024-04-07 16:57:12.996351 gym_aloha-0.1.0/gym_aloha/assets/bimanual_viperx_insertion.xml
--rw-r--r--   0        0        0     2986 2024-04-07 16:57:12.996351 gym_aloha-0.1.0/gym_aloha/assets/bimanual_viperx_transfer_cube.xml
--rw-r--r--   0        0        0     1695 2024-04-07 16:57:12.996351 gym_aloha-0.1.0/gym_aloha/assets/scene.xml
--rw-r--r--   0        0        0      684 2024-04-07 16:57:12.996351 gym_aloha-0.1.0/gym_aloha/assets/tabletop.stl
--rw-r--r--   0        0        0    83384 2024-04-07 16:57:13.000351 gym_aloha-0.1.0/gym_aloha/assets/vx300s_10_custom_finger_left.stl
--rw-r--r--   0        0        0    83384 2024-04-07 16:57:13.000351 gym_aloha-0.1.0/gym_aloha/assets/vx300s_10_custom_finger_right.stl
--rw-r--r--   0        0        0    42884 2024-04-07 16:57:13.000351 gym_aloha-0.1.0/gym_aloha/assets/vx300s_10_gripper_finger.stl
--rw-r--r--   0        0        0     3884 2024-04-07 16:57:13.000351 gym_aloha-0.1.0/gym_aloha/assets/vx300s_11_ar_tag.stl
--rw-r--r--   0        0        0    99984 2024-04-07 16:57:13.000351 gym_aloha-0.1.0/gym_aloha/assets/vx300s_1_base.stl
--rw-r--r--   0        0        0    63884 2024-04-07 16:57:13.000351 gym_aloha-0.1.0/gym_aloha/assets/vx300s_2_shoulder.stl
--rw-r--r--   0        0        0   102984 2024-04-07 16:57:13.000351 gym_aloha-0.1.0/gym_aloha/assets/vx300s_3_upper_arm.stl
--rw-r--r--   0        0        0    49584 2024-04-07 16:57:13.000351 gym_aloha-0.1.0/gym_aloha/assets/vx300s_4_upper_forearm.stl
--rw-r--r--   0        0        0    99884 2024-04-07 16:57:13.004351 gym_aloha-0.1.0/gym_aloha/assets/vx300s_5_lower_forearm.stl
--rw-r--r--   0        0        0    70784 2024-04-07 16:57:13.004351 gym_aloha-0.1.0/gym_aloha/assets/vx300s_6_wrist.stl
--rw-r--r--   0        0        0   450084 2024-04-07 16:57:13.004351 gym_aloha-0.1.0/gym_aloha/assets/vx300s_7_gripper.stl
--rw-r--r--   0        0        0    31684 2024-04-07 16:57:13.004351 gym_aloha-0.1.0/gym_aloha/assets/vx300s_8_gripper_prop.stl
--rw-r--r--   0        0        0   379484 2024-04-07 16:57:13.004351 gym_aloha-0.1.0/gym_aloha/assets/vx300s_9_gripper_bar.stl
--rw-r--r--   0        0        0     1272 2024-04-07 16:57:13.008351 gym_aloha-0.1.0/gym_aloha/assets/vx300s_dependencies.xml
--rw-r--r--   0        0        0     6501 2024-04-07 16:57:13.008351 gym_aloha-0.1.0/gym_aloha/assets/vx300s_left.xml
--rw-r--r--   0        0        0     6556 2024-04-07 16:57:13.008351 gym_aloha-0.1.0/gym_aloha/assets/vx300s_right.xml
--rw-r--r--   0        0        0     4575 2024-04-07 16:57:12.988350 gym_aloha-0.1.0/gym_aloha/constants.py
--rw-r--r--   0        0        0     6752 2024-05-03 13:40:04.625994 gym_aloha-0.1.0/gym_aloha/env.py
--rw-r--r--   0        0        0     9726 2024-04-07 17:04:22.050320 gym_aloha-0.1.0/gym_aloha/tasks/sim.py
--rw-r--r--   0        0        0    11602 2024-04-07 17:04:22.050320 gym_aloha-0.1.0/gym_aloha/tasks/sim_end_effector.py
--rw-r--r--   0        0        0     1098 2024-04-07 16:57:12.996351 gym_aloha-0.1.0/gym_aloha/utils.py
--rw-r--r--   0        0        0     1814 2024-05-03 13:40:16.306466 gym_aloha-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5202 1970-01-01 00:00:00.000000 gym_aloha-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    12582 2024-04-28 15:22:17.980882 gym_aloha-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4014 2024-05-07 08:39:21.378827 gym_aloha-0.1.1/README.md
+-rw-r--r--   0        0        0      746 2024-04-28 15:22:17.981364 gym_aloha-0.1.1/gym_aloha/__init__.py
+-rw-r--r--   0        0        0     3590 2024-04-28 15:22:17.981530 gym_aloha-0.1.1/gym_aloha/assets/bimanual_viperx_end_effector_insertion.xml
+-rw-r--r--   0        0        0     2314 2024-04-28 15:22:17.981783 gym_aloha-0.1.1/gym_aloha/assets/bimanual_viperx_end_effector_transfer_cube.xml
+-rw-r--r--   0        0        0     4262 2024-04-28 15:22:17.981899 gym_aloha-0.1.1/gym_aloha/assets/bimanual_viperx_insertion.xml
+-rw-r--r--   0        0        0     2986 2024-04-28 15:22:17.981999 gym_aloha-0.1.1/gym_aloha/assets/bimanual_viperx_transfer_cube.xml
+-rw-r--r--   0        0        0     1695 2024-04-28 15:22:17.982091 gym_aloha-0.1.1/gym_aloha/assets/scene.xml
+-rw-r--r--   0        0        0      684 2024-04-28 15:22:17.982321 gym_aloha-0.1.1/gym_aloha/assets/tabletop.stl
+-rw-r--r--   0        0        0    83384 2024-04-28 15:22:17.982621 gym_aloha-0.1.1/gym_aloha/assets/vx300s_10_custom_finger_left.stl
+-rw-r--r--   0        0        0    83384 2024-04-28 15:22:17.983504 gym_aloha-0.1.1/gym_aloha/assets/vx300s_10_custom_finger_right.stl
+-rw-r--r--   0        0        0    42884 2024-04-28 15:22:17.983741 gym_aloha-0.1.1/gym_aloha/assets/vx300s_10_gripper_finger.stl
+-rw-r--r--   0        0        0     3884 2024-04-28 15:22:17.983882 gym_aloha-0.1.1/gym_aloha/assets/vx300s_11_ar_tag.stl
+-rw-r--r--   0        0        0    99984 2024-04-28 15:22:17.984229 gym_aloha-0.1.1/gym_aloha/assets/vx300s_1_base.stl
+-rw-r--r--   0        0        0    63884 2024-04-28 15:22:17.984497 gym_aloha-0.1.1/gym_aloha/assets/vx300s_2_shoulder.stl
+-rw-r--r--   0        0        0   102984 2024-04-28 15:22:17.984846 gym_aloha-0.1.1/gym_aloha/assets/vx300s_3_upper_arm.stl
+-rw-r--r--   0        0        0    49584 2024-04-28 15:22:17.985060 gym_aloha-0.1.1/gym_aloha/assets/vx300s_4_upper_forearm.stl
+-rw-r--r--   0        0        0    99884 2024-04-28 15:22:17.985395 gym_aloha-0.1.1/gym_aloha/assets/vx300s_5_lower_forearm.stl
+-rw-r--r--   0        0        0    70784 2024-04-28 15:22:17.985679 gym_aloha-0.1.1/gym_aloha/assets/vx300s_6_wrist.stl
+-rw-r--r--   0        0        0   450084 2024-04-28 15:22:17.986792 gym_aloha-0.1.1/gym_aloha/assets/vx300s_7_gripper.stl
+-rw-r--r--   0        0        0    31684 2024-04-28 15:22:17.987463 gym_aloha-0.1.1/gym_aloha/assets/vx300s_8_gripper_prop.stl
+-rw-r--r--   0        0        0   379484 2024-04-28 15:22:17.988332 gym_aloha-0.1.1/gym_aloha/assets/vx300s_9_gripper_bar.stl
+-rw-r--r--   0        0        0     1272 2024-04-28 15:22:17.988465 gym_aloha-0.1.1/gym_aloha/assets/vx300s_dependencies.xml
+-rw-r--r--   0        0        0     6501 2024-04-28 15:22:17.988593 gym_aloha-0.1.1/gym_aloha/assets/vx300s_left.xml
+-rw-r--r--   0        0        0     6556 2024-04-28 15:22:17.988695 gym_aloha-0.1.1/gym_aloha/assets/vx300s_right.xml
+-rw-r--r--   0        0        0     4575 2024-04-28 15:22:17.988806 gym_aloha-0.1.1/gym_aloha/constants.py
+-rw-r--r--   0        0        0     6752 2024-05-03 09:25:11.876864 gym_aloha-0.1.1/gym_aloha/env.py
+-rw-r--r--   0        0        0     9726 2024-04-28 15:22:17.989157 gym_aloha-0.1.1/gym_aloha/tasks/sim.py
+-rw-r--r--   0        0        0    11602 2024-04-28 15:22:17.989313 gym_aloha-0.1.1/gym_aloha/tasks/sim_end_effector.py
+-rw-r--r--   0        0        0     1098 2024-04-28 15:22:17.989409 gym_aloha-0.1.1/gym_aloha/utils.py
+-rw-r--r--   0        0        0     1822 2024-05-07 08:52:41.597725 gym_aloha-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5159 1970-01-01 00:00:00.000000 gym_aloha-0.1.1/PKG-INFO
```

### Comparing `gym_aloha-0.1.0/LICENSE` & `gym_aloha-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/README.md` & `gym_aloha-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/__init__.py` & `gym_aloha-0.1.1/gym_aloha/__init__.py`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/assets/bimanual_viperx_end_effector_insertion.xml` & `gym_aloha-0.1.1/gym_aloha/assets/bimanual_viperx_end_effector_insertion.xml`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/assets/bimanual_viperx_end_effector_transfer_cube.xml` & `gym_aloha-0.1.1/gym_aloha/assets/bimanual_viperx_end_effector_transfer_cube.xml`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/assets/bimanual_viperx_insertion.xml` & `gym_aloha-0.1.1/gym_aloha/assets/bimanual_viperx_insertion.xml`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/assets/bimanual_viperx_transfer_cube.xml` & `gym_aloha-0.1.1/gym_aloha/assets/bimanual_viperx_transfer_cube.xml`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/assets/scene.xml` & `gym_aloha-0.1.1/gym_aloha/assets/scene.xml`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/assets/tabletop.stl` & `gym_aloha-0.1.1/gym_aloha/assets/tabletop.stl`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/assets/vx300s_10_custom_finger_left.stl` & `gym_aloha-0.1.1/gym_aloha/assets/vx300s_10_custom_finger_left.stl`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/assets/vx300s_10_custom_finger_right.stl` & `gym_aloha-0.1.1/gym_aloha/assets/vx300s_10_custom_finger_right.stl`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/assets/vx300s_10_gripper_finger.stl` & `gym_aloha-0.1.1/gym_aloha/assets/vx300s_10_gripper_finger.stl`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/assets/vx300s_11_ar_tag.stl` & `gym_aloha-0.1.1/gym_aloha/assets/vx300s_11_ar_tag.stl`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/assets/vx300s_1_base.stl` & `gym_aloha-0.1.1/gym_aloha/assets/vx300s_1_base.stl`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/assets/vx300s_2_shoulder.stl` & `gym_aloha-0.1.1/gym_aloha/assets/vx300s_2_shoulder.stl`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/assets/vx300s_3_upper_arm.stl` & `gym_aloha-0.1.1/gym_aloha/assets/vx300s_3_upper_arm.stl`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/assets/vx300s_4_upper_forearm.stl` & `gym_aloha-0.1.1/gym_aloha/assets/vx300s_4_upper_forearm.stl`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/assets/vx300s_5_lower_forearm.stl` & `gym_aloha-0.1.1/gym_aloha/assets/vx300s_5_lower_forearm.stl`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/assets/vx300s_6_wrist.stl` & `gym_aloha-0.1.1/gym_aloha/assets/vx300s_6_wrist.stl`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/assets/vx300s_7_gripper.stl` & `gym_aloha-0.1.1/gym_aloha/assets/vx300s_7_gripper.stl`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/assets/vx300s_8_gripper_prop.stl` & `gym_aloha-0.1.1/gym_aloha/assets/vx300s_8_gripper_prop.stl`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/assets/vx300s_9_gripper_bar.stl` & `gym_aloha-0.1.1/gym_aloha/assets/vx300s_9_gripper_bar.stl`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/assets/vx300s_dependencies.xml` & `gym_aloha-0.1.1/gym_aloha/assets/vx300s_dependencies.xml`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/assets/vx300s_left.xml` & `gym_aloha-0.1.1/gym_aloha/assets/vx300s_left.xml`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/assets/vx300s_right.xml` & `gym_aloha-0.1.1/gym_aloha/assets/vx300s_right.xml`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/constants.py` & `gym_aloha-0.1.1/gym_aloha/constants.py`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/env.py` & `gym_aloha-0.1.1/gym_aloha/env.py`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/tasks/sim.py` & `gym_aloha-0.1.1/gym_aloha/tasks/sim.py`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/tasks/sim_end_effector.py` & `gym_aloha-0.1.1/gym_aloha/tasks/sim_end_effector.py`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/gym_aloha/utils.py` & `gym_aloha-0.1.1/gym_aloha/utils.py`

 * *Files identical despite different names*

### Comparing `gym_aloha-0.1.0/pyproject.toml` & `gym_aloha-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gym-aloha"
-version = "0.1.0"
+version = "0.1.1"
 description = "A gym environment for ALOHA"
 authors = [
     "Rémi Cadène <re.cadene@gmail.com>",
     "Quentin Gallouédec <quentin.gallouedec@ec-lyon.fr>",
     "Alexander Soare <alexander.soare159@gmail.com>",
     "Simon Alibert <alibert.sim@gmail.com>",
 ]
@@ -20,21 +20,21 @@
 ]
 packages = [{include = "gym_aloha"}]
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 mujoco = "^2.3.7"
-gymnasium = "^0.29.1"
-dm-control = "1.0.14"
-imageio = {extras = ["ffmpeg"], version = "^2.34.0"}
-pre-commit = {version = "^3.7.0", optional = true}
-debugpy = {version = "^1.8.1", optional = true}
-pytest = {version = "^8.1.0", optional = true}
-pytest-cov = {version = "^5.0.0", optional = true}
+gymnasium = ">=0.29.1"
+dm-control = ">=1.0.14"
+imageio = {extras = ["ffmpeg"], version = ">=2.34.0"}
+pre-commit = {version = ">=3.7.0", optional = true}
+debugpy = {version = ">=1.8.1", optional = true}
+pytest = {version = ">=8.1.0", optional = true}
+pytest-cov = {version = ">=5.0.0", optional = true}
 
 
 [tool.poetry.extras]
 dev = ["pre-commit", "debugpy"]
 test = ["pytest", "pytest-cov"]
```

### Comparing `gym_aloha-0.1.0/PKG-INFO` & `gym_aloha-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-aloha
-Version: 0.1.0
+Version: 0.1.1
 Summary: A gym environment for ALOHA
 License: Apache-2.0
 Keywords: robotics,deep,reinforcement,learning,aloha,environment,gym,gymnasium,dm-control,mujoco
 Author: Rémi Cadène
 Author-email: re.cadene@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -13,22 +13,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Build Tools
 Provides-Extra: dev
 Provides-Extra: test
-Requires-Dist: debugpy (>=1.8.1,<2.0.0) ; extra == "dev"
-Requires-Dist: dm-control (==1.0.14)
-Requires-Dist: gymnasium (>=0.29.1,<0.30.0)
-Requires-Dist: imageio[ffmpeg] (>=2.34.0,<3.0.0)
+Requires-Dist: debugpy (>=1.8.1) ; extra == "dev"
+Requires-Dist: dm-control (>=1.0.14)
+Requires-Dist: gymnasium (>=0.29.1)
+Requires-Dist: imageio[ffmpeg] (>=2.34.0)
 Requires-Dist: mujoco (>=2.3.7,<3.0.0)
-Requires-Dist: pre-commit (>=3.7.0,<4.0.0) ; extra == "dev"
-Requires-Dist: pytest (>=8.1.0,<9.0.0) ; extra == "test"
-Requires-Dist: pytest-cov (>=5.0.0,<6.0.0) ; extra == "test"
+Requires-Dist: pre-commit (>=3.7.0) ; extra == "dev"
+Requires-Dist: pytest (>=8.1.0) ; extra == "test"
+Requires-Dist: pytest-cov (>=5.0.0) ; extra == "test"
 Description-Content-Type: text/markdown
 
 # gym-aloha
 
 A gym environment for ALOHA
 
 <img src="http://remicadene.com/assets/gif/aloha_act.gif" width="50%" alt="ACT policy on ALOHA env"/>
```

