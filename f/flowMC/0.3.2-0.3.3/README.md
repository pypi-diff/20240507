# Comparing `tmp/flowmc-0.3.2.tar.gz` & `tmp/flowmc-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowmc-0.3.2.tar", last modified: Fri Apr 19 21:33:15 2024, max compression
+gzip compressed data, was "flowmc-0.3.3.tar", last modified: Tue May  7 18:40:45 2024, max compression
```

## Comparing `flowmc-0.3.2.tar` & `flowmc-0.3.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:15.737426 flowmc-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-19 21:33:11.000000 flowmc-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-19 21:33:15.737426 flowmc-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-04-19 21:33:11.000000 flowmc-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-19 21:33:11.000000 flowmc-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-19 21:33:15.737426 flowmc-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:15.729426 flowmc-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:15.733426 flowmc-0.3.2/src/flowMC/
--rw-r--r--   0 runner    (1001) docker     (127)    13136 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/Sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:15.733426 flowmc-0.3.2/src/flowMC/nfmodel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/nfmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/nfmodel/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/nfmodel/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/nfmodel/realNVP.py
--rw-r--r--   0 runner    (1001) docker     (127)    19506 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/nfmodel/rqSpline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:15.733426 flowmc-0.3.2/src/flowMC/proposal/
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/proposal/Gaussian_random_walk.py
--rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/proposal/HMC.py
--rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/proposal/MALA.py
--rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/proposal/NF_proposal.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/proposal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/proposal/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/proposal/flowHMC.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:15.737426 flowmc-0.3.2/src/flowMC/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/strategy/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/strategy/global_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/strategy/importance_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/strategy/optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:15.737426 flowmc-0.3.2/src/flowMC/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/utils/EvolutionaryOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/utils/PythonFunctionWrap.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/utils/postprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:15.737426 flowmc-0.3.2/src/flowMC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-19 21:33:15.000000 flowmc-0.3.2/src/flowMC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-19 21:33:15.000000 flowmc-0.3.2/src/flowMC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:33:15.000000 flowmc-0.3.2/src/flowMC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-19 21:33:15.000000 flowmc-0.3.2/src/flowMC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 21:33:15.000000 flowmc-0.3.2/src/flowMC.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:45.848202 flowmc-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-07 18:40:36.000000 flowmc-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-07 18:40:45.848202 flowmc-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-07 18:40:36.000000 flowmc-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-07 18:40:36.000000 flowmc-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-07 18:40:45.848202 flowmc-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:45.840202 flowmc-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:45.844202 flowmc-0.3.3/src/flowMC/
+-rw-r--r--   0 runner    (1001) docker     (127)    13136 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/Sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:45.844202 flowmc-0.3.3/src/flowMC/nfmodel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/nfmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/nfmodel/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/nfmodel/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/nfmodel/realNVP.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19506 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/nfmodel/rqSpline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:45.844202 flowmc-0.3.3/src/flowMC/proposal/
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/proposal/Gaussian_random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/proposal/HMC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/proposal/MALA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/proposal/NF_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/proposal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/proposal/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/proposal/flowHMC.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:45.844202 flowmc-0.3.3/src/flowMC/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/strategy/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/strategy/global_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/strategy/importance_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/strategy/optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:45.848202 flowmc-0.3.3/src/flowMC/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/utils/EvolutionaryOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/utils/PythonFunctionWrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/utils/postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:45.848202 flowmc-0.3.3/src/flowMC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-07 18:40:45.000000 flowmc-0.3.3/src/flowMC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-07 18:40:45.000000 flowmc-0.3.3/src/flowMC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:40:45.000000 flowmc-0.3.3/src/flowMC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-07 18:40:45.000000 flowmc-0.3.3/src/flowMC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 18:40:45.000000 flowmc-0.3.3/src/flowMC.egg-info/top_level.txt
```

### Comparing `flowmc-0.3.2/LICENSE` & `flowmc-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.2/PKG-INFO` & `flowmc-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowMC
-Version: 0.3.2
+Version: 0.3.3
 Summary: Normalizing flow exhanced sampler in jax
 Home-page: https://github.com/kazewong/flowMC
 Author: Kaze Wong, Marylou Gabrié, Dan Foreman-Mackey
 Author-email: kazewong.physics@gmail.com
 License: MIT
 Keywords: sampling,inference,machine learning,normalizing,autodiff,jax
 Requires-Python: >=3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flowMC Version: 0.3.2 Summary: Normalizing flow
+Metadata-Version: 2.1 Name: flowMC Version: 0.3.3 Summary: Normalizing flow
 exhanced sampler in jax Home-page: https://github.com/kazewong/flowMC Author:
 Kaze Wong, Marylou GabriÃ©, Dan Foreman-Mackey Author-email:
 kazewong.physics@gmail.com License: MIT Keywords: sampling,inference,machine
 learning,normalizing,autodiff,jax Requires-Python: >=3.10 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: jax>=0.4.12 Requires-
 Dist: jaxlib>=0.4.12 Requires-Dist: equinox>=0.10.6 Requires-Dist: optax>=0.1.5
 Requires-Dist: evosax>=0.1.4 Requires-Dist: tqdm Requires-Dist: corner # flowMC
```

### Comparing `flowmc-0.3.2/README.md` & `flowmc-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.2/setup.cfg` & `flowmc-0.3.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flowMC
-version = 0.3.2
+version = 0.3.3
 author = Kaze Wong, Marylou Gabrié, Dan Foreman-Mackey
 author_email = kazewong.physics@gmail.com
 url = https://github.com/kazewong/flowMC
 description = Normalizing flow exhanced sampler in jax
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = sampling, inference, machine learning, normalizing, autodiff, jax
```

### Comparing `flowmc-0.3.2/src/flowMC/Sampler.py` & `flowmc-0.3.3/src/flowMC/Sampler.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.2/src/flowMC/nfmodel/base.py` & `flowmc-0.3.3/src/flowMC/nfmodel/base.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.2/src/flowMC/nfmodel/common.py` & `flowmc-0.3.3/src/flowMC/nfmodel/common.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.2/src/flowMC/nfmodel/realNVP.py` & `flowmc-0.3.3/src/flowMC/nfmodel/realNVP.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.2/src/flowMC/nfmodel/rqSpline.py` & `flowmc-0.3.3/src/flowMC/nfmodel/rqSpline.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.2/src/flowMC/proposal/Gaussian_random_walk.py` & `flowmc-0.3.3/src/flowMC/proposal/Gaussian_random_walk.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.2/src/flowMC/proposal/HMC.py` & `flowmc-0.3.3/src/flowMC/proposal/HMC.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.2/src/flowMC/proposal/MALA.py` & `flowmc-0.3.3/src/flowMC/proposal/MALA.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.2/src/flowMC/proposal/NF_proposal.py` & `flowmc-0.3.3/src/flowMC/proposal/NF_proposal.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.2/src/flowMC/proposal/base.py` & `flowmc-0.3.3/src/flowMC/proposal/base.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.2/src/flowMC/proposal/flowHMC.py` & `flowmc-0.3.3/src/flowMC/proposal/flowHMC.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.2/src/flowMC/strategy/base.py` & `flowmc-0.3.3/src/flowMC/strategy/base.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.2/src/flowMC/strategy/global_tuning.py` & `flowmc-0.3.3/src/flowMC/strategy/global_tuning.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.2/src/flowMC/utils/EvolutionaryOptimizer.py` & `flowmc-0.3.3/src/flowMC/utils/EvolutionaryOptimizer.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.2/src/flowMC/utils/PythonFunctionWrap.py` & `flowmc-0.3.3/src/flowMC/utils/PythonFunctionWrap.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.2/src/flowMC/utils/postprocessing.py` & `flowmc-0.3.3/src/flowMC/utils/postprocessing.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.2/src/flowMC.egg-info/PKG-INFO` & `flowmc-0.3.3/src/flowMC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowMC
-Version: 0.3.2
+Version: 0.3.3
 Summary: Normalizing flow exhanced sampler in jax
 Home-page: https://github.com/kazewong/flowMC
 Author: Kaze Wong, Marylou Gabrié, Dan Foreman-Mackey
 Author-email: kazewong.physics@gmail.com
 License: MIT
 Keywords: sampling,inference,machine learning,normalizing,autodiff,jax
 Requires-Python: >=3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flowMC Version: 0.3.2 Summary: Normalizing flow
+Metadata-Version: 2.1 Name: flowMC Version: 0.3.3 Summary: Normalizing flow
 exhanced sampler in jax Home-page: https://github.com/kazewong/flowMC Author:
 Kaze Wong, Marylou GabriÃ©, Dan Foreman-Mackey Author-email:
 kazewong.physics@gmail.com License: MIT Keywords: sampling,inference,machine
 learning,normalizing,autodiff,jax Requires-Python: >=3.10 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: jax>=0.4.12 Requires-
 Dist: jaxlib>=0.4.12 Requires-Dist: equinox>=0.10.6 Requires-Dist: optax>=0.1.5
 Requires-Dist: evosax>=0.1.4 Requires-Dist: tqdm Requires-Dist: corner # flowMC
```

### Comparing `flowmc-0.3.2/src/flowMC.egg-info/SOURCES.txt` & `flowmc-0.3.3/src/flowMC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

