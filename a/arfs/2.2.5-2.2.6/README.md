# Comparing `tmp/arfs-2.2.5.tar.gz` & `tmp/arfs-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arfs-2.2.5.tar", last modified: Mon Apr 29 18:24:13 2024, max compression
+gzip compressed data, was "arfs-2.2.6.tar", last modified: Tue Apr 30 10:23:58 2024, max compression
```

## Comparing `arfs-2.2.5.tar` & `arfs-2.2.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 18:24:13.825607 arfs-2.2.5/
--rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-2.2.5/LICENSE.md
--rw-rw-rw-   0        0        0    13229 2024-04-29 18:24:13.790377 arfs-2.2.5/PKG-INFO
--rw-rw-rw-   0        0        0    11641 2023-11-27 13:09:08.000000 arfs-2.2.5/README.md
--rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-2.2.5/pyproject.toml
--rw-rw-rw-   0        0        0     1382 2024-04-29 18:24:13.864839 arfs-2.2.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-29 18:24:12.904401 arfs-2.2.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 18:24:13.164327 arfs-2.2.5/src/arfs/
--rw-rw-rw-   0        0        0       92 2024-04-29 15:17:57.000000 arfs-2.2.5/src/arfs/__init__.py
--rw-rw-rw-   0        0        0    84981 2024-04-29 15:15:30.000000 arfs-2.2.5/src/arfs/association.py
--rw-rw-rw-   0        0        0     6829 2023-11-27 13:09:09.000000 arfs-2.2.5/src/arfs/benchmark.py
-drwxrwxrwx   0        0        0        0 2024-04-29 18:24:12.904401 arfs-2.2.5/src/arfs/dataset/
-drwxrwxrwx   0        0        0        0 2024-04-29 18:24:13.339440 arfs-2.2.5/src/arfs/dataset/data/
--rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-2.2.5/src/arfs/dataset/data/boston_bunch.joblib
--rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-2.2.5/src/arfs/dataset/data/housing.zip
-drwxrwxrwx   0        0        0        0 2024-04-29 18:24:13.606289 arfs-2.2.5/src/arfs/feature_selection/
--rw-rw-rw-   0        0        0      711 2023-11-27 13:09:09.000000 arfs-2.2.5/src/arfs/feature_selection/__init__.py
--rw-rw-rw-   0        0        0    97164 2024-04-29 15:11:45.000000 arfs-2.2.5/src/arfs/feature_selection/allrelevant.py
--rw-rw-rw-   0        0        0     5396 2023-11-27 13:09:09.000000 arfs-2.2.5/src/arfs/feature_selection/base.py
--rw-rw-rw-   0        0        0    24197 2023-11-27 13:09:09.000000 arfs-2.2.5/src/arfs/feature_selection/lasso.py
--rw-rw-rw-   0        0        0    13811 2023-11-28 13:14:49.000000 arfs-2.2.5/src/arfs/feature_selection/mrmr.py
--rw-rw-rw-   0        0        0     2473 2023-11-27 13:09:10.000000 arfs-2.2.5/src/arfs/feature_selection/summary.py
--rw-rw-rw-   0        0        0    16361 2024-04-26 08:15:15.000000 arfs-2.2.5/src/arfs/feature_selection/unsupervised.py
--rw-rw-rw-   0        0        0    16032 2024-04-29 15:15:32.000000 arfs-2.2.5/src/arfs/feature_selection/variable_importance.py
--rw-rw-rw-   0        0        0    21847 2023-11-27 13:09:10.000000 arfs-2.2.5/src/arfs/gbm.py
--rw-rw-rw-   0        0        0     6058 2023-11-28 13:14:50.000000 arfs-2.2.5/src/arfs/parallel.py
--rw-rw-rw-   0        0        0    38113 2024-04-29 16:16:15.000000 arfs-2.2.5/src/arfs/preprocessing.py
--rw-rw-rw-   0        0        0    15511 2023-11-27 13:09:10.000000 arfs-2.2.5/src/arfs/sampling.py
--rw-rw-rw-   0        0        0    26942 2023-11-28 13:14:50.000000 arfs-2.2.5/src/arfs/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 18:24:13.751153 arfs-2.2.5/src/arfs.egg-info/
--rw-rw-rw-   0        0        0    13229 2024-04-29 18:24:12.000000 arfs-2.2.5/src/arfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      849 2024-04-29 18:24:12.000000 arfs-2.2.5/src/arfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 18:24:12.000000 arfs-2.2.5/src/arfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-2.2.5/src/arfs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      358 2024-04-29 18:24:12.000000 arfs-2.2.5/src/arfs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-29 18:24:12.000000 arfs-2.2.5/src/arfs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-29 18:24:13.666288 arfs-2.2.5/tests/
--rw-rw-rw-   0        0        0    10867 2023-11-29 14:43:52.000000 arfs-2.2.5/tests/test_allrelevant.py
--rw-rw-rw-   0        0        0    19531 2023-11-29 14:51:48.000000 arfs-2.2.5/tests/test_featselect.py
+drwxrwxrwx   0        0        0        0 2024-04-30 10:23:58.024667 arfs-2.2.6/
+-rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-2.2.6/LICENSE.md
+-rw-rw-rw-   0        0        0    13229 2024-04-30 10:23:57.998981 arfs-2.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0    11641 2023-11-27 13:09:08.000000 arfs-2.2.6/README.md
+-rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-2.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0     1382 2024-04-30 10:23:58.034773 arfs-2.2.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 10:23:56.253195 arfs-2.2.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-30 10:23:56.992465 arfs-2.2.6/src/arfs/
+-rw-rw-rw-   0        0        0       92 2024-04-30 10:21:58.000000 arfs-2.2.6/src/arfs/__init__.py
+-rw-rw-rw-   0        0        0    84981 2024-04-29 15:15:30.000000 arfs-2.2.6/src/arfs/association.py
+-rw-rw-rw-   0        0        0     6829 2023-11-27 13:09:09.000000 arfs-2.2.6/src/arfs/benchmark.py
+drwxrwxrwx   0        0        0        0 2024-04-30 10:23:56.266344 arfs-2.2.6/src/arfs/dataset/
+drwxrwxrwx   0        0        0        0 2024-04-30 10:23:57.353410 arfs-2.2.6/src/arfs/dataset/data/
+-rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-2.2.6/src/arfs/dataset/data/boston_bunch.joblib
+-rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-2.2.6/src/arfs/dataset/data/housing.zip
+drwxrwxrwx   0        0        0        0 2024-04-30 10:23:57.765643 arfs-2.2.6/src/arfs/feature_selection/
+-rw-rw-rw-   0        0        0      711 2023-11-27 13:09:09.000000 arfs-2.2.6/src/arfs/feature_selection/__init__.py
+-rw-rw-rw-   0        0        0    97164 2024-04-29 15:11:45.000000 arfs-2.2.6/src/arfs/feature_selection/allrelevant.py
+-rw-rw-rw-   0        0        0     5396 2023-11-27 13:09:09.000000 arfs-2.2.6/src/arfs/feature_selection/base.py
+-rw-rw-rw-   0        0        0    24197 2023-11-27 13:09:09.000000 arfs-2.2.6/src/arfs/feature_selection/lasso.py
+-rw-rw-rw-   0        0        0    13811 2023-11-28 13:14:49.000000 arfs-2.2.6/src/arfs/feature_selection/mrmr.py
+-rw-rw-rw-   0        0        0     2473 2023-11-27 13:09:10.000000 arfs-2.2.6/src/arfs/feature_selection/summary.py
+-rw-rw-rw-   0        0        0    16361 2024-04-26 08:15:15.000000 arfs-2.2.6/src/arfs/feature_selection/unsupervised.py
+-rw-rw-rw-   0        0        0    16523 2024-04-30 10:17:25.000000 arfs-2.2.6/src/arfs/feature_selection/variable_importance.py
+-rw-rw-rw-   0        0        0    21847 2023-11-27 13:09:10.000000 arfs-2.2.6/src/arfs/gbm.py
+-rw-rw-rw-   0        0        0     6058 2023-11-28 13:14:50.000000 arfs-2.2.6/src/arfs/parallel.py
+-rw-rw-rw-   0        0        0    38113 2024-04-29 16:16:15.000000 arfs-2.2.6/src/arfs/preprocessing.py
+-rw-rw-rw-   0        0        0    15511 2023-11-27 13:09:10.000000 arfs-2.2.6/src/arfs/sampling.py
+-rw-rw-rw-   0        0        0    26942 2023-11-28 13:14:50.000000 arfs-2.2.6/src/arfs/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-30 10:23:57.915145 arfs-2.2.6/src/arfs.egg-info/
+-rw-rw-rw-   0        0        0    13229 2024-04-30 10:23:55.000000 arfs-2.2.6/src/arfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      849 2024-04-30 10:23:56.000000 arfs-2.2.6/src/arfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 10:23:55.000000 arfs-2.2.6/src/arfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-2.2.6/src/arfs.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      358 2024-04-30 10:23:55.000000 arfs-2.2.6/src/arfs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-30 10:23:55.000000 arfs-2.2.6/src/arfs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 10:23:57.837627 arfs-2.2.6/tests/
+-rw-rw-rw-   0        0        0    10867 2023-11-29 14:43:52.000000 arfs-2.2.6/tests/test_allrelevant.py
+-rw-rw-rw-   0        0        0    19531 2023-11-29 14:51:48.000000 arfs-2.2.6/tests/test_featselect.py
```

### Comparing `arfs-2.2.5/LICENSE.md` & `arfs-2.2.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arfs-2.2.5/PKG-INFO` & `arfs-2.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arfs
-Version: 2.2.5
+Version: 2.2.6
 Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
 Author: ThomasBury
 Author-email: bury.thomas@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ThomasBury/arfs
 Project-URL: Source, https://github.com/ThomasBury/arfs
 Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
```

### Comparing `arfs-2.2.5/README.md` & `arfs-2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `arfs-2.2.5/setup.cfg` & `arfs-2.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `arfs-2.2.5/src/arfs/association.py` & `arfs-2.2.6/src/arfs/association.py`

 * *Files identical despite different names*

### Comparing `arfs-2.2.5/src/arfs/benchmark.py` & `arfs-2.2.6/src/arfs/benchmark.py`

 * *Files identical despite different names*

### Comparing `arfs-2.2.5/src/arfs/dataset/data/boston_bunch.joblib` & `arfs-2.2.6/src/arfs/dataset/data/boston_bunch.joblib`

 * *Files identical despite different names*

### Comparing `arfs-2.2.5/src/arfs/dataset/data/housing.zip` & `arfs-2.2.6/src/arfs/dataset/data/housing.zip`

 * *Files identical despite different names*

### Comparing `arfs-2.2.5/src/arfs/feature_selection/__init__.py` & `arfs-2.2.6/src/arfs/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `arfs-2.2.5/src/arfs/feature_selection/allrelevant.py` & `arfs-2.2.6/src/arfs/feature_selection/allrelevant.py`

 * *Files identical despite different names*

### Comparing `arfs-2.2.5/src/arfs/feature_selection/base.py` & `arfs-2.2.6/src/arfs/feature_selection/base.py`

 * *Files identical despite different names*

### Comparing `arfs-2.2.5/src/arfs/feature_selection/lasso.py` & `arfs-2.2.6/src/arfs/feature_selection/lasso.py`

 * *Files identical despite different names*

### Comparing `arfs-2.2.5/src/arfs/feature_selection/mrmr.py` & `arfs-2.2.6/src/arfs/feature_selection/mrmr.py`

 * *Files identical despite different names*

### Comparing `arfs-2.2.5/src/arfs/feature_selection/summary.py` & `arfs-2.2.6/src/arfs/feature_selection/summary.py`

 * *Files identical despite different names*

### Comparing `arfs-2.2.5/src/arfs/feature_selection/unsupervised.py` & `arfs-2.2.6/src/arfs/feature_selection/unsupervised.py`

 * *Files identical despite different names*

### Comparing `arfs-2.2.5/src/arfs/feature_selection/variable_importance.py` & `arfs-2.2.6/src/arfs/feature_selection/variable_importance.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,23 +394,29 @@
                 gbm_model.valid_features, pred_contrib=True
             )
             # the dim changed in lightGBM >= 3.0.0
             if task == "multiclass":
                 # X_SHAP_values (array-like of shape = [n_samples, n_features + 1]
                 # or shape = [n_samples, (n_features + 1) * n_classes])
                 # index starts from 0
-                n_feat = gbm_model.valid_features.shape[1]
+                n_features_plus_bias = gbm_model.valid_features.shape[1] + 1
+                n_samples = gbm_model.valid_features.shape[0]
                 y_freq_table = pd.Series(y.fillna(0)).value_counts(normalize=True)
                 n_classes = y_freq_table.size
-                shap_matrix = np.delete(
-                    shap_matrix,
-                    list(range(n_feat, (n_feat + 1) * n_classes, n_feat + 1)),
-                    axis=1,
-                )
-                shap_imp = np.mean(np.abs(shap_matrix[:, :-1]), axis=0)
+                
+                # Reshape the array to [n_samples, n_features + 1, n_classes]
+                reshaped_values = shap_matrix.reshape(n_samples, n_classes, n_features_plus_bias)
+
+                # Since we need (n_samples, n_features + 1, n_classes), transpose the second and third dimensions
+                reshaped_values = reshaped_values.transpose(0, 2, 1)
+                reshaped_values = reshaped_values[:, :-1, :]
+                reshaped_values.shape
+                # Sum the contributions for each class ignoring the bias term
+                # average on all the samples
+                shap_imp = np.abs(reshaped_values).sum(axis=-1).mean(axis=0)
             else:
                 # for binary, only one class is returned, for regression a single column added as well
                 shap_imp = np.mean(np.abs(shap_matrix[:, :-1]), axis=0)
 
         # Record the feature importances
         feature_importance_values += (
             shap_imp / n_iterations
```

### Comparing `arfs-2.2.5/src/arfs/gbm.py` & `arfs-2.2.6/src/arfs/gbm.py`

 * *Files identical despite different names*

### Comparing `arfs-2.2.5/src/arfs/parallel.py` & `arfs-2.2.6/src/arfs/parallel.py`

 * *Files identical despite different names*

### Comparing `arfs-2.2.5/src/arfs/preprocessing.py` & `arfs-2.2.6/src/arfs/preprocessing.py`

 * *Files identical despite different names*

### Comparing `arfs-2.2.5/src/arfs/sampling.py` & `arfs-2.2.6/src/arfs/sampling.py`

 * *Files identical despite different names*

### Comparing `arfs-2.2.5/src/arfs/utils.py` & `arfs-2.2.6/src/arfs/utils.py`

 * *Files identical despite different names*

### Comparing `arfs-2.2.5/src/arfs.egg-info/PKG-INFO` & `arfs-2.2.6/src/arfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arfs
-Version: 2.2.5
+Version: 2.2.6
 Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
 Author: ThomasBury
 Author-email: bury.thomas@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ThomasBury/arfs
 Project-URL: Source, https://github.com/ThomasBury/arfs
 Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
```

### Comparing `arfs-2.2.5/src/arfs.egg-info/SOURCES.txt` & `arfs-2.2.6/src/arfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arfs-2.2.5/tests/test_allrelevant.py` & `arfs-2.2.6/tests/test_allrelevant.py`

 * *Files identical despite different names*

### Comparing `arfs-2.2.5/tests/test_featselect.py` & `arfs-2.2.6/tests/test_featselect.py`

 * *Files identical despite different names*

