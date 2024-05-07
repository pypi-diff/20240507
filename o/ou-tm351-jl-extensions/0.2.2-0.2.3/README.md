# Comparing `tmp/ou_tm351_jl_extensions-0.2.2.tar.gz` & `tmp/ou_tm351_jl_extensions-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ou_tm351_jl_extensions-0.2.2.tar", max compression
+gzip compressed data, was "ou_tm351_jl_extensions-0.2.3.tar", max compression
```

## Comparing `ou_tm351_jl_extensions-0.2.2.tar` & `ou_tm351_jl_extensions-0.2.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1074 2023-07-21 20:51:46.057210 ou_tm351_jl_extensions-0.2.2/LICENSE
--rw-r--r--   0        0        0     1226 2023-07-21 20:51:46.057210 ou_tm351_jl_extensions-0.2.2/README.md
--rw-r--r--   0        0        0     2388 2023-07-21 20:51:46.061210 ou_tm351_jl_extensions-0.2.2/ou_tm351_jl_extensions/__init__.py
--rw-r--r--   0        0        0      937 2023-07-21 20:51:46.061210 ou_tm351_jl_extensions-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2603 1970-01-01 00:00:00.000000 ou_tm351_jl_extensions-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-04 10:46:43.497008 ou_tm351_jl_extensions-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1226 2023-07-21 20:49:34.016848 ou_tm351_jl_extensions-0.2.3/README.md
+-rw-r--r--   0        0        0     2388 2023-05-04 15:50:37.140962 ou_tm351_jl_extensions-0.2.3/ou_tm351_jl_extensions/__init__.py
+-rw-r--r--   0        0        0      937 2024-05-07 17:05:56.103793 ou_tm351_jl_extensions-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2583 1970-01-01 00:00:00.000000 ou_tm351_jl_extensions-0.2.3/PKG-INFO
```

### Comparing `ou_tm351_jl_extensions-0.2.2/LICENSE` & `ou_tm351_jl_extensions-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ou_tm351_jl_extensions-0.2.2/README.md` & `ou_tm351_jl_extensions-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ou_tm351_jl_extensions-0.2.2/ou_tm351_jl_extensions/__init__.py` & `ou_tm351_jl_extensions-0.2.3/ou_tm351_jl_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_tm351_jl_extensions-0.2.2/pyproject.toml` & `ou_tm351_jl_extensions-0.2.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "ou-tm351-jl-extensions"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = ["Tony Hirst <tony.hirst@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ou_tm351_jl_extensions"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13"
-jupyterlab = "^4.0.1"
-jupyterlab-ou-brand-extension = "^0.2.0"
+jupyterlab = ">=4.1"
+#jupyterlab-ou-brand-extension = "^0.2.0"
 jupyterlab-cell-status-extension = "^0.1.3"
-jupyterlab-myst = "^2.0.0"
-jupyterlab-empinken-extension = "^0.4.0"
+jupyterlab-myst = "^2.4.0"
+jupyterlab-empinken-extension = "^0.5.0"
 jupyterlab-geojson = "^3.3.1"
-jupyterlab-skip-traceback = "^5.0.0"
-jupyterlab-git = "^0.41.0"
-jupytext = "^1.14.5"
-jupyter-archive = "^3.3.4"
-jupyterlab-spellchecker = "^0.8.3"
-jupyterlab-language-pack-fr-fr = "^3.6.post1"
-jupyterlab-language-pack-zh-cn = "^3.6.post1"
-jupyter-resource-usage = "^0.7.2"
+jupyterlab-skip-traceback = "^5.1.0"
+jupyterlab-git = "^0.50.0"
+jupytext = "^1.16.0"
+jupyter-archive = "^3.4.0"
+jupyterlab-spellchecker = "^0.8.4"
+jupyterlab-language-pack-fr-fr = "^4.1.post2"
+jupyterlab-language-pack-zh-cn = "^4.1.post2"
+jupyter-resource-usage = "^1.0.2"
 stickyland = "^0.2.1"
 #jupyterlab-tour = "^3.1.4"
 jupyter-compare-view = "^0.2.4"
-jupyterlab-filesystem-access = "^0.5.3"
+jupyterlab-filesystem-access = "^0.6.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ou_tm351_jl_extensions-0.2.2/PKG-INFO` & `ou_tm351_jl_extensions-0.2.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: ou-tm351-jl-extensions
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: Tony Hirst
 Author-email: tony.hirst@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: jupyter-archive (>=3.3.4,<4.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: jupyter-archive (>=3.4.0,<4.0.0)
 Requires-Dist: jupyter-compare-view (>=0.2.4,<0.3.0)
-Requires-Dist: jupyter-resource-usage (>=0.7.2,<0.8.0)
-Requires-Dist: jupyterlab (>=4.0.1,<5.0.0)
+Requires-Dist: jupyter-resource-usage (>=1.0.2,<2.0.0)
+Requires-Dist: jupyterlab (>=4.1)
 Requires-Dist: jupyterlab-cell-status-extension (>=0.1.3,<0.2.0)
-Requires-Dist: jupyterlab-empinken-extension (>=0.4.0,<0.5.0)
-Requires-Dist: jupyterlab-filesystem-access (>=0.5.3,<0.6.0)
+Requires-Dist: jupyterlab-empinken-extension (>=0.5.0,<0.6.0)
+Requires-Dist: jupyterlab-filesystem-access (>=0.6.0,<0.7.0)
 Requires-Dist: jupyterlab-geojson (>=3.3.1,<4.0.0)
-Requires-Dist: jupyterlab-git (>=0.41.0,<0.42.0)
-Requires-Dist: jupyterlab-language-pack-fr-fr (>=3.6.post1,<4.0)
-Requires-Dist: jupyterlab-language-pack-zh-cn (>=3.6.post1,<4.0)
-Requires-Dist: jupyterlab-myst (>=2.0.0,<3.0.0)
-Requires-Dist: jupyterlab-ou-brand-extension (>=0.2.0,<0.3.0)
-Requires-Dist: jupyterlab-skip-traceback (>=5.0.0,<6.0.0)
-Requires-Dist: jupyterlab-spellchecker (>=0.8.3,<0.9.0)
-Requires-Dist: jupytext (>=1.14.5,<2.0.0)
+Requires-Dist: jupyterlab-git (>=0.50.0,<0.51.0)
+Requires-Dist: jupyterlab-language-pack-fr-fr (>=4.1.post2,<5.0)
+Requires-Dist: jupyterlab-language-pack-zh-cn (>=4.1.post2,<5.0)
+Requires-Dist: jupyterlab-myst (>=2.4.0,<3.0.0)
+Requires-Dist: jupyterlab-skip-traceback (>=5.1.0,<6.0.0)
+Requires-Dist: jupyterlab-spellchecker (>=0.8.4,<0.9.0)
+Requires-Dist: jupytext (>=1.16.0,<2.0.0)
 Requires-Dist: stickyland (>=0.2.1,<0.3.0)
 Description-Content-Type: text/markdown
 
 # ou-tm351-jl-extensions
 
 Install from pypi as `ou-tm351-jl-extensions`
```

