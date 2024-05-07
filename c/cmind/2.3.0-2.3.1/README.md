# Comparing `tmp/cmind-2.3.0.tar.gz` & `tmp/cmind-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmind-2.3.0.tar", last modified: Sun Apr 28 12:43:27 2024, max compression
+gzip compressed data, was "cmind-2.3.1.tar", last modified: Tue May  7 10:06:02 2024, max compression
```

## Comparing `cmind-2.3.0.tar` & `cmind-2.3.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-28 12:43:27.024759 cmind-2.3.0/
--rw-r--r--   0 fursin    (1000) fursin    (1000)    10174 2024-04-28 12:38:52.000000 cmind-2.3.0/LICENSE.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)    11667 2024-04-28 12:43:27.024759 cmind-2.3.0/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)    11260 2024-04-28 12:38:52.000000 cmind-2.3.0/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-28 12:43:27.024759 cmind-2.3.0/cmind/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      190 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      100 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/__main__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     4918 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/artifact.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    47952 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/automation.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     6467 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/cli.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3315 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/config.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    28674 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/core.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     9541 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/index.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2076 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/net.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-28 12:43:27.024759 cmind-2.3.0/cmind/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-28 12:43:27.024759 cmind-2.3.0/cmind/repo/automation/
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-28 12:43:27.024759 cmind-2.3.0/cmind/repo/automation/automation/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2666 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/automation/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/automation/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     4047 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/automation/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/automation/module_dummy.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     8846 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/automation/module_misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/automation/template_list_of_automations.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-28 12:43:27.024759 cmind-2.3.0/cmind/repo/automation/ckx/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1003 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/ckx/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      327 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/ckx/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1109 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/ckx/module.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-28 12:43:27.024759 cmind-2.3.0/cmind/repo/automation/core/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/core/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/core/_cm.json
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-28 12:43:27.024759 cmind-2.3.0/cmind/repo/automation/core/cm_60cb625a46b38610/
--rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1091 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/core/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      269 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/core/module_misc.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-28 12:43:27.024759 cmind-2.3.0/cmind/repo/automation/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      388 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/repo/README-extra.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)    10292 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/repo/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      305 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/repo/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)    39862 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/automation/repo/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo/cmr.yaml
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2038 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repo.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    25467 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/repos.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    47294 2024-04-28 12:38:52.000000 cmind-2.3.0/cmind/utils.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-28 12:43:27.024759 cmind-2.3.0/cmind.egg-info/
--rw-r--r--   0 fursin    (1000) fursin    (1000)    11667 2024-04-28 12:43:26.000000 cmind-2.3.0/cmind.egg-info/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1279 2024-04-28 12:43:26.000000 cmind-2.3.0/cmind.egg-info/SOURCES.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2024-04-28 12:43:26.000000 cmind-2.3.0/cmind.egg-info/dependency_links.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)      176 2024-04-28 12:43:26.000000 cmind-2.3.0/cmind.egg-info/entry_points.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2024-04-28 12:43:26.000000 cmind-2.3.0/cmind.egg-info/not-zip-safe
--rw-r--r--   0 fursin    (1000) fursin    (1000)       39 2024-04-28 12:43:26.000000 cmind-2.3.0/cmind.egg-info/requires.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2024-04-28 12:43:26.000000 cmind-2.3.0/cmind.egg-info/top_level.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2024-04-28 12:43:27.024759 cmind-2.3.0/setup.cfg
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2913 2024-04-28 12:38:52.000000 cmind-2.3.0/setup.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-05-07 10:06:02.400562 cmind-2.3.1/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    10174 2024-05-07 10:05:06.000000 cmind-2.3.1/LICENSE.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    11667 2024-05-07 10:06:02.400562 cmind-2.3.1/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    11260 2024-05-07 10:05:06.000000 cmind-2.3.1/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-05-07 10:06:02.400562 cmind-2.3.1/cmind/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      190 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      100 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/__main__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     4918 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/artifact.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    47952 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/automation.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     6467 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/cli.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     3315 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/config.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    28674 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/core.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     9541 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/index.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2076 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/net.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-05-07 10:06:02.400562 cmind-2.3.1/cmind/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/repo/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-05-07 10:06:02.400562 cmind-2.3.1/cmind/repo/automation/
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-05-07 10:06:02.400562 cmind-2.3.1/cmind/repo/automation/automation/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2666 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/repo/automation/automation/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/repo/automation/automation/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     4047 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/repo/automation/automation/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/repo/automation/automation/module_dummy.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     8846 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/repo/automation/automation/module_misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/repo/automation/automation/template_list_of_automations.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-05-07 10:06:02.400562 cmind-2.3.1/cmind/repo/automation/ckx/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1003 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/repo/automation/ckx/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      327 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/repo/automation/ckx/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1109 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/repo/automation/ckx/module.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-05-07 10:06:02.400562 cmind-2.3.1/cmind/repo/automation/core/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/repo/automation/core/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/repo/automation/core/_cm.json
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-05-07 10:06:02.400562 cmind-2.3.1/cmind/repo/automation/core/cm_60cb625a46b38610/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1091 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/repo/automation/core/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      269 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/repo/automation/core/module_misc.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-05-07 10:06:02.400562 cmind-2.3.1/cmind/repo/automation/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      388 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/repo/automation/repo/README-extra.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    10292 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/repo/automation/repo/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      305 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/repo/automation/repo/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    40088 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/repo/automation/repo/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/repo/cmr.yaml
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2038 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/repo.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    25467 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/repos.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    47294 2024-05-07 10:05:06.000000 cmind-2.3.1/cmind/utils.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-05-07 10:06:02.400562 cmind-2.3.1/cmind.egg-info/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    11667 2024-05-07 10:06:02.000000 cmind-2.3.1/cmind.egg-info/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1279 2024-05-07 10:06:02.000000 cmind-2.3.1/cmind.egg-info/SOURCES.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2024-05-07 10:06:02.000000 cmind-2.3.1/cmind.egg-info/dependency_links.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      176 2024-05-07 10:06:02.000000 cmind-2.3.1/cmind.egg-info/entry_points.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2024-05-07 10:06:02.000000 cmind-2.3.1/cmind.egg-info/not-zip-safe
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       39 2024-05-07 10:06:02.000000 cmind-2.3.1/cmind.egg-info/requires.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2024-05-07 10:06:02.000000 cmind-2.3.1/cmind.egg-info/top_level.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2024-05-07 10:06:02.400562 cmind-2.3.1/setup.cfg
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2913 2024-05-07 10:05:06.000000 cmind-2.3.1/setup.py
```

### Comparing `cmind-2.3.0/LICENSE.md` & `cmind-2.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cmind-2.3.0/PKG-INFO` & `cmind-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmind
-Version: 2.3.0
+Version: 2.3.1
 Summary: cmind
 Home-page: https://github.com/mlcommons/ck
 Author: Grigori Fursin
 Author-email: Grigori.Fursin@cTuning.org
 License: Apache 2.0
 Keywords: collective mind,cmind,ck3,cdatabase,cmeta,automation,portability,reusability,productivity,meta,JSON,YAML,python,api,cli
 Platform: UNKNOWN
```

### Comparing `cmind-2.3.0/README.md` & `cmind-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cmind-2.3.0/cmind/artifact.py` & `cmind-2.3.1/cmind/artifact.py`

 * *Files identical despite different names*

### Comparing `cmind-2.3.0/cmind/automation.py` & `cmind-2.3.1/cmind/automation.py`

 * *Files identical despite different names*

### Comparing `cmind-2.3.0/cmind/cli.py` & `cmind-2.3.1/cmind/cli.py`

 * *Files identical despite different names*

### Comparing `cmind-2.3.0/cmind/config.py` & `cmind-2.3.1/cmind/config.py`

 * *Files identical despite different names*

### Comparing `cmind-2.3.0/cmind/core.py` & `cmind-2.3.1/cmind/core.py`

 * *Files identical despite different names*

### Comparing `cmind-2.3.0/cmind/index.py` & `cmind-2.3.1/cmind/index.py`

 * *Files identical despite different names*

### Comparing `cmind-2.3.0/cmind/net.py` & `cmind-2.3.1/cmind/net.py`

 * *Files identical despite different names*

### Comparing `cmind-2.3.0/cmind/repo/automation/automation/README.md` & `cmind-2.3.1/cmind/repo/automation/automation/README.md`

 * *Files identical despite different names*

### Comparing `cmind-2.3.0/cmind/repo/automation/automation/module.py` & `cmind-2.3.1/cmind/repo/automation/automation/module.py`

 * *Files identical despite different names*

### Comparing `cmind-2.3.0/cmind/repo/automation/automation/module_dummy.py` & `cmind-2.3.1/cmind/repo/automation/automation/module_dummy.py`

 * *Files identical despite different names*

### Comparing `cmind-2.3.0/cmind/repo/automation/automation/module_misc.py` & `cmind-2.3.1/cmind/repo/automation/automation/module_misc.py`

 * *Files identical despite different names*

### Comparing `cmind-2.3.0/cmind/repo/automation/ckx/README.md` & `cmind-2.3.1/cmind/repo/automation/ckx/README.md`

 * *Files identical despite different names*

### Comparing `cmind-2.3.0/cmind/repo/automation/ckx/module.py` & `cmind-2.3.1/cmind/repo/automation/ckx/module.py`

 * *Files identical despite different names*

### Comparing `cmind-2.3.0/cmind/repo/automation/core/README.md` & `cmind-2.3.1/cmind/repo/automation/core/README.md`

 * *Files identical despite different names*

### Comparing `cmind-2.3.0/cmind/repo/automation/core/module.py` & `cmind-2.3.1/cmind/repo/automation/core/module.py`

 * *Files identical despite different names*

### Comparing `cmind-2.3.0/cmind/repo/automation/repo/README.md` & `cmind-2.3.1/cmind/repo/automation/repo/README.md`

 * *Files identical despite different names*

### Comparing `cmind-2.3.0/cmind/repo/automation/repo/module.py` & `cmind-2.3.1/cmind/repo/automation/repo/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # Written by Grigori Fursin
 
 import os
 
 from cmind.automation import Automation
 from cmind import utils
+from cmind import net
 
 class CAutomation(Automation):
     """
     CM "repo" automation actions
     """
 
     ############################################################
@@ -105,14 +106,19 @@
         else:
             # We are migrating cm-mlops repo from mlcommons@ck to a clean and new mlcommons@cm4mlops:
             # https://github.com/mlcommons/ck/issues/1215
             # As discussed, we should have a transparent redirect with a warning
             # unless branch/checkout is used - in such case we keep old repository
             # for backwards compatibility and reproducibility
 
+            r = net.request({'get': {'action': 'check-migration-repo-notes', 'repo': url}})
+            notes = r.get('dict', {}).get('notes','')
+            if notes !='':
+                print (notes)
+
             branch = i.get('branch', '')
             checkout = i.get('checkout', '')
 
             if alias == 'mlcommons@ck' and branch == '' and checkout == '':
                 print ('=========================================================================')
                 print ('Warning: mlcommons@ck was automatically changed to mlcommons@cm4mlops.')
                 print ('If you want to use older mlcommons@ck repository, use branch or checkout.')
```

### Comparing `cmind-2.3.0/cmind/repo.py` & `cmind-2.3.1/cmind/repo.py`

 * *Files identical despite different names*

### Comparing `cmind-2.3.0/cmind/repos.py` & `cmind-2.3.1/cmind/repos.py`

 * *Files identical despite different names*

### Comparing `cmind-2.3.0/cmind/utils.py` & `cmind-2.3.1/cmind/utils.py`

 * *Files identical despite different names*

### Comparing `cmind-2.3.0/cmind.egg-info/PKG-INFO` & `cmind-2.3.1/cmind.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmind
-Version: 2.3.0
+Version: 2.3.1
 Summary: cmind
 Home-page: https://github.com/mlcommons/ck
 Author: Grigori Fursin
 Author-email: Grigori.Fursin@cTuning.org
 License: Apache 2.0
 Keywords: collective mind,cmind,ck3,cdatabase,cmeta,automation,portability,reusability,productivity,meta,JSON,YAML,python,api,cli
 Platform: UNKNOWN
```

### Comparing `cmind-2.3.0/cmind.egg-info/SOURCES.txt` & `cmind-2.3.1/cmind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmind-2.3.0/setup.py` & `cmind-2.3.1/setup.py`

 * *Files identical despite different names*

