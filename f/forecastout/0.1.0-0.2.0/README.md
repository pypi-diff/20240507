# Comparing `tmp/forecastout-0.1.0.tar.gz` & `tmp/forecastout-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forecastout-0.1.0.tar", max compression
+gzip compressed data, was "forecastout-0.2.0.tar", max compression
```

## Comparing `forecastout-0.1.0.tar` & `forecastout-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,47 @@
--rw-r--r--   0        0        0       13 2024-03-12 15:06:56.954081 forecastout-0.1.0/README.md
--rw-r--r--   0        0        0      336 2024-03-12 14:38:44.842875 forecastout-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-12 15:09:40.924641 forecastout-0.1.0/src/forecastout/__init__.py
--rw-r--r--   0        0        0       86 2024-03-12 14:32:00.299108 forecastout-0.1.0/src/forecastout/function_test.py
--rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 forecastout-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       13 2024-03-12 15:06:56.954081 forecastout-0.2.0/README.md
+-rw-r--r--   0        0        0      454 2024-05-07 13:10:46.906155 forecastout-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-12 15:09:40.924641 forecastout-0.2.0/src/forecastout/__init__.py
+-rw-r--r--   0        0        0      140 2024-05-07 13:09:08.222683 forecastout-0.2.0/src/forecastout/a_data_engine/__init__.py
+-rw-r--r--   0        0        0     5041 2024-05-07 13:09:08.224298 forecastout-0.2.0/src/forecastout/a_data_engine/data_handler.py
+-rw-r--r--   0        0        0     1358 2024-05-07 13:09:08.225308 forecastout-0.2.0/src/forecastout/a_data_engine/train_test_split.py
+-rw-r--r--   0        0        0      469 2024-05-07 13:09:08.226598 forecastout-0.2.0/src/forecastout/b_forecast_engine/__init__.py
+-rw-r--r--   0        0        0     2836 2024-05-07 13:09:08.227773 forecastout-0.2.0/src/forecastout/b_forecast_engine/anomaly_detector.py
+-rw-r--r--   0        0        0     2491 2024-05-07 13:09:08.228874 forecastout-0.2.0/src/forecastout/b_forecast_engine/anomaly_fixer.py
+-rw-r--r--   0        0        0     2810 2024-05-07 13:09:08.230198 forecastout-0.2.0/src/forecastout/b_forecast_engine/backtester.py
+-rw-r--r--   0        0        0      776 2024-05-07 13:09:08.231358 forecastout-0.2.0/src/forecastout/b_forecast_engine/decompose_time_series.py
+-rw-r--r--   0        0        0      790 2024-05-07 13:09:08.232612 forecastout-0.2.0/src/forecastout/b_forecast_engine/ensemble_models.py
+-rw-r--r--   0        0        0     2219 2024-05-07 13:09:08.234171 forecastout-0.2.0/src/forecastout/b_forecast_engine/ensembler.py
+-rw-r--r--   0        0        0     1334 2024-04-15 09:42:13.018586 forecastout-0.2.0/src/forecastout/b_forecast_engine/forecast_model_factory.py
+-rw-r--r--   0        0        0      806 2024-05-07 13:09:08.235508 forecastout-0.2.0/src/forecastout/b_forecast_engine/model_predictor.py
+-rw-r--r--   0        0        0     1052 2024-05-07 13:09:08.236510 forecastout-0.2.0/src/forecastout/b_forecast_engine/model_trainer.py
+-rw-r--r--   0        0        0        0 2024-04-15 09:42:13.020204 forecastout-0.2.0/src/forecastout/c_forecast_models/__init__.py
+-rw-r--r--   0        0        0      442 2024-05-07 13:09:08.237995 forecastout-0.2.0/src/forecastout/c_forecast_models/abstract_model.py
+-rw-r--r--   0        0        0     1509 2024-05-07 13:09:08.239910 forecastout-0.2.0/src/forecastout/c_forecast_models/autoarima_model.py
+-rw-r--r--   0        0        0     3755 2024-05-07 13:09:08.242778 forecastout-0.2.0/src/forecastout/c_forecast_models/holtwinters_model.py
+-rw-r--r--   0        0        0     2302 2024-05-07 13:09:08.244724 forecastout-0.2.0/src/forecastout/c_forecast_models/naive_seasonal.py
+-rw-r--r--   0        0        0     1733 2024-05-07 13:09:08.246057 forecastout-0.2.0/src/forecastout/c_forecast_models/prophet_model.py
+-rw-r--r--   0        0        0     1064 2024-05-07 13:09:08.247160 forecastout-0.2.0/src/forecastout/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-15 09:42:13.026330 forecastout-0.2.0/src/forecastout/d_disaggregation_features/__init__.py
+-rw-r--r--   0        0        0     1348 2024-05-07 13:09:08.248081 forecastout-0.2.0/src/forecastout/d_disaggregation_features/add_features.py
+-rw-r--r--   0        0        0     3092 2024-04-15 09:42:13.028468 forecastout-0.2.0/src/forecastout/d_disaggregation_features/feature_creator.py
+-rw-r--r--   0        0        0      612 2024-05-07 13:09:08.249098 forecastout-0.2.0/src/forecastout/d_disaggregation_features/feature_encoding.py
+-rw-r--r--   0        0        0      561 2024-05-07 13:09:08.251015 forecastout-0.2.0/src/forecastout/d_disaggregation_features/feature_normalizer.py
+-rw-r--r--   0        0        0      605 2024-05-07 13:09:08.252649 forecastout-0.2.0/src/forecastout/e_disaggregation_engine/__init__.py
+-rw-r--r--   0        0        0     1154 2024-05-07 13:09:08.253732 forecastout-0.2.0/src/forecastout/e_disaggregation_engine/disaggregate_monthly_to_daily_forecast.py
+-rw-r--r--   0        0        0      560 2024-05-07 13:09:08.255297 forecastout-0.2.0/src/forecastout/e_disaggregation_engine/disaggregation_model_factory.py
+-rw-r--r--   0        0        0     1684 2024-05-07 13:09:08.257323 forecastout-0.2.0/src/forecastout/e_disaggregation_engine/disaggregation_model_predictor.py
+-rw-r--r--   0        0        0      949 2024-05-07 13:09:08.259017 forecastout-0.2.0/src/forecastout/e_disaggregation_engine/disaggregation_model_trainer.py
+-rw-r--r--   0        0        0     1035 2024-05-07 13:09:08.260138 forecastout-0.2.0/src/forecastout/e_disaggregation_engine/get_daily_shares.py
+-rw-r--r--   0        0        0     1537 2024-05-07 13:09:08.261491 forecastout-0.2.0/src/forecastout/e_disaggregation_engine/remake_monthly_forecast_current_month.py
+-rw-r--r--   0        0        0        0 2024-05-07 13:09:08.261646 forecastout-0.2.0/src/forecastout/f_disaggregation_models/__init__.py
+-rw-r--r--   0        0        0      567 2024-05-07 13:09:08.263393 forecastout-0.2.0/src/forecastout/f_disaggregation_models/abstract_model.py
+-rw-r--r--   0        0        0     2419 2024-05-07 13:09:08.265171 forecastout-0.2.0/src/forecastout/f_disaggregation_models/random_forest_model.py
+-rw-r--r--   0        0        0     7593 2024-05-07 13:09:08.266705 forecastout-0.2.0/src/forecastout/forecastout.py
+-rw-r--r--   0        0        0      880 2024-05-07 13:09:08.268226 forecastout-0.2.0/src/forecastout/main.py
+-rw-r--r--   0        0        0      126 2024-05-07 13:09:08.269190 forecastout-0.2.0/src/forecastout/y_utils/__init__.py
+-rw-r--r--   0        0        0     4689 2024-05-07 13:09:08.270168 forecastout-0.2.0/src/forecastout/y_utils/input_checker.py
+-rw-r--r--   0        0        0      819 2024-05-07 13:09:08.270884 forecastout-0.2.0/src/forecastout/y_utils/update_config.py
+-rw-r--r--   0        0        0        0 2024-03-28 08:26:39.480695 forecastout-0.2.0/src/forecastout/z_data_test/__init__.py
+-rw-r--r--   0        0        0      870 2024-03-28 08:26:39.481184 forecastout-0.2.0/src/forecastout/z_data_test/data_test1.csv
+-rw-r--r--   0        0        0    25910 2024-05-07 13:09:08.272120 forecastout-0.2.0/src/forecastout/z_data_test/data_test2.csv
+-rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 forecastout-0.2.0/PKG-INFO
```
