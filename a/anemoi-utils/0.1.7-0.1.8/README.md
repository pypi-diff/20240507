# Comparing `tmp/anemoi_utils-0.1.7.tar.gz` & `tmp/anemoi_utils-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anemoi_utils-0.1.7.tar", last modified: Thu May  2 12:29:13 2024, max compression
+gzip compressed data, was "anemoi_utils-0.1.8.tar", last modified: Tue May  7 09:05:12 2024, max compression
```

## Comparing `anemoi_utils-0.1.7.tar` & `anemoi_utils-0.1.8.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:29:13.537678 anemoi_utils-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:29:13.525678 anemoi_utils-0.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:29:13.529678 anemoi_utils-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15090 2024-05-02 12:29:13.537678 anemoi_utils-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:29:13.529678 anemoi_utils-0.1.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:29:13.529678 anemoi_utils-0.1.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:29:13.529678 anemoi_utils-0.1.7/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/installing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:29:13.529678 anemoi_utils-0.1.7/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/modules/checkpoints.rst
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/modules/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/modules/dates.rst
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/modules/grib.rst
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/modules/humanize.rst
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/modules/provenance.rst
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/modules/text.rst
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 12:29:13.537678 anemoi_utils-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:29:13.525678 anemoi_utils-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:29:13.525678 anemoi_utils-0.1.7/src/anemoi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:29:13.533678 anemoi_utils-0.1.7/src/anemoi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/src/anemoi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 12:29:13.000000 anemoi_utils-0.1.7/src/anemoi/utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/src/anemoi/utils/checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/src/anemoi/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/src/anemoi/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/src/anemoi/utils/grib.py
--rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/src/anemoi/utils/humanize.py
--rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/src/anemoi/utils/provenance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8599 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/src/anemoi/utils/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:29:13.533678 anemoi_utils-0.1.7/src/anemoi_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15090 2024-05-02 12:29:13.000000 anemoi_utils-0.1.7/src/anemoi_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-02 12:29:13.000000 anemoi_utils-0.1.7/src/anemoi_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:29:13.000000 anemoi_utils-0.1.7/src/anemoi_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-02 12:29:13.000000 anemoi_utils-0.1.7/src/anemoi_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 12:29:13.000000 anemoi_utils-0.1.7/src/anemoi_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:29:13.533678 anemoi_utils-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:12.993716 anemoi_utils-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:12.985716 anemoi_utils-0.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:12.985716 anemoi_utils-0.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15090 2024-05-07 09:05:12.993716 anemoi_utils-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:12.989716 anemoi_utils-0.1.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:12.989716 anemoi_utils-0.1.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:12.989716 anemoi_utils-0.1.8/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/installing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:12.989716 anemoi_utils-0.1.8/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/modules/checkpoints.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/modules/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/modules/dates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/modules/grib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/modules/humanize.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/modules/provenance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/modules/text.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 09:05:12.993716 anemoi_utils-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:12.985716 anemoi_utils-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:12.985716 anemoi_utils-0.1.8/src/anemoi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:12.989716 anemoi_utils-0.1.8/src/anemoi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/src/anemoi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 09:05:12.000000 anemoi_utils-0.1.8/src/anemoi/utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/src/anemoi/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/src/anemoi/utils/checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/src/anemoi/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/src/anemoi/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/src/anemoi/utils/grib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/src/anemoi/utils/humanize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/src/anemoi/utils/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8599 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/src/anemoi/utils/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:12.993716 anemoi_utils-0.1.8/src/anemoi_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15090 2024-05-07 09:05:12.000000 anemoi_utils-0.1.8/src/anemoi_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-07 09:05:12.000000 anemoi_utils-0.1.8/src/anemoi_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:05:12.000000 anemoi_utils-0.1.8/src/anemoi_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-07 09:05:12.000000 anemoi_utils-0.1.8/src/anemoi_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 09:05:12.000000 anemoi_utils-0.1.8/src/anemoi_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:12.993716 anemoi_utils-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/tests/test_utils.py
```

### Comparing `anemoi_utils-0.1.7/.github/workflows/python-publish.yml` & `anemoi_utils-0.1.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.7/.gitignore` & `anemoi_utils-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.7/.pre-commit-config.yaml` & `anemoi_utils-0.1.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.7/LICENSE` & `anemoi_utils-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.7/PKG-INFO` & `anemoi_utils-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anemoi-utils
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package to hold various functions to support training of ML models on ECMWF data.
 Author-email: "European Centre for Medium-Range Weather Forecasts (ECMWF)" <software.support@ecmwf.int>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `anemoi_utils-0.1.7/README.md` & `anemoi_utils-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.7/docs/Makefile` & `anemoi_utils-0.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.7/docs/_static/logo.png` & `anemoi_utils-0.1.8/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.7/docs/_static/style.css` & `anemoi_utils-0.1.8/docs/_static/style.css`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.7/docs/conf.py` & `anemoi_utils-0.1.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.7/docs/index.rst` & `anemoi_utils-0.1.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.7/docs/installing.rst` & `anemoi_utils-0.1.8/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.7/pyproject.toml` & `anemoi_utils-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.7/src/anemoi/utils/checkpoints.py` & `anemoi_utils-0.1.8/src/anemoi/utils/checkpoints.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.7/src/anemoi/utils/config.py` & `anemoi_utils-0.1.8/src/anemoi/utils/config.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.7/src/anemoi/utils/dates.py` & `anemoi_utils-0.1.8/src/anemoi/utils/dates.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.7/src/anemoi/utils/grib.py` & `anemoi_utils-0.1.8/src/anemoi/utils/grib.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,18 +12,29 @@
 """
 
 import logging
 import re
 
 import requests
 
+from .caching import cached
+
 LOG = logging.getLogger(__name__)
 
 
-def _search(name):
+@cached(collection="grib", expires=30 * 24 * 60 * 60)
+def _units():
+    r = requests.get("https://codes.ecmwf.int/parameter-database/api/v1/unit/")
+    r.raise_for_status()
+    units = r.json()
+    return {str(u["id"]): u["name"] for u in units}
+
+
+@cached(collection="grib", expires=30 * 24 * 60 * 60)
+def _search_param(name):
     name = re.escape(name)
     r = requests.get(f"https://codes.ecmwf.int/parameter-database/api/v1/param/?search=^{name}$&regex=true")
     r.raise_for_status()
     results = r.json()
     if len(results) == 0:
         raise KeyError(name)
 
@@ -52,15 +63,15 @@
     int
         Parameter id.
 
     >>> shortname_to_paramid("2t")
     167
 
     """
-    return _search(shortname)["id"]
+    return _search_param(shortname)["id"]
 
 
 def paramid_to_shortname(paramid: int) -> str:
     """Return the shortname of a GRIB parameter given its id.
 
     Parameters
     ----------
@@ -72,8 +83,50 @@
     str
         Parameter shortname.
 
     >>> paramid_to_shortname(167)
     '2t'
 
     """
-    return _search(str(paramid))["shortname"]
+    return _search_param(str(paramid))["shortname"]
+
+
+def units(param) -> str:
+    """Return the units of a GRIB parameter given its name or id.
+
+    Parameters
+    ----------
+    paramid : int or str
+        Parameter id ir name.
+
+    Returns
+    -------
+    str
+        Parameter unit.
+
+    >>> unit(167)
+    'K'
+
+    """
+
+    unit_id = str(_search_param(str(param))["unit_id"])
+    return _units()[unit_id]
+
+
+def must_be_positive(param):
+    """Check if a parameter must be positive.
+
+    Parameters
+    ----------
+    param : int or str
+        Parameter id or shortname.
+
+    Returns
+    -------
+    bool
+        True if the parameter must be positive.
+
+    >>> must_be_positive("tp")
+    True
+
+    """
+    return units(param) in ["m", "kg kg**-1", "m of water equivalent"]
```

### Comparing `anemoi_utils-0.1.7/src/anemoi/utils/humanize.py` & `anemoi_utils-0.1.8/src/anemoi/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.7/src/anemoi/utils/provenance.py` & `anemoi_utils-0.1.8/src/anemoi/utils/provenance.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.7/src/anemoi/utils/text.py` & `anemoi_utils-0.1.8/src/anemoi/utils/text.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.7/src/anemoi_utils.egg-info/PKG-INFO` & `anemoi_utils-0.1.8/src/anemoi_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anemoi-utils
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package to hold various functions to support training of ML models on ECMWF data.
 Author-email: "European Centre for Medium-Range Weather Forecasts (ECMWF)" <software.support@ecmwf.int>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `anemoi_utils-0.1.7/src/anemoi_utils.egg-info/SOURCES.txt` & `anemoi_utils-0.1.8/src/anemoi_utils.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 docs/modules/dates.rst
 docs/modules/grib.rst
 docs/modules/humanize.rst
 docs/modules/provenance.rst
 docs/modules/text.rst
 src/anemoi/utils/__init__.py
 src/anemoi/utils/_version.py
+src/anemoi/utils/caching.py
 src/anemoi/utils/checkpoints.py
 src/anemoi/utils/config.py
 src/anemoi/utils/dates.py
 src/anemoi/utils/grib.py
 src/anemoi/utils/humanize.py
 src/anemoi/utils/provenance.py
 src/anemoi/utils/text.py
```

### Comparing `anemoi_utils-0.1.7/tests/test_utils.py` & `anemoi_utils-0.1.8/tests/test_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 
 
 from anemoi.utils.config import DotDict
+from anemoi.utils.grib import paramid_to_shortname
+from anemoi.utils.grib import shortname_to_paramid
 
 
 def test_dotdict():
     d = DotDict(a=1, b=2, c=dict(d=3, e=4))
     assert d.a == 1
     assert d.b == 2
     assert d.c.d == 3
@@ -22,9 +24,14 @@
     d.d = dict(f=5)
     assert d.d.f == 5
 
     d.d.x = 6
     assert d.d.x == 6
 
 
+def test_grib():
+    assert shortname_to_paramid("2t") == 167
+    assert paramid_to_shortname(167) == "2t"
+
+
 if __name__ == "__main__":
-    test_dotdict()
+    test_grib()
```

