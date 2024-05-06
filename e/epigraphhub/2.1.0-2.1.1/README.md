# Comparing `tmp/epigraphhub-2.1.0.tar.gz` & `tmp/epigraphhub-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epigraphhub-2.1.0.tar", max compression
+gzip compressed data, was "epigraphhub-2.1.1.tar", max compression
```

## Comparing `epigraphhub-2.1.0.tar` & `epigraphhub-2.1.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    32471 2023-09-25 16:13:11.293660 epigraphhub-2.1.0/LICENSE
--rw-r--r--   0        0        0     4048 2023-09-25 16:13:11.293660 epigraphhub-2.1.0/README.md
--rw-r--r--   0        0        0      400 2023-09-25 16:16:08.829741 epigraphhub-2.1.0/epigraphhub/__init__.py
--rw-r--r--   0        0        0     1504 2023-09-25 16:13:11.717662 epigraphhub-2.1.0/epigraphhub/__main__.py
--rw-r--r--   0        0        0        0 2023-09-25 16:13:11.717662 epigraphhub-2.1.0/epigraphhub/analysis/__init__.py
--rw-r--r--   0        0        0    10126 2023-09-25 16:13:11.717662 epigraphhub-2.1.0/epigraphhub/analysis/clustering.py
--rw-r--r--   0        0        0     3018 2023-09-25 16:13:11.717662 epigraphhub-2.1.0/epigraphhub/analysis/epistats.py
--rw-r--r--   0        0        0    27999 2023-09-25 16:13:11.717662 epigraphhub-2.1.0/epigraphhub/analysis/forecast_models/lstm_models.py
--rw-r--r--   0        0        0     2476 2023-09-25 16:13:11.717662 epigraphhub-2.1.0/epigraphhub/analysis/forecast_models/metrics.py
--rw-r--r--   0        0        0    13122 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/analysis/forecast_models/ngboost_models.py
--rw-r--r--   0        0        0     3368 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/analysis/forecast_models/plots.py
--rw-r--r--   0        0        0     7250 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/analysis/forecast_models/sklearn_models.py
--rw-r--r--   0        0        0     6925 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/analysis/preprocessing.py
--rw-r--r--   0        0        0       57 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/analysis/rtestim.py
--rw-r--r--   0        0        0     1982 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/connection.py
--rw-r--r--   0        0        0      137 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/.env
--rw-r--r--   0        0        0        0 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/__init__.py
--rw-r--r--   0        0        0     1115 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/_config.py
--rw-r--r--   0        0        0        0 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/brasil/__init__.py
--rw-r--r--   0        0        0      372 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/brasil/sinan/__init__.py
--rw-r--r--   0        0        0     1194 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/brasil/sinan/extract.py
--rw-r--r--   0        0        0     1802 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/brasil/sinan/loading.py
--rw-r--r--   0        0        0     1451 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/brasil/sinan/viz.py
--rw-r--r--   0        0        0        0 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/colombia/__init__.py
--rw-r--r--   0        0        0     2619 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/colombia/extract.py
--rw-r--r--   0        0        0     4433 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/colombia/loading.py
--rw-r--r--   0        0        0     4376 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/epigraphhub_db.py
--rw-r--r--   0        0        0        0 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/foph/__init__.py
--rw-r--r--   0        0        0     5975 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/foph/extract.py
--rw-r--r--   0        0        0     3899 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/foph/loading.py
--rw-r--r--   0        0        0   332069 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/foph/schema.json
--rw-r--r--   0        0        0     1515 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/foph/transform.py
--rw-r--r--   0        0        0     6510 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/foph/viz.py
--rw-r--r--   0        0        0      983 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/geoupload.py
--rw-r--r--   0        0        0     3202 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/ggtrends.py
--rw-r--r--   0        0        0        0 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/owid/__init__.py
--rw-r--r--   0        0        0     3194 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/owid/extract.py
--rw-r--r--   0        0        0     2415 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/owid/loading.py
--rw-r--r--   0        0        0     2212 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/owid/transform.py
--rw-r--r--   0        0        0     4248 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/sinan_fetch.py
--rw-r--r--   0        0        0     7924 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/worldbank.py
--rw-r--r--   0        0        0     2478 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/data/worldpop.py
--rw-r--r--   0        0        0     1377 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/settings.py
--rw-r--r--   0        0        0        0 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/utils/__init__.py
--rw-r--r--   0        0        0     2287 2023-09-25 16:13:11.721662 epigraphhub-2.1.0/epigraphhub/utils/_config.py
--rw-r--r--   0        0        0     5038 2023-09-25 16:16:08.833741 epigraphhub-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     6304 1970-01-01 00:00:00.000000 epigraphhub-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    32471 2024-05-06 21:58:41.705323 epigraphhub-2.1.1/LICENSE
+-rw-r--r--   0        0        0     4048 2024-05-06 21:58:41.705323 epigraphhub-2.1.1/README.md
+-rw-r--r--   0        0        0      400 2024-05-06 22:00:04.281998 epigraphhub-2.1.1/epigraphhub/__init__.py
+-rw-r--r--   0        0        0     1504 2024-05-06 21:58:42.033325 epigraphhub-2.1.1/epigraphhub/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-06 21:58:42.033325 epigraphhub-2.1.1/epigraphhub/analysis/__init__.py
+-rw-r--r--   0        0        0    10126 2024-05-06 21:58:42.033325 epigraphhub-2.1.1/epigraphhub/analysis/clustering.py
+-rw-r--r--   0        0        0     3018 2024-05-06 21:58:42.033325 epigraphhub-2.1.1/epigraphhub/analysis/epistats.py
+-rw-r--r--   0        0        0    27999 2024-05-06 21:58:42.033325 epigraphhub-2.1.1/epigraphhub/analysis/forecast_models/lstm_models.py
+-rw-r--r--   0        0        0     2476 2024-05-06 21:58:42.033325 epigraphhub-2.1.1/epigraphhub/analysis/forecast_models/metrics.py
+-rw-r--r--   0        0        0    13122 2024-05-06 21:58:42.033325 epigraphhub-2.1.1/epigraphhub/analysis/forecast_models/ngboost_models.py
+-rw-r--r--   0        0        0     3368 2024-05-06 21:58:42.033325 epigraphhub-2.1.1/epigraphhub/analysis/forecast_models/plots.py
+-rw-r--r--   0        0        0     7250 2024-05-06 21:58:42.033325 epigraphhub-2.1.1/epigraphhub/analysis/forecast_models/sklearn_models.py
+-rw-r--r--   0        0        0     6925 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/analysis/preprocessing.py
+-rw-r--r--   0        0        0       57 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/analysis/rtestim.py
+-rw-r--r--   0        0        0     1982 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/connection.py
+-rw-r--r--   0        0        0      137 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/.env
+-rw-r--r--   0        0        0        0 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/__init__.py
+-rw-r--r--   0        0        0     1115 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/_config.py
+-rw-r--r--   0        0        0        0 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/brasil/__init__.py
+-rw-r--r--   0        0        0      372 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/brasil/sinan/__init__.py
+-rw-r--r--   0        0        0     1194 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/brasil/sinan/extract.py
+-rw-r--r--   0        0        0     1802 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/brasil/sinan/loading.py
+-rw-r--r--   0        0        0     1451 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/brasil/sinan/viz.py
+-rw-r--r--   0        0        0        0 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/colombia/__init__.py
+-rw-r--r--   0        0        0     2619 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/colombia/extract.py
+-rw-r--r--   0        0        0     4433 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/colombia/loading.py
+-rw-r--r--   0        0        0     4376 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/epigraphhub_db.py
+-rw-r--r--   0        0        0        0 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/foph/__init__.py
+-rw-r--r--   0        0        0     5975 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/foph/extract.py
+-rw-r--r--   0        0        0     3899 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/foph/loading.py
+-rw-r--r--   0        0        0   332069 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/foph/schema.json
+-rw-r--r--   0        0        0     1515 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/foph/transform.py
+-rw-r--r--   0        0        0     6510 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/foph/viz.py
+-rw-r--r--   0        0        0      983 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/geoupload.py
+-rw-r--r--   0        0        0     3202 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/ggtrends.py
+-rw-r--r--   0        0        0        0 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/owid/__init__.py
+-rw-r--r--   0        0        0     3194 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/owid/extract.py
+-rw-r--r--   0        0        0     2415 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/owid/loading.py
+-rw-r--r--   0        0        0     2212 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/owid/transform.py
+-rw-r--r--   0        0        0     4248 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/sinan_fetch.py
+-rw-r--r--   0        0        0     7924 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/worldbank.py
+-rw-r--r--   0        0        0     2478 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/data/worldpop.py
+-rw-r--r--   0        0        0     1377 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/settings.py
+-rw-r--r--   0        0        0        0 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/utils/__init__.py
+-rw-r--r--   0        0        0     2287 2024-05-06 21:58:42.037325 epigraphhub-2.1.1/epigraphhub/utils/_config.py
+-rw-r--r--   0        0        0     5188 2024-05-06 22:00:04.281998 epigraphhub-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6139 1970-01-01 00:00:00.000000 epigraphhub-2.1.1/PKG-INFO
```

### Comparing `epigraphhub-2.1.0/LICENSE` & `epigraphhub-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/README.md` & `epigraphhub-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/__main__.py` & `epigraphhub-2.1.1/epigraphhub/__main__.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/analysis/clustering.py` & `epigraphhub-2.1.1/epigraphhub/analysis/clustering.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/analysis/epistats.py` & `epigraphhub-2.1.1/epigraphhub/analysis/epistats.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/analysis/forecast_models/lstm_models.py` & `epigraphhub-2.1.1/epigraphhub/analysis/forecast_models/lstm_models.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/analysis/forecast_models/metrics.py` & `epigraphhub-2.1.1/epigraphhub/analysis/forecast_models/metrics.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/analysis/forecast_models/ngboost_models.py` & `epigraphhub-2.1.1/epigraphhub/analysis/forecast_models/ngboost_models.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/analysis/forecast_models/plots.py` & `epigraphhub-2.1.1/epigraphhub/analysis/forecast_models/plots.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/analysis/forecast_models/sklearn_models.py` & `epigraphhub-2.1.1/epigraphhub/analysis/forecast_models/sklearn_models.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/analysis/preprocessing.py` & `epigraphhub-2.1.1/epigraphhub/analysis/preprocessing.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/connection.py` & `epigraphhub-2.1.1/epigraphhub/connection.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/data/_config.py` & `epigraphhub-2.1.1/epigraphhub/data/_config.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/data/brasil/sinan/extract.py` & `epigraphhub-2.1.1/epigraphhub/data/brasil/sinan/extract.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/data/brasil/sinan/loading.py` & `epigraphhub-2.1.1/epigraphhub/data/brasil/sinan/loading.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/data/brasil/sinan/viz.py` & `epigraphhub-2.1.1/epigraphhub/data/brasil/sinan/viz.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/data/colombia/extract.py` & `epigraphhub-2.1.1/epigraphhub/data/colombia/extract.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/data/colombia/loading.py` & `epigraphhub-2.1.1/epigraphhub/data/colombia/loading.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/data/epigraphhub_db.py` & `epigraphhub-2.1.1/epigraphhub/data/epigraphhub_db.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/data/foph/extract.py` & `epigraphhub-2.1.1/epigraphhub/data/foph/extract.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/data/foph/loading.py` & `epigraphhub-2.1.1/epigraphhub/data/foph/loading.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/data/foph/schema.json` & `epigraphhub-2.1.1/epigraphhub/data/foph/schema.json`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/data/foph/transform.py` & `epigraphhub-2.1.1/epigraphhub/data/foph/transform.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/data/foph/viz.py` & `epigraphhub-2.1.1/epigraphhub/data/foph/viz.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/data/geoupload.py` & `epigraphhub-2.1.1/epigraphhub/data/geoupload.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/data/ggtrends.py` & `epigraphhub-2.1.1/epigraphhub/data/ggtrends.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/data/owid/extract.py` & `epigraphhub-2.1.1/epigraphhub/data/owid/extract.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/data/owid/loading.py` & `epigraphhub-2.1.1/epigraphhub/data/owid/loading.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/data/owid/transform.py` & `epigraphhub-2.1.1/epigraphhub/data/owid/transform.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/data/sinan_fetch.py` & `epigraphhub-2.1.1/epigraphhub/data/sinan_fetch.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/data/worldbank.py` & `epigraphhub-2.1.1/epigraphhub/data/worldbank.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/data/worldpop.py` & `epigraphhub-2.1.1/epigraphhub/data/worldpop.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/settings.py` & `epigraphhub-2.1.1/epigraphhub/settings.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/epigraphhub/utils/_config.py` & `epigraphhub-2.1.1/epigraphhub/utils/_config.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.1.0/pyproject.toml` & `epigraphhub-2.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "epigraphhub"
-version = "2.1.0"  # changed by semantic-release
+version = "2.1.1"  # changed by semantic-release
 description = "Epigraphhub Python package"
 readme = "README.md"
 authors = ["thegraphnetwork <fccoelho@gmail.com>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/thegraphnetwork/epigraphhub_py"
 homepage = "https://github.com/thegraphnetwork/epigraphhub_py"
 
@@ -30,78 +30,78 @@
 [tool.poetry.scripts]
 # Entry points for the package https://python-poetry.org/docs/pyproject/#scripts
 "epigraphhub" = "epigraphhub.__main__:app"
 "epigraphhub-config" = "epigraphhub.utils._config:create_file"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
-
-typer = {extras = ["all"], version = "^0.4.0"}
+typer = {extras = ["all"], version = ">=0.4.0"}
 rich = ">=12.4.4,<13"
-numpy = "^1.20.3"
-pandas = "^1.2"
-scipy = "^1.8.0"
-sshtunnel = "^0.4.0"
+numpy = ">=1.20.3,<2"
+pandas = ">=1.2,<2"
+# issue with gaussian from signal
+scipy = ">=1.8.0,<1.13"
+sshtunnel = ">=0.4.0"
 SQLAlchemy = ">= 1.4.29,<2.0.0"
-psycopg2-binary = "^2.9.3"
-joblib = "^1.1.0"
-wbgapi = "^1.0.7"
-rioxarray = "^0.10.2"
-wget = "^3.2"
-tabulate = "^0.8.9"
-click = "^8.1.0"
-PyYAML = "^5.0"
-pymc = "^4.2.0"
-loguru = "^0.6.0"
-sodapy = "^2.2.0"
-pangres = "^4.1.2"
-ibis-framework = "^3.2.0"
-jupyter = "^1.0.0"
-GeoAlchemy2 = "^0.10.0"
-geopandas = "^0.10.2"
+psycopg2-binary = ">=2.9.3"
+joblib = ">=1.1.0"
+wbgapi = ">=1.0.7"
+rioxarray = ">=0.10.2"
+wget = ">=3.2"
+tabulate = ">=0.8.9"
+click = ">=8.1.0"
+PyYAML = ">=5.0"
+pymc = ">=4.2.0"
+loguru = ">=0.6.0"
+sodapy = ">=2.2.0"
+pangres = ">=4.1.2"
+ibis-framework = ">=3.2.0,<4"
+jupyter = ">=1.0.0"
+GeoAlchemy2 = ">=0.10.0"
+geopandas = ">=0.10.2"
 # [viz]
-arviz = {version = "^0.12.0", optional = true}
-matplotlib = {version = "^3.5.1", optional = true}
-plotly =  {version = "^5", optional = true}
+arviz = {version = ">=0.12.0", optional = true}
+matplotlib = {version = ">=3.5.1", optional = true}
+plotly =  {version = ">=5", optional = true}
 # [ml]
-pytrends = {version = "^4.7.3", optional = true}
-tensorflow = {version = "^2.5.0", optional = true}
-scikit-learn = {version = "^1.0.2", optional = true}
-ngboost = {version = "^0.3.13", optional = true}
+pytrends = {version = ">=4.7.3", optional = true}
+tensorflow = {version = ">=2.5.0", optional = true}
+# issue with alpha argument in the interval function
+scikit-learn = {version = ">=1.0.2,<1.3", optional = true}
+ngboost = {version = ">=0.3.13,<0.4", optional = true}
 
 [tool.poetry.extras]
 ml = ["pytrends", "tensorflow", "scikit-learn", "ngboost"]
 viz = ["matplotlib", "plotly", "arviz"]
 
-[tool.poetry.dev-dependencies]
-bandit = "^1.7.2"
-black = {version = "^22.1", allow-prereleases = true}
-darglint = "^1.8.1"
-isort = {extras = ["colors"], version = "^5.10.1"}
-mypy = "^0.910"
-mypy-extensions = "^0.4.3"
-pre-commit = "^2.15.0"
-pydocstyle = "^6.1.1"
-pylint = "^2.11.1"
-pytest = "^7.0.1"
-pyupgrade = "^2.29.1"
-safety = "^1.10.3"
-coverage = "^6.3"
-coverage-badge = "^1.1.0"
-pytest-html = "^3.1.1"
-pytest-cov = "^3.0.0"
-Sphinx = "^4.4.0"
-myst-parser = "^0.17.0"
-sphinx-pyproject = "^0.1.0"
-nbsphinx = "^0.8.8"
-
 [tool.poetry.group.dev.dependencies]
+bandit = ">=1.7.2"
+black = {version = ">=22.1", allow-prereleases = true}
+darglint = ">=1.8.1"
+isort = {extras = ["colors"], version = ">=5.10.1"}
+mypy = ">=0.910,<1"
+mypy-extensions = ">=0.4.3,<0.5"
+pre-commit = ">=2.15.0"
+pydocstyle = ">=6.1.1"
+pylint = ">=2.11.1"
+pytest = ">=7.0.1"
+pyupgrade = ">=2.29.1"
+safety = ">=1.10.3"
+coverage = ">=6.3"
+coverage-badge = ">=1.1.0"
+pytest-html = ">=3.1.1"
+pytest-cov = ">=3.0.0"
+Sphinx = ">=4.4.0"
+myst-parser = ">=0.17.0"
+sphinx-pyproject = ">=0.1.0"
+nbsphinx = ">=0.8.8"
 makim = "1.6.4"
 containers-sugar = "1.4.2"
-pysus = "^0.8.0"
+pysus = ">=0.8.0"
+docker = "<7"
 
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py39"]
 line-length = 88
 color = true
 exclude = '''
```

### Comparing `epigraphhub-2.1.0/PKG-INFO` & `epigraphhub-2.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epigraphhub
-Version: 2.1.0
+Version: 2.1.1
 Summary: Epigraphhub Python package
 Home-page: https://github.com/thegraphnetwork/epigraphhub_py
 License: GNU GPL v3.0
 Keywords: epidemiology
 Author: thegraphnetwork
 Author-email: fccoelho@gmail.com
 Requires-Python: >=3.9,<3.11
@@ -15,44 +15,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: ml
 Provides-Extra: viz
-Requires-Dist: GeoAlchemy2 (>=0.10.0,<0.11.0)
-Requires-Dist: PyYAML (>=5.0,<6.0)
+Requires-Dist: GeoAlchemy2 (>=0.10.0)
+Requires-Dist: PyYAML (>=5.0)
 Requires-Dist: SQLAlchemy (>=1.4.29,<2.0.0)
-Requires-Dist: arviz (>=0.12.0,<0.13.0) ; extra == "viz"
-Requires-Dist: click (>=8.1.0,<9.0.0)
-Requires-Dist: geopandas (>=0.10.2,<0.11.0)
-Requires-Dist: ibis-framework (>=3.2.0,<4.0.0)
-Requires-Dist: joblib (>=1.1.0,<2.0.0)
-Requires-Dist: jupyter (>=1.0.0,<2.0.0)
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
-Requires-Dist: matplotlib (>=3.5.1,<4.0.0) ; extra == "viz"
-Requires-Dist: ngboost (>=0.3.13,<0.4.0) ; extra == "ml"
-Requires-Dist: numpy (>=1.20.3,<2.0.0)
-Requires-Dist: pandas (>=1.2,<2.0)
-Requires-Dist: pangres (>=4.1.2,<5.0.0)
-Requires-Dist: plotly (>=5,<6) ; extra == "viz"
-Requires-Dist: psycopg2-binary (>=2.9.3,<3.0.0)
-Requires-Dist: pymc (>=4.2.0,<5.0.0)
-Requires-Dist: pytrends (>=4.7.3,<5.0.0) ; extra == "ml"
+Requires-Dist: arviz (>=0.12.0) ; extra == "viz"
+Requires-Dist: click (>=8.1.0)
+Requires-Dist: geopandas (>=0.10.2)
+Requires-Dist: ibis-framework (>=3.2.0,<4)
+Requires-Dist: joblib (>=1.1.0)
+Requires-Dist: jupyter (>=1.0.0)
+Requires-Dist: loguru (>=0.6.0)
+Requires-Dist: matplotlib (>=3.5.1) ; extra == "viz"
+Requires-Dist: ngboost (>=0.3.13,<0.4) ; extra == "ml"
+Requires-Dist: numpy (>=1.20.3,<2)
+Requires-Dist: pandas (>=1.2,<2)
+Requires-Dist: pangres (>=4.1.2)
+Requires-Dist: plotly (>=5) ; extra == "viz"
+Requires-Dist: psycopg2-binary (>=2.9.3)
+Requires-Dist: pymc (>=4.2.0)
+Requires-Dist: pytrends (>=4.7.3) ; extra == "ml"
 Requires-Dist: rich (>=12.4.4,<13)
-Requires-Dist: rioxarray (>=0.10.2,<0.11.0)
-Requires-Dist: scikit-learn (>=1.0.2,<2.0.0) ; extra == "ml"
-Requires-Dist: scipy (>=1.8.0,<2.0.0)
-Requires-Dist: sodapy (>=2.2.0,<3.0.0)
-Requires-Dist: sshtunnel (>=0.4.0,<0.5.0)
-Requires-Dist: tabulate (>=0.8.9,<0.9.0)
-Requires-Dist: tensorflow (>=2.5.0,<3.0.0) ; extra == "ml"
-Requires-Dist: typer[all] (>=0.4.0,<0.5.0)
-Requires-Dist: wbgapi (>=1.0.7,<2.0.0)
-Requires-Dist: wget (>=3.2,<4.0)
+Requires-Dist: rioxarray (>=0.10.2)
+Requires-Dist: scikit-learn (>=1.0.2,<1.3) ; extra == "ml"
+Requires-Dist: scipy (>=1.8.0,<1.13)
+Requires-Dist: sodapy (>=2.2.0)
+Requires-Dist: sshtunnel (>=0.4.0)
+Requires-Dist: tabulate (>=0.8.9)
+Requires-Dist: tensorflow (>=2.5.0) ; extra == "ml"
+Requires-Dist: typer[all] (>=0.4.0)
+Requires-Dist: wbgapi (>=1.0.7)
+Requires-Dist: wget (>=3.2)
 Project-URL: Repository, https://github.com/thegraphnetwork/epigraphhub_py
 Description-Content-Type: text/markdown
 
 # epigraphhub_py
 
 <div align="center">
```

