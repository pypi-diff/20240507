# Comparing `tmp/mlops_ods-0.1.202405061002.tar.gz` & `tmp/mlops_ods-0.1.202405071027.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlops_ods-0.1.202405061002.tar", max compression
+gzip compressed data, was "mlops_ods-0.1.202405071027.tar", max compression
```

## Comparing `mlops_ods-0.1.202405061002.tar` & `mlops_ods-0.1.202405071027.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0     1015 2024-05-06 10:02:28.327189 mlops_ods-0.1.202405061002/README.md
--rw-r--r--   0        0        0      840 2024-05-06 10:02:56.371161 mlops_ods-0.1.202405061002/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-06 10:02:28.359189 mlops_ods-0.1.202405061002/src/mlops_ods/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 10:02:28.359189 mlops_ods-0.1.202405061002/src/mlops_ods/app/__init__.py
--rw-r--r--   0        0        0       50 2024-05-06 10:02:28.359189 mlops_ods-0.1.202405061002/src/mlops_ods/app/example.py
--rw-r--r--   0        0        0       69 2024-05-06 10:02:28.359189 mlops_ods-0.1.202405061002/src/mlops_ods/conf/config.yaml
--rw-r--r--   0        0        0      287 2024-05-06 10:02:28.359189 mlops_ods-0.1.202405061002/src/mlops_ods/conf/features/features.yaml
--rw-r--r--   0        0        0      103 2024-05-06 10:02:28.359189 mlops_ods-0.1.202405061002/src/mlops_ods/conf/model/fast.yaml
--rw-r--r--   0        0        0      103 2024-05-06 10:02:28.359189 mlops_ods-0.1.202405061002/src/mlops_ods/conf/model/slow.yaml
--rw-r--r--   0        0        0      146 2024-05-06 10:02:28.359189 mlops_ods-0.1.202405061002/src/mlops_ods/conf/settings/predict.yaml
--rw-r--r--   0        0        0      183 2024-05-06 10:02:28.359189 mlops_ods-0.1.202405061002/src/mlops_ods/conf/settings/train.yaml
--rw-r--r--   0        0        0      702 2024-05-06 10:02:28.359189 mlops_ods-0.1.202405061002/src/mlops_ods/config.py
--rw-r--r--   0        0        0      113 2024-05-06 10:02:28.359189 mlops_ods-0.1.202405061002/src/mlops_ods/dataset/.gitignore
--rw-r--r--   0        0        0      122 2024-05-06 10:02:28.359189 mlops_ods-0.1.202405061002/src/mlops_ods/dataset/2015-street-tree-census-tree-data.csv.dvc
--rw-r--r--   0        0        0       21 2024-05-06 10:02:28.359189 mlops_ods-0.1.202405061002/src/mlops_ods/dataset/features/.gitignore
--rw-r--r--   0        0        0       74 2024-05-06 10:02:28.359189 mlops_ods-0.1.202405061002/src/mlops_ods/dataset/prepared/.gitignore
--rw-r--r--   0        0        0       11 2024-05-06 10:02:28.359189 mlops_ods-0.1.202405061002/src/mlops_ods/dataset/processed/.gitignore
--rw-r--r--   0        0        0       47 2024-05-06 10:02:28.359189 mlops_ods-0.1.202405061002/src/mlops_ods/dvc_functions/__init__.py
--rw-r--r--   0        0        0      127 2024-05-06 10:02:28.359189 mlops_ods-0.1.202405061002/src/mlops_ods/dvc_functions/__main__.py
--rw-r--r--   0        0        0       50 2024-05-06 10:02:28.359189 mlops_ods-0.1.202405061002/src/mlops_ods/dvc_functions/cli.py
--rw-r--r--   0        0        0     2192 2024-05-06 10:02:28.359189 mlops_ods-0.1.202405061002/src/mlops_ods/dvc_functions/models.py
--rw-r--r--   0        0        0      500 2024-05-06 10:02:28.359189 mlops_ods-0.1.202405061002/src/mlops_ods/dvc_functions/preprocessing.py
--rw-r--r--   0        0        0     2013 2024-05-06 10:02:28.359189 mlops_ods-0.1.202405061002/src/mlops_ods/dvc_functions/scaler.py
--rw-r--r--   0        0        0       32 2024-05-06 10:02:28.359189 mlops_ods-0.1.202405061002/src/mlops_ods/models/.gitignore
--rw-r--r--   0        0        0  9730898 2024-05-06 10:02:28.387189 mlops_ods-0.1.202405061002/src/mlops_ods/notebooks/eda.ipynb
--rw-r--r--   0        0        0    51114 2024-05-06 10:02:28.387189 mlops_ods-0.1.202405061002/src/mlops_ods/notebooks/model.ipynb
--rw-r--r--   0        0        0     7740 2024-05-06 10:02:28.387189 mlops_ods-0.1.202405061002/src/mlops_ods/snakemake_scripts/dag.svg
--rw-r--r--   0        0        0      647 2024-05-06 10:02:28.387189 mlops_ods-0.1.202405061002/src/mlops_ods/snakemake_scripts/model_fit.py
--rw-r--r--   0        0        0      624 2024-05-06 10:02:28.387189 mlops_ods-0.1.202405061002/src/mlops_ods/snakemake_scripts/model_fit_bigger.py
--rw-r--r--   0        0        0      268 2024-05-06 10:02:28.387189 mlops_ods-0.1.202405061002/src/mlops_ods/snakemake_scripts/preprocess_data_base.py
--rw-r--r--   0        0        0     1046 2024-05-06 10:02:28.387189 mlops_ods-0.1.202405061002/src/mlops_ods/snakemake_scripts/preprocess_data_research.py
--rw-r--r--   0        0        0      628 2024-05-06 10:02:28.387189 mlops_ods-0.1.202405061002/src/mlops_ods/snakemake_scripts/snakemake_steps.md
--rw-r--r--   0        0        0     2364 2024-05-06 10:02:28.387189 mlops_ods-0.1.202405061002/src/mlops_ods/train_predict.py
--rw-r--r--   0        0        0        0 2024-05-06 10:02:28.387189 mlops_ods-0.1.202405061002/src/mlops_ods/utils/__init__.py
--rw-r--r--   0        0        0     2262 2024-05-06 10:02:28.387189 mlops_ods-0.1.202405061002/src/mlops_ods/utils/utils_etl.py
--rw-r--r--   0        0        0     2138 2024-05-06 10:02:28.387189 mlops_ods-0.1.202405061002/src/mlops_ods/utils/utils_model.py
--rw-r--r--   0        0        0     1973 1970-01-01 00:00:00.000000 mlops_ods-0.1.202405061002/PKG-INFO
+-rw-r--r--   0        0        0     1015 2024-05-07 10:26:35.638046 mlops_ods-0.1.202405071027/README.md
+-rw-r--r--   0        0        0      840 2024-05-07 10:27:02.518207 mlops_ods-0.1.202405071027/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-07 10:26:35.666046 mlops_ods-0.1.202405071027/src/mlops_ods/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 10:26:35.666046 mlops_ods-0.1.202405071027/src/mlops_ods/app/__init__.py
+-rw-r--r--   0        0        0       50 2024-05-07 10:26:35.666046 mlops_ods-0.1.202405071027/src/mlops_ods/app/example.py
+-rw-r--r--   0        0        0       69 2024-05-07 10:26:35.666046 mlops_ods-0.1.202405071027/src/mlops_ods/conf/config.yaml
+-rw-r--r--   0        0        0      287 2024-05-07 10:26:35.666046 mlops_ods-0.1.202405071027/src/mlops_ods/conf/features/features.yaml
+-rw-r--r--   0        0        0      103 2024-05-07 10:26:35.666046 mlops_ods-0.1.202405071027/src/mlops_ods/conf/model/fast.yaml
+-rw-r--r--   0        0        0      103 2024-05-07 10:26:35.666046 mlops_ods-0.1.202405071027/src/mlops_ods/conf/model/slow.yaml
+-rw-r--r--   0        0        0      146 2024-05-07 10:26:35.666046 mlops_ods-0.1.202405071027/src/mlops_ods/conf/settings/predict.yaml
+-rw-r--r--   0        0        0      183 2024-05-07 10:26:35.666046 mlops_ods-0.1.202405071027/src/mlops_ods/conf/settings/train.yaml
+-rw-r--r--   0        0        0      702 2024-05-07 10:26:35.666046 mlops_ods-0.1.202405071027/src/mlops_ods/config.py
+-rw-r--r--   0        0        0      113 2024-05-07 10:26:35.666046 mlops_ods-0.1.202405071027/src/mlops_ods/dataset/.gitignore
+-rw-r--r--   0        0        0      122 2024-05-07 10:26:35.666046 mlops_ods-0.1.202405071027/src/mlops_ods/dataset/2015-street-tree-census-tree-data.csv.dvc
+-rw-r--r--   0        0        0       21 2024-05-07 10:26:35.666046 mlops_ods-0.1.202405071027/src/mlops_ods/dataset/features/.gitignore
+-rw-r--r--   0        0        0       74 2024-05-07 10:26:35.666046 mlops_ods-0.1.202405071027/src/mlops_ods/dataset/prepared/.gitignore
+-rw-r--r--   0        0        0       11 2024-05-07 10:26:35.666046 mlops_ods-0.1.202405071027/src/mlops_ods/dataset/processed/.gitignore
+-rw-r--r--   0        0        0       47 2024-05-07 10:26:35.666046 mlops_ods-0.1.202405071027/src/mlops_ods/dvc_functions/__init__.py
+-rw-r--r--   0        0        0      127 2024-05-07 10:26:35.666046 mlops_ods-0.1.202405071027/src/mlops_ods/dvc_functions/__main__.py
+-rw-r--r--   0        0        0       50 2024-05-07 10:26:35.666046 mlops_ods-0.1.202405071027/src/mlops_ods/dvc_functions/cli.py
+-rw-r--r--   0        0        0     1845 2024-05-07 10:26:35.666046 mlops_ods-0.1.202405071027/src/mlops_ods/dvc_functions/dvc-research.md
+-rw-r--r--   0        0        0     2585 2024-05-07 10:26:35.666046 mlops_ods-0.1.202405071027/src/mlops_ods/dvc_functions/models.py
+-rw-r--r--   0        0        0      500 2024-05-07 10:26:35.666046 mlops_ods-0.1.202405071027/src/mlops_ods/dvc_functions/preprocessing.py
+-rw-r--r--   0        0        0     2013 2024-05-07 10:26:35.666046 mlops_ods-0.1.202405071027/src/mlops_ods/dvc_functions/scaler.py
+-rw-r--r--   0        0        0       49 2024-05-07 10:26:35.666046 mlops_ods-0.1.202405071027/src/mlops_ods/models/.gitignore
+-rw-r--r--   0        0        0  9730898 2024-05-07 10:26:35.694047 mlops_ods-0.1.202405071027/src/mlops_ods/notebooks/eda.ipynb
+-rw-r--r--   0        0        0    51114 2024-05-07 10:26:35.694047 mlops_ods-0.1.202405071027/src/mlops_ods/notebooks/model.ipynb
+-rw-r--r--   0        0        0     7740 2024-05-07 10:26:35.694047 mlops_ods-0.1.202405071027/src/mlops_ods/snakemake_scripts/dag.svg
+-rw-r--r--   0        0        0      647 2024-05-07 10:26:35.694047 mlops_ods-0.1.202405071027/src/mlops_ods/snakemake_scripts/model_fit.py
+-rw-r--r--   0        0        0      624 2024-05-07 10:26:35.694047 mlops_ods-0.1.202405071027/src/mlops_ods/snakemake_scripts/model_fit_bigger.py
+-rw-r--r--   0        0        0      268 2024-05-07 10:26:35.694047 mlops_ods-0.1.202405071027/src/mlops_ods/snakemake_scripts/preprocess_data_base.py
+-rw-r--r--   0        0        0     1046 2024-05-07 10:26:35.694047 mlops_ods-0.1.202405071027/src/mlops_ods/snakemake_scripts/preprocess_data_research.py
+-rw-r--r--   0        0        0      628 2024-05-07 10:26:35.694047 mlops_ods-0.1.202405071027/src/mlops_ods/snakemake_scripts/snakemake_steps.md
+-rw-r--r--   0        0        0     2364 2024-05-07 10:26:35.694047 mlops_ods-0.1.202405071027/src/mlops_ods/train_predict.py
+-rw-r--r--   0        0        0        0 2024-05-07 10:26:35.694047 mlops_ods-0.1.202405071027/src/mlops_ods/utils/__init__.py
+-rw-r--r--   0        0        0     2262 2024-05-07 10:26:35.694047 mlops_ods-0.1.202405071027/src/mlops_ods/utils/utils_etl.py
+-rw-r--r--   0        0        0     2138 2024-05-07 10:26:35.694047 mlops_ods-0.1.202405071027/src/mlops_ods/utils/utils_model.py
+-rw-r--r--   0        0        0     1973 1970-01-01 00:00:00.000000 mlops_ods-0.1.202405071027/PKG-INFO
```

### Comparing `mlops_ods-0.1.202405061002/README.md` & `mlops_ods-0.1.202405071027/README.md`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405061002/pyproject.toml` & `mlops_ods-0.1.202405071027/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlops_ods"
-version = "0.1.202405061002"
+version = "0.1.202405071027"
 description = ""
 authors = ["Iuliia Fokina"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^2.2.2"
```

### Comparing `mlops_ods-0.1.202405061002/src/mlops_ods/config.py` & `mlops_ods-0.1.202405071027/src/mlops_ods/config.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405061002/src/mlops_ods/dvc_functions/models.py` & `mlops_ods-0.1.202405071027/src/mlops_ods/dvc_functions/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import json
 import pickle
 from pathlib import Path
+from typing import Union
 
 import click
 import dvc.api
 import matplotlib.pyplot as plt
 import numpy as np
+from catboost import CatBoostClassifier
 from matplotlib.figure import Figure
 from sklearn.linear_model import LogisticRegression
 from sklearn.metrics import ConfusionMatrixDisplay, classification_report
 
 from .cli import cli
 
 
@@ -19,53 +21,64 @@
     ConfusionMatrixDisplay.from_predictions(y_true, y_pred, ax=ax, colorbar=False)
     ax.xaxis.set_tick_params(rotation=90)
     ax.set_title("Confusion Matrix")
     plt.tight_layout()
     return fig
 
 
-def train(data: np.ndarray, target: np.ndarray) -> LogisticRegression:
+def train(
+    data: np.ndarray, target: np.ndarray, model_name: str
+) -> Union[LogisticRegression, CatBoostClassifier]:
     params = dvc.api.params_show()
-    model_lr = LogisticRegression(**params["log_reg"])
-    model_lr.fit(data, target)
-    return model_lr
+    model = None
+    if model_name == "log_reg":
+        model = LogisticRegression(**params[model_name])
+        model.fit(data, target)
+    elif model_name == "catboost":
+        model = CatBoostClassifier(**params[model_name])
+        model.fit(data, target)
+    return model
 
 
 def test(
-    model: LogisticRegression, data: np.ndarray, target: np.ndarray
+    model: Union[LogisticRegression, CatBoostClassifier],
+    data: np.ndarray,
+    target: np.ndarray,
 ) -> tuple[dict, Figure]:
     predicts = model.predict(data)
     fig = conf_matrix(target, predicts)
     return classification_report(target, predicts, output_dict=True), fig
 
 
 @cli.command()
 @click.argument("train_frame_path", type=Path)
 @click.argument("train_target_path", type=Path)
 @click.argument("model_path", type=Path)
+@click.argument("model_name", type=str)
 def cli_train(
-    train_frame_path: Path,
-    train_target_path: Path,
+    train_frame_path: str,
+    train_target_path: str,
     model_path: Path,
+    model_name: str,
 ):
     train_features = np.load(train_frame_path)
     train_target = np.load(train_target_path)
-    model = train(train_features, train_target)
+    model = train(train_features, train_target, model_name)
     pickle.dump(model, model_path.open("wb"))
 
 
 @cli.command()
 @click.argument("test_frame_path", type=Path)
 @click.argument("test_target_path", type=Path)
 @click.argument("model_path", type=Path)
 @click.argument("metric_path", type=Path)
 @click.argument("figure_path", type=Path)
 def cli_test(
-    test_frame_path: Path,
-    test_target_path: Path,
+    test_frame_path: str,
+    test_target_path: str,
     model_path: Path,
     metric_path: Path,
     figure_path: Path,
 ):
     test_features = np.load(test_frame_path)
     test_target = np.load(test_target_path)
     model = pickle.load(model_path.open("rb"))
```

### Comparing `mlops_ods-0.1.202405061002/src/mlops_ods/dvc_functions/scaler.py` & `mlops_ods-0.1.202405071027/src/mlops_ods/dvc_functions/scaler.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405061002/src/mlops_ods/notebooks/eda.ipynb` & `mlops_ods-0.1.202405071027/src/mlops_ods/notebooks/eda.ipynb`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405061002/src/mlops_ods/notebooks/model.ipynb` & `mlops_ods-0.1.202405071027/src/mlops_ods/notebooks/model.ipynb`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405061002/src/mlops_ods/snakemake_scripts/dag.svg` & `mlops_ods-0.1.202405071027/src/mlops_ods/snakemake_scripts/dag.svg`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405061002/src/mlops_ods/snakemake_scripts/model_fit.py` & `mlops_ods-0.1.202405071027/src/mlops_ods/snakemake_scripts/model_fit.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405061002/src/mlops_ods/snakemake_scripts/model_fit_bigger.py` & `mlops_ods-0.1.202405071027/src/mlops_ods/snakemake_scripts/model_fit_bigger.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405061002/src/mlops_ods/snakemake_scripts/preprocess_data_research.py` & `mlops_ods-0.1.202405071027/src/mlops_ods/snakemake_scripts/preprocess_data_research.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405061002/src/mlops_ods/snakemake_scripts/snakemake_steps.md` & `mlops_ods-0.1.202405071027/src/mlops_ods/snakemake_scripts/snakemake_steps.md`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405061002/src/mlops_ods/train_predict.py` & `mlops_ods-0.1.202405071027/src/mlops_ods/train_predict.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405061002/src/mlops_ods/utils/utils_etl.py` & `mlops_ods-0.1.202405071027/src/mlops_ods/utils/utils_etl.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405061002/src/mlops_ods/utils/utils_model.py` & `mlops_ods-0.1.202405071027/src/mlops_ods/utils/utils_model.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405061002/PKG-INFO` & `mlops_ods-0.1.202405071027/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlops_ods
-Version: 0.1.202405061002
+Version: 0.1.202405071027
 Summary: 
 Author: Iuliia Fokina
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

