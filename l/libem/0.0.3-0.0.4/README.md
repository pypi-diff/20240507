# Comparing `tmp/libem-0.0.3.tar.gz` & `tmp/libem-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libem-0.0.3.tar", last modified: Sun May  5 08:34:54 2024, max compression
+gzip compressed data, was "libem-0.0.4.tar", last modified: Tue May  7 17:34:10 2024, max compression
```

## Comparing `libem-0.0.3.tar` & `libem-0.0.4.tar`

### file list

```diff
@@ -1,44 +1,83 @@
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-05 08:34:54.410372 libem-0.0.3/
--rw-r--r--   0 silv       (501) staff       (20)    11357 2024-05-01 02:16:29.000000 libem-0.0.3/LICENSE
--rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-05 08:34:54.410233 libem-0.0.3/PKG-INFO
--rw-r--r--   0 silv       (501) staff       (20)      370 2024-05-05 04:20:33.000000 libem-0.0.3/README.md
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-05 08:34:54.405141 libem-0.0.3/libem/
--rw-r--r--   0 silv       (501) staff       (20)      809 2024-05-05 04:27:53.000000 libem-0.0.3/libem/__init__.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-05 08:34:54.406597 libem-0.0.3/libem/browse/
--rw-r--r--   0 silv       (501) staff       (20)       92 2024-05-05 00:16:54.000000 libem-0.0.3/libem/browse/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     1542 2024-05-03 17:04:24.000000 libem-0.0.3/libem/browse/function.py
--rw-r--r--   0 silv       (501) staff       (20)       85 2024-05-05 01:29:22.000000 libem-0.0.3/libem/browse/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-02 20:20:44.000000 libem-0.0.3/libem/browse/prompt.py
--rw-r--r--   0 silv       (501) staff       (20)      364 2024-05-03 17:03:58.000000 libem-0.0.3/libem/constant.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-05 08:34:54.407305 libem-0.0.3/libem/core/
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:45:38.000000 libem-0.0.3/libem/core/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-05 04:39:03.000000 libem-0.0.3/libem/core/eval.py
--rw-r--r--   0 silv       (501) staff       (20)     2909 2024-05-05 08:08:09.000000 libem-0.0.3/libem/core/model.py
--rw-r--r--   0 silv       (501) staff       (20)      809 2024-05-05 00:31:17.000000 libem-0.0.3/libem/core/struct.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-05 04:43:57.000000 libem-0.0.3/libem/core/tune.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-05 08:34:54.407976 libem-0.0.3/libem/match/
--rw-r--r--   0 silv       (501) staff       (20)       90 2024-05-05 00:16:44.000000 libem-0.0.3/libem/match/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     1184 2024-05-05 07:47:38.000000 libem-0.0.3/libem/match/function.py
--rw-r--r--   0 silv       (501) staff       (20)      215 2024-05-05 08:08:52.000000 libem-0.0.3/libem/match/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)      429 2024-05-05 04:34:57.000000 libem-0.0.3/libem/match/prompt.py
--rw-r--r--   0 silv       (501) staff       (20)      216 2024-05-04 23:40:49.000000 libem-0.0.3/libem/parameter.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-05 08:34:54.408993 libem-0.0.3/libem/prepare/
--rw-r--r--   0 silv       (501) staff       (20)       94 2024-05-05 04:43:06.000000 libem-0.0.3/libem/prepare/__init__.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-05 08:34:54.409518 libem-0.0.3/libem/prepare/datasets/
--rw-r--r--   0 silv       (501) staff       (20)      197 2024-05-05 06:12:44.000000 libem-0.0.3/libem/prepare/datasets/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     2403 2024-05-05 07:13:45.000000 libem-0.0.3/libem/prepare/datasets/amazon_google.py
--rw-r--r--   0 silv       (501) staff       (20)       41 2024-05-05 04:43:28.000000 libem-0.0.3/libem/prepare/function.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:17:55.000000 libem-0.0.3/libem/prepare/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-05 00:06:37.000000 libem-0.0.3/libem/prepare/prompt.py
--rw-r--r--   0 silv       (501) staff       (20)      185 2024-05-05 01:22:34.000000 libem-0.0.3/libem/prompt.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-05 08:34:54.405719 libem-0.0.3/libem.egg-info/
--rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-05 08:34:54.000000 libem-0.0.3/libem.egg-info/PKG-INFO
--rw-r--r--   0 silv       (501) staff       (20)      746 2024-05-05 08:34:54.000000 libem-0.0.3/libem.egg-info/SOURCES.txt
--rw-r--r--   0 silv       (501) staff       (20)        1 2024-05-05 08:34:54.000000 libem-0.0.3/libem.egg-info/dependency_links.txt
--rw-r--r--   0 silv       (501) staff       (20)      133 2024-05-05 08:34:54.000000 libem-0.0.3/libem.egg-info/requires.txt
--rw-r--r--   0 silv       (501) staff       (20)       12 2024-05-05 08:34:54.000000 libem-0.0.3/libem.egg-info/top_level.txt
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-05 08:34:54.409878 libem-0.0.3/serve/
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-04 23:17:56.000000 libem-0.0.3/serve/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)      578 2024-05-04 23:21:19.000000 libem-0.0.3/serve/run.py
--rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-05 08:34:54.410407 libem-0.0.3/setup.cfg
--rw-r--r--   0 silv       (501) staff       (20)      421 2024-05-05 08:34:44.000000 libem-0.0.3/setup.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.918170 libem-0.0.4/
+-rw-r--r--   0 silv       (501) staff       (20)    11357 2024-05-01 02:16:29.000000 libem-0.0.4/LICENSE
+-rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-07 17:34:10.918032 libem-0.0.4/PKG-INFO
+-rw-r--r--   0 silv       (501) staff       (20)      550 2024-05-07 02:02:55.000000 libem-0.0.4/README.md
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.906209 libem-0.0.4/cli/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-05 16:25:37.000000 libem-0.0.4/cli/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)      509 2024-05-06 01:35:06.000000 libem-0.0.4/cli/libem
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.908133 libem-0.0.4/libem/
+-rw-r--r--   0 silv       (501) staff       (20)      144 2024-05-07 06:32:51.000000 libem-0.0.4/libem/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.909707 libem-0.0.4/libem/browse/
+-rw-r--r--   0 silv       (501) staff       (20)       92 2024-05-05 00:16:54.000000 libem-0.0.4/libem/browse/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     1542 2024-05-03 17:04:24.000000 libem-0.0.4/libem/browse/function.py
+-rw-r--r--   0 silv       (501) staff       (20)       85 2024-05-05 01:29:22.000000 libem-0.0.4/libem/browse/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-02 20:20:44.000000 libem-0.0.4/libem/browse/prompt.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.910261 libem-0.0.4/libem/calibrate/
+-rw-r--r--   0 silv       (501) staff       (20)       98 2024-05-07 16:02:23.000000 libem-0.0.4/libem/calibrate/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)      711 2024-05-07 17:18:26.000000 libem-0.0.4/libem/calibrate/function.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:18:01.000000 libem-0.0.4/libem/calibrate/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:18:01.000000 libem-0.0.4/libem/calibrate/prompt.py
+-rw-r--r--   0 silv       (501) staff       (20)      422 2024-05-05 16:22:40.000000 libem-0.0.4/libem/constant.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.910958 libem-0.0.4/libem/core/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:45:38.000000 libem-0.0.4/libem/core/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)      651 2024-05-06 01:38:58.000000 libem-0.0.4/libem/core/eval.py
+-rw-r--r--   0 silv       (501) staff       (20)     2991 2024-05-07 17:07:28.000000 libem-0.0.4/libem/core/model.py
+-rw-r--r--   0 silv       (501) staff       (20)     1097 2024-05-06 01:44:20.000000 libem-0.0.4/libem/core/struct.py
+-rw-r--r--   0 silv       (501) staff       (20)       35 2024-05-07 06:37:47.000000 libem-0.0.4/libem/function.py
+-rw-r--r--   0 silv       (501) staff       (20)      836 2024-05-07 17:32:21.000000 libem-0.0.4/libem/interface.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.911889 libem-0.0.4/libem/match/
+-rw-r--r--   0 silv       (501) staff       (20)       90 2024-05-05 00:16:44.000000 libem-0.0.4/libem/match/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     1126 2024-05-07 16:02:52.000000 libem-0.0.4/libem/match/function.py
+-rw-r--r--   0 silv       (501) staff       (20)      197 2024-05-07 17:01:12.000000 libem-0.0.4/libem/match/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)      429 2024-05-07 16:31:34.000000 libem-0.0.4/libem/match/prompt.py
+-rw-r--r--   0 silv       (501) staff       (20)      216 2024-05-07 06:42:34.000000 libem-0.0.4/libem/parameter.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.912794 libem-0.0.4/libem/prepare/
+-rw-r--r--   0 silv       (501) staff       (20)       94 2024-05-05 04:43:06.000000 libem-0.0.4/libem/prepare/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.914408 libem-0.0.4/libem/prepare/datasets/
+-rw-r--r--   0 silv       (501) staff       (20)      197 2024-05-05 06:12:44.000000 libem-0.0.4/libem/prepare/datasets/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     2842 2024-05-07 02:22:18.000000 libem-0.0.4/libem/prepare/datasets/abt_buy.py
+-rw-r--r--   0 silv       (501) staff       (20)     2465 2024-05-07 02:18:30.000000 libem-0.0.4/libem/prepare/datasets/amazon_google.py
+-rw-r--r--   0 silv       (501) staff       (20)     2637 2024-05-07 02:20:12.000000 libem-0.0.4/libem/prepare/datasets/dblp_acm.py
+-rw-r--r--   0 silv       (501) staff       (20)     2618 2024-05-07 02:20:21.000000 libem-0.0.4/libem/prepare/datasets/dblp_scholar.py
+-rw-r--r--   0 silv       (501) staff       (20)     2646 2024-05-07 02:20:28.000000 libem-0.0.4/libem/prepare/datasets/walmart_amazon.py
+-rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-06 01:50:49.000000 libem-0.0.4/libem/prepare/function.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:17:55.000000 libem-0.0.4/libem/prepare/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-05 00:06:37.000000 libem-0.0.4/libem/prepare/prompt.py
+-rw-r--r--   0 silv       (501) staff       (20)      204 2024-05-07 15:43:38.000000 libem-0.0.4/libem/prompt.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.915185 libem-0.0.4/libem/tune/
+-rw-r--r--   0 silv       (501) staff       (20)       88 2024-05-07 06:19:35.000000 libem-0.0.4/libem/tune/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:18:54.000000 libem-0.0.4/libem/tune/function.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.915793 libem-0.0.4/libem/tune/learn/
+-rw-r--r--   0 silv       (501) staff       (20)       95 2024-05-07 06:21:06.000000 libem-0.0.4/libem/tune/learn/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:19:04.000000 libem-0.0.4/libem/tune/learn/function.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:18:01.000000 libem-0.0.4/libem/tune/learn/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:18:01.000000 libem-0.0.4/libem/tune/learn/prompt.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.916402 libem-0.0.4/libem/tune/load/
+-rw-r--r--   0 silv       (501) staff       (20)       93 2024-05-07 06:19:35.000000 libem-0.0.4/libem/tune/load/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:19:05.000000 libem-0.0.4/libem/tune/load/function.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:18:01.000000 libem-0.0.4/libem/tune/load/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:18:01.000000 libem-0.0.4/libem/tune/load/prompt.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:18:01.000000 libem-0.0.4/libem/tune/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:18:01.000000 libem-0.0.4/libem/tune/prompt.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.916946 libem-0.0.4/libem/tune/save/
+-rw-r--r--   0 silv       (501) staff       (20)       93 2024-05-07 06:19:35.000000 libem-0.0.4/libem/tune/save/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:19:04.000000 libem-0.0.4/libem/tune/save/function.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:18:01.000000 libem-0.0.4/libem/tune/save/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:18:01.000000 libem-0.0.4/libem/tune/save/prompt.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.917523 libem-0.0.4/libem/tune/search/
+-rw-r--r--   0 silv       (501) staff       (20)       97 2024-05-07 06:21:06.000000 libem-0.0.4/libem/tune/search/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)      139 2024-05-07 06:36:20.000000 libem-0.0.4/libem/tune/search/function.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:18:01.000000 libem-0.0.4/libem/tune/search/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:18:01.000000 libem-0.0.4/libem/tune/search/prompt.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:26:56.000000 libem-0.0.4/libem/tune/storage.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.908861 libem-0.0.4/libem.egg-info/
+-rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-07 17:34:10.000000 libem-0.0.4/libem.egg-info/PKG-INFO
+-rw-r--r--   0 silv       (501) staff       (20)     1619 2024-05-07 17:34:10.000000 libem-0.0.4/libem.egg-info/SOURCES.txt
+-rw-r--r--   0 silv       (501) staff       (20)        1 2024-05-07 17:34:10.000000 libem-0.0.4/libem.egg-info/dependency_links.txt
+-rw-r--r--   0 silv       (501) staff       (20)      133 2024-05-07 17:34:10.000000 libem-0.0.4/libem.egg-info/requires.txt
+-rw-r--r--   0 silv       (501) staff       (20)       16 2024-05-07 17:34:10.000000 libem-0.0.4/libem.egg-info/top_level.txt
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-07 17:34:10.917727 libem-0.0.4/serve/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-04 23:17:56.000000 libem-0.0.4/serve/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)      578 2024-05-04 23:21:19.000000 libem-0.0.4/serve/run.py
+-rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-07 17:34:10.918205 libem-0.0.4/setup.cfg
+-rw-r--r--   0 silv       (501) staff       (20)      449 2024-05-07 17:34:06.000000 libem-0.0.4/setup.py
```

### Comparing `libem-0.0.3/LICENSE` & `libem-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `libem-0.0.3/libem/__init__.py` & `libem-0.0.4/libem/interface.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 import random
 
-from libem.constant import *
-
 import libem.core.model as model
 from libem.core.struct import Prompt
 
 from libem import prompt, parameter
-from libem import match as match_tool
+
+"""Chat interface"""
 
 
 def chat(message):
-    """Simple chat interface for libem"""
     return model.call(
         prompt=Prompt.join(prompt.role(), message, sep="\n"),
-        tools=[match_tool],
+        tools=["libem.match"],
         model=parameter.model(),
         temperature=parameter.temperature(),
     )
 
 
-from libem.match import function
+"""Programming interface"""
+from libem.match import func as match_func
 
 
 def match(left, right,
           always=None,
           guess=False,
           seed=42) -> str:
-    """Programming interface for entity matching"""
     if always is not None:
         return always
 
     if guess:
         random.seed(seed)
         return random.choice(["yes", "no"])
 
-    return function.match(left, right)
+    return match_func(left, right)
+
+
+from libem.calibrate import func as calibrate_func
+
+
+def calibrate(*args, **kwargs):
+    return calibrate_func(*args, **kwargs)
```

### Comparing `libem-0.0.3/libem/browse/function.py` & `libem-0.0.4/libem/browse/function.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.3/libem/core/model.py` & `libem-0.0.4/libem/core/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import json
-import types
+import importlib
 
 from openai import OpenAI
 
 import libem
 
 
 def call(*args, **kwargs) -> str:
@@ -16,15 +16,15 @@
 os.environ.setdefault(
     "OPENAI_API_KEY",
     libem.LIBEM_CONFIG.get("OPENAI_API_KEY", "")
 )
 
 
 # LLM call with multiple rounds of tool use
-def openai(prompt: str, tools: list[types.ModuleType],
+def openai(prompt: str, tools: list[str],
            model: str, temperature: float,
            max_model_call: int = 3) -> str:
     if not os.environ.get("OPENAI_API_KEY"):
         raise EnvironmentError(f"OPENAI_API_KEY is not set. "
                                f"Check your environment or {libem.LIBEM_CONFIG_FILE}.")
     client = OpenAI()
 
@@ -34,14 +34,17 @@
             model=model,
             messages=[{"role": "user", "content": prompt}],
             temperature=temperature,
         )
         return response.choices[0].message.content
 
     """ Call with tools """
+    # Load the tool modules
+    tools = [importlib.import_module(tool) for tool in tools]
+
     # Get the functions from the tools
     available_functions = {
         tool.name: tool.func for tool in tools
     }
     # Get the schema from the tools
     tools = [tool.schema for tool in tools]
```

### Comparing `libem-0.0.3/libem/match/function.py` & `libem-0.0.4/libem/match/function.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from libem.match import prompt, parameter
 from libem.core.struct import Prompt
 import libem.core.model as model
 
-
-
 schema = {
     "type": "function",
     "function": {
         "name": "match",
         "description": "Perform entity matching given two entity description.",
         "parameters": {
             "type": "object",
@@ -24,18 +22,14 @@
             "required": ["left", "right"],
         },
     }
 }
 
 
 def func(left, right):
-    return match(left, right)
-
-
-def match(left, right):
     return model.call(
         prompt=Prompt.join(
             prompt.query(
                 left=left,
                 right=right
             ),
             prompt.output(),
```

### Comparing `libem-0.0.3/libem/prepare/datasets/amazon_google.py` & `libem-0.0.4/libem/prepare/datasets/walmart_amazon.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 import json
 
 import libem.prepare.datasets as datasets
 
-path = os.path.join(datasets.LIBEM_SAMPLE_DATA_PATH, "amazon-google")
+path = os.path.join(datasets.LIBEM_SAMPLE_DATA_PATH, "walmart-amazon")
 test_file = os.path.join(path, "test.ndjson")
 train_file = os.path.join(path, "train.ndjson")
 valid_file = os.path.join(path, "valid.ndjson")
 
 
-def read_test(schema=True):
-    # sample data:
-    # {"id_left":"amazon_1191","title_left":"sims 2 glamour life stuff pack","manufacturer_left":"aspyr media","price_left":24.99,"cluster_id_left":810,
-    #  "id_right":"google_567","title_right":"aspyr media inc sims 2 glamour life stuff pack","manufacturer_right":null,"price_right":23.44,"cluster_id_right":810,
-    #  "label":1,"pair_id":"amazon_1191#google_567"}
-    with open(test_file) as f:
+# sample data:
+# {"id_left":"walmart_88","title_left":"balt wheasel easel adjustable melamine dry erase board white","category_left":"stationery & office machinery","brand_left":"balt","modelno_left":"33250","price_left":239.88,"cluster_id_left":463,
+# "id_right":"amazon_3269","title_right":"balt inc. wheasel easel adjustable melamine dry erase board 28 3 4 x 59 1 2 white","category_right":"laminating supplies","brand_right":"mayline","modelno_right":null,"price_right":134.45,"cluster_id_right":463,
+# "label":1,"pair_id":"walmart_88#amazon_3269"}
+def read(file, schema=True):
+    with open(file) as f:
         for line in f:
             data = json.loads(line.strip())
             parsed_data = {'left': {}, 'right': {}, 'label': data.get('label', None)}
 
             # clean the data
             trim = ["cluster_id_left", "cluster_id_right", "id_left", "id_right"]
             if schema:
@@ -45,16 +45,20 @@
                         right_values.append(str(value))
                 parsed_data['left'] = ' '.join(left_values)
                 parsed_data['right'] = ' '.join(right_values)
 
             yield parsed_data
 
 
-def read_train():
-    raise NotImplementedError
+def read_test(schema=True):
+    return read(test_file, schema)
+
+
+def read_train(schema=True):
+    return read(train_file, schema)
 
 
 def read_valid():
     raise NotImplementedError
 
 
 if __name__ == "__main__":
```

### Comparing `libem-0.0.3/serve/run.py` & `libem-0.0.4/serve/run.py`

 * *Files identical despite different names*

