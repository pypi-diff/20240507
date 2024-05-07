# Comparing `tmp/mujoco-mjx-3.1.4.tar.gz` & `tmp/mujoco_mjx-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mujoco-mjx-3.1.4.tar", last modified: Wed Apr 10 17:18:45 2024, max compression
+gzip compressed data, was "mujoco_mjx-3.1.5.tar", last modified: Tue May  7 19:01:29 2024, max compression
```

## Comparing `mujoco-mjx-3.1.4.tar` & `mujoco_mjx-3.1.5.tar`

### file list

```diff
@@ -1,121 +1,119 @@
-drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.080092 mujoco-mjx-3.1.4/
--rw-r--r--   0 root         (0)     1002    11358 2024-04-10 17:18:38.000000 mujoco-mjx-3.1.4/LICENSE
--rw-rw-r--   0 root         (0)     1002       41 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/MANIFEST.in
--rw-r--r--   0 root         (0)     1002     3382 2024-04-10 17:18:45.080092 mujoco-mjx-3.1.4/PKG-INFO
--rw-rw-r--   0 root         (0)     1002     2063 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/README.md
-drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.032087 mujoco-mjx-3.1.4/mujoco/
-drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.036088 mujoco-mjx-3.1.4/mujoco/mjx/
--rw-rw-r--   0 root         (0)     1002     2372 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/__init__.py
-drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.044088 mujoco-mjx-3.1.4/mujoco/mjx/_src/
--rw-rw-r--   0 root         (0)     1002      674 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/__init__.py
--rw-rw-r--   0 root         (0)     1002     1787 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/collision_base.py
--rw-rw-r--   0 root         (0)     1002    32800 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/collision_convex.py
--rw-rw-r--   0 root         (0)     1002    14855 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/collision_driver.py
--rw-rw-r--   0 root         (0)     1002    26782 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/collision_driver_test.py
--rw-rw-r--   0 root         (0)     1002     4957 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/collision_primitive.py
--rw-rw-r--   0 root         (0)     1002     4744 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/collision_sdf.py
--rw-rw-r--   0 root         (0)     1002    12899 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/constraint.py
--rw-rw-r--   0 root         (0)     1002     3831 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/constraint_test.py
--rw-rw-r--   0 root         (0)     1002     4792 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/dataclasses.py
--rw-rw-r--   0 root         (0)     1002    10540 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/device.py
--rw-rw-r--   0 root         (0)     1002     6540 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/device_test.py
--rw-rw-r--   0 root         (0)     1002    10865 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/forward.py
--rw-rw-r--   0 root         (0)     1002     6422 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/forward_test.py
--rw-rw-r--   0 root         (0)     1002    14803 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/io.py
--rw-rw-r--   0 root         (0)     1002    17818 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/io_test.py
--rw-rw-r--   0 root         (0)     1002    10768 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/math.py
--rw-rw-r--   0 root         (0)     1002     7514 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/math_test.py
--rw-rw-r--   0 root         (0)     1002    11153 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/mesh.py
--rw-rw-r--   0 root         (0)     1002     5700 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/mesh_test.py
--rw-rw-r--   0 root         (0)     1002     4472 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/passive.py
--rw-rw-r--   0 root         (0)     1002     2566 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/passive_test.py
--rw-rw-r--   0 root         (0)     1002     8487 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/ray.py
--rw-rw-r--   0 root         (0)     1002     9529 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/ray_test.py
--rw-rw-r--   0 root         (0)     1002    16662 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/scan.py
--rw-rw-r--   0 root         (0)     1002     9042 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/scan_test.py
--rw-rw-r--   0 root         (0)     1002    17959 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/smooth.py
--rw-rw-r--   0 root         (0)     1002     5546 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/smooth_test.py
--rw-rw-r--   0 root         (0)     1002    12100 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/solver.py
--rw-rw-r--   0 root         (0)     1002     4426 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/solver_test.py
--rw-rw-r--   0 root         (0)     1002     5910 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/support.py
--rw-rw-r--   0 root         (0)     1002     4658 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/support_test.py
--rw-rw-r--   0 root         (0)     1002    13854 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/test_util.py
--rw-rw-r--   0 root         (0)     1002    29238 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/_src/types.py
-drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.044088 mujoco-mjx-3.1.4/mujoco/mjx/integration_test/
--rw-rw-r--   0 root         (0)     1002     3045 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/integration_test/collision_driver_test.py
--rw-rw-r--   0 root         (0)     1002     2222 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/integration_test/forward_test.py
--rw-rw-r--   0 root         (0)     1002     2539 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/integration_test/smooth_test.py
-drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.044088 mujoco-mjx-3.1.4/mujoco/mjx/test_data/
-drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.044088 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/
--rw-rw-r--   0 root         (0)     1002     1792 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/README.md
-drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.060090 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/
--rw-rw-r--   0 root         (0)     1002   429334 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/abduction.stl
--rw-rw-r--   0 root         (0)     1002    14998 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/barkour_v0_mjx.xml
--rw-rw-r--   0 root         (0)     1002  1169584 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/body.stl
--rw-rw-r--   0 root         (0)     1002    23384 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/foot.stl
--rw-rw-r--   0 root         (0)     1002   739084 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/handle.stl
--rw-rw-r--   0 root         (0)     1002   267584 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/head.stl
--rw-rw-r--   0 root         (0)     1002   163984 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/head_mount.stl
--rw-rw-r--   0 root         (0)     1002   523084 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/lower_leg_1to1.stl
--rw-rw-r--   0 root         (0)     1002  1199984 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/powercable.stl
--rw-rw-r--   0 root         (0)     1002   530834 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/upper_left_1.stl
--rw-rw-r--   0 root         (0)     1002   628484 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/upper_left_2.stl
--rw-rw-r--   0 root         (0)     1002  1500284 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/upper_left_3.stl
--rw-rw-r--   0 root         (0)     1002  1106034 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/upper_right_1.stl
--rw-rw-r--   0 root         (0)     1002   670284 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/upper_right_2.stl
--rw-rw-r--   0 root         (0)     1002  1521284 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/upper_right_3.stl
--rw-rw-r--   0 root         (0)     1002     1677 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/constraints.xml
--rw-rw-r--   0 root         (0)     1002     2366 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/convex.xml
-drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.064090 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/
--rw-rw-r--   0 root         (0)     1002     7750 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/01_humanoids.xml
--rw-rw-r--   0 root         (0)     1002    13884 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/02_humanoids.xml
--rw-rw-r--   0 root         (0)     1002    19973 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/03_humanoids.xml
--rw-rw-r--   0 root         (0)     1002    26060 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/04_humanoids.xml
--rw-rw-r--   0 root         (0)     1002    32147 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/05_humanoids.xml
--rw-rw-r--   0 root         (0)     1002    38237 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/06_humanoids.xml
--rw-rw-r--   0 root         (0)     1002    44328 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/07_humanoids.xml
--rw-rw-r--   0 root         (0)     1002    50416 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/08_humanoids.xml
--rw-rw-r--   0 root         (0)     1002    56509 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/09_humanoids.xml
--rw-rw-r--   0 root         (0)     1002    62687 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/10_humanoids.xml
--rw-rw-r--   0 root         (0)     1002      909 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/README.md
--rw-rw-r--   0 root         (0)     1002   397686 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/humanoid.png
--rw-rw-r--   0 root         (0)     1002    11271 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/humanoid.xml
-drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.064090 mujoco-mjx-3.1.4/mujoco/mjx/test_data/meshes/
--rw-rw-r--   0 root         (0)     1002     1884 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/meshes/dodecahedron.stl
--rw-rw-r--   0 root         (0)     1002      384 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/meshes/pyramid.stl
--rw-rw-r--   0 root         (0)     1002      284 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/meshes/tetrahedron.stl
--rw-rw-r--   0 root         (0)     1002     3776 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/pendula.xml
--rw-rw-r--   0 root         (0)     1002     1231 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/ray.xml
-drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.068091 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/
--rw-rw-r--   0 root         (0)     1002      961 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/README.md
-drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.076091 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/
--rw-rw-r--   0 root         (0)     1002   341254 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/f_distal_pst.obj
--rw-rw-r--   0 root         (0)     1002     6447 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/f_distal_pst_214.obj
--rw-rw-r--   0 root         (0)     1002    34351 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/f_knuckle.obj
--rw-rw-r--   0 root         (0)     1002    25738 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/f_middle.obj
--rw-rw-r--   0 root         (0)     1002    64846 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/f_proximal.obj
--rw-rw-r--   0 root         (0)     1002    80439 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/forearm_0.obj
--rw-rw-r--   0 root         (0)     1002  1433615 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/forearm_1.obj
--rw-rw-r--   0 root         (0)     1002    26812 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/forearm_collision.obj
--rw-rw-r--   0 root         (0)     1002    88696 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/lf_metacarpal.obj
--rw-rw-r--   0 root         (0)     1002   118690 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/mounting_plate.obj
--rw-rw-r--   0 root         (0)     1002   775747 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/palm.obj
--rw-rw-r--   0 root         (0)     1002   300842 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/th_distal_pst.obj
--rw-rw-r--   0 root         (0)     1002     5639 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/th_distal_pst_190.obj
--rw-rw-r--   0 root         (0)     1002    75080 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/th_middle.obj
--rw-rw-r--   0 root         (0)     1002    23772 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/th_proximal.obj
--rw-rw-r--   0 root         (0)     1002   110838 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/wrist.obj
--rw-rw-r--   0 root         (0)     1002    18568 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/right_hand.xml
--rw-rw-r--   0 root         (0)     1002     1112 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/scene_right.xml
--rw-rw-r--   0 root         (0)     1002  1315458 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/shadow_hand.png
--rw-rw-r--   0 root         (0)     1002     2747 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/testspeed.py
--rw-rw-r--   0 root         (0)     1002     2462 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/mujoco/mjx/viewer.py
-drwxr-sr-x   0 root         (0)     1002        0 2024-04-10 17:18:45.080092 mujoco-mjx-3.1.4/mujoco_mjx.egg-info/
--rw-r--r--   0 root         (0)     1002     3382 2024-04-10 17:18:45.000000 mujoco-mjx-3.1.4/mujoco_mjx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1002     4255 2024-04-10 17:18:45.000000 mujoco-mjx-3.1.4/mujoco_mjx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1002        1 2024-04-10 17:18:45.000000 mujoco-mjx-3.1.4/mujoco_mjx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1002       96 2024-04-10 17:18:45.000000 mujoco-mjx-3.1.4/mujoco_mjx.egg-info/entry_points.txt
--rw-r--r--   0 root         (0)     1002       65 2024-04-10 17:18:45.000000 mujoco-mjx-3.1.4/mujoco_mjx.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1002        7 2024-04-10 17:18:45.000000 mujoco-mjx-3.1.4/mujoco_mjx.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1002     1437 2024-04-10 17:11:23.000000 mujoco-mjx-3.1.4/pyproject.toml
--rw-r--r--   0 root         (0)     1002       38 2024-04-10 17:18:45.080092 mujoco-mjx-3.1.4/setup.cfg
+drwxr-sr-x   0 root         (0)     1002        0 2024-05-07 19:01:29.038615 mujoco_mjx-3.1.5/
+-rw-r--r--   0 root         (0)     1002    11358 2024-05-07 19:01:20.000000 mujoco_mjx-3.1.5/LICENSE
+-rw-rw-r--   0 root         (0)     1002       41 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0)     1002     3382 2024-05-07 19:01:29.038615 mujoco_mjx-3.1.5/PKG-INFO
+-rw-rw-r--   0 root         (0)     1002     2063 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/README.md
+drwxr-sr-x   0 root         (0)     1002        0 2024-05-07 19:01:28.994612 mujoco_mjx-3.1.5/mujoco/
+drwxr-sr-x   0 root         (0)     1002        0 2024-05-07 19:01:28.994612 mujoco_mjx-3.1.5/mujoco/mjx/
+-rw-rw-r--   0 root         (0)     1002     2200 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/__init__.py
+drwxr-sr-x   0 root         (0)     1002        0 2024-05-07 19:01:29.002612 mujoco_mjx-3.1.5/mujoco/mjx/_src/
+-rw-rw-r--   0 root         (0)     1002      674 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/__init__.py
+-rw-rw-r--   0 root         (0)     1002    34043 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/collision_convex.py
+-rw-rw-r--   0 root         (0)     1002    14965 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/collision_driver.py
+-rw-rw-r--   0 root         (0)     1002    29493 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/collision_driver_test.py
+-rw-rw-r--   0 root         (0)     1002     6988 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/collision_primitive.py
+-rw-rw-r--   0 root         (0)     1002     8068 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/collision_sdf.py
+-rw-rw-r--   0 root         (0)     1002     2217 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/collision_types.py
+-rw-rw-r--   0 root         (0)     1002    14871 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/constraint.py
+-rw-rw-r--   0 root         (0)     1002     4832 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/constraint_test.py
+-rw-rw-r--   0 root         (0)     1002     4823 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/dataclasses.py
+-rw-rw-r--   0 root         (0)     1002    10935 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/forward.py
+-rw-rw-r--   0 root         (0)     1002     6422 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/forward_test.py
+-rw-rw-r--   0 root         (0)     1002    15289 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/io.py
+-rw-rw-r--   0 root         (0)     1002    17242 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/io_test.py
+-rw-rw-r--   0 root         (0)     1002    10768 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/math.py
+-rw-rw-r--   0 root         (0)     1002     7514 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/math_test.py
+-rw-rw-r--   0 root         (0)     1002     9549 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/mesh.py
+-rw-rw-r--   0 root         (0)     1002     5548 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/mesh_test.py
+-rw-rw-r--   0 root         (0)     1002     5238 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/passive.py
+-rw-rw-r--   0 root         (0)     1002     2758 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/passive_test.py
+-rw-rw-r--   0 root         (0)     1002     8191 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/ray.py
+-rw-rw-r--   0 root         (0)     1002     9694 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/ray_test.py
+-rw-rw-r--   0 root         (0)     1002    16752 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/scan.py
+-rw-rw-r--   0 root         (0)     1002     9038 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/scan_test.py
+-rw-rw-r--   0 root         (0)     1002    17959 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/smooth.py
+-rw-rw-r--   0 root         (0)     1002     5546 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/smooth_test.py
+-rw-rw-r--   0 root         (0)     1002    11937 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/solver.py
+-rw-rw-r--   0 root         (0)     1002     4426 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/solver_test.py
+-rw-rw-r--   0 root         (0)     1002     7991 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/support.py
+-rw-rw-r--   0 root         (0)     1002     5518 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/support_test.py
+-rw-rw-r--   0 root         (0)     1002    14096 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/test_util.py
+-rw-rw-r--   0 root         (0)     1002    31719 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/_src/types.py
+drwxr-sr-x   0 root         (0)     1002        0 2024-05-07 19:01:29.002612 mujoco_mjx-3.1.5/mujoco/mjx/integration_test/
+-rw-rw-r--   0 root         (0)     1002     3251 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/integration_test/collision_driver_test.py
+-rw-rw-r--   0 root         (0)     1002     2222 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/integration_test/forward_test.py
+-rw-rw-r--   0 root         (0)     1002     2515 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/integration_test/smooth_test.py
+drwxr-sr-x   0 root         (0)     1002        0 2024-05-07 19:01:29.002612 mujoco_mjx-3.1.5/mujoco/mjx/test_data/
+drwxr-sr-x   0 root         (0)     1002        0 2024-05-07 19:01:29.002612 mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/
+-rw-rw-r--   0 root         (0)     1002     1792 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/README.md
+drwxr-sr-x   0 root         (0)     1002        0 2024-05-07 19:01:29.018614 mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/
+-rw-rw-r--   0 root         (0)     1002   429334 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/abduction.stl
+-rw-rw-r--   0 root         (0)     1002    14998 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/barkour_v0_mjx.xml
+-rw-rw-r--   0 root         (0)     1002  1169584 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/body.stl
+-rw-rw-r--   0 root         (0)     1002    23384 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/foot.stl
+-rw-rw-r--   0 root         (0)     1002   739084 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/handle.stl
+-rw-rw-r--   0 root         (0)     1002   267584 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/head.stl
+-rw-rw-r--   0 root         (0)     1002   163984 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/head_mount.stl
+-rw-rw-r--   0 root         (0)     1002   523084 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/lower_leg_1to1.stl
+-rw-rw-r--   0 root         (0)     1002  1199984 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/powercable.stl
+-rw-rw-r--   0 root         (0)     1002   530834 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/upper_left_1.stl
+-rw-rw-r--   0 root         (0)     1002   628484 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/upper_left_2.stl
+-rw-rw-r--   0 root         (0)     1002  1500284 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/upper_left_3.stl
+-rw-rw-r--   0 root         (0)     1002  1106034 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/upper_right_1.stl
+-rw-rw-r--   0 root         (0)     1002   670284 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/upper_right_2.stl
+-rw-rw-r--   0 root         (0)     1002  1521284 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/upper_right_3.stl
+-rw-rw-r--   0 root         (0)     1002     2132 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/constraints.xml
+-rw-rw-r--   0 root         (0)     1002     2366 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/convex.xml
+drwxr-sr-x   0 root         (0)     1002        0 2024-05-07 19:01:29.022614 mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/
+-rw-rw-r--   0 root         (0)     1002     7750 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/01_humanoids.xml
+-rw-rw-r--   0 root         (0)     1002    13884 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/02_humanoids.xml
+-rw-rw-r--   0 root         (0)     1002    19973 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/03_humanoids.xml
+-rw-rw-r--   0 root         (0)     1002    26060 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/04_humanoids.xml
+-rw-rw-r--   0 root         (0)     1002    32147 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/05_humanoids.xml
+-rw-rw-r--   0 root         (0)     1002    38237 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/06_humanoids.xml
+-rw-rw-r--   0 root         (0)     1002    44328 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/07_humanoids.xml
+-rw-rw-r--   0 root         (0)     1002    50416 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/08_humanoids.xml
+-rw-rw-r--   0 root         (0)     1002    56509 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/09_humanoids.xml
+-rw-rw-r--   0 root         (0)     1002    62687 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/10_humanoids.xml
+-rw-rw-r--   0 root         (0)     1002      909 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/README.md
+-rw-rw-r--   0 root         (0)     1002   397686 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/humanoid.png
+-rw-rw-r--   0 root         (0)     1002    11271 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/humanoid.xml
+drwxr-sr-x   0 root         (0)     1002        0 2024-05-07 19:01:29.026614 mujoco_mjx-3.1.5/mujoco/mjx/test_data/meshes/
+-rw-rw-r--   0 root         (0)     1002     1884 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/meshes/dodecahedron.stl
+-rw-rw-r--   0 root         (0)     1002      384 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/meshes/pyramid.stl
+-rw-rw-r--   0 root         (0)     1002      284 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/meshes/tetrahedron.stl
+-rw-rw-r--   0 root         (0)     1002     4475 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/pendula.xml
+-rw-rw-r--   0 root         (0)     1002     1231 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/ray.xml
+drwxr-sr-x   0 root         (0)     1002        0 2024-05-07 19:01:29.026614 mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/
+-rw-rw-r--   0 root         (0)     1002      961 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/README.md
+drwxr-sr-x   0 root         (0)     1002        0 2024-05-07 19:01:29.034615 mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/
+-rw-rw-r--   0 root         (0)     1002   341254 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/f_distal_pst.obj
+-rw-rw-r--   0 root         (0)     1002     6447 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/f_distal_pst_214.obj
+-rw-rw-r--   0 root         (0)     1002    34351 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/f_knuckle.obj
+-rw-rw-r--   0 root         (0)     1002    25738 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/f_middle.obj
+-rw-rw-r--   0 root         (0)     1002    64846 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/f_proximal.obj
+-rw-rw-r--   0 root         (0)     1002    80439 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/forearm_0.obj
+-rw-rw-r--   0 root         (0)     1002  1433615 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/forearm_1.obj
+-rw-rw-r--   0 root         (0)     1002    26812 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/forearm_collision.obj
+-rw-rw-r--   0 root         (0)     1002    88696 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/lf_metacarpal.obj
+-rw-rw-r--   0 root         (0)     1002   118690 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/mounting_plate.obj
+-rw-rw-r--   0 root         (0)     1002   775747 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/palm.obj
+-rw-rw-r--   0 root         (0)     1002   300842 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/th_distal_pst.obj
+-rw-rw-r--   0 root         (0)     1002     5639 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/th_distal_pst_190.obj
+-rw-rw-r--   0 root         (0)     1002    75080 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/th_middle.obj
+-rw-rw-r--   0 root         (0)     1002    23772 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/th_proximal.obj
+-rw-rw-r--   0 root         (0)     1002   110838 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/wrist.obj
+-rw-rw-r--   0 root         (0)     1002    18568 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/right_hand.xml
+-rw-rw-r--   0 root         (0)     1002     1112 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/scene_right.xml
+-rw-rw-r--   0 root         (0)     1002  1315458 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/shadow_hand.png
+-rw-rw-r--   0 root         (0)     1002     2763 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/testspeed.py
+-rw-rw-r--   0 root         (0)     1002     2473 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/mujoco/mjx/viewer.py
+drwxr-sr-x   0 root         (0)     1002        0 2024-05-07 19:01:29.034615 mujoco_mjx-3.1.5/mujoco_mjx.egg-info/
+-rw-r--r--   0 root         (0)     1002     3382 2024-05-07 19:01:28.000000 mujoco_mjx-3.1.5/mujoco_mjx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1002     4199 2024-05-07 19:01:28.000000 mujoco_mjx-3.1.5/mujoco_mjx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1002        1 2024-05-07 19:01:28.000000 mujoco_mjx-3.1.5/mujoco_mjx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1002       96 2024-05-07 19:01:28.000000 mujoco_mjx-3.1.5/mujoco_mjx.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0)     1002       65 2024-05-07 19:01:28.000000 mujoco_mjx-3.1.5/mujoco_mjx.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1002        7 2024-05-07 19:01:28.000000 mujoco_mjx-3.1.5/mujoco_mjx.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1002     1437 2024-05-07 18:51:20.000000 mujoco_mjx-3.1.5/pyproject.toml
+-rw-r--r--   0 root         (0)     1002       38 2024-05-07 19:01:29.038615 mujoco_mjx-3.1.5/setup.cfg
```

### Comparing `mujoco-mjx-3.1.4/LICENSE` & `mujoco_mjx-3.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/PKG-INFO` & `mujoco_mjx-3.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mujoco-mjx
-Version: 3.1.4
+Version: 3.1.5
 Summary: MuJoCo XLA (MJX)
 Author-email: Google DeepMind <mujoco@deepmind.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/google-deepmind/mujoco/tree/main/mjx
-Project-URL: Documentation, https://mujoco.readthedocs.io/en/3.1.4
+Project-URL: Documentation, https://mujoco.readthedocs.io/en/3.1.5
 Project-URL: Repository, https://github.com/google-deepmind/mujoco/tree/main/mjx
-Project-URL: Changelog, https://mujoco.readthedocs.io/en/3.1.4/changelog.html
+Project-URL: Changelog, https://mujoco.readthedocs.io/en/3.1.5/changelog.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -23,15 +23,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: absl-py
 Requires-Dist: etils[epath]
 Requires-Dist: jax
 Requires-Dist: jaxlib
-Requires-Dist: mujoco>=3.1.4.dev0
+Requires-Dist: mujoco>=3.1.5.dev0
 Requires-Dist: scipy
 Requires-Dist: trimesh
 
 # MuJoCo XLA (MJX)
 
 [![PyPI Python Version][pypi-versions-badge]][pypi]
 [![PyPI version][pypi-badge]][pypi]
```

### Comparing `mujoco-mjx-3.1.4/README.md` & `mujoco_mjx-3.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/__init__.py` & `mujoco_mjx-3.1.5/mujoco/mjx/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,20 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Public API for MJX."""
 
 # pylint:disable=g-importing-member
 from mujoco.mjx._src.collision_driver import collision
-from mujoco.mjx._src.collision_driver import get_params
-from mujoco.mjx._src.collision_driver import ncon
-from mujoco.mjx._src.constraint import count_constraints
 from mujoco.mjx._src.constraint import make_constraint
-from mujoco.mjx._src.device import device_get_into
-from mujoco.mjx._src.device import device_put
 from mujoco.mjx._src.forward import euler
 from mujoco.mjx._src.forward import forward
 from mujoco.mjx._src.forward import fwd_acceleration
 from mujoco.mjx._src.forward import fwd_actuation
 from mujoco.mjx._src.forward import fwd_position
 from mujoco.mjx._src.forward import fwd_velocity
 from mujoco.mjx._src.forward import rungekutta4
@@ -43,11 +38,13 @@
 from mujoco.mjx._src.smooth import crb
 from mujoco.mjx._src.smooth import factor_m
 from mujoco.mjx._src.smooth import kinematics
 from mujoco.mjx._src.smooth import rne
 from mujoco.mjx._src.smooth import transmission
 from mujoco.mjx._src.solver import solve
 from mujoco.mjx._src.support import full_m
+from mujoco.mjx._src.support import id2name
 from mujoco.mjx._src.support import is_sparse
 from mujoco.mjx._src.support import mul_m
+from mujoco.mjx._src.support import name2id
 from mujoco.mjx._src.test_util import benchmark
 from mujoco.mjx._src.types import *
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/__init__.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/collision_convex.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/collision_convex.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,20 +16,61 @@
 
 import functools
 from typing import Tuple
 
 import jax
 from jax import numpy as jp
 from mujoco.mjx._src import math
+from mujoco.mjx._src import mesh
 # pylint: disable=g-importing-member
-from mujoco.mjx._src.collision_base import Contact
-from mujoco.mjx._src.collision_base import GeomInfo
+from mujoco.mjx._src.collision_types import Collision
+from mujoco.mjx._src.collision_types import ConvexInfo
+from mujoco.mjx._src.collision_types import FunctionKey
+from mujoco.mjx._src.collision_types import GeomInfo
+from mujoco.mjx._src.types import Data
+from mujoco.mjx._src.types import GeomType
+from mujoco.mjx._src.types import Model
 # pylint: enable=g-importing-member
 
 
+def collider(ncon: int):
+  """Wraps collision functions for use by collision_driver."""
+
+  def wrapper(func):
+    def collide(
+        m: Model, d: Data, key: FunctionKey, geom: jax.Array
+    ) -> Collision:
+      g1, g2 = geom.T
+      infos = [
+          GeomInfo(d.geom_xpos[g1], d.geom_xmat[g1], m.geom_size[g1]),
+          GeomInfo(d.geom_xpos[g2], d.geom_xmat[g2], m.geom_size[g2]),
+      ]
+      in_axes = [0, 0]
+      for i in [0, 1]:
+        if key.types[i] == GeomType.BOX:
+          infos[i] = mesh.box(infos[i])
+          in_axes[i] = jax.tree_util.tree_map(lambda x: None, infos[i]).replace(
+              pos=0, mat=0, face=0, vert=0
+          )
+        elif key.types[i] == GeomType.MESH:
+          infos[i] = mesh.convex(m, key.data_ids[i], infos[i])
+          in_axes[i] = jax.tree_util.tree_map(lambda x: None, infos[i]).replace(
+              pos=0, mat=0
+          )
+      dist, pos, frame = jax.vmap(func, in_axes=in_axes)(*infos)
+      if ncon > 1:
+        return jax.tree_util.tree_map(jp.concatenate, (dist, pos, frame))
+      return dist, pos, frame
+
+    collide.ncon = ncon
+    return collide
+
+  return wrapper
+
+
 def _closest_segment_point_plane(
     a: jax.Array, b: jax.Array, p0: jax.Array, plane_normal: jax.Array
 ) -> jax.Array:
   """Gets the closest point between a line segment and a plane.
 
   Args:
     a: first line segment point
@@ -174,40 +215,42 @@
   bp = b - poly
   dist_bp = jp.abs(bp.dot(bc)) + dist_mask
   dist_ap = jp.abs(ap.dot(ac)) + dist_mask
   d_idx = (dist_bp + dist_ap).argmax() % poly.shape[0]
   return jp.array([a_idx, b_idx, c_idx, d_idx])
 
 
-def plane_convex(plane: GeomInfo, convex: GeomInfo) -> Contact:
+@collider(ncon=4)
+def plane_convex(plane: GeomInfo, convex: ConvexInfo) -> Collision:
   """Calculates contacts between a plane and a convex object."""
   vert = convex.vert
 
   # get points in the convex frame
   plane_pos = convex.mat.T @ (plane.pos - convex.pos)
   n = convex.mat.T @ plane.mat[:, 2]
   support = (plane_pos - vert) @ n
-  idx = _manifold_points(vert, support > 0, n)
+  idx = _manifold_points(vert, support > jp.maximum(0, support.max() - 1e-4), n)
   pos = vert[idx]
 
   # convert to world frame
   pos = convex.pos + pos @ convex.mat.T
   n = plane.mat[:, 2]
 
   frame = jp.stack([math.make_frame(n)] * 4, axis=0)
   unique = jp.tril(idx == idx[:, None]).sum(axis=1) == 1
   dist = jp.where(unique, -support[idx], 1)
   pos = pos - 0.5 * dist[:, None] * n
   return dist, pos, frame
 
 
-def sphere_convex(sphere: GeomInfo, convex: GeomInfo) -> Contact:
+@collider(ncon=1)
+def sphere_convex(sphere: GeomInfo, convex: ConvexInfo) -> Collision:
   """Calculates contact between a sphere and a convex object."""
   faces = convex.face
-  normals = convex.facenorm
+  normals = convex.face_normal
 
   # Put sphere in convex frame.
   sphere_pos = convex.mat.T @ (sphere.pos - convex.pos)
 
   # Get support from face normals.
   @jax.vmap
   def get_support(faces, normal):
@@ -258,24 +301,23 @@
   dist = jp.where(has_separating_axis, 1.0, d - sphere.size[0])
   pos = (pt + spt) * 0.5
 
   # Go back to world frame.
   n = convex.mat @ n
   pos = convex.mat @ pos + convex.pos
 
-  return jax.tree_map(
-      lambda x: jp.expand_dims(x, axis=0), (dist, pos, math.make_frame(n))
-  )
+  return dist, pos, math.make_frame(n)
 
 
-def capsule_convex(cap: GeomInfo, convex: GeomInfo) -> Contact:
+@collider(ncon=2)
+def capsule_convex(cap: GeomInfo, convex: ConvexInfo) -> Collision:
   """Calculates contacts between a capsule and a convex object."""
   # Get convex transformed normals, faces, and vertices.
   faces = convex.face
-  normals = convex.facenorm
+  normals = convex.face_normal
 
   # Put capsule in convex frame.
   cap_pos = convex.mat.T @ (cap.pos - convex.pos)
   axis, length = cap.mat[:, 2], cap.size[1]
   axis = convex.mat.T @ axis
   seg = axis * length
   cap_pts = jp.array([
@@ -343,15 +385,15 @@
   e_idx = jp.abs(res[0]).argmin()
   (
       edge_dist,
       edge_axis,
       degenerate_edge_dir,
       edge_closest_pt,
       cap_closest_pt,
-  ) = jax.tree_map(lambda x, i=e_idx: jp.take(x, i, axis=0), res)
+  ) = jax.tree_util.tree_map(lambda x, i=e_idx: jp.take(x, i, axis=0), res)
 
   edge_face_normals = edge_face_normal[e_idx]
   edge_voronoi_front = ((edge_face_normals @ edge_axis) < 0).all()
   shallow = ~degenerate_edge_dir & edge_voronoi_front
   edge_penetration = jp.where(shallow, cap.size[0] - edge_dist, -1)
 
   # Determine edge contact position.
@@ -865,18 +907,17 @@
   pos = jp.where(
       is_edge_contact,
       jp.tile(0.5 * (a_closest + b_closest), (4, 1)), pos)
 
   return dist, pos, normal
 
 
-def convex_convex(c1: GeomInfo, c2: GeomInfo) -> Contact:
+@collider(ncon=4)
+def convex_convex(c1: ConvexInfo, c2: ConvexInfo) -> Collision:
   """Calculates contacts between two convex objects."""
-  if c1.face is None or c2.face is None or c1.vert is None or c2.vert is None:
-    raise AssertionError('Mesh info missing.')
   # pad face vertices so that we can broadcast between geom1 and geom2
   # face has shape (n_face, n_vert, 3)
   nvert1, nvert2 = c1.face.shape[1], c2.face.shape[1]
   if nvert1 < nvert2:
     face = jp.pad(c1.face, ((0, 0), (0, nvert2 - nvert1), (0, 0)), 'edge')
     c1 = c1.replace(face=face)
   elif nvert2 < nvert1:
@@ -891,22 +932,22 @@
   faces1 = c1.face
   faces2 = c2.face
 
   to_local_pos = c2.mat.T @ (c1.pos - c2.pos)
   to_local_mat = c2.mat.T @ c1.mat
 
   faces1 = to_local_pos + faces1 @ to_local_mat.T
-  normals1 = c1.facenorm @ to_local_mat.T
-  normals2 = c2.facenorm
+  normals1 = c1.face_normal @ to_local_mat.T
+  normals2 = c2.face_normal
 
   vertices1 = to_local_pos + c1.vert @ to_local_mat.T
   vertices2 = c2.vert
 
-  unique_edges1 = jp.take(vertices1, c1.edge, axis=0)
-  unique_edges2 = jp.take(vertices2, c2.edge, axis=0)
+  unique_edges1 = jp.take(vertices1, c1.edge_dir, axis=0)
+  unique_edges2 = jp.take(vertices2, c2.edge_dir, axis=0)
 
   edges1 = jp.take(vertices1, c1.edge, axis=0)
   edges2 = jp.take(vertices2, c2.edge, axis=0)
 
   edge_face_normals1 = c1.edge_face_normal @ to_local_mat.T
   edge_face_normals2 = c2.edge_face_normal
 
@@ -940,17 +981,10 @@
         edge_face_normals2,
     )
 
   # Go back to world frame.
   pos = c2.pos + pos @ c2.mat.T
   normal = normal @ c2.mat.T
   normal = -normal if swapped else normal
-
   frame = jax.vmap(math.make_frame)(normal)
-  return dist, pos, frame
 
-
-# store ncon as function attributes
-plane_convex.ncon = 4
-sphere_convex.ncon = 1
-capsule_convex.ncon = 2
-convex_convex.ncon = 4
+  return dist, pos, frame
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/collision_driver.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/collision_driver.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,431 +8,391 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Collide geometries."""
+"""Runs collision checking for all geoms in a Model.
 
-from typing import Callable, Dict, List, Optional, Sequence, Tuple, Union
+To do this, collision_driver builds a collision function table, and then runs
+the collision functions serially on the parameters in the table.
+
+For example, if a Model has three geoms:
+
+geom   |   type
+---------------
+1      | sphere
+2      | capsule
+3      | sphere
+
+collision_driver organizes it into these functions and runs them:
+
+function       | geom pair
+--------------------------
+sphere_sphere  | (1, 3)
+sphere_capsule | (1, 2), (2, 3)
+
+
+Besides collision function, function tables are keyed on mesh id and condim,
+in order to guarantee static shapes for contacts and jacobians.
+"""
+
+import itertools
+from typing import Dict, Iterator, List, Tuple, Union
 
 import jax
 from jax import numpy as jp
 import mujoco
-from mujoco.mjx._src import collision_base
-from mujoco.mjx._src import mesh
 from mujoco.mjx._src import support
 # pylint: disable=g-importing-member
-from mujoco.mjx._src.collision_base import Candidate
-from mujoco.mjx._src.collision_base import CandidateSet
-from mujoco.mjx._src.collision_base import GeomInfo
-from mujoco.mjx._src.collision_base import SolverParams
 from mujoco.mjx._src.collision_convex import capsule_convex
 from mujoco.mjx._src.collision_convex import convex_convex
 from mujoco.mjx._src.collision_convex import plane_convex
 from mujoco.mjx._src.collision_convex import sphere_convex
 from mujoco.mjx._src.collision_primitive import capsule_capsule
 from mujoco.mjx._src.collision_primitive import plane_capsule
+from mujoco.mjx._src.collision_primitive import plane_cylinder
 from mujoco.mjx._src.collision_primitive import plane_ellipsoid
 from mujoco.mjx._src.collision_primitive import plane_sphere
 from mujoco.mjx._src.collision_primitive import sphere_capsule
 from mujoco.mjx._src.collision_primitive import sphere_sphere
+from mujoco.mjx._src.collision_sdf import capsule_cylinder
 from mujoco.mjx._src.collision_sdf import capsule_ellipsoid
+from mujoco.mjx._src.collision_sdf import cylinder_cylinder
+from mujoco.mjx._src.collision_sdf import ellipsoid_cylinder
 from mujoco.mjx._src.collision_sdf import ellipsoid_ellipsoid
+from mujoco.mjx._src.collision_types import FunctionKey
 from mujoco.mjx._src.types import Contact
 from mujoco.mjx._src.types import Data
 from mujoco.mjx._src.types import DisableBit
 from mujoco.mjx._src.types import GeomType
 from mujoco.mjx._src.types import Model
 # pylint: enable=g-importing-member
+import numpy as np
 
 # pair-wise collision functions
 _COLLISION_FUNC = {
     (GeomType.PLANE, GeomType.SPHERE): plane_sphere,
     (GeomType.PLANE, GeomType.CAPSULE): plane_capsule,
     (GeomType.PLANE, GeomType.BOX): plane_convex,
     (GeomType.PLANE, GeomType.ELLIPSOID): plane_ellipsoid,
+    (GeomType.PLANE, GeomType.CYLINDER): plane_cylinder,
     (GeomType.PLANE, GeomType.MESH): plane_convex,
     (GeomType.SPHERE, GeomType.SPHERE): sphere_sphere,
     (GeomType.SPHERE, GeomType.CAPSULE): sphere_capsule,
     (GeomType.SPHERE, GeomType.BOX): sphere_convex,
     (GeomType.SPHERE, GeomType.MESH): sphere_convex,
     (GeomType.CAPSULE, GeomType.CAPSULE): capsule_capsule,
     (GeomType.CAPSULE, GeomType.BOX): capsule_convex,
     (GeomType.CAPSULE, GeomType.ELLIPSOID): capsule_ellipsoid,
+    (GeomType.CAPSULE, GeomType.CYLINDER): capsule_cylinder,
     (GeomType.CAPSULE, GeomType.MESH): capsule_convex,
     (GeomType.ELLIPSOID, GeomType.ELLIPSOID): ellipsoid_ellipsoid,
+    (GeomType.ELLIPSOID, GeomType.CYLINDER): ellipsoid_cylinder,
+    (GeomType.CYLINDER, GeomType.CYLINDER): cylinder_cylinder,
     (GeomType.BOX, GeomType.BOX): convex_convex,
     (GeomType.BOX, GeomType.MESH): convex_convex,
     (GeomType.MESH, GeomType.MESH): convex_convex,
 }
 
 
-def get_collision_fn(
-    key: Tuple[Union[GeomType, mujoco.mjtGeom], Union[GeomType, mujoco.mjtGeom]]
-) -> Optional[Callable[[GeomInfo, GeomInfo], collision_base.Contact]]:
-  """Returns a collision function given a pair of geom types."""
-  return _COLLISION_FUNC.get(key, None)
+# geoms for which we ignore broadphase
+_GEOM_NO_BROADPHASE = {GeomType.HFIELD, GeomType.PLANE}
 
 
-def _add_candidate(
-    result: CandidateSet,
-    m: Union[Model, mujoco.MjModel],
-    g1: int,
-    g2: int,
-    ipair: int = -1,
-):
-  """Adds a candidate to test for collision."""
-  t1, t2 = m.geom_type[g1], m.geom_type[g2]
-  if t1 > t2:
-    t1, t2, g1, g2 = t2, t1, g2, g1
-
-  # MuJoCo does not collide planes with other planes or hfields
-  if t1 == GeomType.PLANE and t2 == GeomType.PLANE:
-    return
-  if t1 == GeomType.PLANE and t2 == GeomType.HFIELD:
-    return
-
-  def mesh_key(i):
-    convex_data = [[None] * m.ngeom] * 3
-    if isinstance(m, Model):
-      convex_data = [
-          m.geom_convex_face,
-          m.geom_convex_vert,
-          m.geom_convex_edge_dir,
-      ]
-    elif isinstance(m, mujoco.MjModel):
-      kwargs = mesh.get(m)
-      convex_data = [
-          kwargs['geom_convex_face'],
-          kwargs['geom_convex_vert'],
-          kwargs['geom_convex_edge_dir'],
-      ]
-    key = tuple((-1,) if v[i] is None else v[i].shape for v in convex_data)
-    return key
-
-  k1, k2 = mesh_key(g1), mesh_key(g2)
-
-  candidates = {(c.geom1, c.geom2) for c in result.get((t1, t2, k1, k2), [])}
-  if (g1, g2) in candidates:
-    return
-
-  if ipair > -1:
-    candidate = Candidate(g1, g2, ipair, -1, m.pair_dim[ipair])
-  elif m.geom_priority[g1] != m.geom_priority[g2]:
-    gp = g1 if m.geom_priority[g1] > m.geom_priority[g2] else g2
-    candidate = Candidate(g1, g2, -1, gp, m.geom_condim[gp])
-  else:
-    dim = max(m.geom_condim[g1], m.geom_condim[g2])
-    candidate = Candidate(g1, g2, -1, -1, dim)
-
-  result.setdefault((t1, t2, k1, k2), []).append(candidate)
-
-
-def _pair_params(
-    m: Model,
-    candidates: Sequence[Candidate],
-) -> SolverParams:
-  """Gets solver params for pair geoms."""
-  ipair = jp.array([c.ipair for c in candidates])
-  friction = jp.clip(m.pair_friction[ipair], a_min=mujoco.mjMINMU)
-  solref = m.pair_solref[ipair]
-  solreffriction = m.pair_solreffriction[ipair]
-  solimp = m.pair_solimp[ipair]
-  margin = m.pair_margin[ipair]
-  gap = m.pair_gap[ipair]
-
-  return SolverParams(friction, solref, solreffriction, solimp, margin, gap)
-
-
-def _priority_params(
-    m: Model,
-    candidates: Sequence[Candidate],
-) -> SolverParams:
-  """Gets solver params from priority geoms."""
-  geomp = jp.array([c.geomp for c in candidates])
-  friction = m.geom_friction[geomp][:, jp.array([0, 0, 1, 2, 2])]
-  solref = m.geom_solref[geomp]
-  solreffriction = jp.zeros(geomp.shape + (mujoco.mjNREF,))
-  solimp = m.geom_solimp[geomp]
-  g = jp.array([(c.geom1, c.geom2) for c in candidates])
-  margin = jp.amax(m.geom_margin[g.T], axis=0)
-  gap = jp.amax(m.geom_gap[g.T], axis=0)
-
-  return SolverParams(friction, solref, solreffriction, solimp, margin, gap)
-
-
-def _dynamic_params(
-    m: Model,
-    candidates: Sequence[Candidate],
-) -> SolverParams:
-  """Gets solver params for dynamic geoms."""
-  g1 = jp.array([c.geom1 for c in candidates])
-  g2 = jp.array([c.geom2 for c in candidates])
-
-  friction = jp.maximum(m.geom_friction[g1], m.geom_friction[g2])
-  # copy friction terms for the full geom pair
-  friction = friction[:, jp.array([0, 0, 1, 2, 2])]
-
-  minval = jp.array(mujoco.mjMINVAL)
-  solmix1, solmix2 = m.geom_solmix[g1], m.geom_solmix[g2]
-  mix = solmix1 / (solmix1 + solmix2)
-  mix = jp.where((solmix1 < minval) & (solmix2 < minval), 0.5, mix)
-  mix = jp.where((solmix1 < minval) & (solmix2 >= minval), 0.0, mix)
-  mix_fn = jax.vmap(lambda a, b, m: m * a + (1 - m) * b)
-
-  solref1, solref2 = m.geom_solref[g1], m.geom_solref[g2]
-  solref = jp.minimum(solref1, solref2)
-  s_mix = mix_fn(solref1, solref2, mix)
-  solref = jp.where((solref1[0] > 0) & (solref2[0] > 0), s_mix, solref)
-  solreffriction = jp.zeros(g1.shape + (mujoco.mjNREF,))
-  solimp = mix_fn(m.geom_solimp[g1], m.geom_solimp[g2], mix)
-  margin = jp.maximum(m.geom_margin[g1], m.geom_margin[g2])
-  gap = jp.maximum(m.geom_gap[g1], m.geom_gap[g2])
-
-  return SolverParams(friction, solref, solreffriction, solimp, margin, gap)
-
-
-def get_params(
-    m: Union[Model, mujoco.MjModel], candidates: Sequence[Candidate]
-) -> Tuple[List[int], List[int], SolverParams]:
-  """Gets solver params for a list of collision candidates."""
-  # group sol params by different candidate types
-  typ_cands = {}
-  for c in candidates:
-    typ = (c.ipair > -1, c.geomp > -1)
-    typ_cands.setdefault(typ, []).append(c)
-
-  geom1, geom2, params = [], [], []
-  for (pair, priority), candidates in typ_cands.items():
-    geom1.extend([c.geom1 for c in candidates])
-    geom2.extend([c.geom2 for c in candidates])
-    if pair:
-      params.append(_pair_params(m, candidates))
-    elif priority:
-      params.append(_priority_params(m, candidates))
-    else:
-      params.append(_dynamic_params(m, candidates))
+def has_collision_fn(t1: GeomType, t2: GeomType) -> bool:
+  """Returns True if a collision function exists for a pair of geom types."""
+  return (t1, t2) in _COLLISION_FUNC
 
-  params = jax.tree_map(lambda *x: jp.concatenate(x), *params)
-  return geom1, geom2, params
 
+def geom_pairs(
+    m: Union[Model, mujoco.MjModel],
+) -> Iterator[Tuple[int, int, int]]:
+  """Yields geom pairs to check for collisions.
 
-def _pair_info(
-    m: Model, d: Data, geom1: Sequence[int], geom2: Sequence[int]
-) -> Tuple[GeomInfo, GeomInfo, Sequence[Dict[str, Optional[int]]]]:
-  """Returns geom pair info for calculating collision."""
-  def mesh_info(geom):
-    g = jp.array(geom)
-    info = GeomInfo(
-        g,
-        d.geom_xpos[g],
-        d.geom_xmat[g],
-        m.geom_size[g],
-    )
-    in_axes = jax.tree_map(lambda x: 0, info)
-    is_mesh = m.geom_convex_face[geom[0]] is not None
-    if is_mesh:
-      info = info.replace(
-          face=jp.stack([m.geom_convex_face[i] for i in geom]),
-          vert=jp.stack([m.geom_convex_vert[i] for i in geom]),
-          edge_dir=jp.stack([m.geom_convex_edge_dir[i] for i in geom]),
-          facenorm=jp.stack([m.geom_convex_facenormal[i] for i in geom]),
-          edge=jp.stack([m.geom_convex_edge[i] for i in geom]),
-          edge_face_normal=jp.stack(
-              [m.geom_convex_edge_face_normal[i] for i in geom]
-          ),
-      )
-      in_axes = in_axes.replace(
-          face=0,
-          vert=0,
-          edge_dir=0,
-          facenorm=0,
-          edge=0,
-          edge_face_normal=0,
-      )
-    return info, in_axes
-
-  info1, in_axes1 = mesh_info(geom1)
-  info2, in_axes2 = mesh_info(geom2)
-  return info1, info2, [in_axes1, in_axes2]
-
-
-def _body_pair_filter(
-    m: Union[Model, mujoco.MjModel], b1: int, b2: int
-) -> bool:
-  """Filters body pairs for collision."""
-  dsbl_filterparent = m.opt.disableflags & DisableBit.FILTERPARENT
-  weld1 = m.body_weldid[b1]
-  weld2 = m.body_weldid[b2]
-  parent_weld1 = m.body_weldid[m.body_parentid[weld1]]
-  parent_weld2 = m.body_weldid[m.body_parentid[weld2]]
-
-  if weld1 == weld2:
-    # filter out self-collisions
-    return True
-
-  if (
-      not dsbl_filterparent
-      and weld1 != 0
-      and weld2 != 0
-      and (weld1 == parent_weld2 or weld2 == parent_weld1)
-  ):
-    # filter out parent-child collisions
-    return True
-
-  return False
-
-
-def _broadphase_enabled(
-    geom_types: Tuple[GeomType, GeomType],
-    n_pairs: int,
-    max_pairs: int,
-) -> bool:
-  return (
-      GeomType.PLANE not in geom_types
-      and max_pairs > -1
-      and n_pairs > max_pairs
-  )
-
-
-def _collide_geoms(
-    m: Model,
-    d: Data,
-    geom_types: Tuple[GeomType, GeomType],
-    candidates: Sequence[Candidate],
-) -> Contact:
-  """Collides a geom pair."""
-  fn = get_collision_fn(geom_types)
-  if not fn:
-    return Contact.zero()
-
-  geom1, geom2, params = get_params(m, candidates)
-  g1, g2, in_axes = _pair_info(m, d, geom1, geom2)
-
-  # Run a crude version of broadphase.
-  max_pairs = int(support.get_custom_numeric(m, 'max_geom_pairs'))
-  run_broadphase = _broadphase_enabled(geom_types, len(geom1), max_pairs)
-  n_pairs = max_pairs if run_broadphase else len(geom1)
-  if run_broadphase:
-    # broadphase over geom pairs, using bounding spheres
-    size1 = jp.max(m.geom_size[g1.geom_id], axis=-1)
-    size2 = jp.max(m.geom_size[g2.geom_id], axis=-1)
-    dists = jax.vmap(jp.linalg.norm)(g2.pos - g1.pos) - (size1 + size2)
-    _, idx = jax.lax.top_k(-dists, k=n_pairs)
-    g1, g2, params = jax.tree_map(
-        lambda x, idx=idx: x[idx, ...], (g1, g2, params)
-    )
+  Args:
+    m: a MuJoCo or MJX model
 
-  # call contact function
-  res = jax.vmap(fn, in_axes=in_axes)(g1, g2)
-  dist, pos, frame = jax.tree_map(jp.concatenate, res)
-
-  # repeat params by the number of contacts per geom pair
-  geom1, geom2, params = jax.tree_map(
-      lambda x: jp.repeat(x, fn.ncon, axis=0),  # pytype: disable=attribute-error
-      (g1.geom_id, g2.geom_id, params),
-  )
-
-  con = Contact(
-      dist=dist,
-      pos=pos,
-      frame=frame,
-      includemargin=params.margin - params.gap,
-      friction=params.friction,
-      solref=params.solref,
-      solreffriction=params.solreffriction,
-      solimp=params.solimp,
-      geom1=geom1,
-      geom2=geom2,
-  )
-  return con
-
-
-def collision_candidates(m: Union[Model, mujoco.MjModel]) -> CandidateSet:
-  """Returns candidates for collision checking."""
-  candidate_set = {}
-
-  for ipair in range(m.npair):
-    g1, g2 = m.pair_geom1[ipair], m.pair_geom2[ipair]
-    _add_candidate(candidate_set, m, g1, g2, ipair)
+  Yields:
+    geom1, geom2, and pair index if defined in <pair> (else -1)
+  """
+  pairs = set()
+
+  for i in range(m.npair):
+    g1, g2 = m.pair_geom1[i], m.pair_geom2[i]
+    # order pairs by geom_type for correct function mapping
+    if m.geom_type[g1] > m.geom_type[g2]:
+      g1, g2 = g2, g1
+    pairs.add((g1, g2))
+    yield g1, g2, i
 
-  body_pairs = []
   exclude_signature = set(m.exclude_signature)
   geom_con = m.geom_contype | m.geom_conaffinity
+  filterparent = not (m.opt.disableflags & DisableBit.FILTERPARENT)
   b_start = m.body_geomadr
   b_end = b_start + m.body_geomnum
 
   for b1 in range(m.nbody):
     if not geom_con[b_start[b1]:b_end[b1]].any():
       continue
+    w1 = m.body_weldid[b1]
+    w1_p = m.body_weldid[m.body_parentid[w1]]
+
     for b2 in range(b1, m.nbody):
       if not geom_con[b_start[b2]:b_end[b2]].any():
         continue
       signature = (b1 << 16) + (b2)
       if signature in exclude_signature:
         continue
-      if _body_pair_filter(m, b1, b2):
+      w2 = m.body_weldid[b2]
+      # ignore self-collisions
+      if w1 == w2:
         continue
-      body_pairs.append((b1, b2))
-
-  for b1, b2 in body_pairs:
-    for g1 in range(b_start[b1], b_end[b1]):
-      if not geom_con[g1]:
+      w2_p = m.body_weldid[m.body_parentid[w2]]
+      # ignore parent-child collisions
+      if filterparent and w1 != 0 and w2 != 0 and (w1 == w2_p or w2 == w1_p):
         continue
-      for g2 in range(b_start[b2], b_end[b2]):
-        if not geom_con[g2]:
+      g1_range = [g for g in range(b_start[b1], b_end[b1]) if geom_con[g]]
+      g2_range = [g for g in range(b_start[b2], b_end[b2]) if geom_con[g]]
+
+      for g1, g2 in itertools.product(g1_range, g2_range):
+        t1, t2 = m.geom_type[g1], m.geom_type[g2]
+        # order pairs by geom_type for correct function mapping
+        if t1 > t2:
+          g1, g2, t1, t2 = g2, g1, t2, t1
+        # ignore plane<>plane and plane<>hfield
+        if (t1, t2) == (GeomType.PLANE, GeomType.PLANE):
+          continue
+        if (t1, t2) == (GeomType.PLANE, GeomType.HFIELD):
           continue
+        # geoms must match contype and conaffinity on some bit
         mask = m.geom_contype[g1] & m.geom_conaffinity[g2]
         mask |= m.geom_contype[g2] & m.geom_conaffinity[g1]
-        if mask != 0:
-          _add_candidate(candidate_set, m, g1, g2)
+        if not mask:
+          continue
+
+        if (g1, g2) not in pairs:
+          pairs.add((g1, g2))
+          yield g1, g2, -1
 
-  return candidate_set
 
+def _geom_groups(
+    m: Union[Model, mujoco.MjModel],
+) -> Dict[FunctionKey, List[Tuple[int, int, int]]]:
+  """Returns geom pairs to check for collision grouped by collision function.
+
+  The grouping consists of:
+    - The collision function to run, which is determined by geom types
+    - For mesh geoms, convex functions are run for each distinct mesh in the
+      model, because the convex functions expect static mesh size. If a sphere
+      collides with a cube and a tetrahedron, sphere_convex is called twice.
+    - The condim of the collision. This ensures that the size of the resulting
+      constraint jacobian is determined at compile time.
+
+  Args:
+    m: a MuJoCo or MJX model
+
+  Returns:
+    a dict with grouping key and values geom1, geom2, pair index
+  """
+  groups = {}
+
+  for g1, g2, ip in geom_pairs(m):
+    types = m.geom_type[g1], m.geom_type[g2]
+    data_ids = m.geom_dataid[g1], m.geom_dataid[g2]
+    if ip > -1:
+      condim = m.pair_dim[ip]
+    elif m.geom_priority[g1] > m.geom_priority[g2]:
+      condim = m.geom_condim[g1]
+    elif m.geom_priority[g1] < m.geom_priority[g2]:
+      condim = m.geom_condim[g2]
+    else:
+      condim = max(m.geom_condim[g1], m.geom_condim[g2])
+
+    key = FunctionKey(types, data_ids, condim)
+    groups.setdefault(key, []).append((g1, g2, ip))
+
+  return groups
+
+
+def _contact_groups(m: Model, d: Data) -> Dict[FunctionKey, Contact]:
+  """Returns contact groups to check for collisions.
+
+  Contacts are grouped the same way as _geom_groups.  Only one contact is
+  emitted per geom pair, even if the collision function emits multiple contacts.
+
+  Args:
+    m: MJX model
+    d: MJX data
+
+  Returns:
+    a dict where the key is the grouping and value is a Contact
+  """
+  groups = {}
+  eps = mujoco.mjMINVAL
+
+  for key, geom_ids in _geom_groups(m).items():
+    geom = np.array(geom_ids)
+    geom1, geom2, ip = geom.T
+    geom1, geom2, ip = geom1[ip == -1], geom2[ip == -1], ip[ip != -1]
+    params = []
+
+    if ip.size > 0:
+      # pair contacts get their params from m.pair_* fields
+      params.append((
+          m.pair_margin[ip] - m.pair_gap[ip],
+          jp.clip(m.pair_friction[ip], a_min=eps),
+          m.pair_solref[ip],
+          m.pair_solreffriction[ip],
+          m.pair_solimp[ip]
+      ))
+    if geom1.size > 0 and geom2.size > 0:
+      # other contacts get their params from geom fields
+      margin = jp.maximum(m.geom_margin[geom1], m.geom_margin[geom2])
+      gap = jp.maximum(m.geom_gap[geom1], m.geom_gap[geom2])
+      solmix1, solmix2 = m.geom_solmix[geom1], m.geom_solmix[geom2]
+      mix = solmix1 / (solmix1 + solmix2)
+      mix = jp.where((solmix1 < eps) & (solmix2 < eps), 0.5, mix)
+      mix = jp.where((solmix1 < eps) & (solmix2 >= eps), 0.0, mix)
+      mix = jp.where((solmix1 >= eps) & (solmix2 < eps), 1.0, mix)
+      mix = mix[:, None]  # for correct broadcasting
+      # friction: max
+      friction = jp.maximum(m.geom_friction[geom1], m.geom_friction[geom2])
+      solref1, solref2 = m.geom_solref[geom1], m.geom_solref[geom2]
+      # reference standard: mix
+      solref_standard = mix * solref1 + (1 - mix) * solref2
+      # reference direct: min
+      solref_direct = jp.minimum(solref1, solref2)
+      is_standard = (solref1[:, [0, 0]] > 0) & (solref2[:, [0, 0]] > 0)
+      solref = jp.where(is_standard, solref_standard, solref_direct)
+      solreffriction = jp.zeros(geom1.shape + (mujoco.mjNREF,))
+      # impedance: mix
+      solimp = mix * m.geom_solimp[geom1] + (1 - mix) * m.geom_solimp[geom2]
+
+      pri = m.geom_priority[geom1] != m.geom_priority[geom2]
+      if pri.any():
+        # use priority geom when specified instead of mixing
+        gp1, gp2 = m.geom_priority[geom1], m.geom_priority[geom2]
+        gp = np.where(gp1 > gp2, geom1, geom2)[pri]
+        friction = friction.at[pri].set(m.geom_friction[gp])
+        solref = solref.at[pri].set(m.geom_solref[gp])
+        solimp = solimp.at[pri].set(m.geom_solimp[gp])
+
+      # unpack 5d friction:
+      friction = friction[:, [0, 0, 1, 2, 2]]
+      params.append((margin - gap, friction, solref, solreffriction, solimp))
+
+    params = map(jp.concatenate, zip(*params))
+    includemargin, friction, solref, solreffriction, solimp = params
+
+    groups[key] = Contact(
+        # dist, pos, frame get filled in by collision functions:
+        dist=None,
+        pos=None,
+        frame=None,
+        includemargin=includemargin,
+        friction=friction,
+        solref=solref,
+        solreffriction=solreffriction,
+        solimp=solimp,
+        dim=d.contact.dim,
+        geom1=jp.array(geom[:, 0]),
+        geom2=jp.array(geom[:, 1]),
+        geom=jp.array(geom[:, :2]),
+        efc_address=d.contact.efc_address,
+    )
+
+  return groups
 
-def ncon(m: Union[Model, mujoco.MjModel]) -> int:
-  """Returns the number of contacts computed in MJX given a model."""
+
+def _numeric(m: Union[Model, mujoco.MjModel], name: str) -> int:
+  id_ = support.name2id(m, mujoco.mjtObj.mjOBJ_NUMERIC, name)
+  return int(m.numeric_data[id_]) if id_ >= 0 else -1
+
+
+def make_condim(m: Union[Model, mujoco.MjModel]) -> np.ndarray:
+  """Returns the dims of the contacts for a Model."""
   if m.opt.disableflags & DisableBit.CONTACT:
-    return 0
+    return np.empty(0, dtype=int)
 
-  candidates = collision_candidates(m)
-  max_count = int(support.get_custom_numeric(m, 'max_contact_points'))
-  max_pairs = int(support.get_custom_numeric(m, 'max_geom_pairs'))
-
-  count = 0
-  for k, v in candidates.items():
-    fn = get_collision_fn(k[0:2])
-    if fn is None:
-      continue
-    run_broadphase = _broadphase_enabled((k[0], k[1]), len(v), max_pairs)
-    n_pair = max_pairs if run_broadphase else len(v)
-    count += n_pair * fn.ncon  # pytype: disable=attribute-error
+  group_counts = {k: len(v) for k, v in _geom_groups(m).items()}
+
+  # max_geom_pairs limits the number of pairs we process in a collision function
+  # by first running a primitive broad phase culling on the pairs
+  max_geom_pairs = _numeric(m, 'max_geom_pairs')
+
+  if max_geom_pairs > -1:
+    for k in group_counts:
+      if set(k.types) & _GEOM_NO_BROADPHASE:
+        continue
+      group_counts[k] = min(group_counts[k], max_geom_pairs)
+
+  # max_contact_points limits the number of contacts emitted by selecting the
+  # contacts with the most penetration after calling collision functions
+  max_contact_points = _numeric(m, 'max_contact_points')
+
+  condim_counts = {}
+  for k, v in group_counts.items():
+    func = _COLLISION_FUNC[k.types]
+    num_contacts = condim_counts.get(k.condim, 0) + func.ncon * v  # pytype: disable=attribute-error
+    if max_contact_points > -1:
+      num_contacts = min(max_contact_points, num_contacts)
+    condim_counts[k.condim] = num_contacts
+
+  dims = sum(([c] * condim_counts[c] for c in sorted(condim_counts)), [])
 
-  return min(max_count, count) if max_count > -1 else count
+  return np.array(dims)
 
 
 def collision(m: Model, d: Data) -> Data:
   """Collides geometries."""
-  if ncon(m) == 0:
-    return d.replace(contact=Contact.zero())
+  if d.ncon == 0:
+    return d
 
-  candidate_set = collision_candidates(m)
+  groups = _contact_groups(m, d)
+  max_geom_pairs = _numeric(m, 'max_geom_pairs')
+  max_contact_points = _numeric(m, 'max_contact_points')
+
+  # run collision functions on groups
+  for key, contact in groups.items():
+    # determine which contacts we'll use for collision testing by running a
+    # broad phase cull if requested
+    if (
+        max_geom_pairs > -1
+        and contact.geom.shape[0] > max_geom_pairs
+        and not set(key.types) & _GEOM_NO_BROADPHASE
+    ):
+      pos1, pos2 = d.geom_xpos[contact.geom.T]
+      size1, size2 = m.geom_rbound[contact.geom.T]
+      dist = jax.vmap(jp.linalg.norm)(pos2 - pos1) - (size1 + size2)
+      _, idx = jax.lax.top_k(-dist, k=max_geom_pairs)
+      contact = jax.tree_util.tree_map(lambda x, idx=idx: x[idx], contact)
+
+    # run the collision function specified by the grouping key
+    func = _COLLISION_FUNC[key.types]
+    dist, pos, frame = func(m, d, key, contact.geom)
+    ncon = func.ncon  # pytype: disable=attribute-error
+    if ncon > 1:
+      # repeat contacts to match the number of collisions returned
+      repeat_fn = lambda x, r=ncon: jp.repeat(x, r, axis=0)
+      contact = jax.tree_util.tree_map(repeat_fn, contact)
+    groups[key] = contact.replace(dist=dist, pos=pos, frame=frame)
+
+  # collapse contacts together, ensuring they are grouped by condim
+  condim_groups = {}
+  for key, contact in groups.items():
+    condim_groups.setdefault(key.condim, []).append(contact)
+
+  # limit the number of contacts per condim group if requested
+  if max_contact_points > -1:
+    for key, contacts in condim_groups.items():
+      contact = jax.tree_util.tree_map(lambda *x: jp.concatenate(x), *contacts)
+      if contact.geom.shape[0] > max_contact_points:
+        _, idx = jax.lax.top_k(-contact.dist, k=max_contact_points)
+        contact = jax.tree_util.tree_map(lambda x, idx=idx: x[idx], contact)
+      condim_groups[key] = [contact]
 
-  contacts = []
-  for key, candidates in candidate_set.items():
-    geom_types = key[0:2]
-    contacts.append(_collide_geoms(m, d, geom_types, candidates))
-
-  if not contacts:
-    raise RuntimeError('No contacts found.')
-
-  contact = jax.tree_map(lambda *x: jp.concatenate(x), *contacts)
-
-  max_contact_points = int(support.get_custom_numeric(m, 'max_contact_points'))
-  if max_contact_points > -1 and contact.dist.shape[0] > max_contact_points:
-    # get top-k contacts
-    _, idx = jax.lax.top_k(-contact.dist, k=max_contact_points)
-    contact = jax.tree_map(lambda x, idx=idx: jp.take(x, idx, axis=0), contact)
+  contacts = sum([condim_groups[k] for k in sorted(condim_groups)], [])
+  contact = jax.tree_util.tree_map(lambda *x: jp.concatenate(x), *contacts)
 
   return d.replace(contact=contact)
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/collision_driver_test.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/collision_driver_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -260,14 +260,37 @@
     """Tests ellipsoid capsule contact."""
     d, dx = _collide(self._ELLIPSOID_CAPSULE)
     self.assertLess(dx.contact.dist[0], 0)
     for field in dataclasses.fields(Contact):
       _assert_attr_eq(
           dx.contact, d.contact, field.name, 'ellipsoid-capsule', 1e-4)
 
+  _ELLIPSOID_CYLINDER = """
+    <mujoco>
+      <worldbody>
+        <body>
+          <geom size=".15 .05" type="cylinder"/>
+        </body>
+        <body pos="0 0 0.09">
+          <freejoint/>
+          <geom size=".15 .03 .05" type="ellipsoid"/>
+        </body>
+      </worldbody>
+    </mujoco>
+  """
+
+  def test_ellipsoid_cylinder(self):
+    """Tests ellipsoid cylinder contact."""
+    d, dx = _collide(self._ELLIPSOID_CYLINDER)
+    d.contact.pos[0][2] = 0.04  # MJX finds the deepest point on the surface
+    self.assertLess(dx.contact.dist[0], 0)
+    for field in dataclasses.fields(Contact):
+      _assert_attr_eq(
+          dx.contact, d.contact, field.name, 'ellipsoid-cylinder', 1e-4)
+
 
 class CapsuleCollisionTest(parameterized.TestCase):
   _CAP_PLANE = """
     <mujoco>
       <worldbody>
         <geom size="40 40 40" type="plane"/>
         <body pos="0 0 0.4">
@@ -398,15 +421,16 @@
     """Tests edge contact."""
     d, dx = _collide(self._CAP_EDGE_BOX)
 
     c = dx.contact
     self.assertEqual(c.pos.shape[0], 2)
     self.assertGreater(c.dist[1], 0)
     # extract the contact point with penetration
-    c = jax.tree_map(lambda x: jp.take(x, 0, axis=0)[None], dx.contact)
+    c = jax.tree_util.tree_map(lambda x: x[:1], dx.contact)
+    c = c.replace(dim=c.dim[:1], efc_address=c.efc_address[:1])
     for field in dataclasses.fields(Contact):
       _assert_attr_eq(c, d.contact, field.name, 'capsule_convex_edge', 1e-4)
 
   def test_capsule_convex_edge_deep(self):
     """Tests deep edge penetration."""
     xml = self._CAP_EDGE_BOX.replace(
         '<body pos="0.5 0 0.55"', '<body pos="0.5 0 0.42"'
@@ -433,15 +457,16 @@
     xml = xml.replace('<body pos="0.5 0 0.55"', '<body pos="0.58 0 0.55"')
     d, dx = _collide(xml)
 
     c = dx.contact
     self.assertEqual(c.pos.shape[0], 2)
     self.assertGreater(c.dist[1], 0)
     # extract the contact point with penetration
-    c = jax.tree_map(lambda x: jp.take(x, 0, axis=0)[None], dx.contact)
+    c = jax.tree_util.tree_map(lambda x: x[:1], dx.contact)
+    c = c.replace(dim=c.dim[:1], efc_address=c.efc_address[:1])
     for field in dataclasses.fields(Contact):
       _assert_attr_eq(c, d.contact, field.name, 'edge_shallow_tip1', 1e-4)
     np.testing.assert_array_almost_equal(
         dx.contact.frame[0][0, :3], np.array([-0.43952, 0.0, -0.898233])
     )
 
     # the capsule sphere is outside the edge voronoi region, so there is a
@@ -453,22 +478,68 @@
     xml = xml.replace('<body pos="0.5 0 0.55"', '<body pos="0.5 0 0.52"')
     d, dx = _collide(xml)
 
     c = dx.contact
     self.assertEqual(c.pos.shape[0], 2)
     self.assertGreater(c.dist[1], 0)
     # extract the contact point with penetration
-    c = jax.tree_map(lambda x: jp.take(x, 0, axis=0)[None], dx.contact)
+    c = jax.tree_util.tree_map(lambda x: x[:1], dx.contact)
+    c = c.replace(dim=c.dim[:1], efc_address=c.efc_address[:1])
     for field in dataclasses.fields(Contact):
       _assert_attr_eq(c, d.contact, field.name, 'edge_shallow_tip2', 1e-4)
     np.testing.assert_array_almost_equal(
         dx.contact.frame[0][0, :3], np.array([0.0, 0.0, -1.0])
     )
 
 
+class CylinderTest(absltest.TestCase):
+  """Tests the cylinder contact functions."""
+
+  _CYLINDER_PLANE = """
+    <mujoco>
+      <worldbody>
+        <geom size="40 40 40" type="plane"/>
+        <body pos="0 0 0.04">
+          <joint type="free"/>
+          <geom fromto="-0.1 0 0 0.1 0 0" size="0.05" type="cylinder"/>
+        </body>
+      </worldbody>
+    </mujoco>
+  """
+
+  def test_cylinder_plane(self):
+    d, dx = _collide(self._CYLINDER_PLANE)
+
+    # cylinder is lying flat
+    np.testing.assert_array_less(dx.contact.dist[:2], 0)
+    np.testing.assert_array_less(-dx.contact.dist[2:], 0)
+
+    # sort position for comparison
+    idx = np.lexsort((dx.contact.pos[:, 0], dx.contact.pos[:, 1]))
+    dx = dx.tree_replace({'contact.pos': dx.contact.pos[idx]})
+    idx = np.lexsort((d.contact.pos[:, 0], d.contact.pos[:, 1]))
+    d.contact.pos[:] = d.contact.pos[idx]
+
+    # extract the contact points with penetration
+    c = jax.tree_util.tree_map(lambda x: x[:2], dx.contact)
+    c = c.replace(dim=c.dim[:2], efc_address=c.efc_address[:2])
+    for field in dataclasses.fields(Contact):
+      _assert_attr_eq(c, d.contact, field.name, 'cylinder_plane', 1e-5)
+
+    # cylinder is vertical
+    xml = self._CYLINDER_PLANE.replace(
+        '<geom fromto="-0.1 0 0 0.1 0 0"', '<geom fromto="0 0 -0.1 0 0 0.1"')
+    xml = xml.replace('pos="0 0 0.04"', 'pos="0 0 0.095"')
+    d, dx = _collide(xml)
+
+    np.testing.assert_array_less(dx.contact.dist, 0)
+    for field in dataclasses.fields(Contact):
+      _assert_attr_eq(dx.contact, d.contact, field.name, 'cylinder_plane', 1e-5)
+
+
 class ConvexTest(absltest.TestCase):
   """Tests the convex contact functions."""
 
   _BOX_PLANE = """
     <mujoco>
       <worldbody>
         <geom size="40 40 40" type="plane"/>
@@ -483,15 +554,16 @@
   def test_box_plane(self):
     """Tests box collision with a plane."""
     d, dx = _collide(self._BOX_PLANE)
 
     np.testing.assert_array_less(dx.contact.dist[:2], 0)
     np.testing.assert_array_less(-dx.contact.dist[2:], 0)
     # extract the contact points with penetration
-    c = jax.tree_map(lambda x: jp.take(x, jp.array([0, 1]), axis=0), dx.contact)
+    c = jax.tree_util.tree_map(lambda x: jp.take(x, jp.array([0, 1]), axis=0), dx.contact)
+    c = c.replace(dim=c.dim[[0, 1]], efc_address=c.efc_address[[0, 1]])
     for field in dataclasses.fields(Contact):
       _assert_attr_eq(c, d.contact, field.name, 'box_plane', 1e-5)
 
   _FLAT_BOX_PLANE = """
     <mujoco>
       <worldbody>
         <geom size="40 40 40" type="plane"/>
@@ -567,15 +639,16 @@
     """Tests an edge contact for a box-box collision."""
     d, dx = _collide(self._BOX_BOX_EDGE)
 
     # Only one contact point.
     np.testing.assert_array_less(dx.contact.dist[:1], 0)
     np.testing.assert_array_less(-dx.contact.dist[1:], 0)
     # extract the contact point with penetration
-    c = jax.tree_map(lambda x: jp.take(x, 0, axis=0)[None], dx.contact)
+    c = jax.tree_util.tree_map(lambda x: x[:1], dx.contact)
+    c = c.replace(dim=c.dim[:1], efc_address=c.efc_address[:1])
     for field in dataclasses.fields(Contact):
       _assert_attr_eq(c, d.contact, field.name, 'box_box_edge', 1e-2)
 
   _CONVEX_CONVEX = """
     <mujoco>
       <asset>
         <mesh name="dodecahedron" file="meshes/dodecahedron.stl" scale="0.01 0.01 0.01" />
@@ -715,51 +788,52 @@
     dx = collision_jit_fn(mx, dx)
 
     # one collision between parent-child spheres
     self.assertEqual(dx.contact.pos.shape[0], d.contact.pos.shape[0])
     self.assertEqual(dx.contact.pos.shape[0], 1)
 
 
-class NconTest(parameterized.TestCase):
-  """Tests ncon."""
+class DimTest(parameterized.TestCase):
+  """Tests contact dim."""
 
   def test_ncon(self):
     m = test_util.load_test_file('constraints.xml')
-    ncon = collision_driver.ncon(m)
-    self.assertEqual(ncon, 16)
+    dim = collision_driver.make_condim(m)
+    expected = [1] * 4 + [3] * 20 + [4] * 4 + [6] * 4
+    np.testing.assert_array_equal(dim, np.array(expected))
 
   def test_disable_contact(self):
     m = test_util.load_test_file('constraints.xml')
     m.opt.disableflags |= DisableBit.CONTACT
-    ncon = collision_driver.ncon(m)
-    self.assertEqual(ncon, 0)
+    dim = collision_driver.make_condim(m)
+    self.assertEqual(dim.size, 0)
 
   def test_ncon_meshes(self):
     m = test_util.load_test_file('shadow_hand/scene_right.xml')
 
-    ncon = collision_driver.ncon(m)
+    ncon = collision_driver.make_condim(m).size
     self.assertEqual(ncon, 15)
 
     mx = mjx.put_model(m)
-    ncon = collision_driver.ncon(mx)
+    ncon = collision_driver.make_condim(mx).size
     self.assertEqual(ncon, 15)
 
     # get rid of max_contact_points, test only max_geom_pairs
     for i in range(m.nnumeric):
       name_ = (
           m.names[m.name_numericadr[i] :].decode('utf-8').split('\x00', 1)[0]
       )
       if name_ == 'max_contact_points':
         m.numeric_data[m.numeric_adr[i]] = -1
 
-    ncon = collision_driver.ncon(m)
+    ncon = collision_driver.make_condim(m).size
     self.assertEqual(ncon, 98)
 
     mx = mjx.put_model(m)
-    ncon = collision_driver.ncon(mx)
+    ncon = collision_driver.make_condim(mx).size
     self.assertEqual(ncon, 98)
 
 
 class TopKContactTest(absltest.TestCase):
   """Tests top-k contacts."""
 
   _CAPSULES = """
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/collision_primitive.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/collision_primitive.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,125 +16,188 @@
 
 from typing import Tuple
 
 import jax
 from jax import numpy as jp
 from mujoco.mjx._src import math
 # pylint: disable=g-importing-member
-from mujoco.mjx._src.collision_base import Contact
-from mujoco.mjx._src.collision_base import GeomInfo
+from mujoco.mjx._src.collision_types import Collision
+from mujoco.mjx._src.collision_types import GeomInfo
+from mujoco.mjx._src.types import Data
+from mujoco.mjx._src.types import Model
 # pylint: enable=g-importing-member
 
 
+def collider(ncon: int):
+  """Wraps collision functions for use by collision_driver."""
+  def wrapper(func):
+    def collide(m: Model, d: Data, _, geom: jax.Array) -> Collision:
+      g1, g2 = geom.T
+      info1 = GeomInfo(d.geom_xpos[g1], d.geom_xmat[g1], m.geom_size[g1])
+      info2 = GeomInfo(d.geom_xpos[g2], d.geom_xmat[g2], m.geom_size[g2])
+      dist, pos, frame = jax.vmap(func)(info1, info2)
+      if ncon > 1:
+        return jax.tree_util.tree_map(jp.concatenate, (dist, pos, frame))
+      return dist, pos, frame
+
+    collide.ncon = ncon
+    return collide
+
+  return wrapper
+
+
 def _plane_sphere(
     plane_normal: jax.Array,
     plane_pos: jax.Array,
     sphere_pos: jax.Array,
-    radius: jax.Array,
+    sphere_radius: jax.Array,
 ) -> Tuple[jax.Array, jax.Array]:
-  """Returns the penetration and contact point between a plane and sphere."""
-  cdist = jp.dot(sphere_pos - plane_pos, plane_normal)
-  dist = cdist - radius
-  pos = sphere_pos - plane_normal * (radius + 0.5 * dist)
+  """Returns the distance and contact point between a plane and sphere."""
+  dist = jp.dot(sphere_pos - plane_pos, plane_normal) - sphere_radius
+  pos = sphere_pos - plane_normal * (sphere_radius + 0.5 * dist)
   return dist, pos
 
 
-def plane_sphere(plane: GeomInfo, sphere: GeomInfo) -> Contact:
+@collider(ncon=1)
+def plane_sphere(plane: GeomInfo, sphere: GeomInfo) -> Collision:
   """Calculates contact between a plane and a sphere."""
   n = plane.mat[:, 2]
   dist, pos = _plane_sphere(n, plane.pos, sphere.pos, sphere.size[0])
-  return jax.tree_map(
-      lambda x: jp.expand_dims(x, axis=0), (dist, pos, math.make_frame(n))
-  )
+  return dist, pos, math.make_frame(n)
 
 
-def plane_capsule(plane: GeomInfo, cap: GeomInfo) -> Contact:
+@collider(ncon=2)
+def plane_capsule(plane: GeomInfo, cap: GeomInfo) -> Collision:
   """Calculates two contacts between a capsule and a plane."""
   n, axis = plane.mat[:, 2], cap.mat[:, 2]
   # align contact frames with capsule axis
   b, b_norm = math.normalize_with_norm(axis - n * jp.dot(n, axis))
   y, z = jp.array([0.0, 1.0, 0.0]), jp.array([0.0, 0.0, 1.0])
   b = jp.where(b_norm < 0.5, jp.where((-0.5 < n[1]) & (n[1] < 0.5), y, z), b)
   frame = jp.array([[n, b, jp.cross(n, b)]])
   segment = axis * cap.size[1]
-  contacts = []
+  collisions = []
   for offset in [segment, -segment]:
     dist, pos = _plane_sphere(n, plane.pos, cap.pos + offset, cap.size[0])
     dist = jp.expand_dims(dist, axis=0)
     pos = jp.expand_dims(pos, axis=0)
-    contacts.append((dist, pos, frame))
-  return jax.tree_map(lambda *x: jp.concatenate(x), *contacts)
+    collisions.append((dist, pos, frame))
+  return jax.tree_util.tree_map(lambda *x: jp.concatenate(x), *collisions)
 
 
-def plane_ellipsoid(plane: GeomInfo, ellipsoid: GeomInfo) -> Contact:
+@collider(ncon=1)
+def plane_ellipsoid(plane: GeomInfo, ellipsoid: GeomInfo) -> Collision:
   """Calculates one contact between an ellipsoid and a plane."""
   n = plane.mat[:, 2]
   size = ellipsoid.size
   sphere_support = -math.normalize((ellipsoid.mat.T @ n) * size)
   pos = ellipsoid.pos + ellipsoid.mat @ (sphere_support * size)
   dist = jp.dot(n, pos - plane.pos)
   pos = pos - n * dist * 0.5
-  return jax.tree_map(
-      lambda x: jp.expand_dims(x, axis=0), (dist, pos, math.make_frame(n))
+  return dist, pos, math.make_frame(n)
+
+
+@collider(ncon=3)
+def plane_cylinder(plane: GeomInfo, cylinder: GeomInfo) -> Collision:
+  """Calculates one contact between an cylinder and a plane."""
+  n = plane.mat[:, 2]
+  axis = cylinder.mat[:, 2]
+
+  # make sure axis points towards plane
+  prjaxis = jp.dot(n, axis)
+  sign = -math.sign(prjaxis)
+  axis, prjaxis = axis * sign, prjaxis * sign
+
+  # compute normal distance to cylinder center
+  dist0 = jp.dot(cylinder.pos - plane.pos, n)
+
+  # remove component of -normal along axis, compute length
+  vec = axis * prjaxis - n
+  len_ = math.norm(vec)
+
+  vec = jp.where(
+      len_ < 1e-12,
+      # disk parallel to plane: pick x-axis of cylinder, scale by radius
+      cylinder.mat[:, 0] * cylinder.size[0],
+      # general configuration: normalize vector, scale by radius
+      vec / len_ * cylinder.size[0]
+  )
+
+  # project vector on normal
+  prjvec = jp.dot(vec, n)
+
+  # scale axis by half-length
+  axis *= cylinder.size[1]
+  prjaxis *= cylinder.size[1]
+
+  # compute sideways vector: vec1
+  prjvec1 = -prjvec * 0.5
+  vec1 = math.normalize(jp.cross(vec, axis)) * cylinder.size[0]
+  vec1 *= jp.sqrt(3.0) * 0.5
+
+  # disk parallel to plane
+  d1 = dist0 + prjaxis + prjvec
+  d2 = dist0 + prjaxis + prjvec1
+  dist = jp.array([d1, d2, d2])
+  pos = cylinder.pos + axis + jp.array([
+      vec  - n * d1 * 0.5,
+      vec1 + vec * -0.5 - n * d2 * 0.5,
+      -vec1 + vec * -0.5 - n * d2 * 0.5,
+  ])
+
+  # cylinder parallel to plane
+  cond = jp.abs(prjaxis) < 1e-3
+  d3 = dist0 - prjaxis + prjvec
+  dist = jp.where(cond, dist.at[1].set(d3), dist)
+  pos = jp.where(
+      cond, pos.at[1].set(cylinder.pos + vec - axis - n * d3 * 0.5), pos
   )
 
+  frame = jp.stack([math.make_frame(n)] * 3, axis=0)
+  return dist, pos, frame
+
 
 def _sphere_sphere(
     pos1: jax.Array, radius1: jax.Array, pos2: jax.Array, radius2: jax.Array
-) -> Contact:
+) -> Tuple[jax.Array, jax.Array, jax.Array]:
   """Returns the penetration, contact point, and normal between two spheres."""
   n, dist = math.normalize_with_norm(pos2 - pos1)
   n = jp.where(dist == 0.0, jp.array([1.0, 0.0, 0.0]), n)
   dist = dist - (radius1 + radius2)
   pos = pos1 + n * (radius1 + dist * 0.5)
   return dist, pos, n
 
 
-def sphere_sphere(s1: GeomInfo, s2: GeomInfo) -> Contact:
+@collider(ncon=1)
+def sphere_sphere(s1: GeomInfo, s2: GeomInfo) -> Collision:
   """Calculates contact between two spheres."""
   dist, pos, n = _sphere_sphere(s1.pos, s1.size[0], s2.pos, s2.size[0])
-  return jax.tree_map(
-      lambda x: jp.expand_dims(x, axis=0), (dist, pos, math.make_frame(n))
-  )
+  return dist, pos, math.make_frame(n)
 
 
-def sphere_capsule(sphere: GeomInfo, cap: GeomInfo) -> Contact:
+@collider(ncon=1)
+def sphere_capsule(sphere: GeomInfo, cap: GeomInfo) -> Collision:
   """Calculates one contact between a sphere and a capsule."""
   axis, length = cap.mat[:, 2], cap.size[1]
   segment = axis * length
   pt = math.closest_segment_point(
       cap.pos - segment, cap.pos + segment, sphere.pos
   )
   dist, pos, n = _sphere_sphere(sphere.pos, sphere.size[0], pt, cap.size[0])
-  return jax.tree_map(
-      lambda x: jp.expand_dims(x, axis=0), (dist, pos, math.make_frame(n))
-  )
+  return dist, pos, math.make_frame(n)
 
 
-def capsule_capsule(cap1: GeomInfo, cap2: GeomInfo) -> Contact:
+@collider(ncon=1)
+def capsule_capsule(cap1: GeomInfo, cap2: GeomInfo) -> Collision:
   """Calculates one contact between two capsules."""
-  axis1, length1, axis2, length2 = (
-      cap1.mat[:, 2],
-      cap1.size[1],
-      cap2.mat[:, 2],
-      cap2.size[1],
-  )
+  axis1, length1 = cap1.mat[:, 2], cap1.size[1]
+  axis2, length2 = cap2.mat[:, 2], cap2.size[1]
   seg1, seg2 = axis1 * length1, axis2 * length2
   pt1, pt2 = math.closest_segment_to_segment_points(
       cap1.pos - seg1,
       cap1.pos + seg1,
       cap2.pos - seg2,
       cap2.pos + seg2,
   )
   radius1, radius2 = cap1.size[0], cap2.size[0]
   dist, pos, n = _sphere_sphere(pt1, radius1, pt2, radius2)
-  return jax.tree_map(
-      lambda x: jp.expand_dims(x, axis=0), (dist, pos, math.make_frame(n))
-  )
-
-# store ncon as function attributes
-plane_sphere.ncon = 1
-plane_capsule.ncon = 2
-plane_ellipsoid.ncon = 1
-sphere_sphere.ncon = 1
-sphere_capsule.ncon = 1
-capsule_capsule.ncon = 1
+  return dist, pos, math.make_frame(n)
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/constraint.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/constraint.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,24 +20,28 @@
 from jax import numpy as jp
 import mujoco
 from mujoco.mjx._src import collision_driver
 from mujoco.mjx._src import math
 from mujoco.mjx._src import support
 # pylint: disable=g-importing-member
 from mujoco.mjx._src.dataclasses import PyTreeNode
+from mujoco.mjx._src.types import ConstraintType
 from mujoco.mjx._src.types import Contact
 from mujoco.mjx._src.types import Data
 from mujoco.mjx._src.types import DisableBit
 from mujoco.mjx._src.types import EqType
 from mujoco.mjx._src.types import JointType
 from mujoco.mjx._src.types import Model
 # pylint: enable=g-importing-member
 import numpy as np
 
 
+_CONDIM_EFC_COUNT = {1: 1, 3: 4, 4: 6, 6: 10}
+
+
 class _Efc(PyTreeNode):
   """Support data for creating constraint matrices."""
   J: jax.Array
   pos: jax.Array
   pos_norm: jax.Array
   invweight: jax.Array
   solref: jax.Array
@@ -107,15 +111,15 @@
     jacp1, _ = support.jac(m, d, pos1, id1)
     jacp2, _ = support.jac(m, d, pos2, id2)
     j = (jacp1 - jacp2).T
 
     return j, cpos, jp.repeat(math.norm(cpos), 3)
 
   # concatenate to drop connect grouping dimension
-  j, pos, pos_norm = jax.tree_map(jp.concatenate, fn(data, id1, id2))
+  j, pos, pos_norm = jax.tree_util.tree_map(jp.concatenate, fn(data, id1, id2))
   invweight = m.body_invweight0[id1, 0] + m.body_invweight0[id2, 0]
   invweight = jp.repeat(invweight, 3)
   solref = jp.tile(m.eq_solref[ids], (3, 1))
   solimp = jp.tile(m.eq_solimp[ids], (3, 1))
   frictionloss = jp.zeros_like(pos_norm)
 
   return _Efc(j, pos, pos_norm, invweight, solref, solimp, frictionloss)
@@ -160,15 +164,15 @@
 
     j = jp.concatenate((jacdifp.T, jacdifr.T))
     pos = jp.concatenate((cpos, crot * torquescale))
 
     return j, pos, jp.repeat(math.norm(pos), 6)
 
   # concatenate to drop weld grouping dimension
-  j, pos, pos_norm = jax.tree_map(jp.concatenate, fn(data, id1, id2))
+  j, pos, pos_norm = jax.tree_util.tree_map(jp.concatenate, fn(data, id1, id2))
   invweight = m.body_invweight0[id1] + m.body_invweight0[id2]
   invweight = jp.repeat(invweight, 3)
   solref = jp.tile(m.eq_solref[ids], (6, 1))
   solimp = jp.tile(m.eq_solimp[ids], (6, 1))
   frictionloss = jp.zeros_like(pos_norm)
 
   return _Efc(j, pos, pos_norm, invweight, solref, solimp, frictionloss)
@@ -273,79 +277,115 @@
 
   return _Efc(j, pos, pos, invweight, solref, solimp, frictionloss)
 
 
 def _instantiate_contact(m: Model, d: Data) -> Optional[_Efc]:
   """Calculates constraint rows for contacts."""
 
-  if collision_driver.ncon(m) == 0:
+  if d.ncon == 0:
     return None
 
-  @jax.vmap
-  def fn(c: Contact):
-    dist = c.dist - c.includemargin
-    geom_bodyid = jp.array(m.geom_bodyid)
-    body1, body2 = geom_bodyid[c.geom1], geom_bodyid[c.geom2]
-    diff = support.jac_dif_pair(m, d, c.pos, body1, body2)
-    t = m.body_invweight0[body1, 0] + m.body_invweight0[body2, 0]
-
-    # rotate Jacobian differences to contact frame
-    diff_con = c.frame @ diff.T
-
-    # TODO(robotics-simulation): add support for other friction dimensions
-    # 4 pyramidal friction directions
-    js, invweights = [], []
-    for diff_tan, friction in zip(diff_con[1:], c.friction[:2]):
-      for f in (friction, -friction):
-        js.append(diff_con[0] + diff_tan * f)
-        invweights.append((t + f * f * t) * 2 * f * f / m.opt.impratio)
-
-    active = dist < 0
-    j, invweight = jp.stack(js) * active, jp.stack(invweights)
-    pos = jp.repeat(dist, 4) * active
-    solref, solimp = jp.tile(c.solref, (4, 1)), jp.tile(c.solimp, (4, 1))
-
-    return j, invweight, pos, solref, solimp
-
-  res = fn(d.contact)
-  # remove contact grouping dimension:
-  j, invweight, pos, solref, solimp = jax.tree_map(jp.concatenate, res)
+  def contact_efc(c: Contact, condim: int):
+
+    @jax.vmap
+    def fn(c: Contact):
+      dist = c.dist - c.includemargin
+      active = dist < 0
+      body1, body2 = jp.array(m.geom_bodyid)[c.geom]
+      jac1p, jac1r = support.jac(m, d, c.pos, body1)
+      jac2p, jac2r = support.jac(m, d, c.pos, body2)
+      diff = c.frame @ (jac2p - jac1p).T
+      if condim > 3:  # only calculate rotational diff if needed
+        diff = jp.concatenate((diff, c.frame @ (jac2r - jac1r).T), axis=0)
+      tran = m.body_invweight0[body1, 0] + m.body_invweight0[body2, 0]
+
+      if condim == 1:
+        return diff[0] * active, tran, dist * active, c.solref, c.solimp
+
+      # a pair of opposing pyramid edges per friction dimension
+      # repeat friction directions with positive and negative sign
+      fri = jp.repeat(c.friction[: condim - 1], 2, axis=0).at[1::2].mul(-1)
+      # repeat condims of jacdiff to match +/- friction directions
+      j = diff[0] + jp.repeat(diff[1:condim], 2, axis=0) * fri[:, None]
+      # pyramidal has common invweight across all edges
+      diag_approx = tran + fri[0] * fri[0] * tran
+      inv_w = diag_approx * 2 * fri[0] * fri[0] / m.opt.impratio
+      repeat_fn = lambda x: jp.repeat(x[None], (condim - 1) * 2, axis=0)
+      inv_w, pos, solref, solimp = jax.tree_util.tree_map(
+          repeat_fn, (inv_w, dist, c.solref, c.solimp)
+      )
+      return j * active, inv_w, pos * active, solref, solimp
+
+    return fn(c)
+
+  # group efc calculations by condim
+  dims, begs = np.unique(d.contact.dim, return_index=True)
+  efcs = []
+  for i in range(len(dims)):
+    dim, beg = dims[i], begs[i]
+    end = begs[i + 1] if i < len(dims) - 1 else None
+    c = jax.tree_util.tree_map(lambda x, b=beg, e=end: x[b:e], d.contact)
+    efc = contact_efc(c, dim)
+    if dim > 1:
+      # remove efc grouping dimension
+      efc = jax.tree_util.tree_map(jp.concatenate, efc)
+    efcs.append(efc)
+
+  efc = jax.tree_util.tree_map(lambda *x: jp.concatenate(x), *efcs)
+  j, invweight, pos, solref, solimp = efc
   frictionloss = jp.zeros_like(pos)
 
   return _Efc(j, pos, pos, invweight, solref, solimp, frictionloss)
 
 
-def count_constraints(
-    m: Union[Model, mujoco.MjModel], d: Optional[Data] = None
-) -> Tuple[int, int, int, int]:
+def counts(efc_type: np.ndarray) -> Tuple[int, int, int, int]:
   """Returns equality, friction, limit, and contact constraint counts."""
+  ne = (efc_type == ConstraintType.EQUALITY).sum()
+  nf = 0  # no support for friction loss yet
+  nl = (efc_type == ConstraintType.LIMIT_JOINT).sum()
+  nc_f = (efc_type == ConstraintType.CONTACT_FRICTIONLESS).sum()
+  nc_p = (efc_type == ConstraintType.CONTACT_PYRAMIDAL).sum()
+  nc = nc_f + nc_p
+
+  return ne, nf, nl, nc
+
+
+def make_efc_type(
+    m: Union[Model, mujoco.MjModel], dim: Optional[np.ndarray] = None
+) -> np.ndarray:
+  """Returns efc_type that outlines the type of each constraint row."""
   if m.opt.disableflags & DisableBit.CONSTRAINT:
-    return 0, 0, 0, 0
+    return np.empty(0, dtype=int)
 
-  if m.opt.disableflags & DisableBit.EQUALITY:
-    ne = 0
-  else:
-    ne_connect = (m.eq_type == EqType.CONNECT).sum()
-    ne_weld = (m.eq_type == EqType.WELD).sum()
-    ne_joint = (m.eq_type == EqType.JOINT).sum()
-    ne = ne_connect * 3 + ne_weld * 6 + ne_joint
+  dim = collision_driver.make_condim(m) if dim is None else dim
+  efc_types = []
 
-  nf = 0
+  if not m.opt.disableflags & DisableBit.EQUALITY:
+    num_rows = (m.eq_type == EqType.CONNECT).sum() * 3
+    num_rows += (m.eq_type == EqType.WELD).sum() * 6
+    num_rows += (m.eq_type == EqType.JOINT).sum()
+    efc_types.extend([ConstraintType.EQUALITY] * num_rows)
 
-  if m.opt.disableflags & DisableBit.LIMIT:
-    nl = 0
-  else:
-    nl = int(m.jnt_limited.sum())
+  if not m.opt.disableflags & DisableBit.LIMIT:
+    efc_types.extend([ConstraintType.LIMIT_JOINT] * m.jnt_limited.sum())
 
-  if d is None:
-    nc = collision_driver.ncon(m) * 4
-  else:
-    nc = d.efc_J.shape[-2] - ne - nf - nl
+  if not m.opt.disableflags & DisableBit.CONTACT:
+    num_rows = sum(_CONDIM_EFC_COUNT[d] for d in dim)
+    efc_types.extend([ConstraintType.CONTACT_PYRAMIDAL] * num_rows)
 
-  return ne, nf, nl, nc
+  return np.array(efc_types)
+
+
+def make_efc_address(efc_type: np.ndarray, dim: np.ndarray) -> np.ndarray:
+  """Returns efc_address that maps contacts to constraint row address."""
+  nc = (efc_type == ConstraintType.CONTACT_PYRAMIDAL).sum()
+  nc_start = efc_type.size - nc
+  offsets = np.cumsum([0] + [_CONDIM_EFC_COUNT[d] for d in dim])[:-1]
+
+  return nc_start + offsets
 
 
 def make_constraint(m: Model, d: Data) -> Data:
   """Creates constraint jacobians and other supporting data."""
 
   if m.opt.disableflags & DisableBit.CONSTRAINT:
     efcs = ()
@@ -362,15 +402,15 @@
 
   if not efcs:
     z = jp.empty(0)
     d = d.replace(efc_J=jp.empty((0, m.nv)))
     d = d.replace(efc_D=z, efc_aref=z, efc_frictionloss=z)
     return d
 
-  efc = jax.tree_map(lambda *x: jp.concatenate(x), *efcs)
+  efc = jax.tree_util.tree_map(lambda *x: jp.concatenate(x), *efcs)
 
   @jax.vmap
   def fn(efc):
     k, b, imp = _kbi(m, efc.solref, efc.solimp, efc.pos_norm)
     r = jp.maximum(efc.invweight * (1 - imp) / imp, mujoco.mjMINVAL)
     aref = -b * (efc.J @ d.qvel) - k * imp * efc.pos
     return aref, r
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/constraint_test.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/constraint_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -44,61 +44,79 @@
     """Test constraints."""
     m = test_util.load_test_file('constraints.xml')
     d = mujoco.MjData(m)
     mujoco.mj_step(m, d, 100)  # at 100 steps mix of active/inactive constraints
     mujoco.mj_forward(m, d)
     mx = mjx.put_model(m)
     dx = mjx.put_data(m, d)
-
     dx = mjx.make_constraint(mx, dx)
-    nnz = dx.efc_J.any(axis=1)
-    _assert_eq(d.efc_J, dx.efc_J[nnz].reshape(-1), 'efc_J')
-    _assert_eq(d.efc_D, dx.efc_D[nnz], 'efc_D')
-    _assert_eq(d.efc_aref, dx.efc_aref[nnz], 'efc_aref')
-    _assert_eq(d.efc_frictionloss, dx.efc_frictionloss[nnz], 'efc_frictionloss')
+    d_efc_j = d.efc_J.reshape((-1, m.nv))
+
+    # ne, nf, nl order matches
+    efl = d.ne + d.nf + d.nl
+    _assert_eq(d_efc_j[:efl], dx.efc_J[:efl], 'efc_J')
+    _assert_eq(d.efc_D[:efl], dx.efc_D[:efl], 'efc_D')
+    _assert_eq(d.efc_aref[:efl], dx.efc_aref[:efl], 'efc_aref')
+    _assert_eq(dx.efc_frictionloss, 0, 'efc_frictionloss')
+
+    # contact order might not match, so check efcs contact by contact
+    for i in range(d.ncon):
+      geom_match = (dx.contact.geom == d.contact.geom[i]).all(axis=-1)
+      geom_match &= (dx.contact.pos == d.contact.pos[i]).all(axis=-1)
+      self.assertTrue(geom_match.any(), f'contact {i} not found in MJX contact')
+      j = np.nonzero(geom_match)[0][0]
+      self.assertEqual(d.contact.dim[i], dx.contact.dim[j])
+      nc = max(1, (d.contact.dim[i] - 1) * 2)
+      d_beg, dx_beg = d.contact.efc_address[i], dx.contact.efc_address[j]
+      d_end, dx_end = d_beg + nc, dx_beg + nc
+      _assert_eq(d_efc_j[d_beg:d_end], dx.efc_J[dx_beg:dx_end], 'efc_J')
+      _assert_eq(d.efc_D[d_beg:d_end], dx.efc_D[dx_beg:dx_end], 'efc_D')
+      d_efc_aref = d.efc_aref[d_beg:d_end]
+      dx_efc_aref = dx.efc_aref[dx_beg:dx_end]
+      _assert_eq(d_efc_aref, dx_efc_aref, 'efc_aref')
 
   def test_disable_refsafe(self):
     m = test_util.load_test_file('constraints.xml')
 
     timeconst = m.opt.timestep / 4.0  # timeconst < 2 * timestep
     solimp = jp.array([timeconst, 1.0])
     solref = jp.array([0.8, 0.99, 0.001, 0.2, 2])
     pos = jp.ones(3)
 
     m.opt.disableflags = m.opt.disableflags | mjx.DisableBit.REFSAFE
-    mx = mjx.device_put(m)
+    mx = mjx.put_model(m)
     k, *_ = constraint._kbi(mx, solimp, solref, pos)
     self.assertEqual(k, 1 / (0.99**2 * timeconst**2))
 
   def test_disable_constraint(self):
     m = test_util.load_test_file('constraints.xml')
     m.opt.disableflags = m.opt.disableflags | mjx.DisableBit.CONSTRAINT
-    ne, nf, nl, nc = mjx.count_constraints(m)
+    ne, nf, nl, nc = constraint.counts(constraint.make_efc_type(m))
     self.assertEqual(ne, 0)
     self.assertEqual(nf, 0)
     self.assertEqual(nl, 0)
     self.assertEqual(nc, 0)
     dx = constraint.make_constraint(mjx.put_model(m), mjx.make_data(m))
     self.assertEqual(dx.efc_J.shape[0], 0)
 
   def test_disable_equality(self):
     m = test_util.load_test_file('constraints.xml')
     m.opt.disableflags = m.opt.disableflags | mjx.DisableBit.EQUALITY
-    ne, nf, nl, nc = mjx.count_constraints(m)
+    ne, nf, nl, nc = constraint.counts(constraint.make_efc_type(m))
     self.assertEqual(ne, 0)
     self.assertEqual(nf, 0)
     self.assertEqual(nl, 2)
-    self.assertEqual(nc, 64)
+    self.assertEqual(nc, 148)
     dx = constraint.make_constraint(mjx.put_model(m), mjx.make_data(m))
-    self.assertEqual(dx.efc_J.shape[0], 66)  # only joint range, contact
+    self.assertEqual(dx.efc_J.shape[0], 150)  # only joint range, contact
 
   def test_disable_contact(self):
     m = test_util.load_test_file('constraints.xml')
     m.opt.disableflags = m.opt.disableflags | mjx.DisableBit.CONTACT
-    ne, nf, nl, nc = mjx.count_constraints(m)
+    ne, nf, nl, nc = constraint.counts(constraint.make_efc_type(m))
     self.assertEqual(ne, 10)
     self.assertEqual(nf, 0)
     self.assertEqual(nl, 2)
     self.assertEqual(nc, 0)
     dx = constraint.make_constraint(mjx.put_model(m), mjx.make_data(m))
     self.assertEqual(dx.efc_J.shape[0], 12)  # only joint range, limit
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/dataclasses.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/dataclasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # ==============================================================================
 """Wrapper that automatically registers dataclass as a Jax PyTree."""
 
 import copy
 import dataclasses
 
 import typing
-from typing import Any, Dict, Optional, Sequence, TypeVar, Union
+from typing import Dict, Optional, Sequence, Tuple, TypeVar, Union
 import jax
 import numpy as np
 
 _T = TypeVar('_T')
 
 
 def _jax_in_args(typ) -> bool:
@@ -118,15 +118,15 @@
     raise NotImplementedError
 
   def replace(self: TNode, **overrides) -> TNode:
     # stub for pytype
     raise NotImplementedError
 
   @classmethod
-  def fields(cls) -> tuple[dataclasses.Field[Any], ...]:
+  def fields(cls) -> Tuple[dataclasses.Field, ...]:  # pylint: disable=g-bare-generic
     return dataclasses.fields(cls)
 
   def tree_replace(
       self, params: Dict[str, Optional[jax.typing.ArrayLike]]
   ) -> 'PyTreeNode':
     new = self
     for k, v in params.items():
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/forward.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/forward.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,24 +170,25 @@
       m.actuator_forcerange,
       jp.array([-jp.inf, jp.inf]),
   )
   force = jp.clip(force, forcerange[:, 0], forcerange[:, 1])
 
   qfrc_actuator = d.actuator_moment.T @ force
 
+  if m.ngravcomp:
+    # actuator-level gravity compensation, skip if added as passive force
+    qfrc_actuator += d.qfrc_gravcomp * m.jnt_actgravcomp[m.dof_jntid]
+
   # clamp qfrc_actuator
   actfrcrange = jp.where(
       m.jnt_actfrclimited[:, None],
       m.jnt_actfrcrange,
       jp.array([-jp.inf, jp.inf]),
   )
-  ids = sum(
-      ([i] * JointType(j).dof_width() for i, j in enumerate(m.jnt_type)), []
-  )
-  actfrcrange = jp.take(actfrcrange, jp.array(ids), axis=0)
+  actfrcrange = actfrcrange[m.dof_jntid]
   qfrc_actuator = jp.clip(qfrc_actuator, actfrcrange[:, 0], actfrcrange[:, 1])
 
   d = d.replace(act_dot=act_dot, qfrc_actuator=qfrc_actuator)
   return d
 
 
 @named_scope
@@ -306,23 +307,23 @@
   A, B = _RK4_A, _RK4_B
   C = jp.tril(A).sum(axis=0)  # C(i) = sum_j A(i,j)
   T = d.time + C * m.opt.timestep
   # pylint: enable=invalid-name
 
   kqvel = d.qvel  # intermediate RK solution
   # RK solutions sum
-  qvel, qacc, act_dot = jax.tree_map(
+  qvel, qacc, act_dot = jax.tree_util.tree_map(
       lambda k: B[0] * k, (kqvel, d.qacc, d.act_dot)
   )
   integrate_fn = lambda *args: _integrate_pos(*args, dt=m.opt.timestep)
 
   def f(carry, x):
     qvel, qacc, act_dot, kqvel, d = carry
     a, b, t = x  # tableau numbers
-    dqvel, dqacc, dact_dot = jax.tree_map(
+    dqvel, dqacc, dact_dot = jax.tree_util.tree_map(
         lambda k: a * k, (kqvel, d.qacc, d.act_dot)
     )
     # get intermediate RK solutions
     kqpos = scan.flat(m, integrate_fn, 'jqv', 'q', m.jnt_type, d_t0.qpos, dqvel)
     kact = d_t0.act + dact_dot * m.opt.timestep
     kqvel = d_t0.qvel + dqacc * m.opt.timestep
     d = d.replace(qpos=kqpos, qvel=kqvel, act=kact, time=t)
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/forward_test.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/forward_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/io.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/io.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,23 +18,22 @@
 from typing import List, Union
 
 import jax
 from jax import numpy as jp
 import mujoco
 from mujoco.mjx._src import collision_driver
 from mujoco.mjx._src import constraint
-from mujoco.mjx._src import mesh
 from mujoco.mjx._src import support
 from mujoco.mjx._src import types
 import numpy as np
 import scipy
 
 
-def _put_option(o: mujoco.MjOption, device=None) -> types.Option:
-  """Puts mujoco.MjOption onto a device, resulting in mjx.Option."""
+def _make_option(o: mujoco.MjOption) -> types.Option:
+  """Returns mjx.Option given mujoco.MjOption."""
   if o.integrator not in set(types.IntegratorType):
     raise NotImplementedError(f'{mujoco.mjtIntegrator(o.integrator)}')
 
   if o.cone not in set(types.ConeType):
     raise NotImplementedError(f'{mujoco.mjtCone(o.cone)}')
 
   if o.jacobian not in set(types.JacobianType):
@@ -43,68 +42,51 @@
   if o.solver not in set(types.SolverType):
     raise NotImplementedError(f'{mujoco.mjtSolver(o.solver)}')
 
   for i in range(mujoco.mjtEnableBit.mjNENABLE):
     if o.enableflags & 2**i:
       raise NotImplementedError(f'{mujoco.mjtEnableBit(2 ** i)}')
 
-  static_fields = {
-      f.name: copy.copy(getattr(o, f.name))
-      for f in types.Option.fields()
-      if f.type in (int, bytes, np.ndarray)
-  }
-  static_fields['integrator'] = types.IntegratorType(o.integrator)
-  static_fields['cone'] = types.ConeType(o.cone)
-  static_fields['jacobian'] = types.JacobianType(o.jacobian)
-  static_fields['solver'] = types.SolverType(o.solver)
-  static_fields['disableflags'] = types.DisableBit(o.disableflags)
-
-  device_fields = {
-      f.name: copy.copy(getattr(o, f.name))
-      for f in types.Option.fields()
-      if f.type is jax.Array
-  }
-  device_fields = jax.device_put(device_fields, device=device)
-
-  has_fluid_params = o.density > 0 or o.viscosity > 0 or o.wind.any()
-
-  return types.Option(
-      has_fluid_params=has_fluid_params,
-      **static_fields,
-      **device_fields,
-  )
+  fields = {f.name: getattr(o, f.name, None) for f in types.Option.fields()}
+  fields['integrator'] = types.IntegratorType(o.integrator)
+  fields['cone'] = types.ConeType(o.cone)
+  fields['jacobian'] = types.JacobianType(o.jacobian)
+  fields['solver'] = types.SolverType(o.solver)
+  fields['disableflags'] = types.DisableBit(o.disableflags)
+  fields['has_fluid_params'] = o.density > 0 or o.viscosity > 0 or o.wind.any()
+
+  return types.Option(**fields)
 
 
-def _put_statistic(s: mujoco.MjStatistic, device=None) -> types.Statistic:
+def _make_statistic(s: mujoco.MjStatistic) -> types.Statistic:
   """Puts mujoco.MjStatistic onto a device, resulting in mjx.Statistic."""
-  return types.Statistic(
-      meaninertia=jax.device_put(s.meaninertia, device=device)
-  )
+  return types.Statistic(meaninertia=s.meaninertia)
 
 
 def put_model(m: mujoco.MjModel, device=None) -> types.Model:
   """Puts mujoco.MjModel onto a device, resulting in mjx.Model."""
 
   if m.ntendon:
     raise NotImplementedError('tendons are not supported')
 
-  if (m.geom_condim != 3).any() or (m.pair_dim != 3).any():
-    raise NotImplementedError('only condim=3 is supported')
-
-  # check collision geom types
-  for (g1, g2, *_), c in collision_driver.collision_candidates(m).items():
-    g1, g2 = mujoco.mjtGeom(g1), mujoco.mjtGeom(g2)
-    if collision_driver.get_collision_fn((g1, g2)) is None:
-      raise NotImplementedError(f'({g1}, {g2}) has no collision function')
-    *_, params = collision_driver.get_params(m, c)
-    margin_gap = not np.allclose(np.concatenate([params.margin, params.gap]), 0)
-    if mujoco.mjtGeom.mjGEOM_MESH in (g1, g2) and margin_gap:
-      raise NotImplementedError(
-          f'Margin and gap not implemented for ({g1}, {g2})'
-      )
+  for g1, g2, ip in collision_driver.geom_pairs(m):
+    t1, t2 = m.geom_type[[g1, g2]]
+    # check collision function exists for type pair
+    if not collision_driver.has_collision_fn(t1, t2):
+      t1, t2 = mujoco.mjtGeom(t1), mujoco.mjtGeom(t2)
+      raise NotImplementedError(f'({t1}, {t2}) collisions not implemented.')
+    # margin/gap not supported for geoms
+    if mujoco.mjtGeom.mjGEOM_MESH in (t1, t2):
+      if ip != -1:
+        margin = m.pair_margin[ip]
+      else:
+        margin = m.geom_margin[g1] + m.geom_margin[g2]
+      if margin.any():
+        t1, t2 = mujoco.mjtGeom(t1), mujoco.mjtGeom(t2)
+        raise NotImplementedError(f'({t1}, {t2}) margin/gap not implemented.')
 
   for enum_field, enum_type, mj_type in (
       (m.actuator_biastype, types.BiasType, mujoco.mjtBias),
       (m.actuator_dyntype, types.DynType, mujoco.mjtDyn),
       (m.actuator_gaintype, types.GainType, mujoco.mjtGain),
       (m.actuator_trntype, types.TrnType, mujoco.mjtTrn),
       (m.eq_type, types.EqType, mujoco.mjtEq),
@@ -114,48 +96,32 @@
       raise NotImplementedError(
           f'{[mj_type(m) for m in missing]} not supported'
       )
 
   if not np.allclose(m.dof_frictionloss, 0):
     raise NotImplementedError('dof_frictionloss is not implemented.')
 
-  opt = _put_option(m.opt, device=device)
-  stat = _put_statistic(m.stat, device=device)
+  fields = {f.name: getattr(m, f.name) for f in types.Model.fields()}
+  fields['geom_rgba'] = fields['geom_rgba'].reshape((-1, 4))
+  fields['mat_rgba'] = fields['mat_rgba'].reshape((-1, 4))
+  fields['cam_mat0'] = fields['cam_mat0'].reshape((-1, 3, 3))
+  fields['opt'] = _make_option(m.opt)
+  fields['stat'] = _make_statistic(m.stat)
+  model = types.Model(**{k: copy.copy(v) for k, v in fields.items()})
 
-  static_fields = {
-      f.name: getattr(m, f.name)
-      for f in types.Model.fields()
-      if f.type in (int, bytes, np.ndarray)
-  }
-  static_fields['geom_rgba'] = static_fields['geom_rgba'].reshape((-1, 4))
-  static_fields['mat_rgba'] = static_fields['mat_rgba'].reshape((-1, 4))
-
-  device_fields = {
-      f.name: copy.copy(getattr(m, f.name))  # copy because device_put is async
-      for f in types.Model.fields()
-      if f.type is jax.Array
-  }
-  device_fields['cam_mat0'] = device_fields['cam_mat0'].reshape((-1, 3, 3))
-  device_fields.update(mesh.get(m))
-  device_fields = jax.device_put(device_fields, device=device)
-
-  return types.Model(
-      opt=opt,
-      stat=stat,
-      **static_fields,
-      **device_fields,
-  )
+  return jax.device_put(model, device=device)
 
 
 def make_data(m: Union[types.Model, mujoco.MjModel]) -> types.Data:
   """Allocate and initialize Data."""
-
-  ncon = collision_driver.ncon(m)
-  ne, nf, nl, nc = constraint.count_constraints(m)
-  nefc = ne + nf + nl + nc
+  dim = collision_driver.make_condim(m)
+  efc_type = constraint.make_efc_type(m, dim)
+  efc_address = constraint.make_efc_address(efc_type, dim)
+  ne, nf, nl, nc = constraint.counts(efc_type)
+  ncon, nefc = dim.size, ne + nf + nl + nc
 
   zero_0 = jp.zeros(0, dtype=float)
   zero_nv = jp.zeros(m.nv, dtype=float)
   zero_nv_6 = jp.zeros((m.nv, 6), dtype=float)
   zero_nv_nv = jp.zeros((m.nv, m.nv), dtype=float)
   zero_nbody_3 = jp.zeros((m.nbody, 3), dtype=float)
   zero_nbody_6 = jp.zeros((m.nbody, 6), dtype=float)
@@ -163,16 +129,36 @@
   zero_nbody_3_3 = jp.zeros((m.nbody, 3, 3), dtype=float)
   zero_nefc = jp.zeros(nefc, dtype=float)
   zero_na = jp.zeros(m.na, dtype=float)
   zero_nu = jp.zeros(m.nu, dtype=float)
   zero_njnt_3 = jp.zeros((m.njnt, 3), dtype=float)
   zero_nm = jp.zeros(m.nM, dtype=float)
 
-  # create first d to get num contacts and nc
+  contact = types.Contact(
+      dist=jp.zeros(ncon),
+      pos=jp.zeros((ncon, 3)),
+      frame=jp.zeros((ncon, 3, 3)),
+      includemargin=jp.zeros(ncon),
+      friction=jp.zeros((ncon, 5)),
+      solref=jp.zeros((ncon, mujoco.mjNREF)),
+      solreffriction=jp.zeros((ncon, mujoco.mjNREF)),
+      solimp=jp.zeros((ncon, mujoco.mjNIMP)),
+      dim=dim,
+      geom1=jp.zeros(ncon, dtype=int) - 1,
+      geom2=jp.zeros(ncon, dtype=int) - 1,
+      geom=jp.zeros((ncon, 2), dtype=int) - 1,
+      efc_address=efc_address,
+  )
+
   d = types.Data(
+      ne=ne,
+      nf=nf,
+      nl=nl,
+      nefc=nefc,
+      ncon=ncon,
       solver_niter=jp.array(0, dtype=int),
       time=jp.array(0.0),
       qpos=jp.array(m.qpos0),
       qvel=zero_nv,
       act=zero_na,
       qacc_warmstart=zero_nv,
       ctrl=zero_nu,
@@ -199,53 +185,47 @@
       cinert=zero_nbody_10,
       actuator_length=zero_nu,
       actuator_moment=jp.zeros((m.nu, m.nv), dtype=float),
       crb=zero_nbody_10,
       qM=zero_nm if support.is_sparse(m) else zero_nv_nv,
       qLD=zero_nm if support.is_sparse(m) else zero_nv_nv,
       qLDiagInv=zero_nv if support.is_sparse(m) else zero_0,
-      contact=types.Contact.zero(ncon),
+      contact=contact,
+      efc_type=efc_type,
       efc_J=jp.zeros((nefc, m.nv), dtype=float),
       efc_frictionloss=zero_nefc,
       efc_D=zero_nefc,
       actuator_velocity=zero_nu,
       cvel=zero_nbody_6,
       cdof_dot=zero_nv_6,
       qfrc_bias=zero_nv,
+      qfrc_gravcomp=zero_nv,
       qfrc_passive=zero_nv,
       efc_aref=zero_nefc,
       qfrc_actuator=zero_nv,
       qfrc_smooth=zero_nv,
       qacc_smooth=zero_nv,
       qfrc_constraint=zero_nv,
       qfrc_inverse=zero_nv,
       efc_force=zero_nefc,
       userdata=jp.zeros(m.nuserdata, dtype=float),
   )
 
   return d
 
 
-def _get_contact(
-    c: mujoco._structs._MjContactList,
-    cx: types.Contact,
-    efc_start: int,
-):
+def _get_contact(c: mujoco._structs._MjContactList, cx: types.Contact):
   """Converts mjx.Contact to mujoco._structs._MjContactList."""
   con_id = np.nonzero(cx.dist <= 0)[0]
   for field in types.Contact.fields():
     value = getattr(cx, field.name)[con_id]
     if field.name == 'frame':
       value = value.reshape((-1, 9))
     getattr(c, field.name)[:] = value
 
-  ncon = cx.dist.shape[0]
-  c.efc_address[:] = np.arange(efc_start, efc_start + ncon * 4, 4)[con_id]
-  c.dim[:] = 3
-
 
 def get_data(
     m: mujoco.MjModel, d: types.Data
 ) -> Union[mujoco.MjData, List[mujoco.MjData]]:
   """Gets mjx.Data from a device, resulting in mujoco.MjData or List[MjData]."""
   batched = len(d.qpos.shape) > 1
   batch_size = d.qpos.shape[0] if batched else 1
@@ -271,118 +251,123 @@
     raise ValueError('dst is a list, but d is not batched.')
   if not batched and len(d.qpos.shape) >= 2:
     raise ValueError('dst is a an MjData, but d is batched.')
 
   d = jax.device_get(d)
 
   batch_size = d.qpos.shape[0] if batched else 1
-  ne, nf, nl, nc = constraint.count_constraints(m, d)
-  efc_type = np.array([
-      mujoco.mjtConstraint.mjCNSTR_EQUALITY,
-      mujoco.mjtConstraint.mjCNSTR_FRICTION_DOF,
-      mujoco.mjtConstraint.mjCNSTR_LIMIT_JOINT,
-      mujoco.mjtConstraint.mjCNSTR_CONTACT_PYRAMIDAL,
-  ]).repeat([ne, nf, nl, nc])
 
   dof_i, dof_j = [], []
   for i in range(m.nv):
     j = i
     while j > -1:
       dof_i.append(i)
       dof_j.append(j)
       j = m.dof_parentid[j]
 
   for i in range(batch_size):
-    d_i = jax.tree_map(lambda x, i=i: x[i], d) if batched else d
+    d_i = jax.tree_util.tree_map(lambda x, i=i: x[i], d) if batched else d
     result_i = result[i] if batched else result
     ncon = (d_i.contact.dist <= 0).sum()
     efc_active = (d_i.efc_J != 0).any(axis=1)
-    efc_con = efc_type == mujoco.mjtConstraint.mjCNSTR_CONTACT_PYRAMIDAL
-    nefc, nc = int(efc_active.sum()), int((efc_active & efc_con).sum())
+    nefc = int(efc_active.sum())
     result_i.nnzJ = nefc * m.nv
     if ncon != result_i.ncon or nefc != result_i.nefc:
       mujoco._functions._realloc_con_efc(result_i, ncon=ncon, nefc=nefc)  # pylint: disable=protected-access
     result_i.efc_J_rownnz[:] = np.repeat(m.nv, nefc)
     result_i.efc_J_rowadr[:] = np.arange(0, nefc * m.nv, m.nv)
     result_i.efc_J_colind[:] = np.tile(np.arange(m.nv), nefc)
 
     for field in types.Data.fields():
       if field.name == 'contact':
-        _get_contact(result_i.contact, d_i.contact, nefc - nc)
+        _get_contact(result_i.contact, d_i.contact)
+        # efc_address must be updated because rows were deleted above:
+        efc_map = np.cumsum(efc_active) - 1
+        result_i.contact.efc_address[:] = efc_map[result_i.contact.efc_address]
         continue
 
       value = getattr(d_i, field.name)
 
-      if field.name in ('xmat', 'ximat', 'geom_xmat', 'site_xmat', 'cam_xmat'):
+      if field.name in ('nefc', 'ncon'):
+        value = {'nefc': nefc, 'ncon': ncon}[field.name]
+      elif field.name.endswith('xmat') or field.name == 'ximat':
         value = value.reshape((-1, 9))
-
-      if field.name in ('efc_frictionloss', 'efc_D', 'efc_aref', 'efc_force'):
+      elif field.name.startswith('efc_'):
         value = value[efc_active]
-
-      if field.name == 'efc_J':
-        value = value[efc_active].reshape(-1)
-
-      if field.name == 'qM' and not support.is_sparse(m):
+        if field.name == 'efc_J':
+          value = value.reshape(-1)
+      elif field.name == 'qM' and not support.is_sparse(m):
         value = value[dof_i, dof_j]
-
-      if field.name == 'qLD' and not support.is_sparse(m):
+      elif field.name == 'qLD' and not support.is_sparse(m):
         value = value[dof_i, dof_j]
-
-      if field.name == 'qLDiagInv' and not support.is_sparse(m):
+      elif field.name == 'qLDiagInv' and not support.is_sparse(m):
         value = np.ones(m.nv)
 
-      if value.shape:
+      if isinstance(value, np.ndarray) and value.shape:
         getattr(result_i, field.name)[:] = value
       else:
         setattr(result_i, field.name, value)
 
-    result_i.efc_type[:] = efc_type[efc_active]
 
-
-def _put_contact(
-    c: mujoco._structs._MjContactList, ncon: int, device=None
+def _make_contact(
+    c: mujoco._structs._MjContactList,
+    dim: np.ndarray,
+    efc_address: np.ndarray,
 ) -> types.Contact:
-  """Puts mujoco.structs._MjContactList onto a device, resulting in mjx.Contact."""
-  fields = {
-      f.name: copy.copy(getattr(c, f.name)) for f in types.Contact.fields()
-  }
+  """Converts mujoco.structs._MjContactList into mjx.Contact."""
+  fields = {f.name: getattr(c, f.name) for f in types.Contact.fields()}
   fields['frame'] = fields['frame'].reshape((-1, 3, 3))
-  pad_size = ncon - c.dist.shape[0]
-  pad_fn = lambda x: np.concatenate(
-      (x, np.zeros((pad_size,) + x.shape[1:], dtype=x.dtype))
-  )
-  fields = jax.tree_map(pad_fn, fields)
-  fields['dist'][-pad_size:] = np.inf
-  fields = jax.device_put(fields, device=device)
+  # reorder contacts so that their condims match those specified in dim.
+  # if we have fewer Contacts for a condim range, pad the range with zeros
+
+  # build a map for where to find a dim-matching contact, or -1 if none
+  contact_map = np.zeros_like(dim) - 1
+  for i, di in enumerate(fields['dim']):
+    space = [j for j, dj in enumerate(dim) if di == dj and contact_map[j] == -1]
+    if not space:
+      # this can happen if max_geom_pairs or max_contact_points is too low
+      raise ValueError(f'unable to place Contact[{i}], no space in condim {di}')
+    contact_map[space[0]] = i
+
+  if contact_map.size > 0:
+    # reorganize contact according, with a zero contact at the end for -1
+    zero = jax.tree_util.tree_map(
+        lambda x: np.zeros((1,) + x.shape[1:], dtype=x.dtype), fields
+    )
+    zero['dist'][:] = np.finfo(float).max
+    fields = jax.tree_util.tree_map(lambda *x: np.concatenate(x), fields, zero)
+    fields = jax.tree_util.tree_map(lambda x: x[contact_map], fields)
+
+  fields['dim'] = dim
+  fields['efc_address'] = efc_address
 
   return types.Contact(**fields)
 
 
 def put_data(m: mujoco.MjModel, d: mujoco.MjData, device=None) -> types.Data:
   """Puts mujoco.MjData onto a device, resulting in mjx.Data."""
-  ncon = collision_driver.ncon(m)
-  ne, nf, nl, nc = constraint.count_constraints(m)
-  nefc = ne + nf + nl + nc
+  dim = collision_driver.make_condim(m)
+  efc_type = constraint.make_efc_type(m, dim)
+  efc_address = constraint.make_efc_address(efc_type, dim)
+  ne, nf, nl, nc = constraint.counts(efc_type)
+  ncon, nefc = dim.size, ne + nf + nl + nc
 
   for d_val, val, name in (
       (d.ncon, ncon, 'ncon'),
       (d.ne, ne, 'ne'),
       (d.nf, nf, 'nf'),
       (d.nl, nl, 'nl'),
       (d.nefc, nefc, 'nefc'),
   ):
     if d_val > val:
       raise ValueError(f'd.{name} too high, d.{name} = {d_val}, model = {val}')
 
-  fields = {
-      f.name: copy.copy(getattr(d, f.name))  # copy because device_put is async
-      for f in types.Data.fields()
-      if f.type is jax.Array
-  }
+  fields = {f.name: getattr(d, f.name) for f in types.Data.fields()}
 
+  # MJX prefers square matrices for these fields:
   for fname in ('xmat', 'ximat', 'geom_xmat', 'site_xmat', 'cam_xmat'):
     fields[fname] = fields[fname].reshape((-1, 3, 3))
 
   # MJX does not support islanding, so only transfer the first solver_niter
   fields['solver_niter'] = fields['solver_niter'][0]
 
   # pad efc fields: MuJoCo efc arrays are sparse for inactive constraints.
@@ -402,26 +387,29 @@
 
   for fname in ('efc_J', 'efc_frictionloss', 'efc_D', 'efc_aref', 'efc_force'):
     value = np.zeros((nefc, m.nv)) if fname == 'efc_J' else np.zeros(nefc)
     for i in range(4):
       value_beg = sum([ne, nf, nl][:i])
       d_beg = sum([d.ne, d.nf, d.nl][:i])
       size = [d.ne, d.nf, d.nl, d.nefc - d.nl - d.nf - d.ne][i]
-      value[value_beg:value_beg+size] = fields[fname][d_beg:d_beg+size]
+      value[value_beg : value_beg + size] = fields[fname][d_beg : d_beg + size]
     fields[fname] = value
 
   # convert qM and qLD if jacobian is dense
   if not support.is_sparse(m):
     fields['qM'] = np.zeros((m.nv, m.nv))
     mujoco.mj_fullM(m, fields['qM'], d.qM)
     # TODO(erikfrey): derive L*L' from L'*D*L instead of recomputing
     try:
       fields['qLD'], _ = scipy.linalg.cho_factor(fields['qM'])
     except scipy.linalg.LinAlgError:
       # this happens when qM is empty or unstable simulation
       fields['qLD'] = np.zeros((m.nv, m.nv))
     fields['qLDiagInv'] = np.zeros(0)
 
-  fields = jax.device_put(fields, device=device)
-  fields['contact'] = _put_contact(d.contact, ncon, device=device)
+  fields['contact'] = _make_contact(d.contact, dim, efc_address)
+  fields.update(ne=ne, nf=nf, nl=nl, nefc=nefc, ncon=ncon, efc_type=efc_type)
+
+  # copy because device_put is async:
+  data = types.Data(**{k: copy.copy(v) for k, v in fields.items()})
 
-  return types.Data(**fields)
+  return jax.device_put(data, device=device)
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/io_test.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/io_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     </actuator>
   </mujoco>
 """
 
 _MULTIPLE_CONSTRAINTS = """
   <mujoco>
     <worldbody>
-      <geom type="plane" size="3 3 .01"/>
+      <geom type="plane" size="3 3 .01" condim="6"/>
       <body name="cap1" pos="-.3 -.3 .2">
         <freejoint/>
         <geom type="capsule" size=".2 .05"/>
         <body name="cap2" pos=".6 -.3 .3">
           <joint axis="0 1 0" type="hinge" range="-45 45"/>
           <joint axis="1 0 0" type="hinge" range="-0.001 0.001"/>
           <geom type="capsule" size=".2 .05"/>
@@ -104,18 +104,14 @@
     self.assertAlmostEqual(mx.opt.timestep, m.opt.timestep)
 
     np.testing.assert_allclose(mx.body_parentid, m.body_parentid)
     np.testing.assert_allclose(mx.geom_type, m.geom_type)
     np.testing.assert_allclose(mx.geom_bodyid, m.geom_bodyid)
     np.testing.assert_almost_equal(mx.geom_solref, m.geom_solref)
     np.testing.assert_almost_equal(mx.geom_pos, m.geom_pos)
-    self.assertLen(mx.geom_convex_face, 6)
-    self.assertLen(mx.geom_convex_vert, 6)
-    self.assertLen(mx.geom_convex_edge_dir, 6)
-    self.assertLen(mx.geom_convex_facenormal, 6)
 
     np.testing.assert_allclose(mx.jnt_type, m.jnt_type)
     np.testing.assert_allclose(mx.jnt_dofadr, m.jnt_dofadr)
     np.testing.assert_allclose(mx.jnt_bodyid, m.jnt_bodyid)
     np.testing.assert_allclose(mx.jnt_limited, m.jnt_limited)
     np.testing.assert_almost_equal(mx.jnt_axis, m.jnt_axis)
 
@@ -173,30 +169,14 @@
           <tendon>
             <fixed>
               <joint coef="1" joint="left_hip"/>
             </fixed>
           </tendon>
         </mujoco>"""))
 
-  def test_condim_not_implemented(self):
-    with self.assertRaises(NotImplementedError):
-      mjx.put_model(mujoco.MjModel.from_xml_string("""
-        <mujoco>
-          <worldbody>
-            <body>
-              <freejoint/>
-              <geom size="0.05" condim="1"/>
-            </body>
-            <body>
-              <freejoint/>
-              <geom size="0.05" condim="1"/>
-            </body>
-          </worldbody>
-        </mujoco>"""))
-
   def test_cylinder_not_implemented(self):
     with self.assertRaises(NotImplementedError):
       mjx.put_model(mujoco.MjModel.from_xml_string("""
         <mujoco>
           <worldbody>
             <body>
               <freejoint/>
@@ -240,14 +220,15 @@
 
     nq = 22
     nbody = 5
     ncon = 46
     nv = 19
     nefc = 185
 
+    self.assertEqual(d.nefc, nefc)
     self.assertEqual(d.qpos.shape, (nq,))
     self.assertEqual(d.qvel.shape, (nv,))
     self.assertEqual(d.act.shape, (0,))
     self.assertEqual(d.qacc_warmstart.shape, (nv,))
     self.assertEqual(d.ctrl.shape, (1,))
     self.assertEqual(d.qfrc_applied.shape, (nv,))
     self.assertEqual(d.xfrc_applied.shape, (nbody, 6))
@@ -332,29 +313,29 @@
     self.assertEqual(dx.site_xmat.shape, (1, 3, 3))
     np.testing.assert_allclose(dx.xmat.reshape((3, 9)), d.xmat)
     np.testing.assert_allclose(dx.ximat.reshape((3, 9)), d.ximat)
     np.testing.assert_allclose(dx.geom_xmat.reshape((3, 9)), d.geom_xmat)
     np.testing.assert_allclose(dx.site_xmat.reshape((1, 9)), d.site_xmat)
 
     # efc_ are also shape transformed and padded
-    self.assertEqual(dx.efc_J.shape, (21, 8))  # nefc, nv
+    self.assertEqual(dx.efc_J.shape, (45, 8))  # nefc, nv
     d_efc_j = d.efc_J.reshape((-1, 8))
     np.testing.assert_allclose(dx.efc_J[:3], d_efc_j[:3])  # connect eq
     np.testing.assert_allclose(dx.efc_J[3], d_efc_j[3])  # one active limit
     np.testing.assert_allclose(dx.efc_J[4], 0)  # one inactive limit
-    np.testing.assert_allclose(dx.efc_J[5:9], d_efc_j[4:8])  # contact
-    np.testing.assert_allclose(dx.efc_J[9:], 0)  # no contact
+    np.testing.assert_allclose(dx.efc_J[5:15], d_efc_j[4:14])  # contact
+    np.testing.assert_allclose(dx.efc_J[15:], 0)  # no contact
 
     # check another efc_ too
-    self.assertEqual(dx.efc_aref.shape, (21,))  # nefc
+    self.assertEqual(dx.efc_aref.shape, (45,))  # nefc
     np.testing.assert_allclose(dx.efc_aref[:3], d.efc_aref[:3])
     np.testing.assert_allclose(dx.efc_aref[3], d.efc_aref[3])
     np.testing.assert_allclose(dx.efc_aref[4], 0)
-    np.testing.assert_allclose(dx.efc_aref[5:9], d.efc_aref[4:8])
-    np.testing.assert_allclose(dx.efc_aref[9:], 0)
+    np.testing.assert_allclose(dx.efc_aref[5:15], d.efc_aref[4:14])
+    np.testing.assert_allclose(dx.efc_aref[15:], 0)
 
     # check sparse transform is correct
     m.opt.jacobian = mujoco.mjtJacobian.mjJAC_SPARSE
     d = mujoco.MjData(m)
     mujoco.mj_step(m, d, 2)
     dx_sparse = mjx.put_data(m, d)
     np.testing.assert_allclose(dx_sparse.efc_J, dx.efc_J, atol=1e-8)
@@ -403,31 +384,30 @@
     self.assertEqual(d_2.site_xmat.shape, (1, 9))
     np.testing.assert_allclose(d_2.xmat, d.xmat)
     np.testing.assert_allclose(d_2.ximat, d.ximat)
     np.testing.assert_allclose(d_2.geom_xmat, d.geom_xmat)
     np.testing.assert_allclose(d_2.site_xmat, d.site_xmat)
 
     # efc_* are also shape transformed and filtered
-    self.assertEqual(d_2.efc_J.shape, (64,))  # nefc * nv
+    self.assertEqual(d_2.nefc, 14)
+    self.assertEqual(d_2.efc_J.shape, (112,))  # nefc * nv
     np.testing.assert_allclose(d_2.efc_J, d.efc_J)
-    self.assertEqual(d_2.efc_aref.shape, (8,))  # nefc
+    self.assertEqual(d_2.efc_aref.shape, (14,))  # nefc
     np.testing.assert_allclose(d_2.efc_aref, d.efc_aref)
-
-    # efc_address is created on demand
     np.testing.assert_allclose(d_2.contact.efc_address, d.contact.efc_address)
 
   def test_get_data_batched(self):
     """Test that get_data makes correct List[MjData] for batched Data."""
 
     m = mujoco.MjModel.from_xml_string(_MULTIPLE_CONSTRAINTS)
     d = mujoco.MjData(m)
     mujoco.mj_step(m, d, 2)
     dx = mjx.put_data(m, d)
     # second data in batch has contact dist > 0, disables contact
-    dx_b = jax.tree_map(lambda x: jp.stack((x, x + 0.05)), dx)
+    dx_b = jax.tree_util.tree_map(lambda x: jp.stack((x, x + 0.05)), dx)
     ds = mjx.get_data(m, dx_b)
     self.assertLen(ds, 2)
     np.testing.assert_allclose(ds[0].qpos, d.qpos)
     np.testing.assert_allclose(ds[1].qpos, d.qpos + 0.05, atol=1e-8)
     self.assertEqual(ds[0].ncon, 1)
     self.assertEqual(ds[1].ncon, 0)
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/math.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/math.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/math_test.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/math_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/mesh.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/mesh.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,60 +11,31 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Mesh processing."""
 
 import collections
-import dataclasses
 import itertools
-from typing import Dict, List, Optional, Sequence, Tuple
+from typing import Tuple
 import warnings
 
-import mujoco
+import jax
+from jax import numpy as jp
 # pylint: disable=g-importing-member
-from mujoco.mjx._src.types import GeomType
+from mujoco.mjx._src.collision_types import ConvexInfo
+from mujoco.mjx._src.collision_types import GeomInfo
 from mujoco.mjx._src.types import Model
 # pylint: enable=g-importing-member
 import numpy as np
 from scipy import spatial
 import trimesh
 
 
-_BOX_CORNERS = list(itertools.product((-1, 1), (-1, 1), (-1, 1)))
-# pyformat: disable
-# Rectangular box faces using a counter-clockwise winding order convention.
-_BOX_FACES = [
-    0, 4, 5, 1,  # left
-    0, 2, 6, 4,  # bottom
-    6, 7, 5, 4,  # front
-    2, 3, 7, 6,  # right
-    1, 5, 7, 3,  # top
-    0, 1, 3, 2,  # back
-]
-# pyformat: enable
 _MAX_HULL_FACE_VERTICES = 20
-_CONVEX_CACHE: Dict[Tuple[int, int], Dict[str, np.ndarray]] = {}
-_DERIVED_ARGS = [
-    'geom_convex_face',
-    'geom_convex_vert',
-    'geom_convex_edge_dir',
-    'geom_convex_facenormal',
-    'geom_convex_edge',
-    'geom_convex_edge_face_normal',
-]
-DERIVED = {(Model, d) for d in _DERIVED_ARGS}
-
-
-def _box(size: np.ndarray):
-  """Creates a mesh for a box with rectangular faces."""
-  box_corners = np.array(_BOX_CORNERS)
-  vert = box_corners * size.reshape(-1, 3)
-  face = np.array([_BOX_FACES]).reshape(-1, 4)
-  return vert, face
 
 
 def _get_face_norm(vert: np.ndarray, face: np.ndarray) -> np.ndarray:
   """Calculates face normals given vertices and face indexes."""
   assert len(vert.shape) == 2 and len(face.shape) == 2, (
       f'vert and face should have dim of 2, got {len(vert.shape)} and '
       f'{len(face.shape)}'
@@ -166,24 +137,15 @@
   order_ *= np.where(best_axis == 1, -1, 1)
   hull_point_idx = c.vertices[::order_]
   assert (axis_points - c.points).sum() == 0
 
   return hull_point_idx
 
 
-@dataclasses.dataclass
-class MeshInfo:
-  name: str
-  vert: np.ndarray
-  face: np.ndarray
-  convex_vert: Optional[np.ndarray]
-  convex_face: Optional[np.ndarray]
-
-
-def _merge_coplanar(tm: trimesh.Trimesh, mesh_info: MeshInfo) -> np.ndarray:
+def _merge_coplanar(m: Model, tm: trimesh.Trimesh, meshid: int) -> np.ndarray:
   """Merges coplanar facets."""
   if not tm.facets:
     return tm.faces.copy()  # no facets
   if not tm.faces.shape[0]:
     raise ValueError('Mesh has no faces.')
 
   # Get faces.
@@ -200,17 +162,19 @@
 
     # convert triangulated facet to a polygon
     hull_point_idx = _convex_hull_2d(points, normal)
     face = point_idx[hull_point_idx]
 
     # resize faces that exceed max polygon vertices
     if face.shape[0] > _MAX_HULL_FACE_VERTICES:
+      name = m.names[m.name_meshadr[meshid]:]
+      name = name[:name.find(b'\x00')].decode('utf-8')
       warnings.warn(
-          f'Mesh "{mesh_info.name}" has a coplanar face with more than'
-          f' {_MAX_HULL_FACE_VERTICES} vertices. This may lead to performance '
+          f'Mesh "{name}" has a coplanar face with more than '
+          f'{_MAX_HULL_FACE_VERTICES} vertices. This may lead to performance '
           'issues and inaccuracies in collision detection. Consider '
           'decimating the mesh.'
       )
     every = face.shape[0] // _MAX_HULL_FACE_VERTICES + 1
     face = face[::every]
     facets.append(face)
 
@@ -227,110 +191,103 @@
     return np.array(facets)  # no faces, return facets
 
   # Merge faces and facets.
   faces = np.pad(faces, ((0, 0), (0, max_len - faces.shape[1])), 'edge')
   return np.concatenate([faces, facets])
 
 
-def _mesh_info(
-    m: mujoco.MjModel,
-) -> List[MeshInfo]:
-  """Extracts mesh info from MjModel."""
-  mesh_infos = []
-  for i in range(m.nmesh):
-    name = mujoco.mj_id2name(m, mujoco.mjtObj.mjOBJ_MESH.value, i)
-
-    last = (i + 1) >= m.nmesh
-    face_start = m.mesh_faceadr[i]
-    face_end = m.mesh_faceadr[i + 1] if not last else m.mesh_face.shape[0]
-    face = m.mesh_face[face_start:face_end]
-
-    vert_start = m.mesh_vertadr[i]
-    vert_end = m.mesh_vertadr[i + 1] if not last else m.mesh_vert.shape[0]
-    vert = m.mesh_vert[vert_start:vert_end]
-
-    graphadr = m.mesh_graphadr[i]
-    if graphadr < 0:
-      mesh_infos.append(MeshInfo(name, vert, face, None, None))
-      continue
-
-    graph = m.mesh_graph[graphadr:]
-    numvert, numface = graph[0], graph[1]
-
-    # unused vert_edgeadr
-    # vert_edgeadr = graph[2 : numvert + 2]
-    last_idx = numvert + 2
-
-    vert_globalid = graph[last_idx : last_idx + numvert]
-    last_idx += numvert
+def box(info: GeomInfo) -> ConvexInfo:
+  """Creates a box with rectangular faces."""
+  vert = np.array(
+      list(itertools.product((-1, 1), (-1, 1), (-1, 1))), dtype=float
+  )
+  # pyformat: disable
+  # rectangular box faces using a counter-clockwise winding order convention:
+  face = np.array(
+      [
+          0, 4, 5, 1,  # left
+          0, 2, 6, 4,  # bottom
+          6, 7, 5, 4,  # front
+          2, 3, 7, 6,  # right
+          1, 5, 7, 3,  # top
+          0, 1, 3, 2,  # back
+      ]
+  ).reshape((-1, 4))
+  # pyformat: enable
+  face_normal = _get_face_norm(vert, face)
+  edge, edge_face_normal = _get_edge_normals(face, face_normal)
+  edge_dir = _get_unique_edge_dir(vert, face)
+  face = vert[face]  # materialize full nface x nvert matrix
+
+  c = ConvexInfo(
+      info.pos,
+      info.mat,
+      vert,
+      face,
+      face_normal,
+      edge,
+      edge_face_normal,
+      edge_dir,
+  )
+  c = jax.tree_util.tree_map(jp.array, c)
+  vert = jax.vmap(jp.multiply, in_axes=(None, 0))(c.vert, info.size)
+  face = jax.vmap(jp.multiply, in_axes=(None, 0))(c.face, info.size)
+  c = c.replace(vert=vert, face=face)
 
-    # unused edge_localid
-    # edge_localid = graph[last_idx : last_idx + numvert + 3 * numface]
-    last_idx += numvert + 3 * numface
+  return c
 
-    face_globalid = graph[last_idx : last_idx + 3 * numface]
-    face_globalid = face_globalid.reshape((numface, 3))
 
-    convex_vert = vert[vert_globalid]
-    vertex_map = dict(zip(vert_globalid, np.arange(vert_globalid.shape[0])))
-    convex_face = np.vectorize(vertex_map.get)(face_globalid)
-    mesh_infos.append(MeshInfo(name, vert, face, convex_vert, convex_face))
+def convex(m: Model, mesh_id: int, info: GeomInfo) -> ConvexInfo:
+  """Processes a mesh for use in convex collision algorithms.
 
-  return mesh_infos
+  Args:
+    m: an MJX model
+    mesh_id: the mesh id to process
+    info: pos, mat, size of this geom
 
+  Returns:
+    a convex mesh info
+  """
+  vert_beg = m.mesh_vertadr[mesh_id]
+  vert_end = m.mesh_vertadr[mesh_id + 1] if mesh_id < m.nmesh - 1 else None
+  vert = m.mesh_vert[vert_beg:vert_end]
+
+  graphadr = m.mesh_graphadr[mesh_id]
+  graph = m.mesh_graph[graphadr:]
+  graph_idx = 0
+
+  numvert, numface = graph[0], graph[1]
+  graph_idx += 2
+
+  # skip vert_edgeadr  (numvert,)
+  graph_idx += numvert
+  vert_globalid = graph[graph_idx : graph_idx + numvert]
+  graph_idx += numvert
+
+  # skip edge_localid  (numvert, 3)
+  graph_idx += numvert + 3 * numface
+  face_globalid = graph[graph_idx : graph_idx + 3 * numface].reshape((-1, 3))
+
+  vert = vert[vert_globalid]
+  vertex_map = dict(zip(vert_globalid, np.arange(vert_globalid.shape[0])))
+  face = np.vectorize(vertex_map.get)(face_globalid)
 
-def _geom_mesh_kwargs(
-    mesh_info: MeshInfo,
-) -> Dict[str, np.ndarray]:
-  """Generates convex mesh attributes for mjx.Model."""
-  tm_convex = trimesh.Trimesh(
-      vertices=mesh_info.convex_vert, faces=mesh_info.convex_face
-  )
+  tm_convex = trimesh.Trimesh(vertices=vert, faces=face)
   vert = np.array(tm_convex.vertices)
-  face = _merge_coplanar(tm_convex, mesh_info)
-  facenormal = _get_face_norm(vert, face)
-  edge, edge_face_normal = _get_edge_normals(face, facenormal)
-  return {
-      'geom_convex_face': vert[face],
-      'geom_convex_face_vert_idx': face,
-      'geom_convex_vert': vert,
-      'geom_convex_edge_dir': _get_unique_edge_dir(vert, face),
-      'geom_convex_facenormal': facenormal,
-      'geom_convex_edge': edge,
-      'geom_convex_edge_face_normal': edge_face_normal,
-  }
-
-
-def get(m: mujoco.MjModel) -> Dict[str, Sequence[Optional[np.ndarray]]]:
-  """Derives geom mesh attributes for mjx.Model from MjModel."""
-  kwargs = {k: [] for k in _DERIVED_ARGS}
-  mesh_infos = _mesh_info(m)
-  geom_con = m.geom_conaffinity | m.geom_contype
-  for geomid in range(m.ngeom):
-    mesh_info = None
-    dataid = m.geom_dataid[geomid]
-    if not geom_con[geomid]:
-      # ignore visual-only meshes
-      kwargs = {k: kwargs[k] + [None] for k in _DERIVED_ARGS}
-      continue
-    elif m.geom_type[geomid] == GeomType.BOX:
-      vert, face = _box(m.geom_size[geomid])
-      mesh_info = MeshInfo(
-          name='box',
-          vert=vert,
-          face=face,
-          convex_vert=vert,
-          convex_face=face,
-      )
-    elif dataid < 0:
-      kwargs = {k: kwargs[k] + [None] for k in _DERIVED_ARGS}
-      continue
-
-    mesh_info = mesh_info or mesh_infos[dataid]
-    vert, face = mesh_info.vert, mesh_info.face
-    key = (hash(vert.data.tobytes()), hash(face.data.tobytes()))
-    if key not in _CONVEX_CACHE:
-      _CONVEX_CACHE[key] = _geom_mesh_kwargs(mesh_info)
-
-    kwargs = {k: kwargs[k] + [_CONVEX_CACHE[key][k]] for k in _DERIVED_ARGS}
+  face = _merge_coplanar(m, tm_convex, mesh_id)
+  face_normal = _get_face_norm(vert, face)
+  edge, edge_face_normal = _get_edge_normals(face, face_normal)
+  edge_dir = _get_unique_edge_dir(vert, face)
+  face = vert[face]  # materialize full nface x nvert matrix
+
+  c = ConvexInfo(
+      info.pos,
+      info.mat,
+      vert,
+      face,
+      face_normal,
+      edge,
+      edge_face_normal,
+      edge_dir,
+  )
 
-  return kwargs
+  return jax.tree_util.tree_map(jp.array, c)
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/mesh_test.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/mesh_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from absl.testing import absltest
 from mujoco.mjx._src import mesh
 import numpy as np
 import trimesh
 
 
-class GeomMeshKwargsTest(absltest.TestCase):
+class MeshTest(absltest.TestCase):
 
   def test_pyramid(self):
     """Tests that a triangulated pyramid converts to merged coplanar faces."""
     vert = np.array([
         [-0.025, 0.05, 0.05],
         [-0.025, -0.05, -0.05],
         [-0.025, -0.05, 0.05],
@@ -33,58 +33,52 @@
     ])
     face = np.array(
         [[0, 1, 2], [0, 3, 1], [0, 4, 3], [0, 2, 4], [2, 1, 4], [1, 3, 4]]
     )
     tm = trimesh.Trimesh(vertices=vert, faces=face)
     tm_convex = trimesh.convex.convex_hull(tm)
     convex_vert = np.array(tm_convex.vertices)
-    convex_face = np.array(tm_convex.faces)
-    mesh_info = mesh.MeshInfo(
-        name='test',
-        vert=vert,
-        face=face,
-        convex_vert=convex_vert,
-        convex_face=convex_face,
-    )
-    h = mesh._geom_mesh_kwargs(mesh_info)
+    convex_face = mesh._merge_coplanar(None, tm_convex, 0)
 
     # get index of vertices in h['geom_convex_vert'] for vertices in vert
     dist = np.repeat(vert, vert.shape[0], axis=0) - np.tile(
-        h['geom_convex_vert'], (vert.shape[0], 1)
+        convex_vert, (vert.shape[0], 1)
     )
     dist = (dist**2).sum(axis=1).reshape((vert.shape[0], -1))
     vidx = np.argmin(dist, axis=0)
 
     # check verts
-    np.testing.assert_array_equal(h['geom_convex_vert'], vert[vidx])
+    np.testing.assert_array_equal(convex_vert, vert[vidx])
 
     # check face vertices
     map_ = {v: k for k, v in enumerate(vidx)}
-    h_face = np.vectorize(map_.get)(h['geom_convex_face_vert_idx'])
+    h_face = np.vectorize(map_.get)(convex_face)
     face_verts = sorted([tuple(sorted(set(s))) for s in h_face.tolist()])
     expected_face_verts = sorted([
         (0, 3, 4), (1, 3, 4), (0, 2, 4), (0, 1, 2, 3), (1, 2, 4)])
     self.assertSequenceEqual(
         face_verts,
         expected_face_verts,
     )
 
     # check edges
-    unique_edge = np.vectorize(map_.get)(h['geom_convex_edge_dir'])
+    edge_dir = mesh._get_unique_edge_dir(convex_vert, convex_face)
+    unique_edge = np.vectorize(map_.get)(edge_dir)
     unique_edge = np.array(sorted(unique_edge.tolist()))
     np.testing.assert_array_equal(
         unique_edge,
         np.array([[0, 2], [0, 3], [0, 4], [1, 4], [2, 4], [3, 4]]),
     )
 
     # face normals
-    self.assertEqual(h['geom_convex_facenormal'].shape, (5, 3))
+    face_normal = mesh._get_face_norm(convex_vert, convex_face)
+    self.assertEqual(face_normal.shape, (5, 3))
 
     # face edges
-    edges = h['geom_convex_edge']
+    edges, edge_normal = mesh._get_edge_normals(convex_face, face_normal)
     edges = np.vectorize(map_.get)(edges)
     mask = edges[:, 0] != edges[:, 1]
     edges = edges[mask]
     sort_col_idx = np.argsort(edges, axis=1)
     edges = np.take_along_axis(edges, sort_col_idx, axis=1)
     sort_row_idx = np.lexsort((edges[:, 1], edges[:, 0]))
     edges = edges[sort_row_idx]
@@ -99,15 +93,14 @@
             [1, 4],
             [2, 4],
             [3, 4],
         ]),
     )
 
     # face edge normals
-    edge_normal = h['geom_convex_edge_face_normal']
     edge_normal = edge_normal[mask]
     edge_normal = np.take_along_axis(
         edge_normal, sort_col_idx[..., None], axis=1
     )
     edge_normal = edge_normal[sort_row_idx]
     edge_normal_02 = np.array([[0.4472136, -0.0, 0.89442719], [-1.0, 0.0, 0.0]])
     np.testing.assert_array_almost_equal(
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/passive.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/passive.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,14 +25,108 @@
 from mujoco.mjx._src.types import Data
 from mujoco.mjx._src.types import DisableBit
 from mujoco.mjx._src.types import JointType
 from mujoco.mjx._src.types import Model
 # pylint: enable=g-importing-member
 
 
+def _spring_damper(m: Model, d: Data) -> jax.Array:
+  """Applies joint level spring and damping forces."""
+  def fn(jnt_typs, stiffness, qpos_spring, qpos):
+    qpos_i = 0
+    qfrcs = []
+    for i in range(len(jnt_typs)):
+      jnt_typ = JointType(jnt_typs[i])
+      q = qpos[qpos_i : qpos_i + jnt_typ.qpos_width()]
+      qs = qpos_spring[qpos_i : qpos_i + jnt_typ.qpos_width()]
+      qfrc = jp.zeros(jnt_typ.dof_width())
+      if jnt_typ == JointType.FREE:
+        qfrc = qfrc.at[:3].set(-stiffness[i] * (q[:3] - qs[:3]))
+        qfrc = qfrc.at[3:6].set(-stiffness[i] * math.quat_sub(q[3:7], qs[3:7]))
+      elif jnt_typ == JointType.BALL:
+        qfrc = -stiffness[i] * math.quat_sub(q, qs)
+      elif jnt_typ in (
+          JointType.SLIDE,
+          JointType.HINGE,
+      ):
+        qfrc = -stiffness[i] * (q - qs)
+      else:
+        raise RuntimeError(f'unrecognized joint type: {jnt_typ}')
+      qfrcs.append(qfrc)
+      qpos_i += jnt_typ.qpos_width()
+    return jp.concatenate(qfrcs)
+
+  # dof-level springs
+  qfrc = scan.flat(
+      m,
+      fn,
+      'jjqq',
+      'v',
+      m.jnt_type,
+      m.jnt_stiffness,
+      m.qpos_spring,
+      d.qpos,
+  )
+
+  # dof-level dampers
+  qfrc -= m.dof_damping * d.qvel
+
+  return qfrc
+
+
+def _gravcomp(m: Model, d: Data) -> jax.Array:
+  """Applies body-level gravity compensation."""
+  force = -m.opt.gravity * (m.body_mass * m.body_gravcomp)[:, None]
+
+  apply_f = lambda f, pos, body_id: support.jac(m, d, pos, body_id)[0] @ f
+  qfrc = jax.vmap(apply_f)(force, d.xipos, jp.arange(m.nbody)).sum(axis=0)
+
+  return qfrc
+
+
+def _fluid(m: Model, d: Data) -> jax.Array:
+  """Applies body-level viscosity, lift and drag."""
+  force, torque = jax.vmap(
+      _inertia_box_fluid_model, in_axes=(None, 0, 0, 0, 0, 0, 0)
+  )(
+      m,
+      m.body_inertia,
+      m.body_mass,
+      d.subtree_com[jp.array(m.body_rootid)],
+      d.xipos,
+      d.ximat,
+      d.cvel,
+  )
+  qfrc = jax.vmap(support.apply_ft, in_axes=(None, None, 0, 0, 0, 0))(
+      m, d, force, torque, d.xipos, jp.arange(m.nbody)
+  )
+
+  return jp.sum(qfrc, axis=0)
+
+
+def passive(m: Model, d: Data) -> Data:
+  """Adds all passive forces."""
+  if m.opt.disableflags & DisableBit.PASSIVE:
+    return d.replace(qfrc_passive=jp.zeros(m.nv), qfrc_gravcomp=jp.zeros(m.nv))
+
+  qfrc_passive = _spring_damper(m, d)
+  qfrc_gravcomp = jp.zeros(m.nv)
+
+  if m.ngravcomp and not m.opt.disableflags & DisableBit.GRAVITY:
+    qfrc_gravcomp = _gravcomp(m, d)
+    # add gravcomp unless added via actuators
+    qfrc_passive += qfrc_gravcomp * (1 - m.jnt_actgravcomp[m.dof_jntid])
+
+  if m.opt.has_fluid_params:
+    qfrc_passive += _fluid(m, d)
+
+  d = d.replace(qfrc_passive=qfrc_passive, qfrc_gravcomp=qfrc_gravcomp)
+  return d
+
+
 def _inertia_box_fluid_model(
     m: Model,
     inertia: jax.Array,
     mass: jax.Array,
     root_com: jax.Array,
     xipos: jax.Array,
     ximat: jax.Array,
@@ -67,75 +161,7 @@
       1.0 * m.opt.density * scale_ang * jp.abs(lvel[:3]) * lvel[:3] / 64.0
   )
 
   # rotate to global orientation: lfrc -> bfrc
   force, torque = ximat @ lfrc_vel, ximat @ lfrc_ang
 
   return force, torque
-
-
-def passive(m: Model, d: Data) -> Data:
-  """Adds all passive forces."""
-  if m.opt.disableflags & DisableBit.PASSIVE:
-    return d.replace(qfrc_passive=jp.zeros(m.nv))
-
-  # joint-level springs
-  def fn(jnt_typs, stiffness, qpos_spring, qpos):
-    qpos_i = 0
-    qfrcs = []
-    for i in range(len(jnt_typs)):
-      jnt_typ = JointType(jnt_typs[i])
-      q = qpos[qpos_i : qpos_i + jnt_typ.qpos_width()]
-      qs = qpos_spring[qpos_i : qpos_i + jnt_typ.qpos_width()]
-      qfrc = jp.zeros(jnt_typ.dof_width())
-      if jnt_typ == JointType.FREE:
-        qfrc = qfrc.at[:3].set(-stiffness[i] * (q[:3] - qs[:3]))
-        qfrc = qfrc.at[3:6].set(-stiffness[i] * math.quat_sub(q[3:7], qs[3:7]))
-      elif jnt_typ == JointType.BALL:
-        qfrc = -stiffness[i] * math.quat_sub(q, qs)
-      elif jnt_typ in (
-          JointType.SLIDE,
-          JointType.HINGE,
-      ):
-        qfrc = -stiffness[i] * (q - qs)
-      else:
-        raise RuntimeError(f'unrecognized joint type: {jnt_typ}')
-      qfrcs.append(qfrc)
-      qpos_i += jnt_typ.qpos_width()
-    return jp.concatenate(qfrcs)
-
-  qfrc_passive = scan.flat(
-      m,
-      fn,
-      'jjqq',
-      'v',
-      m.jnt_type,
-      m.jnt_stiffness,
-      m.qpos_spring,
-      d.qpos,
-  )
-
-  # dof-level dampers
-  qfrc_passive -= m.dof_damping * d.qvel
-
-  # TODO(robotics-simulation): body-level gravity compensation
-
-  # body-level viscosity, lift and drag
-  if m.opt.has_fluid_params:
-    force, torque = jax.vmap(
-        _inertia_box_fluid_model, in_axes=(None, 0, 0, 0, 0, 0, 0)
-    )(
-        m,
-        m.body_inertia,
-        m.body_mass,
-        d.subtree_com[jp.array(m.body_rootid)],
-        d.xipos,
-        d.ximat,
-        d.cvel,
-    )
-    qfrc_target = jax.vmap(support.apply_ft, in_axes=(None, None, 0, 0, 0, 0))(
-        m, d, force, torque, d.xipos, jp.arange(m.nbody)
-    )
-    qfrc_passive += jp.sum(qfrc_target, axis=0)
-
-  d = d.replace(qfrc_passive=qfrc_passive)
-  return d
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/passive_test.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/passive_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,40 +38,44 @@
 
 class PassiveTest(absltest.TestCase):
 
   def test_passive(self):
     m = test_util.load_test_file('pendula.xml')
     d = mujoco.MjData(m)
     # give the system a little kick to ensure we have non-identity rotations
-    d.ctrl = np.array([0.1, -0.1, 0.2, 0.3, -0.4])
+    d.ctrl = np.array([0.1, -0.1, 0.2, 0.3, -0.4, 0.5, -0.6, 0.1])
     mujoco.mj_step(m, d, 10)  # let dynamics get state significantly non-zero
     mujoco.mj_forward(m, d)
     mx = mjx.put_model(m)
 
     dx = jax.jit(mjx.passive)(mx, mjx.put_data(m, d))
     _assert_attr_eq(d, dx, 'qfrc_passive')
+    _assert_attr_eq(d, dx, 'qfrc_gravcomp')
 
     # test with fluid forces
     m.opt.density = 0.01
     mujoco.mj_forward(m, d)
     mx = mjx.put_model(m)
     dx = jax.jit(mjx.passive)(mx, mjx.put_data(m, d))
     _assert_attr_eq(d, dx, 'qfrc_passive')
+    _assert_attr_eq(d, dx, 'qfrc_gravcomp')
 
     m.opt.viscosity = 0.02
     mujoco.mj_forward(m, d)
     mx = mjx.put_model(m)
     dx = jax.jit(mjx.passive)(mx, mjx.put_data(m, d))
     _assert_attr_eq(d, dx, 'qfrc_passive')
+    _assert_attr_eq(d, dx, 'qfrc_gravcomp')
 
     m.opt.wind = np.array([0.03, 0.04, 0.05])
     mujoco.mj_forward(m, d)
     mx = mjx.put_model(m)
     dx = jax.jit(mjx.passive)(mx, mjx.put_data(m, d))
     _assert_attr_eq(d, dx, 'qfrc_passive')
+    _assert_attr_eq(d, dx, 'qfrc_gravcomp')
 
     # test disable passive
     mx = mx.tree_replace({'opt.disableflags': mjx.DisableBit.PASSIVE})
     dx = jax.jit(mjx.passive)(mx, mjx.put_data(m, d))
     np.testing.assert_allclose(dx.qfrc_passive, 0)
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/ray.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/ray.py`

 * *Files 6% similar despite different names*

```diff
@@ -130,81 +130,72 @@
   return jp.min(jp.where(valid, x, jp.inf))
 
 
 def _ray_triangle(
     vert: jax.Array,
     pnt: jax.Array,
     vec: jax.Array,
-    b0: jax.Array,
-    b1: jax.Array,
+    basis: jax.Array,
 ) -> jax.Array:
   """Returns the distance at which a ray intersects with a triangle."""
   # project difference vectors in ray normal plane
-  planar = jp.dot(jp.array([b0, b1]), (vert - pnt).T)
+  planar = jp.dot(vert - pnt, basis)
 
   # determine if origin is inside planar projection of triangle
   # A = (p0-p2, p1-p2), b = -p2, solve A*t = b
-  A = jp.array(  # pylint: disable=invalid-name
-      [planar[:, 0] - planar[:, 2], planar[:, 1] - planar[:, 2]]
-  ).T.flatten()
-  b = -planar[:, 2]
-  det = A[0] * A[3] - A[1] * A[2]
-  valid = jp.abs(det) >= mujoco.mjMINVAL
-
-  t0 = (A[3] * b[0] - A[1] * b[1]) / det
-  t1 = (-A[2] * b[0] + A[0] * b[1]) / det
-  valid &= (t0 >= 0) & (t1 >= 0) & (t0 + t1 <= 1)
+  A = planar[0:2] - planar[2]  # pylint: disable=invalid-name
+  b = -planar[2]
+  det = A[0, 0] * A[1, 1] - A[1, 0] * A[0, 1]
+
+  t0 = (A[1, 1] * b[0] - A[1, 0] * b[1]) / det
+  t1 = (-A[0, 1] * b[0] + A[0, 0] * b[1]) / det
+  valid = (t0 >= 0) & (t1 >= 0) & (t0 + t1 <= 1)
 
   # intersect ray with plane of triangle
   nrm = jp.cross(vert[0] - vert[2], vert[1] - vert[2])
-  denom = jp.dot(vec, nrm)
-  valid &= jp.abs(denom) >= mujoco.mjMINVAL
-
-  dist = jp.where(valid, -jp.dot(pnt - vert[2], nrm) / denom, jp.inf)
+  dist = jp.dot(vert[2] - pnt, nrm) / jp.dot(vec, nrm)
+  valid &= dist >= 0
+  dist = jp.where(valid, dist, jp.inf)
 
   return dist
 
 
 def _ray_mesh(
     m: Model,
     geom_id: np.ndarray,
     unused_size: jax.Array,
     pnt: jax.Array,
     vec: jax.Array,
 ) -> Tuple[jax.Array, jax.Array]:
   """Returns the best distance and geom_id for ray mesh intersections."""
   data_id = m.geom_dataid[geom_id]
 
-  ray_basis = lambda x: math.orthogonals(math.normalize(x))
-  b0, b1 = jax.vmap(ray_basis)(vec)
+  ray_basis = lambda x: jp.array(math.orthogonals(math.normalize(x))).T
+  basis = jax.vmap(ray_basis)(vec)
 
   faceadr = np.append(m.mesh_faceadr, m.nmeshface)
   vertadr = np.append(m.mesh_vertadr, m.nmeshvert)
 
-  dists = []
+  dists, geom_ids = [], []
   for i, id_ in enumerate(data_id):
     face = m.mesh_face[faceadr[id_] : faceadr[id_ + 1]]
     vert = m.mesh_vert[vertadr[id_] : vertadr[id_ + 1]]
-    dist = jax.vmap(_ray_triangle, in_axes=(0, None, None, None, None))(
-        vert[face], pnt[i], vec[i], b0[i], b1[i]
+    vert = jp.array(vert[face])
+    dist = jax.vmap(_ray_triangle, in_axes=(0, None, None, None))(
+        vert, pnt[i], vec[i], basis[i]
     )
     dists.append(dist)
-
-  # map the triangle id to data id
-  tri_id = np.append(0, (faceadr[data_id + 1] - faceadr[data_id]).cumsum())
-  tri_data_id = np.zeros(tri_id[-1], dtype=np.int32)
-  tri_data_id[tri_id[:-1]] = 1
-  tri_data_id = tri_data_id.cumsum() - 1
+    geom_ids.append(np.repeat(geom_id[i], dist.size))
 
   dists = jp.concatenate(dists)
   min_id = jp.argmin(dists)
   # Grab the best distance amongst all meshes, bypassing the argmin in `ray`.
   # This avoids having to compute the best distance per mesh.
   dist = dists[min_id, None]
-  id_ = jp.array(geom_id)[jp.array(tri_data_id)[min_id], None]
+  id_ = jp.array(np.concatenate(geom_ids))[min_id, None]
 
   return dist, id_
 
 
 _RAY_FUNC = {
     GeomType.PLANE: _ray_plane,
     GeomType.SPHERE: _ray_sphere,
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/ray_test.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/ray_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,34 +148,32 @@
     """Tests MJX ray<>mesh matches MuJoCo."""
     m = test_util.load_test_file('ray.xml')
     d = mujoco.MjData(m)
     mujoco.mj_forward(m, d)
     mx, dx = mjx.put_model(m), mjx.put_data(m, d)
 
     # look at the tetrahedron
-    pnt, vec = jp.array([2.0, 2.0, 2.0]), -jp.array([
-        1.0,
-        1.0,
-        1.0,
-    ])
+    pnt, vec = jp.array([2.0, 2.0, 2.0]), -jp.array([1.0, 1.0, 1.0])
     vec /= jp.linalg.norm(vec)
     dist, geomid = jax.jit(mjx.ray)(mx, dx, pnt, vec)
     _assert_eq(geomid, 4, 'geom_id')
 
     pnt, vec, geomid = np.array(pnt), np.array(vec), np.zeros(1, dtype=np.int32)
     mj_dist = mujoco.mj_ray(m, d, pnt, vec, None, 1, -1, geomid)
     _assert_eq(geomid, 4, 'geom_id')
     _assert_eq(dist, mj_dist, 'dist-tetrahedron')
 
+    # look away from the dodecahedron
+    pnt, vec = jp.array([4.0, 2.0, 2.0]), jp.array([2.0, 1.0, 1.0])
+    vec /= jp.linalg.norm(vec)
+    _, geomid = jax.jit(mjx.ray)(mx, dx, pnt, vec)
+    _assert_eq(geomid, -1, 'geom_id')
+
     # look at the dodecahedron
-    pnt, vec = jp.array([4.0, 2.0, 2.0]), -jp.array([
-        2.0,
-        1.0,
-        1.0,
-    ])
+    pnt, vec = jp.array([4.0, 2.0, 2.0]), -jp.array([2.0, 1.0, 1.0])
     vec /= jp.linalg.norm(vec)
     dist, geomid = jax.jit(mjx.ray)(mx, dx, pnt, vec)
     _assert_eq(geomid, 5, 'geom_id')
 
     pnt, vec, geomid = np.array(pnt), np.array(vec), np.zeros(1, dtype=np.int32)
     mj_dist = mujoco.mj_ray(m, d, pnt, vec, None, 1, -1, geomid)
     _assert_eq(geomid, 5, 'geom_id')
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/scan.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         and (idx > 0).all()
     ):
       x = x[idx[0] : idx[-1] + 1]
     else:
       x = x.take(jp.array(idx), axis=0, mode='wrap')
     return x
 
-  return jax.tree_map(take, obj)
+  return jax.tree_util.tree_map(take, obj)
 
 
 def _q_bodyid(m: Model) -> np.ndarray:
   """Returns the bodyid for each qpos adress."""
   q_bodyids = [np.array([], dtype=np.int32)]
   for jnt_type, jnt_bodyid in zip(m.jnt_type, m.jnt_bodyid):
     width = {JointType.FREE: 7, JointType.BALL: 4}.get(jnt_type, 1)
@@ -116,15 +116,15 @@
       raise RuntimeError(f'numpy arg elements do not match: {arg}')
 
   # split out numpy and jax args
   np_args = [a[0] if isinstance(a, np.ndarray) else None for a in args]
   args = [a if n is None else None for n, a in zip(np_args, args)]
 
   # remove empty args that we should not vmap over
-  args = jax.tree_map(lambda a: a if a.shape[0] else None, args)
+  args = jax.tree_util.tree_map(lambda a: a if a.shape[0] else None, args)
   in_axes = [None if a is None else 0 for a in args]
 
   def outer_f(*args, np_args=np_args):
     args = [a if n is None else n for n, a in zip(args, np_args)]
     return f(*args)
 
   return jax.vmap(outer_f, in_axes=in_axes)(*args)
@@ -318,15 +318,15 @@
   f_ret_is_seq = isinstance(ys[0], (list, tuple))
   ys = ys if f_ret_is_seq else [[y] for y in ys]
   flat_ = {'j': 'b', 'u': 'uaj', 'c': 'c'}[group_by]
   ys = [
       [v if typ in flat_ else jp.concatenate(v) for v, typ in zip(y, out_types)]
       for y in ys
   ]
-  ys = jax.tree_map(lambda *x: jp.concatenate(x), *ys)
+  ys = jax.tree_util.tree_map(lambda *x: jp.concatenate(x), *ys)
 
   # put concatenated results back in order
   reordered_ys = []
   for i, (y, typ) in enumerate(zip(ys, out_types)):
     _check_output(y, order[typ], typ, i)
     ids = np.concatenate([np.hstack(v[typ]) for _, v in key_typ_ids])
     input_order = order[typ][np.where(order[typ] != -1)]
@@ -461,39 +461,39 @@
         body_ids = key_body_ids[key]
         parent_ids = m.body_parentid[key_body_ids[child_key]]
         id_map = _index(body_ids, parent_ids)
 
         def index_sum(x, i=id_map, s=body_ids.size):
           return jax.ops.segment_sum(x, i, s)
 
-        y = jax.tree_map(index_sum, y)
-        carry = y if carry is None else jax.tree_map(jp.add, carry, y)
+        y = jax.tree_util.tree_map(index_sum, y)
+        carry = y if carry is None else jax.tree_util.tree_map(jp.add, carry, y)
     elif key in key_parents:
       ys = [key_y[p] for p in key_parents[key]]
-      y = jax.tree_map(lambda *x: jp.concatenate(x), *ys)
+      y = jax.tree_util.tree_map(lambda *x: jp.concatenate(x), *ys)
       body_ids = np.concatenate([key_body_ids[p] for p in key_parents[key]])
       parent_ids = m.body_parentid[key_body_ids[key]]
       take_fn = lambda x, i=_index(body_ids, parent_ids): _take(x, i)
-      carry = jax.tree_map(take_fn, y)
+      carry = jax.tree_util.tree_map(take_fn, y)
 
     f_args = [_take(arg, ids) for arg, ids in zip(args, key_in_take[key])]
     key_y[key] = _nvmap(f, carry, *f_args)
 
   # slice None results from the final output
   keys = [k for k in keys if key_y[k] is not None]
 
   # concatenate ys, drop grouping dimensions, put back in order
   y = []
   for i, typ in enumerate(out_types):
     y_typ = [key_y[key] for key in keys]
     if len(out_types) > 1:
       y_typ = [y_[i] for y_ in y_typ]
     if typ != 'b':
-      y_typ = jax.tree_map(jp.concatenate, y_typ)
-    y_typ = jax.tree_map(lambda *x: jp.concatenate(x), *y_typ)
+      y_typ = jax.tree_util.tree_map(jp.concatenate, y_typ)
+    y_typ = jax.tree_util.tree_map(lambda *x: jp.concatenate(x), *y_typ)
     y_take = np.argsort(np.concatenate([key_y_take[key][i] for key in keys]))
     _check_output(y_typ, y_take, typ, i)
     y.append(_take(y_typ, y_take))
 
   y = y[0] if len(out_types) == 1 else y
 
   return y
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/scan_test.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/scan_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,29 +51,29 @@
   def test_flat_empty(self):
     """Test scanning over just world body."""
     m = mujoco.MjModel.from_xml_string("""
       <mujoco model="world_body">
         <worldbody/>
       </mujoco>
     """)
-    m = mjx.device_put(m)
+    m = mjx.put_model(m)
 
     def fn(body_id):
       return body_id + 1
 
     b_in = jp.array([1])
     b_expect = jp.array([2])
     b_out = scan.flat(m, fn, 'b', 'b', b_in)
 
     np.testing.assert_equal(np.array(b_out), np.array(b_expect))
 
   def test_flat_joints(self):
     """Tests scanning over bodies with joints of different types."""
     m = mujoco.MjModel.from_xml_string(self._MULTI_DOF_XML)
-    m = mjx.device_put(m)
+    m = mjx.put_model(m)
 
     # we will test two functions:
     #   1) j_fn receives jnt_types as a jp array
     #   2) s_fn receives jnt_types as a static np array and can switch on it
     j_fn = lambda jnt_pos, val: val + jp.sum(jnt_pos)
     s_fn = lambda jnt_types, val: val + sum(jnt_types)
 
@@ -101,15 +101,15 @@
       return val + sum(jnt_types)
     v_in = jp.ones((m.nv, 1))
     scan.flat(m, no_world, 'jv', 'v', m.jnt_type, v_in)
 
   def test_body_tree(self):
     """Tests tree scanning over bodies with different joint counts."""
     m = mujoco.MjModel.from_xml_string(self._MULTI_DOF_XML)
-    m = mjx.device_put(m)
+    m = mjx.put_model(m)
 
     # we will test two functions:
     #   1) j_fn receives jnt_pos which is a jp array
     #   2) s_fn receives jnt_types which is a static np array
     def j_fn(carry, jnt_pos, val):
       carry = jp.zeros_like(val) if carry is None else carry
       return carry + val + jp.sum(jnt_pos)
@@ -192,15 +192,15 @@
       </actuator>
     </mujoco>
   """
 
   def test_scan_actuators(self):
     """Tests scanning over actuators."""
     m = mujoco.MjModel.from_xml_string(self._MULTI_ACT_XML)
-    m = mjx.device_put(m)
+    m = mjx.put_model(m)
 
     fn = lambda *args: args
     args = (
         m.actuator_gear,
         m.jnt_type,
         jp.arange(m.nq),
         jp.arange(m.nv),
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/smooth.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/smooth.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/smooth_test.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/smooth_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/solver.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/solver.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 # ==============================================================================
 """Constraint solvers."""
 
 import jax
 from jax import numpy as jp
 import mujoco
-from mujoco.mjx._src import constraint
 from mujoco.mjx._src import math
 from mujoco.mjx._src import smooth
 from mujoco.mjx._src import support
 # pylint: disable=g-importing-member
 from mujoco.mjx._src.dataclasses import PyTreeNode
 from mujoco.mjx._src.types import Data
 from mujoco.mjx._src.types import DisableBit
@@ -77,15 +76,15 @@
         Mgrad=nv_0,
         search=nv_0,
         gauss=0.0,
         cost=jp.inf,
         prev_cost=0.0,
         solver_niter=0,
     )
-    ctx = _update_constraint(m, d, ctx)
+    ctx = _update_constraint(d, ctx)
     if grad:
       ctx = _update_gradient(m, d, ctx)
       ctx = ctx.replace(search=-ctx.Mgrad)  # start with preconditioned gradient
 
     return ctx
 
 
@@ -103,27 +102,26 @@
   cost: jax.Array
   deriv_0: jax.Array
   deriv_1: jax.Array
 
   @classmethod
   def create(
       cls,
-      m: Model,
+      d: Data,
       ctx: _Context,
       alpha: jax.Array,
       jv: jax.Array,
       quad: jax.Array,
       quad_gauss: jax.Array,
   ) -> '_LSPoint':
     """Creates a linesearch point with first and second derivatives."""
     # roughly corresponds to CGEval in mujoco/src/engine/engine_solver.c
 
     # TODO(robotics-team): change this to support friction constraints
-    ne, nf, *_ = constraint.count_constraints(m)
-    active = ((ctx.Jaref + alpha * jv) < 0).at[:ne + nf].set(True)
+    active = ((ctx.Jaref + alpha * jv) < 0).at[:d.ne + d.nf].set(True)
     quad = jax.vmap(jp.multiply)(quad, active)  # only active
     quad_total = quad_gauss + jp.sum(quad, axis=0)
 
     cost = alpha * alpha * quad_total[2] + alpha * quad_total[1] + quad_total[0]
     deriv_0 = 2 * alpha * quad_total[2] + quad_total[1]
     deriv_1 = 2 * quad_total[2] + (quad_total[2] == 0) * mujoco.mjMINVAL
     return _LSPoint(alpha=alpha, cost=cost, deriv_0=deriv_0, deriv_1=deriv_1)
@@ -157,32 +155,30 @@
     # When cond is met, we start doing no-ops.
     return jax.lax.cond(cond, _iter, lambda x: (x, False), val), it
 
   init = (init_val, cond_fun(init_val))
   return jax.lax.scan(_fun, init, None, length=max_iter)[0][0]
 
 
-def _update_constraint(m: Model, d: Data, ctx: _Context) -> _Context:
+def _update_constraint(d: Data, ctx: _Context) -> _Context:
   """Updates constraint force and resulting cost given latst solver iteration.
 
   Corresponds to CGupdateConstraint in mujoco/src/engine/engine_solver.c
 
   Args:
-    m: model defining constraints
     d: data which contains latest qacc and smooth terms
     ctx: current solver context
 
   Returns:
     context with new constraint force and costs
   """
   # TODO(robotics-team): add friction constraints
 
   # only count active constraints
-  ne, nf, *_ = constraint.count_constraints(m)
-  active = (ctx.Jaref < 0).at[:ne + nf].set(True)
+  active = (ctx.Jaref < 0).at[:d.ne + d.nf].set(True)
 
   efc_force = d.efc_D * -ctx.Jaref * active
   qfrc_constraint = d.efc_J.T @ efc_force
   gauss = 0.5 * jp.dot(ctx.Ma - d.qfrc_smooth, ctx.qacc - d.qacc_smooth)
   cost = 0.5 * jp.sum(d.efc_D * ctx.Jaref * ctx.Jaref * active) + gauss
 
   ctx = ctx.replace(
@@ -213,16 +209,15 @@
   """
 
   grad = ctx.Ma - d.qfrc_smooth - ctx.qfrc_constraint
 
   if m.opt.solver == SolverType.CG:
     mgrad = smooth.solve_m(m, d, grad)
   elif m.opt.solver == SolverType.NEWTON:
-    ne, nf, *_ = constraint.count_constraints(m)
-    active = (ctx.Jaref < 0).at[: ne + nf].set(True)
+    active = (ctx.Jaref < 0).at[: d.ne + d.nf].set(True)
     h = (d.efc_J.T * d.efc_D * active) @ d.efc_J
     h = support.full_m(m, d) + h
     h_ = jax.scipy.linalg.cho_factor(h)
     mgrad = jax.scipy.linalg.cho_solve(h_, grad)
   else:
     raise NotImplementedError(f'unsupported solver type: {m.opt.solver}')
 
@@ -258,15 +253,15 @@
       ctx.gauss,
       jp.dot(ctx.search, ctx.Ma) - jp.dot(ctx.search, d.qfrc_smooth),
       0.5 * jp.dot(ctx.search, mv),
   ))
   quad = jp.stack((0.5 * ctx.Jaref * ctx.Jaref, jv * ctx.Jaref, 0.5 * jv * jv))
   quad = (quad * d.efc_D).T
 
-  point_fn = lambda a: _LSPoint.create(m, ctx, a, jv, quad, quad_gauss)
+  point_fn = lambda a: _LSPoint.create(d, ctx, a, jv, quad, quad_gauss)
 
   def cond(ctx: _LSContext) -> jax.Array:
     done = ctx.ls_iter >= m.opt.ls_iterations
     done |= ~ctx.swap  # if we did not adjust the interval
     done |= (ctx.lo.deriv_0 < 0) & (ctx.lo.deriv_0 > -gtol)
     done |= (ctx.hi.deriv_0 > 0) & (ctx.hi.deriv_0 < gtol)
 
@@ -279,35 +274,35 @@
     hi_next = point_fn(hi.alpha - hi.deriv_0 / hi.deriv_1)
     mid = point_fn(0.5 * (lo.alpha + hi.alpha))
 
     # we swap lo/hi if:
     # 1) they are not correctly at a bracket boundary (e.g. lo.deriv_0 > 0), OR
     # 2) if moving to next or mid narrows the bracket
     swap_lo_next = (lo.deriv_0 > 0) | (lo.deriv_0 < lo_next.deriv_0)
-    lo = jax.tree_map(lambda x, y: jp.where(swap_lo_next, y, x), lo, lo_next)
+    lo = jax.tree_util.tree_map(lambda x, y: jp.where(swap_lo_next, y, x), lo, lo_next)
     swap_lo_mid = (mid.deriv_0 < 0) & (lo.deriv_0 < mid.deriv_0)
-    lo = jax.tree_map(lambda x, y: jp.where(swap_lo_mid, y, x), lo, mid)
+    lo = jax.tree_util.tree_map(lambda x, y: jp.where(swap_lo_mid, y, x), lo, mid)
 
     swap_hi_next = (hi.deriv_0 < 0) | (hi.deriv_0 > hi_next.deriv_0)
-    hi = jax.tree_map(lambda x, y: jp.where(swap_hi_next, y, x), hi, hi_next)
+    hi = jax.tree_util.tree_map(lambda x, y: jp.where(swap_hi_next, y, x), hi, hi_next)
     swap_hi_mid = (mid.deriv_0 > 0) & (hi.deriv_0 > mid.deriv_0)
-    hi = jax.tree_map(lambda x, y: jp.where(swap_hi_mid, y, x), hi, mid)
+    hi = jax.tree_util.tree_map(lambda x, y: jp.where(swap_hi_mid, y, x), hi, mid)
 
     swap = swap_lo_next | swap_lo_mid | swap_hi_next | swap_hi_mid
 
     ctx = ctx.replace(lo=lo, hi=hi, swap=swap, ls_iter=ctx.ls_iter + 1)
 
     return ctx
 
   # initialize interval
   p0 = point_fn(jp.array(0.0))
   lo = point_fn(p0.alpha - p0.deriv_0 / p0.deriv_1)
   lesser_fn = lambda x, y: jp.where(lo.deriv_0 < p0.deriv_0, x, y)
-  hi = jax.tree_map(lesser_fn, p0, lo)
-  lo = jax.tree_map(lesser_fn, lo, p0)
+  hi = jax.tree_util.tree_map(lesser_fn, p0, lo)
+  lo = jax.tree_util.tree_map(lesser_fn, lo, p0)
   ls_ctx = _LSContext(lo=lo, hi=hi, swap=jp.array(True), ls_iter=0)
   ls_ctx = _while_loop_scan(cond, body, ls_ctx, m.opt.ls_iterations)
 
   # move to new solution if improved
   lo, hi = ls_ctx.lo, ls_ctx.hi
   improved = (lo.cost < p0.cost) | (hi.cost < p0.cost)
   alpha = jp.where(lo.cost < hi.cost, lo.alpha, hi.alpha)
@@ -332,15 +327,15 @@
     done |= gradient < m.opt.tolerance
 
     return ~done
 
   def body(ctx: _Context) -> _Context:
     ctx = _linesearch(m, d, ctx)
     prev_grad, prev_Mgrad = ctx.grad, ctx.Mgrad  # pylint: disable=invalid-name
-    ctx = _update_constraint(m, d, ctx)
+    ctx = _update_constraint(d, ctx)
     ctx = _update_gradient(m, d, ctx)
 
     # polak-ribiere:
     beta = jp.dot(ctx.grad, ctx.Mgrad - prev_Mgrad)
     beta = beta / jp.maximum(mujoco.mjMINVAL, jp.dot(prev_grad, prev_Mgrad))
     beta = jp.maximum(0, beta)
     search = -ctx.Mgrad + beta * ctx.search
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/solver_test.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/solver_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/support_test.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/support_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -112,24 +112,51 @@
           d.xipos[i],
           i,
           qfrc_expected,
       )
 
     np.testing.assert_almost_equal(qfrc, qfrc_expected, 6)
 
-  def test_custom_numeric(self):
+  def test_custom(self):
     xml = """
     <mujoco model="right_shadow_hand">
         <custom>
           <numeric data="15" name="max_contact_points"/>
           <numeric data="42" name="max_geom_pairs"/>
         </custom>
     </mujoco>
     """
     m = mujoco.MjModel.from_xml_string(xml)
-    self.assertEqual(support.get_custom_numeric(m, 'something'), -1)
-    self.assertEqual(support.get_custom_numeric(m, 'max_contact_points'), 15)
-    self.assertEqual(support.get_custom_numeric(m, 'max_geom_pairs'), 42)
+
+    def _get_numeric(m, name):
+      id_ = support.name2id(m, mujoco.mjtObj.mjOBJ_NUMERIC, name)
+      return int(m.numeric_data[id_]) if id_ >= 0 else -1
+
+    self.assertEqual(_get_numeric(m, 'something'), -1)
+    self.assertEqual(_get_numeric(m, 'max_contact_points'), 15)
+    self.assertEqual(_get_numeric(m, 'max_geom_pairs'), 42)
+
+    mx = mjx.put_model(m)
+    self.assertEqual(_get_numeric(mx, 'something'), -1)
+    self.assertEqual(_get_numeric(mx, 'max_contact_points'), 15)
+    self.assertEqual(_get_numeric(mx, 'max_geom_pairs'), 42)
+
+  def test_names_and_ids(self):
+    m = test_util.load_test_file('pendula.xml')
+    mx = mjx.put_model(m)
+
+    nums = {
+        mujoco.mjtObj.mjOBJ_JOINT: m.njnt,
+        mujoco.mjtObj.mjOBJ_GEOM: m.ngeom,
+        mujoco.mjtObj.mjOBJ_BODY: m.nbody,
+    }
+
+    for obj in nums:
+      names = [mujoco.mj_id2name(m, obj.value, i) for i in range(nums[obj])]
+      for i, n in enumerate(names):
+        self.assertEqual(support.id2name(mx, obj, i), n)
+        i = i if n is not None else -1
+        self.assertEqual(support.name2id(mx, obj, n), i)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/test_util.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/test_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 """Utilities for testing."""
 
 import os
 import sys
 import time
-from typing import Dict, Tuple
+from typing import Dict, Optional, Tuple
 from xml.etree import ElementTree as ET
 
 from etils import epath
 import jax
 import mujoco
 # pylint: disable=g-importing-member
 from mujoco.mjx._src import forward
@@ -148,14 +148,15 @@
     lb, ub = -np.random.uniform(), np.random.uniform()
     joint_attr['actuatorfrcrange'] = f'{lb:.2f} {ub:.2f}'
 
   if joint_type not in ('free',):
     joint_attr['damping'] = '{:.2f}'.format(np.random.uniform() * 20)
     joint_attr['stiffness'] = '{:.2f}'.format(np.random.uniform() * 20)
 
+  joint_attr['actuatorgravcomp'] = np.random.choice(['true', 'false'])
   return joint_attr
 
 
 def _geom_solparams(
     pair: bool = False, enable_contact: bool = True
 ) -> Dict[str, str]:
   """Returns geom solver parameters."""
@@ -197,17 +198,17 @@
   attr.update(_geom_solparams(pair=False, enable_contact=enable_contact))
 
   return attr
 
 
 def _make_actuator(
     actuator_type: str,
-    joint: str | None = None,
-    site: str | None = None,
-    refsite: str | None = None,
+    joint: Optional[str] = None,
+    site: Optional[str] = None,
+    refsite: Optional[str] = None,
 ) -> Dict[str, str]:
   """Returns attributes for an actuator."""
   if joint:
     attr = {'joint': joint}
   elif site:
     attr = {'site': site}
   else:
@@ -330,15 +331,24 @@
   def make_tree(body: ET.Element, depth: int) -> None:
     if depth >= tree_depth:
       return
 
     z_pos = np.random.uniform(low=-1, high=1) * 0.01  # small jitter
     pos = f'{body_pos[0]:.3f} {body_pos[1]:.3f} {body_pos[2] + z_pos:.3f}'
     n_bodies = len(list(mjcf.iter('body')))
-    child = ET.SubElement(body, 'body', {'pos': pos, 'name': f'body{n_bodies}'})
+    gravcomp = np.random.uniform() * p(50)
+    child = ET.SubElement(
+        body,
+        'body',
+        {
+            'pos': pos,
+            'name': f'body{n_bodies}',
+            'gravcomp': f'{gravcomp:.3f}',
+        },
+    )
     ET.SubElement(child, 'site', {'name': f'site{n_bodies}'})
 
     n_joints = len(list(mjcf.iter('joint')))
     for nj in range(np.random.randint(1, max_stacked_joints + 1)):
       joint_type = np.random.choice(_JOINT_TYPES)
       if nj == 0 and depth == 0 and root_always_free:
         joint_type = 'free'
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/_src/types.py` & `mujoco_mjx-3.1.5/mujoco/mjx/_src/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,18 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Base types used in MJX."""
 
 import enum
-from typing import List, Optional
 
 import jax
-import jax.numpy as jp
 import mujoco
 from mujoco.mjx._src.dataclasses import PyTreeNode  # pylint: disable=g-importing-member
 import numpy as np
 
 
 class DisableBit(enum.IntFlag):
   """Disable default feature bitflags.
@@ -96,14 +94,15 @@
     HFIELD: height field
     SPHERE: sphere
     CAPSULE: capsule
     ELLIPSOID: ellipsoid
     CYLINDER: cylinder
     BOX: box
     MESH: mesh
+    SDF: signed distance field
   """
 
   PLANE = mujoco.mjtGeom.mjGEOM_PLANE
   HFIELD = mujoco.mjtGeom.mjGEOM_HFIELD
   SPHERE = mujoco.mjtGeom.mjGEOM_SPHERE
   CAPSULE = mujoco.mjtGeom.mjGEOM_CAPSULE
   ELLIPSOID = mujoco.mjtGeom.mjGEOM_ELLIPSOID
@@ -209,14 +208,32 @@
     AFFINE: const + kp*length + kv*velocity
   """
   NONE = mujoco.mjtBias.mjBIAS_NONE
   AFFINE = mujoco.mjtBias.mjBIAS_AFFINE
   # unsupported: MUSCLE, USER
 
 
+class ConstraintType(enum.IntEnum):
+  """Type of constraint.
+
+  Attributes:
+    EQUALITY: equality constraint
+    LIMIT_JOINT: joint limit
+    CONTACT_FRICTIONLESS: frictionless contact
+    CONTACT_PYRAMIDAL: frictional contact, pyramidal friction cone
+  """
+  EQUALITY = mujoco.mjtConstraint.mjCNSTR_EQUALITY
+  # unsupported: FRICTION_DOF, FRICTION_TENDON
+  LIMIT_JOINT = mujoco.mjtConstraint.mjCNSTR_LIMIT_JOINT
+  # unsupported: LIMIT_TENDON
+  CONTACT_FRICTIONLESS = mujoco.mjtConstraint.mjCNSTR_CONTACT_FRICTIONLESS
+  CONTACT_PYRAMIDAL = mujoco.mjtConstraint.mjCNSTR_CONTACT_PYRAMIDAL
+  # unsupported: CONTACT_ELLIPTIC
+
+
 class CamLightType(enum.IntEnum):
   """Type of camera light.
 
   Attributes:
     FIXED: pos and rot fixed in body
     TRACK: pos tracks body, rot fixed in global
     TRACKCOM: pos tracks subtree com, rot fixed in body
@@ -305,15 +322,19 @@
     nmesh: number of meshes
     nmeshvert: number of vertices in all meshes
     nmeshface: number of triangular faces in all meshes
     nmat: number of materials
     npair: number of predefined geom pairs
     nexclude: number of excluded geom pairs
     neq: number of equality constraints
+    ngravcomp: number of bodies with nonzero gravcomp
     nnumeric: number of numeric custom fields
+    ntuple: number of tuple custom fields
+    nsensor: number of sensors
+    nkey: number of keyframes
     nuserdata: size of userdata array
     nM: number of non-zeros in sparse inertia matrix
     opt: physics options
     stat: model statistics
     qpos0: qpos values at default pose                        (nq,)
     qpos_spring: reference pose for springs                   (nq,)
     body_parentid: id of body's parent                        (nbody,)
@@ -328,21 +349,24 @@
     body_pos: position offset rel. to parent body             (nbody, 3)
     body_quat: orientation offset rel. to parent body         (nbody, 4)
     body_ipos: local position of center of mass               (nbody, 3)
     body_iquat: local orientation of inertia ellipsoid        (nbody, 4)
     body_mass: mass                                           (nbody,)
     body_subtreemass: mass of subtree starting at this body   (nbody,)
     body_inertia: diagonal inertia in ipos/iquat frame        (nbody, 3)
+    body_gravcomp: antigravity force, units of body weight    (nbody,)
     body_invweight0: mean inv inert in qpos0 (trn, rot)       (nbody, 2)
     jnt_type: type of joint (mjtJoint)                        (njnt,)
     jnt_qposadr: start addr in 'qpos' for joint's data        (njnt,)
     jnt_dofadr: start addr in 'qvel' for joint's data         (njnt,)
     jnt_bodyid: id of joint's body                            (njnt,)
     jnt_group: group for visibility                           (njnt,)
     jnt_limited: does joint have limits                       (njnt,)
+    jnt_actfrclimited: does joint have actuator force limits  (njnt,)
+    jnt_actgravcomp: is gravcomp force applied via actuators  (njnt,)
     jnt_solref: constraint solver reference: limit            (njnt, mjNREF)
     jnt_solimp: constraint solver impedance: limit            (njnt, mjNIMP)
     jnt_pos: local anchor position                            (njnt, 3)
     jnt_axis: local joint axis                                (njnt, 3)
     jnt_stiffness: stiffness coefficient                      (njnt,)
     jnt_range: joint limits                                   (njnt, 2)
     jnt_actfrcrange: range of total actuator force            (njnt, 2)
@@ -367,14 +391,15 @@
     geom_group: group for visibility                          (ngeom,)
     geom_matid: material id for rendering                     (ngeom,)
     geom_priority: geom contact priority                      (ngeom,)
     geom_solmix: mixing coef for solref/imp in geom pair      (ngeom,)
     geom_solref: constraint solver reference: contact         (ngeom, mjNREF)
     geom_solimp: constraint solver impedance: contact         (ngeom, mjNIMP)
     geom_size: geom-specific size parameters                  (ngeom, 3)
+    geom_rbound: radius of bounding sphere                    (ngeom,)
     geom_pos: local position offset rel. to body              (ngeom, 3)
     geom_quat: local orientation offset rel. to body          (ngeom, 4)
     geom_friction: friction for (slide, spin, roll)           (ngeom, 3)
     geom_margin: include in solver if dist<margin-gap         (ngeom,)
     geom_gap: include in solver if dist<margin-gap            (ngeom,)
     geom_rgba: rgba when material is omitted                  (ngeom, 4)
     site_bodyid: id of site's body                            (nsite,)
@@ -384,25 +409,21 @@
     cam_bodyid:  id of camera's body                          (ncam,)
     cam_targetbodyid:  id of targeted body; -1: none          (ncam,)
     cam_pos:  position rel. to body frame                     (ncam, 3)
     cam_quat:  orientation rel. to body frame                 (ncam, 4)
     cam_poscom0:  global position rel. to sub-com in qpos0    (ncam, 3)
     cam_pos0:  global position rel. to body in qpos0          (ncam, 3)
     cam_mat0:  global orientation in qpos0                    (ncam, 9)
-    mat_rgba: rgba                                            (nmat, 4)
-    mesh_vertadr: first vertex address                        (nmesh x 1)
-    mesh_faceadr: first face address                          (nmesh x 1)
+    mesh_vertadr: first vertex address                        (nmesh,)
+    mesh_faceadr: first face address                          (nmesh,)
+    mesh_graphadr: graph data address; -1: no graph           (nmesh,)
     mesh_vert: vertex positions for all meshes                (nmeshvert, 3)
     mesh_face: vertex face data                               (nmeshface, 3)
-    geom_convex_face: vertex face data, MJX only              (ngeom,)
-    geom_convex_vert: vertex data, MJX only                   (ngeom,)
-    geom_convex_edge_dir: unique edge direction, MJX only     (ngeom,)
-    geom_convex_facenormal: normal face data, MJX only        (ngeom,)
-    geom_convex_face_edge: edges for each face                (ngeom,)
-    geom_convex_face_edge_normal: edge normals for each face  (ngeom,)
+    mesh_graph: convex graph data                             (nmeshgraph,)
+    mat_rgba: rgba                                            (nmat, 4)
     pair_dim: contact dimensionality                          (npair,)
     pair_geom1: id of geom1                                   (npair,)
     pair_geom2: id of geom2                                   (npair,)
     pair_solref: solver reference: contact normal             (npair, mjNREF)
     pair_solreffriction: solver reference: contact friction   (npair, mjNREF)
     pair_solimp: solver impedance: contact                    (npair, mjNIMP)
     pair_margin: include in solver if dist<margin-gap         (npair,)
@@ -431,15 +452,32 @@
     actuator_biasprm: bias parameters                         (nu, mjNBIAS)
     actuator_ctrlrange: range of controls                     (nu, 2)
     actuator_forcerange: range of forces                      (nu, 2)
     actuator_actrange: range of activations                   (nu, 2)
     actuator_gear: scale length and transmitted force         (nu, 6)
     numeric_adr: address of field in numeric_data             (nnumeric,)
     numeric_data: array of all numeric fields                 (nnumericdata,)
+    tuple_adr: address of text in text_data                   (ntuple,)
+    tuple_size: number of objects in tuple                    (ntuple,)
+    tuple_objtype: array of object types in all tuples        (ntupledata,)
+    tuple_objid: array of object ids in all tuples            (ntupledata,)
+    tuple_objprm: array of object params in all tuples        (ntupledata,)
+    name_bodyadr: body name pointers                          (nbody,)
+    name_jntadr: joint name pointers                          (njnt,)
+    name_geomadr: geom name pointers                          (ngeom,)
+    name_siteadr: site name pointers                          (nsite,)
+    name_camadr: camera name pointers                         (ncam,)
+    name_meshadr: mesh name pointers                          (nmesh,)
+    name_pairadr: geom pair name pointers                     (npair,)
+    name_eqadr: equality constraint name pointers             (neq,)
+    name_actuatoradr: actuator name pointers                  (nu,)
+    name_sensoradr: sensor name pointers                      (nsensor,)
     name_numericadr: numeric name pointers                    (nnumeric,)
+    name_tupleadr: tuple name pointers                        (ntuple,)
+    name_keyadr: keyframe name pointers                       (nkey,)
     names: names of all objects, 0-terminated                 (nnames,)
   """
   nq: int
   nv: int
   nu: int
   na: int
   nbody: int
@@ -450,16 +488,20 @@
   nmesh: int
   nmeshvert: int
   nmeshface: int
   nmat: int
   npair: int
   nexclude: int
   neq: int
+  ngravcomp: int
   nnumeric: int
   nuserdata: int
+  ntuple: int
+  nsensor: int
+  nkey: int
   nM: int  # pylint:disable=invalid-name
   opt: Option
   stat: Statistic
   qpos0: jax.Array
   qpos_spring: jax.Array
   body_parentid: np.ndarray
   body_rootid: np.ndarray
@@ -473,21 +515,23 @@
   body_pos: jax.Array
   body_quat: jax.Array
   body_ipos: jax.Array
   body_iquat: jax.Array
   body_mass: jax.Array
   body_subtreemass: jax.Array
   body_inertia: jax.Array
+  body_gravcomp: jax.Array
   body_invweight0: jax.Array
   jnt_type: np.ndarray
   jnt_qposadr: np.ndarray
   jnt_dofadr: np.ndarray
   jnt_bodyid: np.ndarray
   jnt_limited: np.ndarray
   jnt_actfrclimited: np.ndarray
+  jnt_actgravcomp: np.ndarray
   jnt_solref: jax.Array
   jnt_solimp: jax.Array
   jnt_pos: jax.Array
   jnt_axis: jax.Array
   jnt_stiffness: jax.Array
   jnt_range: jax.Array
   jnt_actfrcrange: jax.Array
@@ -512,14 +556,15 @@
   geom_group: np.ndarray
   geom_matid: np.ndarray
   geom_priority: np.ndarray
   geom_solmix: jax.Array
   geom_solref: jax.Array
   geom_solimp: jax.Array
   geom_size: jax.Array
+  geom_rbound: jax.Array
   geom_pos: jax.Array
   geom_quat: jax.Array
   geom_friction: jax.Array
   geom_margin: jax.Array
   geom_gap: jax.Array
   geom_rgba: np.ndarray
   site_bodyid: np.ndarray
@@ -531,26 +576,22 @@
   cam_pos: jax.Array
   cam_quat: jax.Array
   cam_poscom0: jax.Array
   cam_pos0: jax.Array
   cam_mat0: jax.Array
   mesh_vertadr: np.ndarray
   mesh_faceadr: np.ndarray
+  mesh_graphadr: np.ndarray
   mesh_vert: np.ndarray
   mesh_face: np.ndarray
+  mesh_graph: np.ndarray
   mat_rgba: np.ndarray
   pair_dim: np.ndarray
   pair_geom1: np.ndarray
   pair_geom2: np.ndarray
-  geom_convex_face: List[Optional[jax.Array]]
-  geom_convex_vert: List[Optional[jax.Array]]
-  geom_convex_edge_dir: List[Optional[jax.Array]]
-  geom_convex_facenormal: List[Optional[jax.Array]]
-  geom_convex_edge: List[Optional[jax.Array]]
-  geom_convex_edge_face_normal: List[Optional[jax.Array]]
   pair_solref: jax.Array
   pair_solreffriction: jax.Array
   pair_solimp: jax.Array
   pair_margin: jax.Array
   pair_gap: jax.Array
   pair_friction: jax.Array
   exclude_signature: np.ndarray
@@ -576,15 +617,32 @@
   actuator_biasprm: jax.Array
   actuator_ctrlrange: jax.Array
   actuator_forcerange: jax.Array
   actuator_actrange: jax.Array
   actuator_gear: jax.Array
   numeric_adr: np.ndarray
   numeric_data: np.ndarray
+  tuple_adr: np.ndarray
+  tuple_size: np.ndarray
+  tuple_objtype: np.ndarray
+  tuple_objid: np.ndarray
+  tuple_objprm: np.ndarray
+  name_bodyadr: np.ndarray
+  name_jntadr: np.ndarray
+  name_geomadr: np.ndarray
+  name_siteadr: np.ndarray
+  name_camadr: np.ndarray
+  name_meshadr: np.ndarray
+  name_pairadr: np.ndarray
+  name_eqadr: np.ndarray
+  name_actuatoradr: np.ndarray
+  name_sensoradr: np.ndarray
   name_numericadr: np.ndarray
+  name_tupleadr: np.ndarray
+  name_keyadr: np.ndarray
   names: bytes
 
 
 class Contact(PyTreeNode):
   """Result of collision detection functions.
 
   Attributes:
@@ -592,52 +650,47 @@
     pos: position of contact point: midpoint between geoms            (3,)
     frame: normal is in [0-2]                                         (9,)
     includemargin: include if dist<includemargin=margin-gap           (1,)
     friction: tangent1, 2, spin, roll1, 2                             (5,)
     solref: constraint solver reference, normal direction             (mjNREF,)
     solreffriction: constraint solver reference, friction directions  (mjNREF,)
     solimp: constraint solver impedance                               (mjNIMP,)
-    geom1: id of geom 1
-    geom2: id of geom 2
+    dim: contact space dimensionality: 1, 3, 4, or 6
+    geom1: id of geom 1; deprecated, use geom[0]
+    geom2: id of geom 2; deprecated, use geom[1]
+    geom: geom ids                                                    (2,)
+    efc_address: address in efc; -1: not included
   """
   dist: jax.Array
   pos: jax.Array
   frame: jax.Array
   includemargin: jax.Array
   friction: jax.Array
   solref: jax.Array
   solreffriction: jax.Array
   solimp: jax.Array
-  # unsupported: mu, H, dim
+  # unsupported: mu, H
+  dim: np.ndarray
   geom1: jax.Array
   geom2: jax.Array
-  # unsupported: efc_address, exclude
-
-  @classmethod
-  def zero(cls, ncon: int = 0) -> 'Contact':
-    """Returns a contact filled with zeros."""
-    return Contact(
-        dist=jp.zeros(ncon),
-        pos=jp.zeros((ncon, 3,)),
-        frame=jp.zeros((ncon, 3, 3)),
-        includemargin=jp.zeros(ncon),
-        friction=jp.zeros((ncon, 5)),
-        solref=jp.zeros((ncon, mujoco.mjNREF)),
-        solreffriction=jp.zeros((ncon, mujoco.mjNREF)),
-        solimp=jp.zeros((ncon, mujoco.mjNIMP,)),
-        geom1=jp.zeros(ncon, dtype=int),
-        geom2=jp.zeros(ncon, dtype=int),
-    )
+  geom: jax.Array
+  # unsupported: flex, elem, vert, exclude
+  efc_address: np.ndarray
 
 
 class Data(PyTreeNode):
-  r"""Dynamic state that updates each step.\
+  r"""\Dynamic state that updates each step.
 
   Attributes:
-    solver_niter: number of solver iterations, per island         (mjNISLAND,)
+    ne: number of equality constraints
+    nf: number of friction constraints
+    nl: number of limit constraints
+    nefc: number of constraints
+    ncon: number of contacts
+    solver_niter: number of solver iterations
     time: simulation time
     qpos: position                                                (nq,)
     qvel: velocity                                                (nv,)
     act: actuator activation                                      (na,)
     qacc_warmstart: acceleration used for warmstart               (nv,)
     ctrl: control                                                 (nu,)
     qfrc_applied: applied generalized force                       (nv,)
@@ -659,40 +712,48 @@
     cam_xpos: Cartesian camera position                           (ncam, 3)
     cam_xmat: Cartesian camera orientation                        (ncam, 9)
     subtree_com: center of mass of each subtree                   (nbody, 3)
     cdof: com-based motion axis of each dof                       (nv, 6)
     cinert: com-based body inertia and mass                       (nbody, 10)
     actuator_length: actuator lengths                             (nu,)
     actuator_moment: actuator moments                             (nu, nv)
-    crb: com-based composite inertia and mass                     (nbody, 10)
+    crb: com-based composite inertia and mass                     (nbody, 10)  \
     qM: total inertia                                  if sparse: (nM,)
                                                        if dense:  (nv, nv)
     qLD: L'*D*L (or Cholesky) factorization of M.      if sparse: (nM,)
                                                        if dense:  (nv, nv)
     qLDiagInv: 1/diag(D)                               if sparse: (nv,)
                                                        if dense:  (0,)
-    contact: list of all detected contacts                        (ncon,)
+    contact: all detected contacts                                (ncon,)
+    efc_type: constraint type                                     (nefc,)
     efc_J: constraint Jacobian                                    (nefc, nv)
     efc_frictionloss: frictionloss (friction)                     (nefc,)
     efc_D: constraint mass                                        (nefc,)
     actuator_velocity: actuator velocities                        (nu,)
     cvel: com-based velocity [3D rot; 3D tran]                    (nbody, 6)
     cdof_dot: time-derivative of cdof                             (nv, 6)
     qfrc_bias: C(qpos,qvel)                                       (nv,)
+    qfrc_gravcomp: passive gravity compensation force             (nv,)
     qfrc_passive: passive force                                   (nv,)
     efc_aref: reference pseudo-acceleration                       (nefc,)
     qfrc_actuator: actuator force                                 (nv,)
     qfrc_smooth: net unconstrained force                          (nv,)
     qacc_smooth: unconstrained acceleration                       (nv,)
     qfrc_constraint: constraint force                             (nv,)
     qfrc_inverse: net external force; should equal:               (nv,)
       qfrc_applied + J'*xfrc_applied + qfrc_actuator
     efc_force: constraint force in constraint space               (nefc,)
     userdata: user data, not touched by engine                    (nuserdata,)
   """
+  # constant sizes:
+  ne: int
+  nf: int
+  nl: int
+  nefc: int
+  ncon: int
   # solver statistics:
   solver_niter: jax.Array
   # global properties:
   time: jax.Array
   # state:
   qpos: jax.Array
   qvel: jax.Array
@@ -728,23 +789,25 @@
   crb: jax.Array
   actuator_length: jax.Array
   actuator_moment: jax.Array
   qM: jax.Array  # pylint:disable=invalid-name
   qLD: jax.Array  # pylint:disable=invalid-name
   qLDiagInv: jax.Array  # pylint:disable=invalid-name
   contact: Contact
+  efc_type: np.ndarray
   efc_J: jax.Array  # pylint:disable=invalid-name
   efc_frictionloss: jax.Array
   efc_D: jax.Array  # pylint:disable=invalid-name
   # position, velocity dependent:
   actuator_velocity: jax.Array
   cvel: jax.Array
   cdof_dot: jax.Array
   qfrc_bias: jax.Array
   qfrc_passive: jax.Array
+  qfrc_gravcomp: jax.Array
   efc_aref: jax.Array
   # position, velcoity, control & acceleration dependent:
   qfrc_actuator: jax.Array
   qfrc_smooth: jax.Array
   qacc_smooth: jax.Array
   qfrc_constraint: jax.Array
   qfrc_inverse: jax.Array
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/integration_test/collision_driver_test.py` & `mujoco_mjx-3.1.5/mujoco/mjx/integration_test/collision_driver_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,18 @@
 from mujoco.mjx._src.types import Contact
 # pylint: enable=g-importing-member
 import numpy as np
 
 
 def _assert_attr_eq(mjx_d, mj_d, attr, name, atol):
   if attr == 'efc_address':
-    # we do not test efc_address since it gets set in constraint logic
+    # contact order not guaranteed to match
+    np.testing.assert_array_equal(
+        np.sort(mjx_d.efc_address), np.sort(mj_d.efc_address)
+    )
     return
   err_msg = f'mismatch: {attr} in run: {name}'
   mjx_d, mj_d = getattr(mjx_d, attr), getattr(mj_d, attr)
   if attr == 'frame':
     mj_d = mj_d.reshape((-1, 3, 3))
   if mjx_d.shape != mj_d.shape:
     raise AssertionError(f'{attr} shape mismatch: {mjx_d.shape}, {mj_d.shape}')
@@ -75,16 +78,19 @@
     # re-order MJX contacts to match MJ order
     idx_mj = list(zip(d.contact.geom1, d.contact.geom2))
     idx_mjx = list(zip(dx.contact.geom1, dx.contact.geom2))
     idx_mjx = [tuple(np.array(i)) for i in idx_mjx]
     self.assertSequenceEqual(set(idx_mjx), set(idx_mj))
     idx = sorted(range(len(idx_mj)), key=lambda x: idx_mj.index(idx_mjx[x]))
 
-    mjx_contact = jax.tree_map(
+    mjx_contact = jax.tree_util.tree_map(
         lambda x: x.take(np.array(idx), axis=0), dx.contact
     )
+    mjx_contact = mjx_contact.replace(
+        dim=mjx_contact.dim[idx], efc_address=mjx_contact.efc_address[idx]
+    )
     for field in dataclasses.fields(Contact):
       _assert_attr_eq(mjx_contact, d.contact, field.name, seed, 1e-7)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/integration_test/forward_test.py` & `mujoco_mjx-3.1.5/mujoco/mjx/integration_test/forward_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/integration_test/smooth_test.py` & `mujoco_mjx-3.1.5/mujoco/mjx/integration_test/smooth_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     # put on device
     mx = mjx.put_model(m)
     dx = mjx.put_data(m, d)
 
     mujoco.mj_transmission(m, d)
     dx = transmission_jit_fn(mx, dx)
 
-    _assert_attr_eq(d, dx, 'actuator_length', seed, f'transmission{seed}')
-    _assert_attr_eq(
-        d, dx, 'actuator_moment', seed, f'transmission{seed}', atol=1e-4
-    )
+    for field in ['actuator_length', 'actuator_moment']:
+      _assert_attr_eq(
+          d, dx, field, seed, f'transmission{seed}', atol=1e-4
+      )
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/README.md` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/README.md`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/abduction.stl` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/abduction.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/barkour_v0_mjx.xml` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/barkour_v0_mjx.xml`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/body.stl` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/body.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/foot.stl` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/foot.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/handle.stl` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/handle.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/head.stl` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/head.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/head_mount.stl` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/head_mount.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/lower_leg_1to1.stl` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/lower_leg_1to1.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/powercable.stl` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/powercable.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/upper_left_1.stl` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/upper_left_1.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/upper_left_2.stl` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/upper_left_2.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/upper_left_3.stl` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/upper_left_3.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/upper_right_1.stl` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/upper_right_1.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/upper_right_2.stl` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/upper_right_2.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/barkour_v0/assets/upper_right_3.stl` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/barkour_v0/assets/upper_right_3.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/convex.xml` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/convex.xml`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/01_humanoids.xml` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/01_humanoids.xml`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/02_humanoids.xml` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/02_humanoids.xml`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/03_humanoids.xml` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/03_humanoids.xml`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/04_humanoids.xml` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/04_humanoids.xml`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/05_humanoids.xml` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/05_humanoids.xml`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/06_humanoids.xml` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/06_humanoids.xml`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/07_humanoids.xml` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/07_humanoids.xml`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/08_humanoids.xml` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/08_humanoids.xml`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/09_humanoids.xml` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/09_humanoids.xml`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/10_humanoids.xml` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/10_humanoids.xml`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/README.md` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/README.md`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/humanoid.png` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/humanoid.png`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/humanoid/humanoid.xml` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/humanoid/humanoid.xml`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/meshes/dodecahedron.stl` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/meshes/dodecahedron.stl`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/pendula.xml` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/pendula.xml`

 * *Files 10% similar despite different names*

#### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/pendula.xml` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/pendula.xml`

```diff
@@ -95,16 +95,32 @@
         <geom/>
         <body pos="0 -0.7 0">
           <joint name="joint14" axis="0.7 0.8 0.9" type="hinge" damping="0.75" range="-30 30"/>
           <geom/>
         </body>
       </body>
     </body>
+    <!-- triple pendulum of hinges with gravcomp -->
+    <body pos="3.0 0 0" gravcomp="1">
+      <joint name="joint15" axis="0.1 0.2 0.3" type="hinge"/>
+      <geom/>
+      <body pos="0 0 -0.8" gravcomp="2">
+        <joint name="joint16" axis="0.4 0.5 0.6" type="hinge" armature="0.02" range="-20 20"/>
+        <geom/>
+        <body pos="0 -0.7 0" gravcomp="3">
+          <joint name="joint17" axis="0.7 0.8 0.9" type="hinge" damping="0.75" range="-30 30" actuatorgravcomp="true"/>
+          <geom/>
+        </body>
+      </body>
+    </body>
   </worldbody>
   <actuator>
     <motor gear="250 0 0" joint="joint1" name="act1"/>
     <motor gear="0 275 0" joint="joint1" name="act2"/>
     <motor gear="0 0 300" joint="joint1" name="act3"/>
     <motor gear="275" joint="joint2" name="act4"/>
     <motor gear="275" joint="joint3" name="act5"/>
+    <motor gear="150" joint="joint15" name="act6"/>
+    <motor gear="150" joint="joint16" name="act7"/>
+    <motor gear="150" joint="joint17" name="act8"/>
   </actuator>
 </mujoco>
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/ray.xml` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/ray.xml`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/README.md` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/README.md`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/f_distal_pst.obj` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/f_distal_pst.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/f_distal_pst_214.obj` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/f_distal_pst_214.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/f_knuckle.obj` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/f_knuckle.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/f_middle.obj` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/f_middle.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/f_proximal.obj` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/f_proximal.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/forearm_0.obj` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/forearm_0.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/forearm_1.obj` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/forearm_1.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/forearm_collision.obj` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/forearm_collision.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/lf_metacarpal.obj` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/lf_metacarpal.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/mounting_plate.obj` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/mounting_plate.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/palm.obj` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/palm.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/th_distal_pst.obj` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/th_distal_pst.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/th_distal_pst_190.obj` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/th_distal_pst_190.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/th_middle.obj` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/th_middle.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/th_proximal.obj` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/th_proximal.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/assets/wrist.obj` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/assets/wrist.obj`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/right_hand.xml` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/right_hand.xml`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/scene_right.xml` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/scene_right.xml`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/test_data/shadow_hand/shadow_hand.png` & `mujoco_mjx-3.1.5/mujoco/mjx/test_data/shadow_hand/shadow_hand.png`

 * *Files identical despite different names*

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/testspeed.py` & `mujoco_mjx-3.1.5/mujoco/mjx/testspeed.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,16 +43,17 @@
 _OUTPUT = flags.DEFINE_enum(
     'output', 'text', ['text', 'tsv'], 'format to print results'
 )
 
 
 def _main(argv: Sequence[str]):
   """Runs testpeed function."""
-  base_path = _BASE_PATH.value or epath.resource_path('mujoco.mjx')
-  f = base_path / 'test_data' / _MJCF.value
+  path = epath.resource_path('mujoco.mjx') / 'test_data'
+  path = _BASE_PATH.value or path
+  f = epath.Path(path) / _MJCF.value
   m = mujoco.MjModel.from_xml_path(f.as_posix())
 
   print(f'Rolling out {_NSTEP.value} steps at dt = {m.opt.timestep:.3f}...')
   jit_time, run_time, steps = mjx.benchmark(
       m,
       _NSTEP.value,
       _BATCH_SIZE.value,
```

### Comparing `mujoco-mjx-3.1.4/mujoco/mjx/viewer.py` & `mujoco_mjx-3.1.5/mujoco/mjx/viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
   print(f'Compilation took {elapsed}s.')
 
   with mujoco.viewer.launch_passive(m, d) as v:
     while True:
       start = time.time()
 
       # TODO(robotics-simulation): recompile when changing disable flags, etc.
-      dx = dx.replace(ctrl=d.ctrl, xfrc_applied=d.xfrc_applied)
+      dx = dx.replace(ctrl=d.ctrl, act=d.act, xfrc_applied=d.xfrc_applied)
       dx = dx.replace(qpos=d.qpos, qvel=d.qvel, time=d.time)  # handle resets
       mx = mx.tree_replace({
           'opt.gravity': m.opt.gravity,
           'opt.tolerance': m.opt.tolerance,
           'opt.ls_tolerance': m.opt.ls_tolerance,
           'opt.timestep': m.opt.timestep,
       })
```

### Comparing `mujoco-mjx-3.1.4/mujoco_mjx.egg-info/PKG-INFO` & `mujoco_mjx-3.1.5/mujoco_mjx.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mujoco-mjx
-Version: 3.1.4
+Version: 3.1.5
 Summary: MuJoCo XLA (MJX)
 Author-email: Google DeepMind <mujoco@deepmind.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/google-deepmind/mujoco/tree/main/mjx
-Project-URL: Documentation, https://mujoco.readthedocs.io/en/3.1.4
+Project-URL: Documentation, https://mujoco.readthedocs.io/en/3.1.5
 Project-URL: Repository, https://github.com/google-deepmind/mujoco/tree/main/mjx
-Project-URL: Changelog, https://mujoco.readthedocs.io/en/3.1.4/changelog.html
+Project-URL: Changelog, https://mujoco.readthedocs.io/en/3.1.5/changelog.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -23,15 +23,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: absl-py
 Requires-Dist: etils[epath]
 Requires-Dist: jax
 Requires-Dist: jaxlib
-Requires-Dist: mujoco>=3.1.4.dev0
+Requires-Dist: mujoco>=3.1.5.dev0
 Requires-Dist: scipy
 Requires-Dist: trimesh
 
 # MuJoCo XLA (MJX)
 
 [![PyPI Python Version][pypi-versions-badge]][pypi]
 [![PyPI version][pypi-badge]][pypi]
```

### Comparing `mujoco-mjx-3.1.4/mujoco_mjx.egg-info/SOURCES.txt` & `mujoco_mjx-3.1.5/mujoco_mjx.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,23 @@
 MANIFEST.in
 README.md
 pyproject.toml
 mujoco/mjx/__init__.py
 mujoco/mjx/testspeed.py
 mujoco/mjx/viewer.py
 mujoco/mjx/_src/__init__.py
-mujoco/mjx/_src/collision_base.py
 mujoco/mjx/_src/collision_convex.py
 mujoco/mjx/_src/collision_driver.py
 mujoco/mjx/_src/collision_driver_test.py
 mujoco/mjx/_src/collision_primitive.py
 mujoco/mjx/_src/collision_sdf.py
+mujoco/mjx/_src/collision_types.py
 mujoco/mjx/_src/constraint.py
 mujoco/mjx/_src/constraint_test.py
 mujoco/mjx/_src/dataclasses.py
-mujoco/mjx/_src/device.py
-mujoco/mjx/_src/device_test.py
 mujoco/mjx/_src/forward.py
 mujoco/mjx/_src/forward_test.py
 mujoco/mjx/_src/io.py
 mujoco/mjx/_src/io_test.py
 mujoco/mjx/_src/math.py
 mujoco/mjx/_src/math_test.py
 mujoco/mjx/_src/mesh.py
```

### Comparing `mujoco-mjx-3.1.4/pyproject.toml` & `mujoco_mjx-3.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="mujoco-mjx"
-version = "3.1.4"
+version = "3.1.5"
 authors = [
     {name = "Google DeepMind", email = "mujoco@deepmind.com"},
 ]
 description = "MuJoCo XLA (MJX)"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {text = "Apache License 2.0"}
 classifiers = [
@@ -27,21 +27,21 @@
 ]
 requires-python = ">=3.8"
 dependencies = [
     "absl-py",
     "etils[epath]",
     "jax",
     "jaxlib",
-    "mujoco>=3.1.4.dev0",
+    "mujoco>=3.1.5.dev0",
     "scipy",
     "trimesh",
 ]
 
 [project.scripts]
 mjx-testspeed = "mujoco.mjx.testspeed:main"
 mjx-viewer = "mujoco.mjx.viewer:main"
 
 [project.urls]
 Homepage = "https://github.com/google-deepmind/mujoco/tree/main/mjx"
-Documentation = "https://mujoco.readthedocs.io/en/3.1.4"
+Documentation = "https://mujoco.readthedocs.io/en/3.1.5"
 Repository = "https://github.com/google-deepmind/mujoco/tree/main/mjx"
-Changelog = "https://mujoco.readthedocs.io/en/3.1.4/changelog.html"
+Changelog = "https://mujoco.readthedocs.io/en/3.1.5/changelog.html"
```

