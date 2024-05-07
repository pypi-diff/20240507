# Comparing `tmp/thc_mg_env-0.0.1.tar.gz` & `tmp/thc_mg_env-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thc_mg_env-0.0.1.tar", last modified: Tue May  7 15:58:41 2024, max compression
+gzip compressed data, was "thc_mg_env-0.0.3.tar", last modified: Tue May  7 20:21:08 2024, max compression
```

## Comparing `thc_mg_env-0.0.1.tar` & `thc_mg_env-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 15:58:41.352480 thc_mg_env-0.0.1/
--rw-rw-rw-   0        0        0      141 2024-05-07 15:58:41.352480 thc_mg_env-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-07 14:21:14.000000 thc_mg_env-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-07 15:58:41.352480 thc_mg_env-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      344 2024-05-07 14:25:54.000000 thc_mg_env-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 15:58:41.340170 thc_mg_env-0.0.1/thc_MG_env/
--rw-rw-rw-   0        0        0      154 2024-05-07 14:45:20.000000 thc_mg_env-0.0.1/thc_MG_env/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 15:58:41.351264 thc_mg_env-0.0.1/thc_MG_env/envs/
--rw-rw-rw-   0        0        0       42 2024-05-07 15:55:45.000000 thc_mg_env-0.0.1/thc_MG_env/envs/__init__.py
--rw-rw-rw-   0        0        0     2032 2024-05-07 15:57:36.000000 thc_mg_env-0.0.1/thc_MG_env/envs/env_thc.py
-drwxrwxrwx   0        0        0        0 2024-05-07 15:58:41.351264 thc_mg_env-0.0.1/thc_MG_env.egg-info/
--rw-rw-rw-   0        0        0      141 2024-05-07 15:58:41.000000 thc_mg_env-0.0.1/thc_MG_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-05-07 15:58:41.000000 thc_mg_env-0.0.1/thc_MG_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 15:58:41.000000 thc_mg_env-0.0.1/thc_MG_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-05-07 15:58:41.000000 thc_mg_env-0.0.1/thc_MG_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-07 15:58:41.000000 thc_mg_env-0.0.1/thc_MG_env.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 20:21:08.835438 thc_mg_env-0.0.3/
+-rw-rw-rw-   0        0        0      141 2024-05-07 20:21:08.835438 thc_mg_env-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-07 14:21:14.000000 thc_mg_env-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-07 20:21:08.835438 thc_mg_env-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      344 2024-05-07 20:19:04.000000 thc_mg_env-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 20:21:08.823856 thc_mg_env-0.0.3/thc_MG_env/
+-rw-rw-rw-   0        0        0      181 2024-05-07 20:10:46.000000 thc_mg_env-0.0.3/thc_MG_env/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 20:21:08.833932 thc_mg_env-0.0.3/thc_MG_env/envs/
+-rw-rw-rw-   0        0        0       61 2024-05-07 19:52:56.000000 thc_mg_env-0.0.3/thc_MG_env/envs/__init__.py
+-rw-rw-rw-   0        0        0     2000 2024-05-07 15:59:57.000000 thc_mg_env-0.0.3/thc_MG_env/envs/env_thc.py
+drwxrwxrwx   0        0        0        0 2024-05-07 20:21:08.834434 thc_mg_env-0.0.3/thc_MG_env.egg-info/
+-rw-rw-rw-   0        0        0      141 2024-05-07 20:21:08.000000 thc_mg_env-0.0.3/thc_MG_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-05-07 20:21:08.000000 thc_mg_env-0.0.3/thc_MG_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 20:21:08.000000 thc_mg_env-0.0.3/thc_MG_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-05-07 20:21:08.000000 thc_mg_env-0.0.3/thc_MG_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-07 20:21:08.000000 thc_mg_env-0.0.3/thc_MG_env.egg-info/top_level.txt
```

### Comparing `thc_mg_env-0.0.1/thc_MG_env/envs/env_thc.py` & `thc_mg_env-0.0.3/thc_MG_env/envs/env_thc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import gym
 from gym import Env
 from gym.spaces import Discrete, Box
 import numpy as np
 
-from setuptools import setup
-
 
 class TwohoirzontalcartEnv_chen(Env):
     def __init__(self):
         # Actions we can take, down, stay, up
         self.action_space = Box(low=np.array([-100]), high=np.array([100]), shape=(1,))
         # Temperature array
         self.observation_space = Box(low=np.array([-100, -100]), high=np.array([100, 100]), shape=(2,))
```

