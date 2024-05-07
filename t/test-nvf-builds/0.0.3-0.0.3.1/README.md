# Comparing `tmp/test_nvf_builds-0.0.3.tar.gz` & `tmp/test_nvf_builds-0.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_nvf_builds-0.0.3.tar", last modified: Mon May  6 16:00:07 2024, max compression
+gzip compressed data, was "test_nvf_builds-0.0.3.1.tar", last modified: Tue May  7 07:58:19 2024, max compression
```

## Comparing `test_nvf_builds-0.0.3.tar` & `test_nvf_builds-0.0.3.1.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 16:00:07.405554 test_nvf_builds-0.0.3/
--rw-r--r--   0 mostafa    (501) staff       (20)      402 2024-05-06 16:00:07.405484 test_nvf_builds-0.0.3/PKG-INFO
--rw-r--r--   0 mostafa    (501) staff       (20)       85 2024-05-06 07:53:59.000000 test_nvf_builds-0.0.3/README.md
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 16:00:07.400495 test_nvf_builds-0.0.3/oasysnow/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:25.000000 test_nvf_builds-0.0.3/oasysnow/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 16:00:07.400629 test_nvf_builds-0.0.3/oasysnow/federated/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:50:57.000000 test_nvf_builds-0.0.3/oasysnow/federated/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 16:00:07.400750 test_nvf_builds-0.0.3/oasysnow/federated/client/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:25:11.000000 test_nvf_builds-0.0.3/oasysnow/federated/client/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 16:00:07.401459 test_nvf_builds-0.0.3/oasysnow/federated/client/filters/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:35.000000 test_nvf_builds-0.0.3/oasysnow/federated/client/filters/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     3468 2024-05-06 15:57:38.000000 test_nvf_builds-0.0.3/oasysnow/federated/client/filters/filter_data.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2471 2024-05-06 15:57:38.000000 test_nvf_builds-0.0.3/oasysnow/federated/client/filters/filter_results.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 16:00:07.401982 test_nvf_builds-0.0.3/oasysnow/federated/client/trainer/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:41.000000 test_nvf_builds-0.0.3/oasysnow/federated/client/trainer/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     5234 2024-05-06 15:59:26.000000 test_nvf_builds-0.0.3/oasysnow/federated/client/trainer/trainer.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 16:00:07.402730 test_nvf_builds-0.0.3/oasysnow/federated/model/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:36:02.000000 test_nvf_builds-0.0.3/oasysnow/federated/model/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2460 2024-05-02 13:22:42.000000 test_nvf_builds-0.0.3/oasysnow/federated/model/gennet_model.py
--rw-r--r--   0 mostafa    (501) staff       (20)     1930 2024-05-06 15:58:12.000000 test_nvf_builds-0.0.3/oasysnow/federated/model/global_model.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 16:00:07.402996 test_nvf_builds-0.0.3/oasysnow/federated/server/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:11.000000 test_nvf_builds-0.0.3/oasysnow/federated/server/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 16:00:07.403408 test_nvf_builds-0.0.3/oasysnow/federated/server/filters/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:45.000000 test_nvf_builds-0.0.3/oasysnow/federated/server/filters/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 16:00:07.403919 test_nvf_builds-0.0.3/oasysnow/federated/server/filters/attestation_service/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:56:34.000000 test_nvf_builds-0.0.3/oasysnow/federated/server/filters/attestation_service/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:46:21.000000 test_nvf_builds-0.0.3/oasysnow/federated/server/filters/attestation_service/server.py
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:56:28.000000 test_nvf_builds-0.0.3/oasysnow/federated/server/filters/attestation_service/verification.py
--rw-r--r--   0 mostafa    (501) staff       (20)     4442 2024-05-06 15:57:39.000000 test_nvf_builds-0.0.3/oasysnow/federated/server/filters/filter_data.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2475 2024-04-19 21:41:54.000000 test_nvf_builds-0.0.3/oasysnow/federated/server/filters/filter_results.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 16:00:07.404167 test_nvf_builds-0.0.3/oasysnow/federated/server/model_runner/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:45:46.000000 test_nvf_builds-0.0.3/oasysnow/federated/server/model_runner/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     5424 2024-05-06 15:59:11.000000 test_nvf_builds-0.0.3/oasysnow/federated/server/model_runner/model_runner.py
--rw-r--r--   0 mostafa    (501) staff       (20)       36 2024-05-06 15:40:29.000000 test_nvf_builds-0.0.3/requirements.txt
--rw-r--r--   0 mostafa    (501) staff       (20)      435 2024-05-06 16:00:07.405815 test_nvf_builds-0.0.3/setup.cfg
--rw-r--r--   0 mostafa    (501) staff       (20)      322 2024-05-06 15:10:01.000000 test_nvf_builds-0.0.3/setup.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 16:00:07.405241 test_nvf_builds-0.0.3/test_nvf_builds.egg-info/
--rw-r--r--   0 mostafa    (501) staff       (20)      402 2024-05-06 16:00:07.000000 test_nvf_builds-0.0.3/test_nvf_builds.egg-info/PKG-INFO
--rw-r--r--   0 mostafa    (501) staff       (20)     1177 2024-05-06 16:00:07.000000 test_nvf_builds-0.0.3/test_nvf_builds.egg-info/SOURCES.txt
--rw-r--r--   0 mostafa    (501) staff       (20)        1 2024-05-06 16:00:07.000000 test_nvf_builds-0.0.3/test_nvf_builds.egg-info/dependency_links.txt
--rw-r--r--   0 mostafa    (501) staff       (20)       36 2024-05-06 16:00:07.000000 test_nvf_builds-0.0.3/test_nvf_builds.egg-info/requires.txt
--rw-r--r--   0 mostafa    (501) staff       (20)        9 2024-05-06 16:00:07.000000 test_nvf_builds-0.0.3/test_nvf_builds.egg-info/top_level.txt
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 07:58:19.296339 test_nvf_builds-0.0.3.1/
+-rw-r--r--   0 mostafa    (501) staff       (20)    11357 2024-05-07 07:57:47.000000 test_nvf_builds-0.0.3.1/LICENSE
+-rw-r--r--   0 mostafa    (501) staff       (20)      473 2024-05-07 07:58:19.296245 test_nvf_builds-0.0.3.1/PKG-INFO
+-rw-r--r--   0 mostafa    (501) staff       (20)       85 2024-05-06 07:53:59.000000 test_nvf_builds-0.0.3.1/README.md
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 07:58:19.290740 test_nvf_builds-0.0.3.1/oasysnow/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:25.000000 test_nvf_builds-0.0.3.1/oasysnow/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 07:58:19.290856 test_nvf_builds-0.0.3.1/oasysnow/federated/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:50:57.000000 test_nvf_builds-0.0.3.1/oasysnow/federated/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 07:58:19.290971 test_nvf_builds-0.0.3.1/oasysnow/federated/client/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:25:11.000000 test_nvf_builds-0.0.3.1/oasysnow/federated/client/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 07:58:19.291720 test_nvf_builds-0.0.3.1/oasysnow/federated/client/filters/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:35.000000 test_nvf_builds-0.0.3.1/oasysnow/federated/client/filters/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     3468 2024-05-06 15:57:38.000000 test_nvf_builds-0.0.3.1/oasysnow/federated/client/filters/filter_data.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2471 2024-05-06 15:57:38.000000 test_nvf_builds-0.0.3.1/oasysnow/federated/client/filters/filter_results.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 07:58:19.292165 test_nvf_builds-0.0.3.1/oasysnow/federated/client/trainer/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:41.000000 test_nvf_builds-0.0.3.1/oasysnow/federated/client/trainer/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     5234 2024-05-06 15:59:26.000000 test_nvf_builds-0.0.3.1/oasysnow/federated/client/trainer/trainer.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 07:58:19.293157 test_nvf_builds-0.0.3.1/oasysnow/federated/model/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:36:02.000000 test_nvf_builds-0.0.3.1/oasysnow/federated/model/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2460 2024-05-02 13:22:42.000000 test_nvf_builds-0.0.3.1/oasysnow/federated/model/gennet_model.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1930 2024-05-06 15:58:12.000000 test_nvf_builds-0.0.3.1/oasysnow/federated/model/global_model.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 07:58:19.293436 test_nvf_builds-0.0.3.1/oasysnow/federated/server/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:11.000000 test_nvf_builds-0.0.3.1/oasysnow/federated/server/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 07:58:19.293856 test_nvf_builds-0.0.3.1/oasysnow/federated/server/filters/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:45.000000 test_nvf_builds-0.0.3.1/oasysnow/federated/server/filters/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 07:58:19.294410 test_nvf_builds-0.0.3.1/oasysnow/federated/server/filters/attestation_service/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:56:34.000000 test_nvf_builds-0.0.3.1/oasysnow/federated/server/filters/attestation_service/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:46:21.000000 test_nvf_builds-0.0.3.1/oasysnow/federated/server/filters/attestation_service/server.py
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:56:28.000000 test_nvf_builds-0.0.3.1/oasysnow/federated/server/filters/attestation_service/verification.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     4442 2024-05-06 15:57:39.000000 test_nvf_builds-0.0.3.1/oasysnow/federated/server/filters/filter_data.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2475 2024-04-19 21:41:54.000000 test_nvf_builds-0.0.3.1/oasysnow/federated/server/filters/filter_results.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 07:58:19.294642 test_nvf_builds-0.0.3.1/oasysnow/federated/server/model_runner/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:45:46.000000 test_nvf_builds-0.0.3.1/oasysnow/federated/server/model_runner/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     5424 2024-05-06 15:59:11.000000 test_nvf_builds-0.0.3.1/oasysnow/federated/server/model_runner/model_runner.py
+-rw-r--r--   0 mostafa    (501) staff       (20)       36 2024-05-06 15:40:29.000000 test_nvf_builds-0.0.3.1/requirements.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)      479 2024-05-07 07:58:19.296619 test_nvf_builds-0.0.3.1/setup.cfg
+-rw-r--r--   0 mostafa    (501) staff       (20)      322 2024-05-06 15:10:01.000000 test_nvf_builds-0.0.3.1/setup.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-07 07:58:19.295954 test_nvf_builds-0.0.3.1/test_nvf_builds.egg-info/
+-rw-r--r--   0 mostafa    (501) staff       (20)      473 2024-05-07 07:58:19.000000 test_nvf_builds-0.0.3.1/test_nvf_builds.egg-info/PKG-INFO
+-rw-r--r--   0 mostafa    (501) staff       (20)     1185 2024-05-07 07:58:19.000000 test_nvf_builds-0.0.3.1/test_nvf_builds.egg-info/SOURCES.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)        1 2024-05-07 07:58:19.000000 test_nvf_builds-0.0.3.1/test_nvf_builds.egg-info/dependency_links.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)       36 2024-05-07 07:58:19.000000 test_nvf_builds-0.0.3.1/test_nvf_builds.egg-info/requires.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)        9 2024-05-07 07:58:19.000000 test_nvf_builds-0.0.3.1/test_nvf_builds.egg-info/top_level.txt
```

### Comparing `test_nvf_builds-0.0.3/oasysnow/federated/client/filters/filter_data.py` & `test_nvf_builds-0.0.3.1/oasysnow/federated/client/filters/filter_data.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3/oasysnow/federated/client/filters/filter_results.py` & `test_nvf_builds-0.0.3.1/oasysnow/federated/client/filters/filter_results.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3/oasysnow/federated/client/trainer/trainer.py` & `test_nvf_builds-0.0.3.1/oasysnow/federated/client/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3/oasysnow/federated/model/gennet_model.py` & `test_nvf_builds-0.0.3.1/oasysnow/federated/model/gennet_model.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3/oasysnow/federated/model/global_model.py` & `test_nvf_builds-0.0.3.1/oasysnow/federated/model/global_model.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3/oasysnow/federated/server/filters/filter_data.py` & `test_nvf_builds-0.0.3.1/oasysnow/federated/server/filters/filter_data.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3/oasysnow/federated/server/filters/filter_results.py` & `test_nvf_builds-0.0.3.1/oasysnow/federated/server/filters/filter_results.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3/oasysnow/federated/server/model_runner/model_runner.py` & `test_nvf_builds-0.0.3.1/oasysnow/federated/server/model_runner/model_runner.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3/test_nvf_builds.egg-info/SOURCES.txt` & `test_nvf_builds-0.0.3.1/test_nvf_builds.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 requirements.txt
 setup.cfg
 setup.py
 oasysnow/__init__.py
 oasysnow/federated/__init__.py
 oasysnow/federated/client/__init__.py
```

