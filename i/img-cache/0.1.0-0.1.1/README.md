# Comparing `tmp/img_cache-0.1.0.tar.gz` & `tmp/img_cache-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "img_cache-0.1.0.tar", last modified: Mon May  6 13:48:18 2024, max compression
+gzip compressed data, was "img_cache-0.1.1.tar", last modified: Mon May  6 14:03:26 2024, max compression
```

## Comparing `img_cache-0.1.0.tar` & `img_cache-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 13:48:18.084911 img_cache-0.1.0/
--rw-rw-rw-   0        0        0      435 2024-05-06 13:48:18.084911 img_cache-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      225 2024-05-06 13:00:36.000000 img_cache-0.1.0/README.md
--rw-rw-rw-   0        0        0      914 2024-05-06 13:48:06.000000 img_cache-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-06 13:48:18.084911 img_cache-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-06 13:48:18.067939 img_cache-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 13:48:18.067939 img_cache-0.1.0/src/img_cache/
--rw-rw-rw-   0        0        0        0 2024-05-06 12:47:08.000000 img_cache-0.1.0/src/img_cache/__init__.py
--rw-rw-rw-   0        0        0      448 2024-05-06 13:43:24.000000 img_cache-0.1.0/src/img_cache/func.py
--rw-rw-rw-   0        0        0      903 2024-05-06 13:40:02.000000 img_cache-0.1.0/src/img_cache/sample.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:48:18.084911 img_cache-0.1.0/src/img_cache.egg-info/
--rw-rw-rw-   0        0        0      435 2024-05-06 13:48:18.000000 img_cache-0.1.0/src/img_cache.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-05-06 13:48:18.000000 img_cache-0.1.0/src/img_cache.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 13:48:18.000000 img_cache-0.1.0/src/img_cache.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-06 13:48:18.000000 img_cache-0.1.0/src/img_cache.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-06 13:48:18.084911 img_cache-0.1.0/tests/
--rw-rw-rw-   0        0        0     1677 2024-05-06 13:45:59.000000 img_cache-0.1.0/tests/test_func.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:03:26.818319 img_cache-0.1.1/
+-rw-rw-rw-   0        0        0      430 2024-05-06 14:03:26.818319 img_cache-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-05-06 13:00:36.000000 img_cache-0.1.1/README.md
+-rw-rw-rw-   0        0        0      930 2024-05-06 14:00:48.000000 img_cache-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 14:03:26.818319 img_cache-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 14:03:26.802694 img_cache-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 14:03:26.818319 img_cache-0.1.1/src/img_cache/
+-rw-rw-rw-   0        0        0        0 2024-05-06 12:47:08.000000 img_cache-0.1.1/src/img_cache/__init__.py
+-rw-rw-rw-   0        0        0      477 2024-05-06 13:58:57.000000 img_cache-0.1.1/src/img_cache/func.py
+-rw-rw-rw-   0        0        0      987 2024-05-06 14:00:39.000000 img_cache-0.1.1/src/img_cache/sample.py
+-rw-rw-rw-   0        0        0      187 2024-05-06 13:59:22.000000 img_cache-0.1.1/src/img_cache/types.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:03:26.818319 img_cache-0.1.1/src/img_cache.egg-info/
+-rw-rw-rw-   0        0        0      430 2024-05-06 14:03:26.000000 img_cache-0.1.1/src/img_cache.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2024-05-06 14:03:26.000000 img_cache-0.1.1/src/img_cache.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 14:03:26.000000 img_cache-0.1.1/src/img_cache.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-06 14:03:26.000000 img_cache-0.1.1/src/img_cache.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 14:03:26.818319 img_cache-0.1.1/tests/
+-rw-rw-rw-   0        0        0     1677 2024-05-06 13:45:59.000000 img_cache-0.1.1/tests/test_func.py
```

### Comparing `img_cache-0.1.0/pyproject.toml` & `img_cache-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [project]
 name = "img_cache"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = [
     {name = "svtter", email = "svtter@qq.com"},
     {name = "svtter", email = "svtter@163.com"},
 ]
 dependencies = [
 ]
 requires-python = "<4.0,>=3.9"
 readme = "README.md"
-license = {text = "not open"}
+license = {text = "BSD"}
 
 [tool.pdm]
 distribution = true
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest<8.0.0,>=7.2.0",
     "pytest-xdist<4.0.0,>=3.0.2",
     "pre-commit<3.0.0,>=2.20.0",
     "mkdocs<2.0.0,>=1.4.2",
     "mkdocs-material<9.0.0,>=8.5.11",
     "ruff>=0.4.3",
     "-e file:///${PROJECT_ROOT}/#egg=img-cache",
+    "twine>=5.0.0",
 ]
 
 [tool.pdm.build]
 includes = ["src/*"]
 
 [[tool.pdm.source]]
 name = "pypi"
```

### Comparing `img_cache-0.1.0/src/img_cache/sample.py` & `img_cache-0.1.1/src/img_cache/sample.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # sample function for judge_function, cache_function
 import typing as t
+from . import types as T
 
 # import functools
 
 
 def md5_serialize():
     # TODO: implement md5_serialize
     pass
 
 
-def memory_cache_func(serialize: t.Callable[[t.Any], str]):
+def memory_cache_func(serialize: T.Serialize) -> t.Tuple[T.ReadCache, T.WriteCache]:
     """save cache in memory
 
     serialize: serialize the img to normal string
     """
     return cache_func(lambda: {}, serialize)
 
 
-def cache_func(get_default_cache: t.Callable, serialize: t.Callable[[t.Any], str]):
-    """save cache in memory
+def cache_func(get_default_cache: t.Callable, serialize: T.Serialize) -> t.Tuple[T.ReadCache, T.WriteCache]:
+    """save cache in provided cache
 
     get_default_cache: return a default cache
     serialize: serialize the img to normal string
     """
     cache = get_default_cache()
 
     def read_cache(img):
```

### Comparing `img_cache-0.1.0/tests/test_func.py` & `img_cache-0.1.1/tests/test_func.py`

 * *Files identical despite different names*

