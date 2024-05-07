# Comparing `tmp/forecastout-0.2.4.tar.gz` & `tmp/forecastout-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forecastout-0.2.4.tar", max compression
+gzip compressed data, was "forecastout-0.2.5.tar", max compression
```

## Comparing `forecastout-0.2.4.tar` & `forecastout-0.2.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0       13 2024-03-12 15:06:56.954081 forecastout-0.2.4/README.md
--rw-r--r--   0        0        0      505 2024-05-07 13:34:25.270943 forecastout-0.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-07 13:28:34.056676 forecastout-0.2.4/src/forecastout/__init__.py
--rw-r--r--   0        0        0      140 2024-05-07 13:09:08.222683 forecastout-0.2.4/src/forecastout/a_data_engine/__init__.py
--rw-r--r--   0        0        0     5041 2024-05-07 13:09:08.224298 forecastout-0.2.4/src/forecastout/a_data_engine/data_handler.py
--rw-r--r--   0        0        0     1358 2024-05-07 13:09:08.225308 forecastout-0.2.4/src/forecastout/a_data_engine/train_test_split.py
--rw-r--r--   0        0        0      469 2024-05-07 13:09:08.226598 forecastout-0.2.4/src/forecastout/b_forecast_engine/__init__.py
--rw-r--r--   0        0        0     2836 2024-05-07 13:09:08.227773 forecastout-0.2.4/src/forecastout/b_forecast_engine/anomaly_detector.py
--rw-r--r--   0        0        0     2491 2024-05-07 13:09:08.228874 forecastout-0.2.4/src/forecastout/b_forecast_engine/anomaly_fixer.py
--rw-r--r--   0        0        0     2810 2024-05-07 13:09:08.230198 forecastout-0.2.4/src/forecastout/b_forecast_engine/backtester.py
--rw-r--r--   0        0        0      776 2024-05-07 13:09:08.231358 forecastout-0.2.4/src/forecastout/b_forecast_engine/decompose_time_series.py
--rw-r--r--   0        0        0      790 2024-05-07 13:09:08.232612 forecastout-0.2.4/src/forecastout/b_forecast_engine/ensemble_models.py
--rw-r--r--   0        0        0     2219 2024-05-07 13:09:08.234171 forecastout-0.2.4/src/forecastout/b_forecast_engine/ensembler.py
--rw-r--r--   0        0        0     1334 2024-04-15 09:42:13.018586 forecastout-0.2.4/src/forecastout/b_forecast_engine/forecast_model_factory.py
--rw-r--r--   0        0        0      806 2024-05-07 13:09:08.235508 forecastout-0.2.4/src/forecastout/b_forecast_engine/model_predictor.py
--rw-r--r--   0        0        0     1052 2024-05-07 13:09:08.236510 forecastout-0.2.4/src/forecastout/b_forecast_engine/model_trainer.py
--rw-r--r--   0        0        0        0 2024-04-15 09:42:13.020204 forecastout-0.2.4/src/forecastout/c_forecast_models/__init__.py
--rw-r--r--   0        0        0      442 2024-05-07 13:09:08.237995 forecastout-0.2.4/src/forecastout/c_forecast_models/abstract_model.py
--rw-r--r--   0        0        0     1509 2024-05-07 13:09:08.239910 forecastout-0.2.4/src/forecastout/c_forecast_models/autoarima_model.py
--rw-r--r--   0        0        0     3755 2024-05-07 13:09:08.242778 forecastout-0.2.4/src/forecastout/c_forecast_models/holtwinters_model.py
--rw-r--r--   0        0        0     2302 2024-05-07 13:09:08.244724 forecastout-0.2.4/src/forecastout/c_forecast_models/naive_seasonal.py
--rw-r--r--   0        0        0     1733 2024-05-07 13:09:08.246057 forecastout-0.2.4/src/forecastout/c_forecast_models/prophet_model.py
--rw-r--r--   0        0        0     1064 2024-05-07 13:09:08.247160 forecastout-0.2.4/src/forecastout/config.yaml
--rw-r--r--   0        0        0        0 2024-04-15 09:42:13.026330 forecastout-0.2.4/src/forecastout/d_disaggregation_features/__init__.py
--rw-r--r--   0        0        0     1348 2024-05-07 13:09:08.248081 forecastout-0.2.4/src/forecastout/d_disaggregation_features/add_features.py
--rw-r--r--   0        0        0     3092 2024-04-15 09:42:13.028468 forecastout-0.2.4/src/forecastout/d_disaggregation_features/feature_creator.py
--rw-r--r--   0        0        0      612 2024-05-07 13:09:08.249098 forecastout-0.2.4/src/forecastout/d_disaggregation_features/feature_encoding.py
--rw-r--r--   0        0        0      561 2024-05-07 13:09:08.251015 forecastout-0.2.4/src/forecastout/d_disaggregation_features/feature_normalizer.py
--rw-r--r--   0        0        0      605 2024-05-07 13:09:08.252649 forecastout-0.2.4/src/forecastout/e_disaggregation_engine/__init__.py
--rw-r--r--   0        0        0     1154 2024-05-07 13:09:08.253732 forecastout-0.2.4/src/forecastout/e_disaggregation_engine/disaggregate_monthly_to_daily_forecast.py
--rw-r--r--   0        0        0      560 2024-05-07 13:09:08.255297 forecastout-0.2.4/src/forecastout/e_disaggregation_engine/disaggregation_model_factory.py
--rw-r--r--   0        0        0     1684 2024-05-07 13:09:08.257323 forecastout-0.2.4/src/forecastout/e_disaggregation_engine/disaggregation_model_predictor.py
--rw-r--r--   0        0        0      949 2024-05-07 13:09:08.259017 forecastout-0.2.4/src/forecastout/e_disaggregation_engine/disaggregation_model_trainer.py
--rw-r--r--   0        0        0     1035 2024-05-07 13:09:08.260138 forecastout-0.2.4/src/forecastout/e_disaggregation_engine/get_daily_shares.py
--rw-r--r--   0        0        0     1537 2024-05-07 13:09:08.261491 forecastout-0.2.4/src/forecastout/e_disaggregation_engine/remake_monthly_forecast_current_month.py
--rw-r--r--   0        0        0        0 2024-05-07 13:09:08.261646 forecastout-0.2.4/src/forecastout/f_disaggregation_models/__init__.py
--rw-r--r--   0        0        0      567 2024-05-07 13:09:08.263393 forecastout-0.2.4/src/forecastout/f_disaggregation_models/abstract_model.py
--rw-r--r--   0        0        0     2419 2024-05-07 13:09:08.265171 forecastout-0.2.4/src/forecastout/f_disaggregation_models/random_forest_model.py
--rw-r--r--   0        0        0     7593 2024-05-07 13:09:08.266705 forecastout-0.2.4/src/forecastout/forecastout.py
--rw-r--r--   0        0        0      880 2024-05-07 13:09:08.268226 forecastout-0.2.4/src/forecastout/main.py
--rw-r--r--   0        0        0      126 2024-05-07 13:09:08.269190 forecastout-0.2.4/src/forecastout/y_utils/__init__.py
--rw-r--r--   0        0        0     4689 2024-05-07 13:09:08.270168 forecastout-0.2.4/src/forecastout/y_utils/input_checker.py
--rw-r--r--   0        0        0      819 2024-05-07 13:09:08.270884 forecastout-0.2.4/src/forecastout/y_utils/update_config.py
--rw-r--r--   0        0        0        0 2024-03-28 08:26:39.480695 forecastout-0.2.4/src/forecastout/z_data_test/__init__.py
--rw-r--r--   0        0        0      870 2024-03-28 08:26:39.481184 forecastout-0.2.4/src/forecastout/z_data_test/data_test1.csv
--rw-r--r--   0        0        0    25910 2024-05-07 13:09:08.272120 forecastout-0.2.4/src/forecastout/z_data_test/data_test2.csv
--rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 forecastout-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       13 2024-03-12 15:06:56.954081 forecastout-0.2.5/README.md
+-rw-r--r--   0        0        0       41 2024-05-07 13:53:54.042126 forecastout-0.2.5/forecastout/__init__.py
+-rw-r--r--   0        0        0      132 2024-05-07 13:50:24.462801 forecastout-0.2.5/forecastout/a_data_engine/__init__.py
+-rw-r--r--   0        0        0     5041 2024-05-07 13:09:08.224000 forecastout-0.2.5/forecastout/a_data_engine/data_handler.py
+-rw-r--r--   0        0        0     1358 2024-05-07 13:09:08.225000 forecastout-0.2.5/forecastout/a_data_engine/train_test_split.py
+-rw-r--r--   0        0        0      445 2024-05-07 13:50:24.303349 forecastout-0.2.5/forecastout/b_forecast_engine/__init__.py
+-rw-r--r--   0        0        0     2836 2024-05-07 13:09:08.227000 forecastout-0.2.5/forecastout/b_forecast_engine/anomaly_detector.py
+-rw-r--r--   0        0        0     2461 2024-05-07 13:50:24.522141 forecastout-0.2.5/forecastout/b_forecast_engine/anomaly_fixer.py
+-rw-r--r--   0        0        0     2780 2024-05-07 13:50:24.334676 forecastout-0.2.5/forecastout/b_forecast_engine/backtester.py
+-rw-r--r--   0        0        0      776 2024-05-07 13:09:08.231000 forecastout-0.2.5/forecastout/b_forecast_engine/decompose_time_series.py
+-rw-r--r--   0        0        0      780 2024-05-07 13:50:24.492189 forecastout-0.2.5/forecastout/b_forecast_engine/ensemble_models.py
+-rw-r--r--   0        0        0     2219 2024-05-07 13:09:08.234000 forecastout-0.2.5/forecastout/b_forecast_engine/ensembler.py
+-rw-r--r--   0        0        0     1294 2024-05-07 13:50:24.370831 forecastout-0.2.5/forecastout/b_forecast_engine/forecast_model_factory.py
+-rw-r--r--   0        0        0      806 2024-05-07 13:09:08.235000 forecastout-0.2.5/forecastout/b_forecast_engine/model_predictor.py
+-rw-r--r--   0        0        0     1048 2024-05-07 13:50:24.344533 forecastout-0.2.5/forecastout/b_forecast_engine/model_trainer.py
+-rw-r--r--   0        0        0        0 2024-04-15 09:42:13.020000 forecastout-0.2.5/forecastout/c_forecast_models/__init__.py
+-rw-r--r--   0        0        0      442 2024-05-07 13:09:08.237000 forecastout-0.2.5/forecastout/c_forecast_models/abstract_model.py
+-rw-r--r--   0        0        0     1499 2024-05-07 13:50:24.391425 forecastout-0.2.5/forecastout/c_forecast_models/autoarima_model.py
+-rw-r--r--   0        0        0     3745 2024-05-07 13:50:24.413897 forecastout-0.2.5/forecastout/c_forecast_models/holtwinters_model.py
+-rw-r--r--   0        0        0     2298 2024-05-07 13:50:24.583771 forecastout-0.2.5/forecastout/c_forecast_models/naive_seasonal.py
+-rw-r--r--   0        0        0     1723 2024-05-07 13:50:24.339749 forecastout-0.2.5/forecastout/c_forecast_models/prophet_model.py
+-rw-r--r--   0        0        0     1064 2024-05-07 13:09:08.247000 forecastout-0.2.5/forecastout/config.yaml
+-rw-r--r--   0        0        0     7573 2024-05-07 13:50:24.447021 forecastout-0.2.5/forecastout/core.py
+-rw-r--r--   0        0        0        0 2024-04-15 09:42:13.026000 forecastout-0.2.5/forecastout/d_disaggregation_features/__init__.py
+-rw-r--r--   0        0        0     1336 2024-05-07 13:50:24.396345 forecastout-0.2.5/forecastout/d_disaggregation_features/add_features.py
+-rw-r--r--   0        0        0     3092 2024-04-15 09:42:13.028000 forecastout-0.2.5/forecastout/d_disaggregation_features/feature_creator.py
+-rw-r--r--   0        0        0      612 2024-05-07 13:09:08.249000 forecastout-0.2.5/forecastout/d_disaggregation_features/feature_encoding.py
+-rw-r--r--   0        0        0      561 2024-05-07 13:09:08.251000 forecastout-0.2.5/forecastout/d_disaggregation_features/feature_normalizer.py
+-rw-r--r--   0        0        0      585 2024-05-07 13:50:24.516029 forecastout-0.2.5/forecastout/e_disaggregation_engine/__init__.py
+-rw-r--r--   0        0        0     1154 2024-05-07 13:09:08.253000 forecastout-0.2.5/forecastout/e_disaggregation_engine/disaggregate_monthly_to_daily_forecast.py
+-rw-r--r--   0        0        0      556 2024-05-07 13:50:24.375781 forecastout-0.2.5/forecastout/e_disaggregation_engine/disaggregation_model_factory.py
+-rw-r--r--   0        0        0     1680 2024-05-07 13:50:24.324360 forecastout-0.2.5/forecastout/e_disaggregation_engine/disaggregation_model_predictor.py
+-rw-r--r--   0        0        0      945 2024-05-07 13:50:24.360961 forecastout-0.2.5/forecastout/e_disaggregation_engine/disaggregation_model_trainer.py
+-rw-r--r--   0        0        0     1035 2024-05-07 13:09:08.260000 forecastout-0.2.5/forecastout/e_disaggregation_engine/get_daily_shares.py
+-rw-r--r--   0        0        0     1537 2024-05-07 13:09:08.261000 forecastout-0.2.5/forecastout/e_disaggregation_engine/remake_monthly_forecast_current_month.py
+-rw-r--r--   0        0        0        0 2024-05-07 13:09:08.261000 forecastout-0.2.5/forecastout/f_disaggregation_models/__init__.py
+-rw-r--r--   0        0        0      567 2024-05-07 13:09:08.263000 forecastout-0.2.5/forecastout/f_disaggregation_models/abstract_model.py
+-rw-r--r--   0        0        0     2415 2024-05-07 13:50:24.511339 forecastout-0.2.5/forecastout/f_disaggregation_models/random_forest_model.py
+-rw-r--r--   0        0        0      864 2024-05-07 13:53:54.037888 forecastout-0.2.5/forecastout/main.py
+-rw-r--r--   0        0        0      118 2024-05-07 13:50:24.385366 forecastout-0.2.5/forecastout/y_utils/__init__.py
+-rw-r--r--   0        0        0     4685 2024-05-07 13:50:24.547551 forecastout-0.2.5/forecastout/y_utils/input_checker.py
+-rw-r--r--   0        0        0      819 2024-05-07 13:09:08.270000 forecastout-0.2.5/forecastout/y_utils/update_config.py
+-rw-r--r--   0        0        0        0 2024-03-28 08:26:39.480000 forecastout-0.2.5/forecastout/z_data_test/__init__.py
+-rw-r--r--   0        0        0      870 2024-03-28 08:26:39.481000 forecastout-0.2.5/forecastout/z_data_test/data_test1.csv
+-rw-r--r--   0        0        0    25910 2024-05-07 13:09:08.272000 forecastout-0.2.5/forecastout/z_data_test/data_test2.csv
+-rw-r--r--   0        0        0      454 2024-05-07 13:54:41.067900 forecastout-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 forecastout-0.2.5/PKG-INFO
```

### Comparing `forecastout-0.2.4/src/forecastout/a_data_engine/data_handler.py` & `forecastout-0.2.5/forecastout/a_data_engine/data_handler.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.2.4/src/forecastout/a_data_engine/train_test_split.py` & `forecastout-0.2.5/forecastout/a_data_engine/train_test_split.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.2.4/src/forecastout/b_forecast_engine/anomaly_detector.py` & `forecastout-0.2.5/forecastout/b_forecast_engine/anomaly_detector.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.2.4/src/forecastout/b_forecast_engine/anomaly_fixer.py` & `forecastout-0.2.5/forecastout/b_forecast_engine/anomaly_fixer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import pandas as pd
-from src.forecastout.b_forecast_engine.anomaly_detector \
-    import AnomalyDetector
-from src.forecastout.b_forecast_engine.model_trainer \
-    import ModelTrainer
-from src.forecastout.b_forecast_engine.model_predictor \
-    import ModelPredictor
+from forecastout.b_forecast_engine.anomaly_detector import AnomalyDetector
+from forecastout.b_forecast_engine.model_trainer import ModelTrainer
+from forecastout.b_forecast_engine.model_predictor import ModelPredictor
 
 
 class AnomalyFixer:
     def __init__(
             self,
             df_forecast: pd.DataFrame,
             df_actual: pd.DataFrame,
```

### Comparing `forecastout-0.2.4/src/forecastout/b_forecast_engine/backtester.py` & `forecastout-0.2.5/forecastout/b_forecast_engine/backtester.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # Main forecasting c_forecast_models
 
 # -- Python main packages
 import pandas as pd
-from src.forecastout.a_data_engine.train_test_split \
-    import TrainTestSplit
-from src.forecastout.b_forecast_engine.model_trainer \
-    import ModelTrainer
-from src.forecastout.b_forecast_engine.model_predictor \
-    import ModelPredictor
+from forecastout.a_data_engine.train_test_split import TrainTestSplit
+from forecastout.b_forecast_engine.model_trainer import ModelTrainer
+from forecastout.b_forecast_engine.model_predictor import ModelPredictor
 
 
 class Backtester:
     def __init__(self, df, model_names, config):
         self.df = df
         self.model_names = model_names
         self.config = config
```

### Comparing `forecastout-0.2.4/src/forecastout/b_forecast_engine/decompose_time_series.py` & `forecastout-0.2.5/forecastout/b_forecast_engine/decompose_time_series.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.2.4/src/forecastout/b_forecast_engine/ensemble_models.py` & `forecastout-0.2.5/forecastout/b_forecast_engine/ensemble_models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from src.forecastout.b_forecast_engine.ensembler \
-    import Ensembler
+from forecastout.b_forecast_engine.ensembler import Ensembler
 import pandas as pd
 
 
 def ensemble_models(
         df_predictions: pd.DataFrame,
         df_models_ranked: pd.DataFrame,
         ensemble_method: str,
```

### Comparing `forecastout-0.2.4/src/forecastout/b_forecast_engine/ensembler.py` & `forecastout-0.2.5/forecastout/b_forecast_engine/ensembler.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.2.4/src/forecastout/b_forecast_engine/forecast_model_factory.py` & `forecastout-0.2.5/forecastout/b_forecast_engine/forecast_model_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 # Main forecasting c_forecast_models
 # -- Python main packages
-from src.forecastout.c_forecast_models.autoarima_model \
-    import AutoArimaModel
-from src.forecastout.c_forecast_models.prophet_model \
-    import ProphetModel
-from src.forecastout.c_forecast_models.holtwinters_model \
-    import HoltWintersModel
-from src.forecastout.c_forecast_models.naive_seasonal \
-    import NaiveSeasonalModel
+from forecastout.c_forecast_models.autoarima_model import AutoArimaModel
+from forecastout.c_forecast_models.prophet_model import ProphetModel
+from forecastout.c_forecast_models.holtwinters_model import HoltWintersModel
+from forecastout.c_forecast_models.naive_seasonal import NaiveSeasonalModel
 
 
 class ForecastModelFactory:
     @staticmethod
     def get_model(model, df_train_y, dict_config, series_train_dates):
         if model == "autoarima":
             return AutoArimaModel(
```

### Comparing `forecastout-0.2.4/src/forecastout/b_forecast_engine/model_predictor.py` & `forecastout-0.2.5/forecastout/b_forecast_engine/model_predictor.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.2.4/src/forecastout/b_forecast_engine/model_trainer.py` & `forecastout-0.2.5/forecastout/b_forecast_engine/model_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pandas as pd
-from src.forecastout.b_forecast_engine.forecast_model_factory \
+from forecastout.b_forecast_engine.forecast_model_factory \
     import ForecastModelFactory
 
 
 class ModelTrainer:
     def __init__(self, model_names, df_train, config):
         self.model_names = model_names
         self.df_train = df_train
```

### Comparing `forecastout-0.2.4/src/forecastout/c_forecast_models/autoarima_model.py` & `forecastout-0.2.5/forecastout/c_forecast_models/autoarima_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from src.forecastout.c_forecast_models.abstract_model \
-    import ForecastModel
+from forecastout.c_forecast_models.abstract_model import ForecastModel
 from pmdarima.arima import auto_arima
 import pandas as pd
 import numpy as np
 
 
 class AutoArimaModel(ForecastModel):
     """
```

### Comparing `forecastout-0.2.4/src/forecastout/c_forecast_models/holtwinters_model.py` & `forecastout-0.2.5/forecastout/c_forecast_models/holtwinters_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from src.forecastout.c_forecast_models.abstract_model \
-    import ForecastModel
+from forecastout.c_forecast_models.abstract_model import ForecastModel
 from statsforecast.models import HoltWinters
 from statsforecast import StatsForecast
 import pandas as pd
 import numpy as np
 
 
 class HoltWintersModel(ForecastModel):
```

### Comparing `forecastout-0.2.4/src/forecastout/c_forecast_models/naive_seasonal.py` & `forecastout-0.2.5/forecastout/c_forecast_models/naive_seasonal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src.forecastout.c_forecast_models.abstract_model import ForecastModel
+from forecastout.c_forecast_models.abstract_model import ForecastModel
 from statsforecast.models import SeasonalNaive
 from statsforecast import StatsForecast
 import pandas as pd
 
 
 class NaiveSeasonalModel(ForecastModel):
     def __init__(self,
```

### Comparing `forecastout-0.2.4/src/forecastout/c_forecast_models/prophet_model.py` & `forecastout-0.2.5/forecastout/c_forecast_models/prophet_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from src.forecastout.c_forecast_models.abstract_model \
-    import ForecastModel
+from forecastout.c_forecast_models.abstract_model import ForecastModel
 from prophet import Prophet
 import pandas as pd
 
 
 class ProphetModel(ForecastModel):
     def __init__(self,
                  series_train_dates: pd.Series,
```

### Comparing `forecastout-0.2.4/src/forecastout/config.yaml` & `forecastout-0.2.5/forecastout/config.yaml`

 * *Files identical despite different names*

### Comparing `forecastout-0.2.4/src/forecastout/d_disaggregation_features/add_features.py` & `forecastout-0.2.5/forecastout/d_disaggregation_features/add_features.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
-from src.forecastout.d_disaggregation_features.feature_creator \
+from forecastout.d_disaggregation_features.feature_creator \
     import FeatureCreator
-from src.forecastout.d_disaggregation_features.feature_normalizer \
+from forecastout.d_disaggregation_features.feature_normalizer \
     import FeatureNormalizer
-from src.forecastout.d_disaggregation_features.feature_encoding \
+from forecastout.d_disaggregation_features.feature_encoding \
     import FeatureEncoder
 
 
 def add_features(
         df: pd.DataFrame,
 ) -> pd.DataFrame:
     """
```

### Comparing `forecastout-0.2.4/src/forecastout/d_disaggregation_features/feature_creator.py` & `forecastout-0.2.5/forecastout/d_disaggregation_features/feature_creator.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.2.4/src/forecastout/d_disaggregation_features/feature_encoding.py` & `forecastout-0.2.5/forecastout/d_disaggregation_features/feature_encoding.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.2.4/src/forecastout/d_disaggregation_features/feature_normalizer.py` & `forecastout-0.2.5/forecastout/d_disaggregation_features/feature_normalizer.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.2.4/src/forecastout/e_disaggregation_engine/__init__.py` & `forecastout-0.2.5/forecastout/e_disaggregation_engine/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from src.forecastout.e_disaggregation_engine.disaggregation_model_trainer \
+from forecastout.e_disaggregation_engine.disaggregation_model_trainer \
     import DisaggregationModelTrainer
-from src.forecastout.e_disaggregation_engine.disaggregation_model_predictor \
+from forecastout.e_disaggregation_engine.disaggregation_model_predictor \
     import DisaggregationModelPredictor
-from src.forecastout.e_disaggregation_engine.get_daily_shares import \
+from forecastout.e_disaggregation_engine.get_daily_shares import \
     get_daily_shares
-from src.forecastout.e_disaggregation_engine\
+from forecastout.e_disaggregation_engine\
     .disaggregate_monthly_to_daily_forecast \
     import disaggregate_monthly_to_daily_forecast
-from src.forecastout.e_disaggregation_engine\
+from forecastout.e_disaggregation_engine\
     .remake_monthly_forecast_current_month \
     import remake_monthly_forecast_current_month
```

### Comparing `forecastout-0.2.4/src/forecastout/e_disaggregation_engine/disaggregate_monthly_to_daily_forecast.py` & `forecastout-0.2.5/forecastout/e_disaggregation_engine/disaggregate_monthly_to_daily_forecast.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.2.4/src/forecastout/e_disaggregation_engine/disaggregation_model_factory.py` & `forecastout-0.2.5/forecastout/e_disaggregation_engine/disaggregation_model_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
 
-from src.forecastout.f_disaggregation_models.random_forest_model \
+from forecastout.f_disaggregation_models.random_forest_model \
     import RandomForestModel
 
 
 class DisaggregationModelFactory:
     @staticmethod
     def get_model(
             disaggregation_model:str,
```

### Comparing `forecastout-0.2.4/src/forecastout/e_disaggregation_engine/disaggregation_model_predictor.py` & `forecastout-0.2.5/forecastout/e_disaggregation_engine/disaggregation_model_predictor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pandas as pd
-from src.forecastout.d_disaggregation_features.feature_creator \
+from forecastout.d_disaggregation_features.feature_creator \
     import FeatureCreator
 
 
 class DisaggregationModelPredictor:
     def __init__(self, model, df: pd.DataFrame, config: dict):
         self.model = model
         self.df = df
```

### Comparing `forecastout-0.2.4/src/forecastout/e_disaggregation_engine/disaggregation_model_trainer.py` & `forecastout-0.2.5/forecastout/e_disaggregation_engine/disaggregation_model_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pandas as pd
-from src.forecastout.e_disaggregation_engine.disaggregation_model_factory \
+from forecastout.e_disaggregation_engine.disaggregation_model_factory \
     import DisaggregationModelFactory
 
 
 class DisaggregationModelTrainer:
     def __init__(
             self,
             df_train: pd.DataFrame,
```

### Comparing `forecastout-0.2.4/src/forecastout/e_disaggregation_engine/get_daily_shares.py` & `forecastout-0.2.5/forecastout/e_disaggregation_engine/get_daily_shares.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.2.4/src/forecastout/e_disaggregation_engine/remake_monthly_forecast_current_month.py` & `forecastout-0.2.5/forecastout/e_disaggregation_engine/remake_monthly_forecast_current_month.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.2.4/src/forecastout/f_disaggregation_models/abstract_model.py` & `forecastout-0.2.5/forecastout/f_disaggregation_models/abstract_model.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.2.4/src/forecastout/f_disaggregation_models/random_forest_model.py` & `forecastout-0.2.5/forecastout/f_disaggregation_models/random_forest_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src.forecastout.f_disaggregation_models.abstract_model \
+from forecastout.f_disaggregation_models.abstract_model \
     import DisaggregationModel
 from sklearn.ensemble import RandomForestRegressor
 from sklearn.model_selection import GridSearchCV, RepeatedKFold
 import pandas as pd
 
 
 class RandomForestModel(DisaggregationModel):
```

### Comparing `forecastout-0.2.4/src/forecastout/forecastout.py` & `forecastout-0.2.5/forecastout/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from src.forecastout.a_data_engine import DataHandler, TrainTestSplit
-from src.forecastout.b_forecast_engine import (
+from forecastout.a_data_engine import DataHandler, TrainTestSplit
+from forecastout.b_forecast_engine import (
     ModelTrainer,
     ModelPredictor,
     Backtester,
     ensemble_models,
     AnomalyFixer,
     create_df_ts_decomposition
 )
-from src.forecastout.d_disaggregation_features.add_features \
+from forecastout.d_disaggregation_features.add_features \
     import add_features
-from src.forecastout.e_disaggregation_engine import (
+from forecastout.e_disaggregation_engine import (
     DisaggregationModelTrainer,
     DisaggregationModelPredictor,
     get_daily_shares,
     disaggregate_monthly_to_daily_forecast,
     remake_monthly_forecast_current_month
 )
-from src.forecastout.y_utils import update_config, InputChecker
+from forecastout.y_utils import update_config, InputChecker
 from logging import Logger
 import pandas as pd
 import os.path as op
 import yaml
 
 
 class ForecastOut:
```

### Comparing `forecastout-0.2.4/src/forecastout/main.py` & `forecastout-0.2.5/forecastout/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pandas as pd
 import os.path as op
-from src.forecastout.forecastout import ForecastOut
+from forecastout import ForecastOut
 
 # -- set options
 pd.set_option('display.max_columns', 100)
 pd.set_option('display.width', 1000)
 
 if __name__ == "__main__":
     # -- Read Data
     current_path = op.dirname(__file__)
-    df = pd.read_csv(op.join(current_path, 'z_data_test/data_test2.csv'))
+    df = pd.read_csv(op.join(current_path, 'z_data_test/data_test1.csv'))
     # -- ForecastOut
     forecastout = ForecastOut(
         df=df.copy(),
         sum_aggregation=True,
         horizon=3,
         months_to_backtest=3,
         models_to_use=['autoarima', 'holtwinters', 'prophet'],
```

### Comparing `forecastout-0.2.4/src/forecastout/y_utils/input_checker.py` & `forecastout-0.2.5/forecastout/y_utils/input_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pandas as pd
-from src.forecastout.a_data_engine.data_handler import DataHandler
+from forecastout.a_data_engine.data_handler import DataHandler
 
 
 class InputChecker:
 
     def __init__(
             self,
             df: pd.DataFrame,
```

### Comparing `forecastout-0.2.4/src/forecastout/y_utils/update_config.py` & `forecastout-0.2.5/forecastout/y_utils/update_config.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.2.4/src/forecastout/z_data_test/data_test1.csv` & `forecastout-0.2.5/forecastout/z_data_test/data_test1.csv`

 * *Files identical despite different names*

### Comparing `forecastout-0.2.4/src/forecastout/z_data_test/data_test2.csv` & `forecastout-0.2.5/forecastout/z_data_test/data_test2.csv`

 * *Files identical despite different names*

