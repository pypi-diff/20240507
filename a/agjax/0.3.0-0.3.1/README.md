# Comparing `tmp/agjax-0.3.0.tar.gz` & `tmp/agjax-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agjax-0.3.0.tar", last modified: Wed Feb 21 04:04:10 2024, max compression
+gzip compressed data, was "agjax-0.3.1.tar", last modified: Tue May  7 19:13:43 2024, max compression
```

## Comparing `agjax-0.3.0.tar` & `agjax-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 04:04:10.512479 agjax-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-02-21 04:03:55.000000 agjax-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-02-21 04:04:10.512479 agjax-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-02-21 04:03:55.000000 agjax-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-02-21 04:03:55.000000 agjax-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 04:04:10.512479 agjax-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 04:04:10.508479 agjax-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 04:04:10.508479 agjax-0.3.0/src/agjax/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-21 04:03:55.000000 agjax-0.3.0/src/agjax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 04:04:10.508479 agjax-0.3.0/src/agjax/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-21 04:03:55.000000 agjax-0.3.0/src/agjax/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-02-21 04:03:55.000000 agjax-0.3.0/src/agjax/experimental/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 04:03:55.000000 agjax-0.3.0/src/agjax/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-02-21 04:03:55.000000 agjax-0.3.0/src/agjax/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-02-21 04:03:55.000000 agjax-0.3.0/src/agjax/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 04:04:10.508479 agjax-0.3.0/src/agjax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-02-21 04:04:10.000000 agjax-0.3.0/src/agjax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-02-21 04:04:10.000000 agjax-0.3.0/src/agjax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 04:04:10.000000 agjax-0.3.0/src/agjax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-21 04:04:10.000000 agjax-0.3.0/src/agjax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-21 04:04:10.000000 agjax-0.3.0/src/agjax.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 04:04:10.508479 agjax-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-02-21 04:03:55.000000 agjax-0.3.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-02-21 04:03:55.000000 agjax-0.3.0/tests/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:13:43.567096 agjax-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-07 19:13:32.000000 agjax-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-07 19:13:43.567096 agjax-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-07 19:13:32.000000 agjax-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-07 19:13:32.000000 agjax-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 19:13:43.567096 agjax-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:13:43.559096 agjax-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:13:43.563096 agjax-0.3.1/src/agjax/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-07 19:13:32.000000 agjax-0.3.1/src/agjax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:13:43.563096 agjax-0.3.1/src/agjax/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-07 19:13:32.000000 agjax-0.3.1/src/agjax/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-07 19:13:32.000000 agjax-0.3.1/src/agjax/experimental/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:13:32.000000 agjax-0.3.1/src/agjax/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-07 19:13:32.000000 agjax-0.3.1/src/agjax/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-07 19:13:32.000000 agjax-0.3.1/src/agjax/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:13:43.563096 agjax-0.3.1/src/agjax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-07 19:13:43.000000 agjax-0.3.1/src/agjax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-07 19:13:43.000000 agjax-0.3.1/src/agjax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:13:43.000000 agjax-0.3.1/src/agjax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-07 19:13:43.000000 agjax-0.3.1/src/agjax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 19:13:43.000000 agjax-0.3.1/src/agjax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:13:43.563096 agjax-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-07 19:13:32.000000 agjax-0.3.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-05-07 19:13:32.000000 agjax-0.3.1/tests/test_wrapper.py
```

### Comparing `agjax-0.3.0/LICENSE` & `agjax-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `agjax-0.3.0/PKG-INFO` & `agjax-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agjax
-Version: 0.3.0
+Version: 0.3.1
 Summary: A jax wrapper for autograd-differentiable functions.
 Author-email: "Martin F. Schubert" <mfschubert@gmail.com>
 Maintainer-email: "Martin F. Schubert" <mfschubert@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Martin Schubert
         
@@ -42,22 +42,22 @@
 Provides-Extra: docs
 Requires-Dist: matplotlib; extra == "docs"
 Requires-Dist: jupyter-book==1.0.0; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: sphinx-click; extra == "docs"
 Requires-Dist: ceviche_challenges; extra == "docs"
 Provides-Extra: dev
-Requires-Dist: agjax[examples,tests]; extra == "dev"
+Requires-Dist: agjax[docs,tests]; extra == "dev"
 Requires-Dist: bump-my-version; extra == "dev"
 Requires-Dist: darglint; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 
 # Agjax -- jax wrapper for autograd-differentiable functions.
-`v0.3.0`
+`v0.3.1`
 
 Agjax allows existing code built with autograd to be used with the jax framework.
 
 In particular, `agjax.wrap_for_jax` allows arbitrary autograd functions ot be differentiated using `jax.grad`. Several other function transformations (e.g. compilation via `jax.jit`) are not supported.
 
 Meanwhile, `agjax.experimental.wrap_for_jax` supports `grad`, `jit`, `vmap`, and `jacrev`. However, it depends on certain under-the-hood behavior by jax, which is not guaranteed to remain unchanged. It also is more restrictive in terms of the valid function signatures of functions to be wrapped: all arguments and outputs must be convertible to valid jax types. (`agjax.wrap_for_jax` also supports non-jax inputs and outputs, e.g. strings.)
 
@@ -90,15 +90,15 @@
 # [[ 0.28366217  0.          0.          0.          0.        ]
 #  [ 0.          0.96017027  0.          0.          0.        ]
 #  [ 0.          0.          0.75390226  0.          0.        ]
 #  [ 0.          0.          0.         -0.14550003  0.        ]
 #  [ 0.          0.          0.          0.         -0.91113025]]
 ```
 
-Agjax wrappers are intended to be quite general, and can support functions with multiple inputs and outputs as well as functions that have nondifferentiable outputs or arguments that cannot be differentiated with respect to. These should be specified using `nondiff_argnums` and `nondiff_outputnums` arguments. In the experimental wrapper, these must still be jax-convertible types, while in the standard wrapper they may have arbitrary typess.
+Agjax wrappers are intended to be quite general, and can support functions with multiple inputs and outputs as well as functions that have nondifferentiable outputs or arguments that cannot be differentiated with respect to. These should be specified using `nondiff_argnums` and `nondiff_outputnums` arguments. In the experimental wrapper, these must still be jax-convertible types, while in the standard wrapper they may have arbitrary types.
 
 ```python
 @functools.partial(
   agjax.wrap_for_jax, nondiff_argnums=(2,), nondiff_outputnums=(1,)
 )
 def fn(x, y, string_arg):
   return x * npa.cos(y), string_arg * 2
```

### Comparing `agjax-0.3.0/README.md` & `agjax-0.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Agjax -- jax wrapper for autograd-differentiable functions.
-`v0.3.0`
+`v0.3.1`
 
 Agjax allows existing code built with autograd to be used with the jax framework.
 
 In particular, `agjax.wrap_for_jax` allows arbitrary autograd functions ot be differentiated using `jax.grad`. Several other function transformations (e.g. compilation via `jax.jit`) are not supported.
 
 Meanwhile, `agjax.experimental.wrap_for_jax` supports `grad`, `jit`, `vmap`, and `jacrev`. However, it depends on certain under-the-hood behavior by jax, which is not guaranteed to remain unchanged. It also is more restrictive in terms of the valid function signatures of functions to be wrapped: all arguments and outputs must be convertible to valid jax types. (`agjax.wrap_for_jax` also supports non-jax inputs and outputs, e.g. strings.)
 
@@ -36,15 +36,15 @@
 # [[ 0.28366217  0.          0.          0.          0.        ]
 #  [ 0.          0.96017027  0.          0.          0.        ]
 #  [ 0.          0.          0.75390226  0.          0.        ]
 #  [ 0.          0.          0.         -0.14550003  0.        ]
 #  [ 0.          0.          0.          0.         -0.91113025]]
 ```
 
-Agjax wrappers are intended to be quite general, and can support functions with multiple inputs and outputs as well as functions that have nondifferentiable outputs or arguments that cannot be differentiated with respect to. These should be specified using `nondiff_argnums` and `nondiff_outputnums` arguments. In the experimental wrapper, these must still be jax-convertible types, while in the standard wrapper they may have arbitrary typess.
+Agjax wrappers are intended to be quite general, and can support functions with multiple inputs and outputs as well as functions that have nondifferentiable outputs or arguments that cannot be differentiated with respect to. These should be specified using `nondiff_argnums` and `nondiff_outputnums` arguments. In the experimental wrapper, these must still be jax-convertible types, while in the standard wrapper they may have arbitrary types.
 
 ```python
 @functools.partial(
   agjax.wrap_for_jax, nondiff_argnums=(2,), nondiff_outputnums=(1,)
 )
 def fn(x, y, string_arg):
   return x * npa.cos(y), string_arg * 2
```

### Comparing `agjax-0.3.0/pyproject.toml` & `agjax-0.3.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "agjax"
-version = "v0.3.0"
+version = "v0.3.1"
 description = "A jax wrapper for autograd-differentiable functions."
 keywords = ["autograd", "jax", "python", "wrapper", "gradient"]
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 
 authors = [
@@ -33,27 +33,27 @@
     "matplotlib",
     "jupyter-book==1.0.0",
     "sphinx-autodoc-typehints",
     "sphinx-click",
     "ceviche_challenges",
 ]
 dev = [
-    "agjax[tests, examples]",
+    "agjax[tests, docs]",
     "bump-my-version",
     "darglint",
     "mypy",
     "pre-commit",
 ]
 
 [build-system]
 requires = ["setuptools>=45", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.package-data]
-"invrs_gym" = ["py.typed"]
+"agjax" = ["py.typed"]
 
 [tool.pytest.ini_options]
 addopts = ["--import-mode=importlib"]  # Allow tests with same name in different dirs.
 pythonpath = ["src"]
 
 [tool.black]
 line-length = 88
```

### Comparing `agjax-0.3.0/src/agjax/experimental/wrapper.py` & `agjax-0.3.1/src/agjax/experimental/wrapper.py`

 * *Files identical despite different names*

### Comparing `agjax-0.3.0/src/agjax/utils.py` & `agjax-0.3.1/src/agjax/utils.py`

 * *Files identical despite different names*

### Comparing `agjax-0.3.0/src/agjax/wrapper.py` & `agjax-0.3.1/src/agjax/wrapper.py`

 * *Files identical despite different names*

### Comparing `agjax-0.3.0/src/agjax.egg-info/PKG-INFO` & `agjax-0.3.1/src/agjax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agjax
-Version: 0.3.0
+Version: 0.3.1
 Summary: A jax wrapper for autograd-differentiable functions.
 Author-email: "Martin F. Schubert" <mfschubert@gmail.com>
 Maintainer-email: "Martin F. Schubert" <mfschubert@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Martin Schubert
         
@@ -42,22 +42,22 @@
 Provides-Extra: docs
 Requires-Dist: matplotlib; extra == "docs"
 Requires-Dist: jupyter-book==1.0.0; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: sphinx-click; extra == "docs"
 Requires-Dist: ceviche_challenges; extra == "docs"
 Provides-Extra: dev
-Requires-Dist: agjax[examples,tests]; extra == "dev"
+Requires-Dist: agjax[docs,tests]; extra == "dev"
 Requires-Dist: bump-my-version; extra == "dev"
 Requires-Dist: darglint; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 
 # Agjax -- jax wrapper for autograd-differentiable functions.
-`v0.3.0`
+`v0.3.1`
 
 Agjax allows existing code built with autograd to be used with the jax framework.
 
 In particular, `agjax.wrap_for_jax` allows arbitrary autograd functions ot be differentiated using `jax.grad`. Several other function transformations (e.g. compilation via `jax.jit`) are not supported.
 
 Meanwhile, `agjax.experimental.wrap_for_jax` supports `grad`, `jit`, `vmap`, and `jacrev`. However, it depends on certain under-the-hood behavior by jax, which is not guaranteed to remain unchanged. It also is more restrictive in terms of the valid function signatures of functions to be wrapped: all arguments and outputs must be convertible to valid jax types. (`agjax.wrap_for_jax` also supports non-jax inputs and outputs, e.g. strings.)
 
@@ -90,15 +90,15 @@
 # [[ 0.28366217  0.          0.          0.          0.        ]
 #  [ 0.          0.96017027  0.          0.          0.        ]
 #  [ 0.          0.          0.75390226  0.          0.        ]
 #  [ 0.          0.          0.         -0.14550003  0.        ]
 #  [ 0.          0.          0.          0.         -0.91113025]]
 ```
 
-Agjax wrappers are intended to be quite general, and can support functions with multiple inputs and outputs as well as functions that have nondifferentiable outputs or arguments that cannot be differentiated with respect to. These should be specified using `nondiff_argnums` and `nondiff_outputnums` arguments. In the experimental wrapper, these must still be jax-convertible types, while in the standard wrapper they may have arbitrary typess.
+Agjax wrappers are intended to be quite general, and can support functions with multiple inputs and outputs as well as functions that have nondifferentiable outputs or arguments that cannot be differentiated with respect to. These should be specified using `nondiff_argnums` and `nondiff_outputnums` arguments. In the experimental wrapper, these must still be jax-convertible types, while in the standard wrapper they may have arbitrary types.
 
 ```python
 @functools.partial(
   agjax.wrap_for_jax, nondiff_argnums=(2,), nondiff_outputnums=(1,)
 )
 def fn(x, y, string_arg):
   return x * npa.cos(y), string_arg * 2
```

### Comparing `agjax-0.3.0/tests/test_utils.py` & `agjax-0.3.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `agjax-0.3.0/tests/test_wrapper.py` & `agjax-0.3.1/tests/test_wrapper.py`

 * *Files identical despite different names*

