# Comparing `tmp/hello_robot_stretch_body_tools-0.7.7.tar.gz` & `tmp/hello_robot_stretch_body_tools-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello_robot_stretch_body_tools-0.7.7.tar", last modified: Mon Mar  4 18:42:38 2024, max compression
+gzip compressed data, was "hello_robot_stretch_body_tools-0.7.8.tar", last modified: Tue May  7 04:08:58 2024, max compression
```

## Comparing `hello_robot_stretch_body_tools-0.7.7.tar` & `hello_robot_stretch_body_tools-0.7.8.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-03-04 18:42:38.871269 hello_robot_stretch_body_tools-0.7.7/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      923 2024-03-03 04:39:15.000000 hello_robot_stretch_body_tools-0.7.7/LICENSE.md
--rw-r--r--   0 hello-robot  (1000) hello-robot  (1000)     3676 2024-03-04 18:42:38.871269 hello_robot_stretch_body_tools-0.7.7/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2405 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/README.md
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-03-04 18:42:38.871269 hello_robot_stretch_body_tools-0.7.7/bin/
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2339 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_about.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      790 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_about_text.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      366 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_arm_home.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3240 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_arm_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      484 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_audio_test.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     6251 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_base_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     8350 2024-03-03 04:39:15.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_camera_streams_check.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    15767 2024-03-04 18:35:53.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_configure_tool.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      406 2024-01-29 18:48:53.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_dex_wrist_float.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3324 2024-03-03 04:39:15.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_dex_wrist_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      637 2024-01-29 18:48:53.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_free_robot_process.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      318 2024-01-29 18:48:53.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_gamepad_teleop.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      439 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_gripper_home.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2672 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_gripper_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4384 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_hardware_echo.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3998 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_head_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      385 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_lift_home.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3245 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_lift_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2105 2024-03-03 04:39:15.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_params.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1965 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_pimu_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     8759 2023-10-18 18:57:46.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_pimu_scope.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    15625 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_realsense_visualizer.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    11374 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_respeaker_test.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      997 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_robot_battery_check.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5570 2024-03-03 04:39:15.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_robot_collision_visualizer.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      766 2023-11-03 01:48:43.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_robot_dynamixel_reboot.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5356 2024-01-29 18:48:53.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_robot_home.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4426 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_robot_keyboard_teleop.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      597 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_robot_monitor.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      448 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_robot_stow.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      197 2024-03-03 04:39:15.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_robot_system_check.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     8829 2023-12-21 19:38:42.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_robot_urdf_visualizer.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2332 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_rp_lidar_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    25823 2024-03-03 04:39:15.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_system_check.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    17476 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_trajectory_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1874 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_version.sh
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1336 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_wacc_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2882 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_wacc_scope.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2447 2024-01-29 18:48:53.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_wrist_pitch_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2450 2024-01-29 18:48:53.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_wrist_roll_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      404 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_wrist_yaw_home.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2446 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_wrist_yaw_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    25967 2023-12-21 19:38:42.000000 hello_robot_stretch_body_tools-0.7.7/bin/stretch_xbox_controller_teleop.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      267 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/deploy.sh
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-03-04 18:42:38.871269 hello_robot_stretch_body_tools-0.7.7/hello_robot_stretch_body_tools.egg-info/
--rw-r--r--   0 hello-robot  (1000) hello-robot  (1000)     3676 2024-03-04 18:42:38.000000 hello_robot_stretch_body_tools-0.7.7/hello_robot_stretch_body_tools.egg-info/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2937 2024-03-04 18:42:38.000000 hello_robot_stretch_body_tools-0.7.7/hello_robot_stretch_body_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        1 2024-03-04 18:42:38.000000 hello_robot_stretch_body_tools-0.7.7/hello_robot_stretch_body_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      366 2024-03-04 18:42:38.000000 hello_robot_stretch_body_tools-0.7.7/hello_robot_stretch_body_tools.egg-info/requires.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        5 2024-03-04 18:42:38.000000 hello_robot_stretch_body_tools-0.7.7/hello_robot_stretch_body_tools.egg-info/top_level.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       38 2024-03-04 18:42:38.871269 hello_robot_stretch_body_tools-0.7.7/setup.cfg
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1533 2024-03-04 18:41:44.000000 hello_robot_stretch_body_tools-0.7.7/setup.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-03-04 18:42:38.871269 hello_robot_stretch_body_tools-0.7.7/test/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       34 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/test/__init__.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2173 2023-10-03 23:52:48.000000 hello_robot_stretch_body_tools-0.7.7/test/test_tools_launch.py
+drwxrwxr-x   0 hello-user  (1001) hello-user  (1001)        0 2024-05-07 04:08:58.344573 hello_robot_stretch_body_tools-0.7.8/
+-rw-rw-r--   0 hello-user  (1001) hello-user  (1001)      923 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/LICENSE.md
+-rw-rw-r--   0 hello-user  (1001) hello-user  (1001)     2885 2024-05-07 04:08:58.344573 hello_robot_stretch_body_tools-0.7.8/PKG-INFO
+-rw-rw-r--   0 hello-user  (1001) hello-user  (1001)     2405 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/README.md
+drwxrwxr-x   0 hello-user  (1001) hello-user  (1001)        0 2024-05-07 04:08:58.344573 hello_robot_stretch_body_tools-0.7.8/bin/
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     2339 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_about.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      790 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_about_text.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      366 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_arm_home.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     3240 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_arm_jog.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      484 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_audio_test.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     6251 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_base_jog.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     8350 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_camera_streams_check.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)    15767 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_configure_tool.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      406 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_dex_wrist_float.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     3324 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_dex_wrist_jog.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      309 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_free_robot_process.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      318 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_gamepad_teleop.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      439 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_gripper_home.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     2672 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_gripper_jog.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     4384 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_hardware_echo.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     3998 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_head_jog.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      385 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_lift_home.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     3245 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_lift_jog.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     2105 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_params.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     1965 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_pimu_jog.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     8759 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_pimu_scope.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)    17359 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_realsense_visualizer.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)    11374 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_respeaker_test.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     1049 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_battery_check.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     5570 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_collision_visualizer.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      766 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_dynamixel_reboot.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     5296 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_home.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     4461 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_keyboard_teleop.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      597 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_monitor.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      448 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_stow.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      197 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_system_check.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     8829 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_urdf_visualizer.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     2333 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_rp_lidar_jog.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)    25882 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_system_check.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)    17476 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_trajectory_jog.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     1874 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_version.sh
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     1336 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_wacc_jog.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     2882 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_wacc_scope.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     2447 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_wrist_pitch_jog.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     2450 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_wrist_roll_jog.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      404 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_wrist_yaw_home.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)     2446 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_wrist_yaw_jog.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)    25967 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/bin/stretch_xbox_controller_teleop.py
+-rwxrwxr-x   0 hello-user  (1001) hello-user  (1001)      267 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/deploy.sh
+drwxrwxr-x   0 hello-user  (1001) hello-user  (1001)        0 2024-05-07 04:08:58.344573 hello_robot_stretch_body_tools-0.7.8/hello_robot_stretch_body_tools.egg-info/
+-rw-rw-r--   0 hello-user  (1001) hello-user  (1001)     2885 2024-05-07 04:08:58.000000 hello_robot_stretch_body_tools-0.7.8/hello_robot_stretch_body_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 hello-user  (1001) hello-user  (1001)     2937 2024-05-07 04:08:58.000000 hello_robot_stretch_body_tools-0.7.8/hello_robot_stretch_body_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello-user  (1001) hello-user  (1001)        1 2024-05-07 04:08:58.000000 hello_robot_stretch_body_tools-0.7.8/hello_robot_stretch_body_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello-user  (1001) hello-user  (1001)      366 2024-05-07 04:08:58.000000 hello_robot_stretch_body_tools-0.7.8/hello_robot_stretch_body_tools.egg-info/requires.txt
+-rw-rw-r--   0 hello-user  (1001) hello-user  (1001)        5 2024-05-07 04:08:58.000000 hello_robot_stretch_body_tools-0.7.8/hello_robot_stretch_body_tools.egg-info/top_level.txt
+-rw-rw-r--   0 hello-user  (1001) hello-user  (1001)       38 2024-05-07 04:08:58.344573 hello_robot_stretch_body_tools-0.7.8/setup.cfg
+-rw-rw-r--   0 hello-user  (1001) hello-user  (1001)     1533 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/setup.py
+drwxrwxr-x   0 hello-user  (1001) hello-user  (1001)        0 2024-05-07 04:08:58.344573 hello_robot_stretch_body_tools-0.7.8/test/
+-rw-rw-r--   0 hello-user  (1001) hello-user  (1001)       34 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/test/__init__.py
+-rw-rw-r--   0 hello-user  (1001) hello-user  (1001)     2173 2024-05-07 04:06:45.000000 hello_robot_stretch_body_tools-0.7.8/test/test_tools_launch.py
```

### Comparing `hello_robot_stretch_body_tools-0.7.7/LICENSE.md` & `hello_robot_stretch_body_tools-0.7.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/README.md` & `hello_robot_stretch_body_tools-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_about.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_about.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_about_text.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_about_text.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_arm_jog.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_arm_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_base_jog.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_base_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_camera_streams_check.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_camera_streams_check.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_configure_tool.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_configure_tool.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_dex_wrist_jog.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_dex_wrist_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_gripper_jog.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_gripper_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_hardware_echo.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_hardware_echo.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_head_jog.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_head_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_lift_jog.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_lift_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_params.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_params.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_pimu_jog.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_pimu_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_pimu_scope.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_pimu_scope.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_realsense_visualizer.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_realsense_visualizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,18 @@
                     help="Show no GUI while reading images.")
 parser.add_argument("--colormap", type=int, default=cv2.COLORMAP_OCEAN,
                     help="Valid OpenCV colormaps at 'https://docs.opencv.org/master/d3/d50/group__imgproc__colormap.html'.")
 parser.add_argument("--save", nargs="?", type=str, const="",
                     help="Save as .avi video to given filepath at end of script.")
 parser.add_argument("--save_limit", type=int, default=60,
                     help="The number of minutes of data to save.")
+parser.add_argument("--d405", action="store_true",
+                    help="By default, this tool shows the D435if head camera imagery. Setting this flag causes the tool to instead show the D405 wrist imagery.")
+parser.add_argument('--exposure', action='store', type=str, default='auto',
+                    help="Set the D405 exposure to ['low', 'medium', 'auto'] or an integer in the range [0, 165000]")
 args, _ = parser.parse_known_args()
 output_filepath = args.save
 
 ####################################
 # Additional settings
 ####################################
 
@@ -66,18 +70,36 @@
 apply_local_histogram_equalization = False
 apply_global_histogram_equalization = False
 
 ####################################
 # Initialize
 ####################################
 
-# Configure depth and color streams.
-# Note: width/heights are swapped since the images will be rotated 90 degrees from what the camera captures.
+serial_no = None
+rs_cameras = [{'name': device.get_info(rs.camera_info.name), 'serial_number': device.get_info(rs.camera_info.serial_number)}
+    for device in rs.context().devices]
+if args.d405:
+    for info in rs_cameras:
+        if 'D405' in info['name']:
+            serial_no = info['serial_number']
+    if serial_no is None:
+        print("Wrist D405 camera not found. Exiting.")
+        sys.exit(1)
+else:
+    for info in rs_cameras:
+        if 'D435' in info['name']:
+            serial_no = info['serial_number']
+    if serial_no is None:
+        print("Head D435 camera not found. Exiting.")
+        sys.exit(1)
 pipeline = rs.pipeline()
 config = rs.config()
+config.enable_device(serial_no)
+# Configure depth and color streams.
+# Note: width/heights are swapped since the images will be rotated 90 degrees from what the camera captures.
 config.enable_stream(rs.stream.depth, resolution_depth[0], resolution_depth[1], rs.format.z16, fps_color) # note that the fps downsampling will be applied later
 config.enable_stream(rs.stream.color, resolution_color[0], resolution_color[1], rs.format.bgr8, fps_color)
 frame_width_colorAndDepth = resolution_color[1] + resolution_depth[1]
 frame_height_colorAndDepth = max(resolution_color[0], resolution_depth[0])
 frame_width_color = resolution_color[1]
 frame_height_color = resolution_color[0]
 frame_width_depth = resolution_depth[1]
@@ -126,14 +148,31 @@
 frameBuffer_depth = []
 frameBuffer_colorAndDepth = []
 frameBuffer_limit_color = round(frameBuffer_limit_s * fps_color)
 frameBuffer_limit_depth = round(frameBuffer_limit_s * fps_color / fps_depth_downsample_factor)
 capture_limit_color = round(fps_color * 60 * args.save_limit)
 
 pipeline.start(config)
+# Set exposure for D405
+if args.d405:
+    if args.exposure == 'auto':
+        # Use autoexposure
+        stereo_sensor = pipeline.get_active_profile().get_device().query_sensors()[0]
+        stereo_sensor.set_option(rs.option.enable_auto_exposure, True)
+    else:
+        if args.exposure == 'low':
+            exposure_value = 33000
+        elif args.exposure == 'medium':
+            exposure_value = 85000
+        else:
+            exposure_value = int(args.exposure)
+
+        stereo_sensor = pipeline.get_active_profile().get_device().query_sensors()[0]
+        stereo_sensor.set_option(rs.option.exposure, exposure_value)
+
 start_capture_time_s = time.time()
 end_capture_time_color_s = start_capture_time_s
 end_capture_time_depth_s = start_capture_time_s
 frame_count_color = 0
 frame_count_depth = 0
 print("Press Ctrl-C to exit...")
 try:
@@ -164,19 +203,20 @@
             color_image_l_equalized = cv2.equalizeHist(color_image_l) # apply global equalization to the L-channel
             color_image_lab = cv2.merge((color_image_l_equalized, color_image_a, color_image_b))  # merge channels
             color_image = cv2.cvtColor(color_image_lab, cv2.COLOR_LAB2BGR)  # convert from LAB to BGR
 
         # Apply colormap on depth image (image must be converted to 8-bit per pixel first).
         depth_image = cv2.applyColorMap(cv2.convertScaleAbs(depth_image, alpha=-0.04, beta=255.0), args.colormap)
 
-        # Rotate and flip images.
-        color_image = np.moveaxis(color_image, 0, 1)
-        color_image = np.fliplr(color_image)
-        depth_image = np.moveaxis(depth_image, 0, 1)
-        depth_image = np.fliplr(depth_image)
+        if not args.d405:
+            # Rotate and flip images.
+            color_image = np.moveaxis(color_image, 0, 1)
+            color_image = np.fliplr(color_image)
+            depth_image = np.moveaxis(depth_image, 0, 1)
+            depth_image = np.fliplr(depth_image)
 
         # Concatenate images horizontally if desired.
         if save_video_colorAndDepth or not args.no_gui:
             # Pad images if they are different heights
             pad_y = color_image.shape[0] - depth_image.shape[0]
             if pad_y > 0:
                 color_image_padded = color_image
```

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_respeaker_test.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_respeaker_test.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_robot_collision_visualizer.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_collision_visualizer.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_robot_dynamixel_reboot.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_dynamixel_reboot.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_robot_home.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_home.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,14 @@
         print('background: saved to scan logger dir', time.time() - start, flush=True)
     except:
         pass
 background_process = multiprocessing.Process(target=fetch_updates_in_background)
 
 r=robot.Robot()
 if not r.startup():
-    r.logger.error('Failed to startup connection to robot')
     sys.exit(1)
 if r.pimu.status['runstop_event']:
     r.logger.error('Cannot home while run-stopped')
     r.stop()
     sys.exit(1)
 
 background_process.start()
```

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_robot_keyboard_teleop.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_keyboard_teleop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #!/usr/bin/env python3
 from __future__ import print_function
 import sys, tty, termios
 import stretch_body.robot as hello_robot
 from stretch_body.hello_utils import *
 import argparse
+import sys
 print_stretch_re_use()
 
 
 parser=argparse.ArgumentParser(description='Control the robot base, lift, arm, head, and tool from the keyboard')
 args=parser.parse_args()
 
 
 robot=hello_robot.Robot()
-robot.startup()
+if not robot.startup():
+    sys.exit(1)
 
 small_move_m=.01
 large_move_m=0.1
 small_rotate_rad=deg_to_rad(1.0)
 large_rotate_rad=deg_to_rad(10.0)
 
 small_lift_move_m=.01
```

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_robot_monitor.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_monitor.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_robot_urdf_visualizer.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_robot_urdf_visualizer.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_rp_lidar_jog.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_rp_lidar_jog.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
                 old_t = now
                 continue
             delta = now - old_t
             print('Points-per-sec: %.2f Rate: %.2f Hz, Scan len %d' % (len(scan)/delta, 1/delta, len(scan)))
             data.append(delta)
             old_t = now
     except KeyboardInterrupt:
-        print('Stoping. Computing mean...')
+        print('Stopping. Computing mean...')
         # lidar.stop()
         # lidar.disconnect()
         delta = sum(data)/len(data)
         print('Mean: %.2f Hz, %.2f RPM' % (1/delta, 60/delta))
 
 if not args.motor_on: #Turn off motor by default
     lidar.stop_motor()
```

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_system_check.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_system_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import stretch_body.hello_utils as hu
 hu.print_stretch_re_use()
 
 import os
 import sh
 import re
+import sys
 import apt
 import git
 import yaml
 import distro
 import fnmatch
 import pathlib
 import datetime
@@ -64,16 +65,19 @@
     print(Fore.LIGHTBLUE_EX + 'Tool = ' + Fore.CYAN + 'DexWrist 3 w/ Gripper')
 else:
     print(Fore.LIGHTBLUE_EX + 'Tool = ' + Fore.CYAN + stretch_tool)
 if args.verbose:
     print(Fore.LIGHTBLUE_EX + 'Batch = ' + Fore.CYAN + stretch_batch)
 print(Fore.LIGHTBLUE_EX + 'Serial Number = ' + Fore.CYAN + stretch_serial_no)
 # create robot instance
+print(Style.RESET_ALL)
 r=robot.Robot()
-r.startup()
+if not r.startup():
+    sys.exit(1)
+
 r.monitor.logger.setLevel('WARN')
 
 # ###################  HARDWARE  ######################
 def is_comms_ready():
     # Establish what USB devices we expect to see
     usb_device_seen = {
         'hello-wacc': False,
```

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_trajectory_jog.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_trajectory_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_version.sh` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_version.sh`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_wacc_jog.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_wacc_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_wacc_scope.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_wacc_scope.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_wrist_pitch_jog.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_wrist_pitch_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_wrist_roll_jog.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_wrist_roll_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_wrist_yaw_jog.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_wrist_yaw_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/bin/stretch_xbox_controller_teleop.py` & `hello_robot_stretch_body_tools-0.7.8/bin/stretch_xbox_controller_teleop.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/hello_robot_stretch_body_tools.egg-info/SOURCES.txt` & `hello_robot_stretch_body_tools-0.7.8/hello_robot_stretch_body_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.7.7/setup.py` & `hello_robot_stretch_body_tools-0.7.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 script_path='./bin'
 ex_scripts = glob.glob(script_path+'/*.py') + glob.glob(script_path+'/*.sh')
 stretch_scripts=[f for f in ex_scripts if isfile(f)]
 
 setuptools.setup(
     name="hello_robot_stretch_body_tools",
-    version="0.7.7",
+    version="0.7.8",
     author="Hello Robot Inc",
     author_email="support@hello-robot.com",
     description="Stretch Body Tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hello-robot/stretch_body",
     scripts = stretch_scripts,
```

### Comparing `hello_robot_stretch_body_tools-0.7.7/test/test_tools_launch.py` & `hello_robot_stretch_body_tools-0.7.8/test/test_tools_launch.py`

 * *Files identical despite different names*

