# Comparing `tmp/biorobot-0.1.7.tar.gz` & `tmp/biorobot-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biorobot-0.1.7.tar", last modified: Fri Apr 12 11:53:19 2024, max compression
+gzip compressed data, was "biorobot-0.1.8.tar", last modified: Tue May  7 21:22:49 2024, max compression
```

## Comparing `biorobot-0.1.7.tar` & `biorobot-0.1.8.tar`

### file list

```diff
@@ -1,106 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.145481 biorobot-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-12 11:53:14.000000 biorobot-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 11:53:14.000000 biorobot-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-04-12 11:53:19.141481 biorobot-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-12 11:53:14.000000 biorobot-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.129481 biorobot-0.1.7/biorobot/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.129481 biorobot-0.1.7/biorobot/brittle_star/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.129481 biorobot-0.1.7/biorobot/brittle_star/environment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.133481 biorobot-0.1.7/biorobot/brittle_star/environment/directed_locomotion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/directed_locomotion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/directed_locomotion/dual.py
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/directed_locomotion/mjc_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/directed_locomotion/mjx_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/directed_locomotion/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.133481 biorobot-0.1.7/biorobot/brittle_star/environment/light_escape/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/light_escape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/light_escape/dual.py
--rw-r--r--   0 runner    (1001) docker     (127)    10085 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/light_escape/mjc_env.py
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/light_escape/mjx_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/light_escape/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.133481 biorobot-0.1.7/biorobot/brittle_star/environment/shared/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/shared/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7554 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/shared/mjc_observables.py
--rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/shared/mjx_observables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.133481 biorobot-0.1.7/biorobot/brittle_star/environment/undirected_locomotion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/undirected_locomotion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/undirected_locomotion/dual.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/undirected_locomotion/mjc_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/undirected_locomotion/mjx_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/undirected_locomotion/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.133481 biorobot-0.1.7/biorobot/brittle_star/mjcf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/mjcf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.133481 biorobot-0.1.7/biorobot/brittle_star/mjcf/arena/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/mjcf/arena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/mjcf/arena/aquarium.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.137481 biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/morphology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.137481 biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/parts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/parts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/parts/arm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/parts/arm_segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/parts/disk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.137481 biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/specification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/specification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/specification/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/specification/specification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.137481 biorobot-0.1.7/biorobot/brittle_star/usage_examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/usage_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/usage_examples/directed_locomotion_single.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/usage_examples/light_escape_single.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/usage_examples/light_escape_vectorized.py
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/usage_examples/undirected_locomotion_single.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.137481 biorobot-0.1.7/biorobot/toy_example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.137481 biorobot-0.1.7/biorobot/toy_example/environment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13905 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/environment/mjc_env.py
--rw-r--r--   0 runner    (1001) docker     (127)    11924 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/environment/mjx_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.137481 biorobot-0.1.7/biorobot/toy_example/mjcf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.137481 biorobot-0.1.7/biorobot/toy_example/mjcf/arena/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/arena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/arena/arena.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/arena/target.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.141481 biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/morphology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.141481 biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/parts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/parts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/parts/arm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/parts/arm_segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/parts/torso.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.141481 biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/specification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/specification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/specification/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/specification/specification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.141481 biorobot-0.1.7/biorobot/toy_example/usage_examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/usage_examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.141481 biorobot-0.1.7/biorobot/toy_example/usage_examples/mjc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/usage_examples/mjc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/usage_examples/mjc/example_usage_single.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/usage_examples/mjc/example_usage_vectorized.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.141481 biorobot-0.1.7/biorobot/toy_example/usage_examples/mjx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/usage_examples/mjx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/usage_examples/mjx/example_usage_single.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/usage_examples/mjx/example_usage_vectorized.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.141481 biorobot-0.1.7/biorobot/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/utils/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.141481 biorobot-0.1.7/biorobot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-04-12 11:53:19.000000 biorobot-0.1.7/biorobot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-12 11:53:19.000000 biorobot-0.1.7/biorobot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:53:19.000000 biorobot-0.1.7/biorobot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-12 11:53:19.000000 biorobot-0.1.7/biorobot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 11:53:19.000000 biorobot-0.1.7/biorobot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-12 11:53:14.000000 biorobot-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-12 11:53:14.000000 biorobot-0.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 11:53:19.145481 biorobot-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-12 11:53:14.000000 biorobot-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:49.541134 biorobot-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-07 21:22:43.000000 biorobot-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 21:22:43.000000 biorobot-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-05-07 21:22:49.537134 biorobot-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-05-07 21:22:43.000000 biorobot-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:49.529134 biorobot-0.1.8/biorobot/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:49.529134 biorobot-0.1.8/biorobot/brittle_star/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:49.529134 biorobot-0.1.8/biorobot/brittle_star/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:49.533134 biorobot-0.1.8/biorobot/brittle_star/environment/directed_locomotion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/environment/directed_locomotion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/environment/directed_locomotion/dual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/environment/directed_locomotion/mjc_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/environment/directed_locomotion/mjx_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/environment/directed_locomotion/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:49.533134 biorobot-0.1.8/biorobot/brittle_star/environment/light_escape/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/environment/light_escape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/environment/light_escape/dual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10085 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/environment/light_escape/mjc_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/environment/light_escape/mjx_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/environment/light_escape/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:49.533134 biorobot-0.1.8/biorobot/brittle_star/environment/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/environment/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/environment/shared/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/environment/shared/mjc_observables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/environment/shared/mjx_observables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:49.533134 biorobot-0.1.8/biorobot/brittle_star/environment/undirected_locomotion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/environment/undirected_locomotion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/environment/undirected_locomotion/dual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/environment/undirected_locomotion/mjc_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/environment/undirected_locomotion/mjx_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/environment/undirected_locomotion/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:49.533134 biorobot-0.1.8/biorobot/brittle_star/mjcf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/mjcf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:49.533134 biorobot-0.1.8/biorobot/brittle_star/mjcf/arena/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/mjcf/arena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/mjcf/arena/aquarium.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:49.537134 biorobot-0.1.8/biorobot/brittle_star/mjcf/morphology/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/mjcf/morphology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/mjcf/morphology/morphology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:49.537134 biorobot-0.1.8/biorobot/brittle_star/mjcf/morphology/parts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/mjcf/morphology/parts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/mjcf/morphology/parts/arm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/mjcf/morphology/parts/arm_segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/mjcf/morphology/parts/disk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:49.537134 biorobot-0.1.8/biorobot/brittle_star/mjcf/morphology/specification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/mjcf/morphology/specification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/mjcf/morphology/specification/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/mjcf/morphology/specification/specification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:49.537134 biorobot-0.1.8/biorobot/brittle_star/usage_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/usage_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/usage_examples/directed_locomotion_single.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/usage_examples/light_escape_single.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/usage_examples/light_escape_vectorized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/brittle_star/usage_examples/undirected_locomotion_single.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:49.537134 biorobot-0.1.8/biorobot/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/utils/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-07 21:22:43.000000 biorobot-0.1.8/biorobot/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:22:49.537134 biorobot-0.1.8/biorobot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-05-07 21:22:49.000000 biorobot-0.1.8/biorobot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-07 21:22:49.000000 biorobot-0.1.8/biorobot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 21:22:49.000000 biorobot-0.1.8/biorobot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-07 21:22:49.000000 biorobot-0.1.8/biorobot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 21:22:49.000000 biorobot-0.1.8/biorobot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-07 21:22:43.000000 biorobot-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-07 21:22:43.000000 biorobot-0.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 21:22:49.541134 biorobot-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-07 21:22:43.000000 biorobot-0.1.8/setup.py
```

### Comparing `biorobot-0.1.7/LICENSE` & `biorobot-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/PKG-INFO` & `biorobot-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biorobot
-Version: 0.1.7
+Version: 0.1.8
 Summary: The Bio-inspired Robotics Testbed (BRT).
 Home-page: https://github.com/Co-Evolve/brb
 Author-email: Dries Marzougui <dries.marzougui@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Co-Evolve/brt
 Project-URL: Repository, https://github.com/Co-Evolve/brt
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: biorobot Version: 0.1.7 Summary: The Bio-inspired
+Metadata-Version: 2.1 Name: biorobot Version: 0.1.8 Summary: The Bio-inspired
 Robotics Testbed (BRT). Home-page: https://github.com/Co-Evolve/brb Author-
 email: Dries Marzougui
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/Co-Evolve/brt
 Project-URL: Repository, https://github.com/Co-Evolve/brt Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
```

### Comparing `biorobot-0.1.7/README.md` & `biorobot-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/brittle_star/environment/directed_locomotion/dual.py` & `biorobot-0.1.8/biorobot/brittle_star/environment/directed_locomotion/dual.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/brittle_star/environment/directed_locomotion/mjc_env.py` & `biorobot-0.1.8/biorobot/brittle_star/environment/directed_locomotion/mjc_env.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/brittle_star/environment/directed_locomotion/mjx_env.py` & `biorobot-0.1.8/biorobot/brittle_star/environment/directed_locomotion/mjx_env.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/brittle_star/environment/directed_locomotion/shared.py` & `biorobot-0.1.8/biorobot/brittle_star/environment/directed_locomotion/shared.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/brittle_star/environment/light_escape/dual.py` & `biorobot-0.1.8/biorobot/brittle_star/environment/light_escape/dual.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/brittle_star/environment/light_escape/mjc_env.py` & `biorobot-0.1.8/biorobot/brittle_star/environment/light_escape/mjc_env.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/brittle_star/environment/light_escape/mjx_env.py` & `biorobot-0.1.8/biorobot/brittle_star/environment/light_escape/mjx_env.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/brittle_star/environment/light_escape/shared.py` & `biorobot-0.1.8/biorobot/brittle_star/environment/light_escape/shared.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/brittle_star/environment/shared/base.py` & `biorobot-0.1.8/biorobot/brittle_star/environment/shared/base.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/brittle_star/environment/shared/mjc_observables.py` & `biorobot-0.1.8/biorobot/brittle_star/environment/shared/mjc_observables.py`

 * *Files 9% similar despite different names*

```diff
@@ -91,44 +91,26 @@
     indexer = count(0)
     segment_capsule_geom_id_to_contact_idx = {}
     for geom_id in range(mj_model.ngeom):
         geom_name = mj_model.geom(geom_id).name
         if "segment" in geom_name and "capsule" in geom_name:
             segment_capsule_geom_id_to_contact_idx[geom_id] = next(indexer)
 
-    #   Get non-morphology geom ids to check contacts with
-    external_contact_geom_ids = {
-        mj_model.geom("groundplane").id,
-        mj_model.geom("north_wall").id,
-        mj_model.geom("east_wall").id,
-        mj_model.geom("south_wall").id,
-        mj_model.geom("west_wall").id,
-    }
-
     def get_segment_contacts(state: MJCEnvState) -> np.ndarray:
-        contacts = np.zeros(len(segment_capsule_geom_id_to_contact_idx))
+        contacts = np.zeros(len(segment_capsule_geom_id_to_contact_idx), dtype=int)
         # based on https://gist.github.com/WuXinyang2012/b6649817101dfcb061eff901e9942057
         for contact_id in range(state.mj_data.ncon):
             contact = state.mj_data.contact[contact_id]
-            if contact.geom1 in external_contact_geom_ids:
+            if contact.dist < 0:
+                if contact.geom1 in segment_capsule_geom_id_to_contact_idx:
+                    contacts[segment_capsule_geom_id_to_contact_idx[contact.geom1]] = 1
                 if contact.geom2 in segment_capsule_geom_id_to_contact_idx:
-                    c_array = np.zeros(6, dtype=np.float64)
-                    mujoco.mj_contactForce(
-                        m=state.mj_model, d=state.mj_data, id=contact_id, result=c_array
-                    )
-
-                    # Convert the contact force from contact frame to world frame
-                    ref = np.reshape(contact.frame, (3, 3))
-                    c_force = np.dot(np.linalg.inv(ref), c_array[0:3])
-
-                    index = segment_capsule_geom_id_to_contact_idx[contact.geom2]
-                    contacts[index] = max(np.linalg.norm(c_force), contacts[index])
+                    contacts[segment_capsule_geom_id_to_contact_idx[contact.geom2]] = 1
 
-        ground_contacts = (contacts > 0).astype(int)
-        return ground_contacts
+        return contacts
 
     touch_observable = MJCObservable(
         name="segment_contact",
         low=np.zeros(len(segment_capsule_geom_id_to_contact_idx)),
         high=np.ones(len(segment_capsule_geom_id_to_contact_idx)),
         retriever=get_segment_contacts,
     )
```

### Comparing `biorobot-0.1.7/biorobot/brittle_star/environment/shared/mjx_observables.py` & `biorobot-0.1.8/biorobot/brittle_star/environment/shared/mjx_observables.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,19 +91,18 @@
             mj_model.geom("west_wall").id,
         ]
     )
 
     def get_segment_contacts(state: MJXEnvState) -> jnp.ndarray:
         contact_data = state.mjx_data.contact
         contacts = contact_data.dist <= 0
-        valid_geom1s = jnp.isin(contact_data.geom1, external_contact_geom_ids)
 
         def solve_contact(geom_id: int) -> jnp.ndarray:
             return (
-                jnp.sum(contacts * valid_geom1s * (contact_data.geom2 == geom_id)) > 0
+                jnp.sum(contacts * jnp.any(geom_id == contact_data.geom, axis=-1)) > 0
             ).astype(int)
 
         return jax.vmap(solve_contact)(segment_capsule_geom_ids)
 
     touch_observable = MJXObservable(
         name="segment_contact",
         low=jnp.zeros(len(segment_capsule_geom_ids)),
```

### Comparing `biorobot-0.1.7/biorobot/brittle_star/environment/undirected_locomotion/dual.py` & `biorobot-0.1.8/biorobot/brittle_star/environment/undirected_locomotion/dual.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/brittle_star/environment/undirected_locomotion/mjc_env.py` & `biorobot-0.1.8/biorobot/brittle_star/environment/undirected_locomotion/mjc_env.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/brittle_star/environment/undirected_locomotion/mjx_env.py` & `biorobot-0.1.8/biorobot/brittle_star/environment/undirected_locomotion/mjx_env.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/brittle_star/environment/undirected_locomotion/shared.py` & `biorobot-0.1.8/biorobot/brittle_star/environment/undirected_locomotion/shared.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/brittle_star/mjcf/arena/aquarium.py` & `biorobot-0.1.8/biorobot/brittle_star/mjcf/arena/aquarium.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/morphology.py` & `biorobot-0.1.8/biorobot/brittle_star/mjcf/morphology/morphology.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self._build_arms()
         self._configure_camera()
 
     def _configure_compiler(self) -> None:
         self.mjcf_model.compiler.angle = "radian"
 
     def _configure_defaults(self) -> None:
-        self.mjcf_model.default.geom.condim = 3
+        self.mjcf_model.default.geom.condim = 6
         self.mjcf_model.default.geom.contype = 1
         self.mjcf_model.default.geom.conaffinity = 0
 
     def _build_disk(self) -> None:
         self._disk = MJCFBrittleStarDisk(
             parent=self, name="central_disk", pos=np.zeros(3), euler=np.zeros(3)
         )
```

### Comparing `biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/parts/arm.py` & `biorobot-0.1.8/biorobot/brittle_star/mjcf/morphology/parts/arm.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/parts/arm_segment.py` & `biorobot-0.1.8/biorobot/brittle_star/mjcf/morphology/parts/arm_segment.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/parts/disk.py` & `biorobot-0.1.8/biorobot/brittle_star/mjcf/morphology/parts/disk.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/specification/default.py` & `biorobot-0.1.8/biorobot/brittle_star/mjcf/morphology/specification/default.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/specification/specification.py` & `biorobot-0.1.8/biorobot/brittle_star/mjcf/morphology/specification/specification.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/brittle_star/usage_examples/directed_locomotion_single.py` & `biorobot-0.1.8/biorobot/brittle_star/usage_examples/directed_locomotion_single.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/brittle_star/usage_examples/light_escape_single.py` & `biorobot-0.1.8/biorobot/brittle_star/usage_examples/light_escape_single.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/brittle_star/usage_examples/light_escape_vectorized.py` & `biorobot-0.1.8/biorobot/brittle_star/usage_examples/light_escape_vectorized.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/brittle_star/usage_examples/undirected_locomotion_single.py` & `biorobot-0.1.8/biorobot/brittle_star/usage_examples/undirected_locomotion_single.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/utils/colors.py` & `biorobot-0.1.8/biorobot/utils/colors.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/utils/noise.py` & `biorobot-0.1.8/biorobot/utils/noise.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot/utils/video.py` & `biorobot-0.1.8/biorobot/utils/video.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.7/biorobot.egg-info/PKG-INFO` & `biorobot-0.1.8/biorobot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biorobot
-Version: 0.1.7
+Version: 0.1.8
 Summary: The Bio-inspired Robotics Testbed (BRT).
 Home-page: https://github.com/Co-Evolve/brb
 Author-email: Dries Marzougui <dries.marzougui@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Co-Evolve/brt
 Project-URL: Repository, https://github.com/Co-Evolve/brt
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: biorobot Version: 0.1.7 Summary: The Bio-inspired
+Metadata-Version: 2.1 Name: biorobot Version: 0.1.8 Summary: The Bio-inspired
 Robotics Testbed (BRT). Home-page: https://github.com/Co-Evolve/brb Author-
 email: Dries Marzougui
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/Co-Evolve/brt
 Project-URL: Repository, https://github.com/Co-Evolve/brt Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
```

### Comparing `biorobot-0.1.7/biorobot.egg-info/SOURCES.txt` & `biorobot-0.1.8/biorobot.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -44,35 +44,11 @@
 biorobot/brittle_star/mjcf/morphology/specification/default.py
 biorobot/brittle_star/mjcf/morphology/specification/specification.py
 biorobot/brittle_star/usage_examples/__init__.py
 biorobot/brittle_star/usage_examples/directed_locomotion_single.py
 biorobot/brittle_star/usage_examples/light_escape_single.py
 biorobot/brittle_star/usage_examples/light_escape_vectorized.py
 biorobot/brittle_star/usage_examples/undirected_locomotion_single.py
-biorobot/toy_example/__init__.py
-biorobot/toy_example/environment/__init__.py
-biorobot/toy_example/environment/mjc_env.py
-biorobot/toy_example/environment/mjx_env.py
-biorobot/toy_example/mjcf/__init__.py
-biorobot/toy_example/mjcf/arena/__init__.py
-biorobot/toy_example/mjcf/arena/arena.py
-biorobot/toy_example/mjcf/arena/target.py
-biorobot/toy_example/mjcf/morphology/__init__.py
-biorobot/toy_example/mjcf/morphology/morphology.py
-biorobot/toy_example/mjcf/morphology/parts/__init__.py
-biorobot/toy_example/mjcf/morphology/parts/arm.py
-biorobot/toy_example/mjcf/morphology/parts/arm_segment.py
-biorobot/toy_example/mjcf/morphology/parts/torso.py
-biorobot/toy_example/mjcf/morphology/specification/__init__.py
-biorobot/toy_example/mjcf/morphology/specification/default.py
-biorobot/toy_example/mjcf/morphology/specification/specification.py
-biorobot/toy_example/usage_examples/__init__.py
-biorobot/toy_example/usage_examples/mjc/__init__.py
-biorobot/toy_example/usage_examples/mjc/example_usage_single.py
-biorobot/toy_example/usage_examples/mjc/example_usage_vectorized.py
-biorobot/toy_example/usage_examples/mjx/__init__.py
-biorobot/toy_example/usage_examples/mjx/example_usage_single.py
-biorobot/toy_example/usage_examples/mjx/example_usage_vectorized.py
 biorobot/utils/__init__.py
 biorobot/utils/colors.py
 biorobot/utils/noise.py
 biorobot/utils/video.py
```

### Comparing `biorobot-0.1.7/pyproject.toml` & `biorobot-0.1.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "biorobot"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
     { name = "Dries Marzougui", email = "dries.marzougui@gmail.com" },
 ]
 description = "The Bio-inspired Robotics Testbed (BRT)."
 readme = { file = "README.md", content-type = "text/markdown" }
 license = { text = "MIT" }
 classifiers = [
```

### Comparing `biorobot-0.1.7/setup.py` & `biorobot-0.1.8/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     license = f.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
         name='biorobot',
-        version='0.1.7',
+        version='0.1.8',
         description='The Bio-inspired Robotics Testbed.',
         long_description=readme,
         url='https://github.com/Co-Evolve/brb',
         license=license,
         packages=find_packages(exclude=('tests', 'docs')),
         install_requires=required
         )
```

