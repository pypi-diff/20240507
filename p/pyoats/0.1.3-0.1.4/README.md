# Comparing `tmp/pyoats-0.1.3.tar.gz` & `tmp/pyoats-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoats-0.1.3.tar", max compression
+gzip compressed data, was "pyoats-0.1.4.tar", max compression
```

## Comparing `pyoats-0.1.3.tar` & `pyoats-0.1.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0    11347 2022-11-25 14:22:15.619091 pyoats-0.1.3/LICENSE
--rw-r--r--   0        0        0    15741 2023-02-27 20:58:54.090808 pyoats-0.1.3/README.md
--rw-r--r--   0        0        0       30 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/__init__.py
--rw-r--r--   0        0        0        0 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/_data/__init__.py
--rw-r--r--   0        0        0      659 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/_data/base.py
--rw-r--r--   0        0        0     2618 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/_data/ucrdata.py
--rw-r--r--   0        0        0       66 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/_utils/__init__.py
--rw-r--r--   0        0        0    13251 2024-03-08 19:46:04.908225 pyoats-0.1.3/oats/_utils/dlutils.py
--rw-r--r--   0        0        0     1046 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/_utils/utils.py
--rw-r--r--   0        0        0      750 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/_utils/visualizer.py
--rw-r--r--   0        0        0      103 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/generator/__init__.py
--rw-r--r--   0        0        0      429 2022-11-25 14:41:11.083874 pyoats-0.1.3/oats/generator/_base.py
--rw-r--r--   0        0        0     9228 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/generator/univariate_wave.py
--rw-r--r--   0        0        0     1241 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/models/__init__.py
--rw-r--r--   0        0        0     1518 2022-11-25 14:40:53.523874 pyoats-0.1.3/oats/models/_base.py
--rw-r--r--   0        0        0     7658 2023-02-27 20:58:54.090808 pyoats-0.1.3/oats/models/_darts_model.py
--rw-r--r--   0        0        0     6287 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/models/_darts_simple.py
--rw-r--r--   0        0        0     2507 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/models/_pyod_model.py
--rw-r--r--   0        0        0       48 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/models/distance/__init__.py
--rw-r--r--   0        0        0      415 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/models/distance/iforest.py
--rw-r--r--   0        0        0     1708 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/models/distance/matrixprofile.py
--rw-r--r--   0        0        0       44 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/models/predictive/__init__.py
--rw-r--r--   0        0        0     1923 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/models/predictive/arima.py
--rw-r--r--   0        0        0    14023 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/models/predictive/fluxev.py
--rw-r--r--   0        0        0     2119 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/models/predictive/lightgbm.py
--rw-r--r--   0        0        0     1181 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/models/predictive/ma.py
--rw-r--r--   0        0        0     2070 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/models/predictive/nbeats.py
--rw-r--r--   0        0        0     1951 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/models/predictive/nhits.py
--rw-r--r--   0        0        0     1891 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/models/predictive/randomforest.py
--rw-r--r--   0        0        0     1392 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/models/predictive/regression.py
--rw-r--r--   0        0        0     2108 2022-11-25 14:42:45.108485 pyoats-0.1.3/oats/models/predictive/rnn.py
--rw-r--r--   0        0        0     1924 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/models/predictive/tcn.py
--rw-r--r--   0        0        0     2159 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/models/predictive/tft.py
--rw-r--r--   0        0        0     1955 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/models/predictive/transformer.py
--rw-r--r--   0        0        0       54 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/models/reconstruction/__init__.py
--rw-r--r--   0        0        0     6674 2024-03-08 19:49:52.505468 pyoats-0.1.3/oats/models/reconstruction/tranad.py
--rw-r--r--   0        0        0     1520 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/models/reconstruction/vae.py
--rw-r--r--   0        0        0       44 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/models/rule_based/__init__.py
--rw-r--r--   0        0        0     1275 2022-11-25 14:44:14.601176 pyoats-0.1.3/oats/models/rule_based/quantile.py
--rw-r--r--   0        0        0      105 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/preprocessor/__init__.py
--rw-r--r--   0        0        0     1306 2022-11-25 14:41:27.985335 pyoats-0.1.3/oats/preprocessor/_base.py
--rw-r--r--   0        0        0     5072 2024-03-08 19:47:55.722223 pyoats-0.1.3/oats/preprocessor/spectral_residual.py
--rw-r--r--   0        0        0    20480 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/scorer/.spot.py.swp
--rw-r--r--   0        0        0      155 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/scorer/__init__.py
--rw-r--r--   0        0        0      968 2022-11-25 14:41:40.405335 pyoats-0.1.3/oats/scorer/_base.py
--rw-r--r--   0        0        0     5040 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/scorer/qualitative_metrics.py
--rw-r--r--   0        0        0     3132 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/scorer/supervised_scorer.py
--rw-r--r--   0        0        0      232 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/threshold/__init__.py
--rw-r--r--   0        0        0     1259 2022-11-25 14:42:00.416219 pyoats-0.1.3/oats/threshold/_base.py
--rw-r--r--   0        0        0      952 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/threshold/jenks.py
--rw-r--r--   0        0        0     2437 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/threshold/pot.py
--rw-r--r--   0        0        0      953 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/threshold/quantile.py
--rw-r--r--   0        0        0     8262 2022-11-25 14:22:15.619091 pyoats-0.1.3/oats/threshold/spot.py
--rw-r--r--   0        0        0      992 2024-03-08 19:58:37.662059 pyoats-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    16891 1970-01-01 00:00:00.000000 pyoats-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11347 2022-11-25 14:22:15.619091 pyoats-0.1.4/LICENSE
+-rw-r--r--   0        0        0    15749 2024-05-06 21:17:38.108899 pyoats-0.1.4/README.md
+-rw-r--r--   0        0        0       30 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/_data/__init__.py
+-rw-r--r--   0        0        0      659 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/_data/base.py
+-rw-r--r--   0        0        0     2618 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/_data/ucrdata.py
+-rw-r--r--   0        0        0       66 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/_utils/__init__.py
+-rw-r--r--   0        0        0    13251 2024-05-06 21:17:38.108899 pyoats-0.1.4/oats/_utils/dlutils.py
+-rw-r--r--   0        0        0     1046 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/_utils/utils.py
+-rw-r--r--   0        0        0      750 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/_utils/visualizer.py
+-rw-r--r--   0        0        0      103 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/generator/__init__.py
+-rw-r--r--   0        0        0      429 2022-11-25 14:41:11.083874 pyoats-0.1.4/oats/generator/_base.py
+-rw-r--r--   0        0        0     9228 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/generator/univariate_wave.py
+-rw-r--r--   0        0        0     1241 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/models/__init__.py
+-rw-r--r--   0        0        0     1518 2022-11-25 14:40:53.523874 pyoats-0.1.4/oats/models/_base.py
+-rw-r--r--   0        0        0     7658 2023-02-27 20:58:54.090808 pyoats-0.1.4/oats/models/_darts_model.py
+-rw-r--r--   0        0        0     6287 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/models/_darts_simple.py
+-rw-r--r--   0        0        0     2507 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/models/_pyod_model.py
+-rw-r--r--   0        0        0       48 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/models/distance/__init__.py
+-rw-r--r--   0        0        0      415 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/models/distance/iforest.py
+-rw-r--r--   0        0        0     1708 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/models/distance/matrixprofile.py
+-rw-r--r--   0        0        0       44 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/models/predictive/__init__.py
+-rw-r--r--   0        0        0     1923 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/models/predictive/arima.py
+-rw-r--r--   0        0        0    14023 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/models/predictive/fluxev.py
+-rw-r--r--   0        0        0     2119 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/models/predictive/lightgbm.py
+-rw-r--r--   0        0        0     1181 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/models/predictive/ma.py
+-rw-r--r--   0        0        0     2070 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/models/predictive/nbeats.py
+-rw-r--r--   0        0        0     1951 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/models/predictive/nhits.py
+-rw-r--r--   0        0        0     1891 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/models/predictive/randomforest.py
+-rw-r--r--   0        0        0     1392 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/models/predictive/regression.py
+-rw-r--r--   0        0        0     2108 2022-11-25 14:42:45.108485 pyoats-0.1.4/oats/models/predictive/rnn.py
+-rw-r--r--   0        0        0     1924 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/models/predictive/tcn.py
+-rw-r--r--   0        0        0     2159 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/models/predictive/tft.py
+-rw-r--r--   0        0        0     1955 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/models/predictive/transformer.py
+-rw-r--r--   0        0        0       54 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/models/reconstruction/__init__.py
+-rw-r--r--   0        0        0     6674 2024-03-08 19:49:52.505468 pyoats-0.1.4/oats/models/reconstruction/tranad.py
+-rw-r--r--   0        0        0     1520 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/models/reconstruction/vae.py
+-rw-r--r--   0        0        0       44 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/models/rule_based/__init__.py
+-rw-r--r--   0        0        0     1275 2022-11-25 14:44:14.601176 pyoats-0.1.4/oats/models/rule_based/quantile.py
+-rw-r--r--   0        0        0      105 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/preprocessor/__init__.py
+-rw-r--r--   0        0        0     1306 2022-11-25 14:41:27.985335 pyoats-0.1.4/oats/preprocessor/_base.py
+-rw-r--r--   0        0        0     5115 2024-05-06 21:28:31.568840 pyoats-0.1.4/oats/preprocessor/spectral_residual.py
+-rw-r--r--   0        0        0    20480 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/scorer/.spot.py.swp
+-rw-r--r--   0        0        0      155 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/scorer/__init__.py
+-rw-r--r--   0        0        0      968 2022-11-25 14:41:40.405335 pyoats-0.1.4/oats/scorer/_base.py
+-rw-r--r--   0        0        0     5040 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/scorer/qualitative_metrics.py
+-rw-r--r--   0        0        0     3132 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/scorer/supervised_scorer.py
+-rw-r--r--   0        0        0      232 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/threshold/__init__.py
+-rw-r--r--   0        0        0     1259 2022-11-25 14:42:00.416219 pyoats-0.1.4/oats/threshold/_base.py
+-rw-r--r--   0        0        0      952 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/threshold/jenks.py
+-rw-r--r--   0        0        0     2437 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/threshold/pot.py
+-rw-r--r--   0        0        0      953 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/threshold/quantile.py
+-rw-r--r--   0        0        0     8262 2022-11-25 14:22:15.619091 pyoats-0.1.4/oats/threshold/spot.py
+-rw-r--r--   0        0        0     1000 2024-05-06 22:12:06.788602 pyoats-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    16997 1970-01-01 00:00:00.000000 pyoats-0.1.4/PKG-INFO
```

### Comparing `pyoats-0.1.3/LICENSE` & `pyoats-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/README.md` & `pyoats-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
   </a>
 
 <h3 align="center"> OATS</h3>
 
   <p align="center">
     Quick and Easy Outlier Detection for Time Series 
     <br />
-    <a href="https://georgian-io.github.io/pyoats-docs/"><strong>Explore the docs »</strong></a>
+    <a href="https://georgian-io-archive.github.io/pyoats-docs/"><strong>Explore the docs »</strong></a>
     <br />
     <br />
     <a href="https://georgian-io.medium.com/time-series-anomaly-detection-a-field-study-d13b35ee4344">View Demo</a>
     ·
     <a href="https://github.com/georgian-io/pyoats/issues">Report Bug</a>
     ·
     <a href="https://github.com/georgian-io/pyoats/issues">Request Feature</a>
```

### Comparing `pyoats-0.1.3/oats/_data/base.py` & `pyoats-0.1.4/oats/_data/base.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/_data/ucrdata.py` & `pyoats-0.1.4/oats/_data/ucrdata.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/_utils/dlutils.py` & `pyoats-0.1.4/oats/_utils/dlutils.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/_utils/utils.py` & `pyoats-0.1.4/oats/_utils/utils.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/_utils/visualizer.py` & `pyoats-0.1.4/oats/_utils/visualizer.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/generator/univariate_wave.py` & `pyoats-0.1.4/oats/generator/univariate_wave.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/models/__init__.py` & `pyoats-0.1.4/oats/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/models/_base.py` & `pyoats-0.1.4/oats/models/_base.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/models/_darts_model.py` & `pyoats-0.1.4/oats/models/_darts_model.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/models/_darts_simple.py` & `pyoats-0.1.4/oats/models/_darts_simple.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/models/_pyod_model.py` & `pyoats-0.1.4/oats/models/_pyod_model.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/models/distance/matrixprofile.py` & `pyoats-0.1.4/oats/models/distance/matrixprofile.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/models/predictive/arima.py` & `pyoats-0.1.4/oats/models/predictive/arima.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/models/predictive/fluxev.py` & `pyoats-0.1.4/oats/models/predictive/fluxev.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/models/predictive/lightgbm.py` & `pyoats-0.1.4/oats/models/predictive/lightgbm.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/models/predictive/ma.py` & `pyoats-0.1.4/oats/models/predictive/ma.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/models/predictive/nbeats.py` & `pyoats-0.1.4/oats/models/predictive/nbeats.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/models/predictive/nhits.py` & `pyoats-0.1.4/oats/models/predictive/nhits.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/models/predictive/randomforest.py` & `pyoats-0.1.4/oats/models/predictive/randomforest.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/models/predictive/regression.py` & `pyoats-0.1.4/oats/models/predictive/regression.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/models/predictive/rnn.py` & `pyoats-0.1.4/oats/models/predictive/rnn.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/models/predictive/tcn.py` & `pyoats-0.1.4/oats/models/predictive/tcn.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/models/predictive/tft.py` & `pyoats-0.1.4/oats/models/predictive/tft.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/models/predictive/transformer.py` & `pyoats-0.1.4/oats/models/predictive/transformer.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/models/reconstruction/tranad.py` & `pyoats-0.1.4/oats/models/reconstruction/tranad.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/models/reconstruction/vae.py` & `pyoats-0.1.4/oats/models/reconstruction/vae.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/models/rule_based/quantile.py` & `pyoats-0.1.4/oats/models/rule_based/quantile.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/preprocessor/_base.py` & `pyoats-0.1.4/oats/preprocessor/_base.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/preprocessor/spectral_residual.py` & `pyoats-0.1.4/oats/preprocessor/spectral_residual.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,23 +52,25 @@
     """
     Extrapolates the next value by sum up the slope of the last value with previous values.
     :param values: a list or numpy array of time-series
     :return: the next value of time-series
     """
 
     last_value = values[-1]
-    slope = [(last_value - v) / (i+1e-5) for (i, v) in enumerate(values[::-1])]
+    slope = np.array(
+        [(last_value - v) / (i + 1e-5) for (i, v) in enumerate(values[::-1])]
+    )
+    slope = slope
     slope[0] = 0
     next_values = last_value + np.cumsum(slope)
 
     return next_values
 
 
 def _merge_series(values, extend_num=5, forward=5):
-
     next_value = _extrapolate_next(values)[forward]
     extension = [next_value] * extend_num
 
     if isinstance(values, list):
         marge_values = values + extension
     else:
         marge_values = np.append(values, extension)
```

### Comparing `pyoats-0.1.3/oats/scorer/.spot.py.swp` & `pyoats-0.1.4/oats/scorer/.spot.py.swp`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/scorer/_base.py` & `pyoats-0.1.4/oats/scorer/_base.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/scorer/qualitative_metrics.py` & `pyoats-0.1.4/oats/scorer/qualitative_metrics.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/scorer/supervised_scorer.py` & `pyoats-0.1.4/oats/scorer/supervised_scorer.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/threshold/_base.py` & `pyoats-0.1.4/oats/threshold/_base.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/threshold/jenks.py` & `pyoats-0.1.4/oats/threshold/jenks.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/threshold/pot.py` & `pyoats-0.1.4/oats/threshold/pot.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/threshold/quantile.py` & `pyoats-0.1.4/oats/threshold/quantile.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/oats/threshold/spot.py` & `pyoats-0.1.4/oats/threshold/spot.py`

 * *Files identical despite different names*

### Comparing `pyoats-0.1.3/PKG-INFO` & `pyoats-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: pyoats
-Version: 0.1.3
+Version: 0.1.4
 Summary: Quick and Easy Time Series Outlier Detection
 License: Apache-2.0
 Author: Benjamin Ye
 Author-email: benjamin.ye@georgian.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: darts (==0.28.0)
 Requires-Dist: jenkspy (>=0.2.4,<0.3.0)
+Requires-Dist: keras (>=2.9.0,<3.0.0)
 Requires-Dist: lightgbm (>=4.3.0,<5.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: nvidia-cudnn-cu11 (==8.9.4.25)
 Requires-Dist: optuna (>=2.10.1,<3.0.0)
 Requires-Dist: pyod (==1.1.3)
+Requires-Dist: pytorch-lightning (>=1.7,<2.0)
 Requires-Dist: scipy (>=1.12.0,<2.0.0)
 Requires-Dist: statsforecast (>=1.7.3,<2.0.0)
 Requires-Dist: statsmodels (>=0.14.1,<0.15.0)
 Requires-Dist: stumpy (>=1.12.0,<2.0.0)
-Requires-Dist: tensorflow (>=2.15.0) ; sys_platform != "darwin"
-Requires-Dist: tensorflow-macos (>=2.15.0) ; sys_platform == "darwin"
-Requires-Dist: tensorflow-metal (==0.5.0) ; sys_platform == "darwin"
+Requires-Dist: tensorflow (==2.15.1) ; sys_platform != "darwin"
+Requires-Dist: tensorflow-metal (==1.1.0) ; sys_platform == "darwin"
+Requires-Dist: torch (>=2.3.0,<3.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 <!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
 <a name="readme-top"></a>
 <!--
 *** Thanks for checking out the Best-README-Template. If you have a suggestion
@@ -63,15 +66,15 @@
   </a>
 
 <h3 align="center"> OATS</h3>
 
   <p align="center">
     Quick and Easy Outlier Detection for Time Series 
     <br />
-    <a href="https://georgian-io.github.io/pyoats-docs/"><strong>Explore the docs »</strong></a>
+    <a href="https://georgian-io-archive.github.io/pyoats-docs/"><strong>Explore the docs »</strong></a>
     <br />
     <br />
     <a href="https://georgian-io.medium.com/time-series-anomaly-detection-a-field-study-d13b35ee4344">View Demo</a>
     ·
     <a href="https://github.com/georgian-io/pyoats/issues">Report Bug</a>
     ·
     <a href="https://github.com/georgian-io/pyoats/issues">Request Feature</a>
```

#### html2text {}

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 2.1 Name: pyoats Version: 0.1.3 Summary: Quick and Easy Time
+Metadata-Version: 2.1 Name: pyoats Version: 0.1.4 Summary: Quick and Easy Time
 Series Outlier Detection License: Apache-2.0 Author: Benjamin Ye Author-email:
 benjamin.ye@georgian.io Requires-Python: >=3.9,<3.12 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: darts (==0.28.0) Requires-Dist: jenkspy (>=0.2.4,<0.3.0)
-Requires-Dist: lightgbm (>=4.3.0,<5.0.0) Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Requires-Dist: optuna (>=2.10.1,<3.0.0) Requires-Dist: pyod (==1.1.3) Requires-
-Dist: scipy (>=1.12.0,<2.0.0) Requires-Dist: statsforecast (>=1.7.3,<2.0.0)
-Requires-Dist: statsmodels (>=0.14.1,<0.15.0) Requires-Dist: stumpy
-(>=1.12.0,<2.0.0) Requires-Dist: tensorflow (>=2.15.0) ; sys_platform !=
-"darwin" Requires-Dist: tensorflow-macos (>=2.15.0) ; sys_platform == "darwin"
-Requires-Dist: tensorflow-metal (==0.5.0) ; sys_platform == "darwin" Requires-
-Dist: tqdm (>=4.66.2,<5.0.0) Description-Content-Type: text/markdown [!
-[Contributors][contributors-shield]][contributors-url] [![Stargazers][stars-
-shield]][stars-url] [![Issues][issues-shield]][issues-url] [![Apache 2.0
-License][license-shield]][license-url] [![Last Commit][last_commit-shield]]
-[last_commit-url]
+Requires-Dist: keras (>=2.9.0,<3.0.0) Requires-Dist: lightgbm (>=4.3.0,<5.0.0)
+Requires-Dist: numpy (>=1.26.4,<2.0.0) Requires-Dist: nvidia-cudnn-cu11
+(==8.9.4.25) Requires-Dist: optuna (>=2.10.1,<3.0.0) Requires-Dist: pyod
+(==1.1.3) Requires-Dist: pytorch-lightning (>=1.7,<2.0) Requires-Dist: scipy
+(>=1.12.0,<2.0.0) Requires-Dist: statsforecast (>=1.7.3,<2.0.0) Requires-Dist:
+statsmodels (>=0.14.1,<0.15.0) Requires-Dist: stumpy (>=1.12.0,<2.0.0)
+Requires-Dist: tensorflow (==2.15.1) ; sys_platform != "darwin" Requires-Dist:
+tensorflow-metal (==1.1.0) ; sys_platform == "darwin" Requires-Dist: torch
+(>=2.3.0,<3.0.0) Requires-Dist: tqdm (>=4.66.2,<5.0.0) Description-Content-
+Type: text/markdown [![Contributors][contributors-shield]][contributors-url] [!
+[Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]][issues-url]
+[![Apache 2.0 License][license-shield]][license-url] [![Last Commit]
+[last_commit-shield]][last_commit-url]
                                     _[_L_o_g_o_]
                                 ******** OOAATTSS ********
                Quick and Easy Outlier Detection for Time Series
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 
                   _V_i_e_w_ _D_e_m_o Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 Table of Contents
```

