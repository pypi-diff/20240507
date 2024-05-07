# Comparing `tmp/canswim-0.0.8.tar.gz` & `tmp/canswim-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canswim-0.0.8.tar", last modified: Tue Mar  5 19:25:26 2024, max compression
+gzip compressed data, was "canswim-0.0.9.tar", last modified: Fri Mar 29 23:00:46 2024, max compression
```

## Comparing `canswim-0.0.8.tar` & `canswim-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 ivelin    (1000) ivelin    (1000)        0 2024-03-05 19:25:26.103789 canswim-0.0.8/
--rw-rw-r--   0 ivelin    (1000) ivelin    (1000)     4177 2024-03-01 18:35:40.000000 canswim-0.0.8/LICENSE.txt
--rw-r--r--   0 ivelin    (1000) ivelin    (1000)     2288 2024-03-05 19:25:26.103789 canswim-0.0.8/PKG-INFO
--rw-rw-r--   0 ivelin    (1000) ivelin    (1000)     1737 2024-03-05 13:09:36.000000 canswim-0.0.8/README.md
--rw-rw-r--   0 ivelin    (1000) ivelin    (1000)      784 2024-03-05 19:25:26.103789 canswim-0.0.8/setup.cfg
--rw-rw-r--   0 ivelin    (1000) ivelin    (1000)     7974 2024-03-01 18:35:40.000000 canswim-0.0.8/setup.py
-drwxrwxr-x   0 ivelin    (1000) ivelin    (1000)        0 2024-03-05 19:25:26.099789 canswim-0.0.8/src/
-drwxrwxr-x   0 ivelin    (1000) ivelin    (1000)        0 2024-03-05 19:25:26.103789 canswim-0.0.8/src/canswim/
--rw-rw-r--   0 ivelin    (1000) ivelin    (1000)        0 2024-03-01 18:35:40.000000 canswim-0.0.8/src/canswim/__init__.py
--rw-rw-r--   0 ivelin    (1000) ivelin    (1000)     3815 2024-03-01 18:35:40.000000 canswim-0.0.8/src/canswim/__main__.py
--rw-rw-r--   0 ivelin    (1000) ivelin    (1000)      121 2024-03-01 18:35:40.000000 canswim-0.0.8/src/canswim/constants.py
--rw-rw-r--   0 ivelin    (1000) ivelin    (1000)    34447 2024-03-01 18:35:40.000000 canswim-0.0.8/src/canswim/covariates.py
-drwxrwxr-x   0 ivelin    (1000) ivelin    (1000)        0 2024-03-05 19:25:26.103789 canswim-0.0.8/src/canswim/dashboard/
--rw-rw-r--   0 ivelin    (1000) ivelin    (1000)     4947 2024-03-05 18:43:29.000000 canswim-0.0.8/src/canswim/dashboard/__init__.py
--rw-rw-r--   0 ivelin    (1000) ivelin    (1000)     2634 2024-03-01 18:35:40.000000 canswim-0.0.8/src/canswim/dashboard/advanced.py
--rw-rw-r--   0 ivelin    (1000) ivelin    (1000)    16075 2024-03-05 03:05:15.000000 canswim-0.0.8/src/canswim/dashboard/charts.py
--rw-rw-r--   0 ivelin    (1000) ivelin    (1000)     2967 2024-03-04 14:28:04.000000 canswim-0.0.8/src/canswim/dashboard/scans.py
--rw-rw-r--   0 ivelin    (1000) ivelin    (1000)     7253 2024-03-01 18:35:40.000000 canswim-0.0.8/src/canswim/forecast.py
--rw-rw-r--   0 ivelin    (1000) ivelin    (1000)    24099 2024-03-05 03:24:53.000000 canswim-0.0.8/src/canswim/gather_data.py
--rw-rw-r--   0 ivelin    (1000) ivelin    (1000)     6937 2024-03-01 18:35:40.000000 canswim-0.0.8/src/canswim/hfhub.py
--rw-rw-r--   0 ivelin    (1000) ivelin    (1000)    45898 2024-03-05 19:17:59.000000 canswim-0.0.8/src/canswim/model.py
--rw-rw-r--   0 ivelin    (1000) ivelin    (1000)     1861 2024-03-01 18:35:40.000000 canswim-0.0.8/src/canswim/model_search.py
--rw-rw-r--   0 ivelin    (1000) ivelin    (1000)     5409 2024-03-01 18:35:40.000000 canswim-0.0.8/src/canswim/targets.py
--rw-rw-r--   0 ivelin    (1000) ivelin    (1000)     6950 2024-03-01 18:35:40.000000 canswim-0.0.8/src/canswim/train.py
-drwxrwxr-x   0 ivelin    (1000) ivelin    (1000)        0 2024-03-05 19:25:26.103789 canswim-0.0.8/src/canswim.egg-info/
--rw-r--r--   0 ivelin    (1000) ivelin    (1000)     2288 2024-03-05 19:25:26.000000 canswim-0.0.8/src/canswim.egg-info/PKG-INFO
--rw-rw-r--   0 ivelin    (1000) ivelin    (1000)      643 2024-03-05 19:25:26.000000 canswim-0.0.8/src/canswim.egg-info/SOURCES.txt
--rw-rw-r--   0 ivelin    (1000) ivelin    (1000)        1 2024-03-05 19:25:26.000000 canswim-0.0.8/src/canswim.egg-info/dependency_links.txt
--rw-rw-r--   0 ivelin    (1000) ivelin    (1000)        1 2024-02-04 02:37:57.000000 canswim-0.0.8/src/canswim.egg-info/not-zip-safe
--rw-rw-r--   0 ivelin    (1000) ivelin    (1000)       73 2024-03-05 19:25:26.000000 canswim-0.0.8/src/canswim.egg-info/requires.txt
--rw-rw-r--   0 ivelin    (1000) ivelin    (1000)        8 2024-03-05 19:25:26.000000 canswim-0.0.8/src/canswim.egg-info/top_level.txt
+drwxrwxr-x   0 ivelin    (1000) ivelin    (1000)        0 2024-03-29 23:00:46.178596 canswim-0.0.9/
+-rw-rw-r--   0 ivelin    (1000) ivelin    (1000)     4177 2024-03-01 18:35:40.000000 canswim-0.0.9/LICENSE.txt
+-rw-r--r--   0 ivelin    (1000) ivelin    (1000)     1912 2024-03-29 23:00:46.178596 canswim-0.0.9/PKG-INFO
+-rw-rw-r--   0 ivelin    (1000) ivelin    (1000)     1361 2024-03-14 01:32:45.000000 canswim-0.0.9/README.md
+-rw-rw-r--   0 ivelin    (1000) ivelin    (1000)      784 2024-03-29 23:00:46.178596 canswim-0.0.9/setup.cfg
+-rw-rw-r--   0 ivelin    (1000) ivelin    (1000)     7974 2024-03-01 18:35:40.000000 canswim-0.0.9/setup.py
+drwxrwxr-x   0 ivelin    (1000) ivelin    (1000)        0 2024-03-29 23:00:46.174596 canswim-0.0.9/src/
+drwxrwxr-x   0 ivelin    (1000) ivelin    (1000)        0 2024-03-29 23:00:46.178596 canswim-0.0.9/src/canswim/
+-rw-rw-r--   0 ivelin    (1000) ivelin    (1000)        0 2024-03-01 18:35:40.000000 canswim-0.0.9/src/canswim/__init__.py
+-rw-rw-r--   0 ivelin    (1000) ivelin    (1000)     3711 2024-03-14 01:32:45.000000 canswim-0.0.9/src/canswim/__main__.py
+-rw-rw-r--   0 ivelin    (1000) ivelin    (1000)      121 2024-03-01 18:35:40.000000 canswim-0.0.9/src/canswim/constants.py
+-rw-rw-r--   0 ivelin    (1000) ivelin    (1000)    46986 2024-03-25 22:34:49.000000 canswim-0.0.9/src/canswim/covariates.py
+drwxrwxr-x   0 ivelin    (1000) ivelin    (1000)        0 2024-03-29 23:00:46.178596 canswim-0.0.9/src/canswim/dashboard/
+-rw-rw-r--   0 ivelin    (1000) ivelin    (1000)     5304 2024-03-27 21:44:33.000000 canswim-0.0.9/src/canswim/dashboard/__init__.py
+-rw-rw-r--   0 ivelin    (1000) ivelin    (1000)     2758 2024-03-27 13:39:55.000000 canswim-0.0.9/src/canswim/dashboard/advanced.py
+-rw-rw-r--   0 ivelin    (1000) ivelin    (1000)    16461 2024-03-27 21:58:53.000000 canswim-0.0.9/src/canswim/dashboard/charts.py
+-rw-rw-r--   0 ivelin    (1000) ivelin    (1000)     3238 2024-03-27 22:03:15.000000 canswim-0.0.9/src/canswim/dashboard/scans.py
+-rw-rw-r--   0 ivelin    (1000) ivelin    (1000)    11942 2024-03-18 16:38:57.000000 canswim-0.0.9/src/canswim/forecast.py
+-rw-rw-r--   0 ivelin    (1000) ivelin    (1000)    29563 2024-03-29 14:38:29.000000 canswim-0.0.9/src/canswim/gather_data.py
+-rw-rw-r--   0 ivelin    (1000) ivelin    (1000)     7947 2024-03-29 18:40:03.000000 canswim-0.0.9/src/canswim/hfhub.py
+-rw-rw-r--   0 ivelin    (1000) ivelin    (1000)    47536 2024-03-18 16:33:51.000000 canswim-0.0.9/src/canswim/model.py
+-rw-rw-r--   0 ivelin    (1000) ivelin    (1000)     1861 2024-03-01 18:35:40.000000 canswim-0.0.9/src/canswim/model_search.py
+-rw-rw-r--   0 ivelin    (1000) ivelin    (1000)     5504 2024-03-14 01:32:45.000000 canswim-0.0.9/src/canswim/targets.py
+-rw-rw-r--   0 ivelin    (1000) ivelin    (1000)     6950 2024-03-14 01:32:45.000000 canswim-0.0.9/src/canswim/train.py
+drwxrwxr-x   0 ivelin    (1000) ivelin    (1000)        0 2024-03-29 23:00:46.178596 canswim-0.0.9/src/canswim.egg-info/
+-rw-r--r--   0 ivelin    (1000) ivelin    (1000)     1912 2024-03-29 23:00:46.000000 canswim-0.0.9/src/canswim.egg-info/PKG-INFO
+-rw-rw-r--   0 ivelin    (1000) ivelin    (1000)      643 2024-03-29 23:00:46.000000 canswim-0.0.9/src/canswim.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivelin    (1000) ivelin    (1000)        1 2024-03-29 23:00:46.000000 canswim-0.0.9/src/canswim.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivelin    (1000) ivelin    (1000)        1 2024-02-04 02:37:57.000000 canswim-0.0.9/src/canswim.egg-info/not-zip-safe
+-rw-rw-r--   0 ivelin    (1000) ivelin    (1000)       73 2024-03-29 23:00:46.000000 canswim-0.0.9/src/canswim.egg-info/requires.txt
+-rw-rw-r--   0 ivelin    (1000) ivelin    (1000)        8 2024-03-29 23:00:46.000000 canswim-0.0.9/src/canswim.egg-info/top_level.txt
```

### Comparing `canswim-0.0.8/LICENSE.txt` & `canswim-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `canswim-0.0.8/PKG-INFO` & `canswim-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canswim
-Version: 0.0.8
+Version: 0.0.9
 Summary: "Developer toolkit for IBD CANSLIM practitioners"
 Author: Ivelin Ivanov
 Author-email: ivelin117@gmail.com
 License: Apache-2.0
 Keywords: stock market,analytics
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -42,30 +42,22 @@
 ```
 $ python -m canswim -h
 usage: canswim [-h] {dashboard,train}
 
 CANSWIM is a toolkit for CANSLIM style investors. Aims to complement the Simple Moving Average and other technical indicators.
 
 positional arguments:
-  {dashboard,gatherdata,uploaddata,modelsearch,train,finetune,forecast}
+  {dashboard,gatherdata,uploaddata,modelsearch,train,forecast}
                         Which canswim task to run:
-                        `dashboard` for stock charting and scans of recorded forecasts.
+                        `dashboard` - start Web App service with stock charting and forecast scans.
                         'gatherdata` to gather 3rd party stock market data and save to HF Hub.
                         'uploaddata` upload to HF Hub any interim changes to local data storage.
                         `modelsearch` to find and save optimal hyperparameters for model training.
                         `train` for continuous model training.
-                        `finetune` to fine tune pretrained model on new stock market data. `forecast` to run forecast on stocks and upload dataset to HF Hub.
 
 options:
   -h, --help            show this help message and exit
   --forecast_start_date FORECAST_START_DATE
                         Optional argument for the `forecast` task. Indicate forecast start date in YYYY-MM-DD format. If not specified, forecast will start from the end of the target series.
 
 NOTE: NOT FINANCIAL OR INVESTMENT ADVICE. USE AT YOUR OWN RISK.
 ```
-
-## Interactive Dashboard hosted on Hugging Face Hub
-
-
-https://huggingface.co/spaces/ivelin/canswim_playground
-
-![canswim playground](https://github.com/ivelin/canswim/assets/2234901/26fb1a5d-49e0-4888-bc1b-042800bcef8f)
```

### Comparing `canswim-0.0.8/README.md` & `canswim-0.0.9/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -21,30 +21,22 @@
 ```
 $ python -m canswim -h
 usage: canswim [-h] {dashboard,train}
 
 CANSWIM is a toolkit for CANSLIM style investors. Aims to complement the Simple Moving Average and other technical indicators.
 
 positional arguments:
-  {dashboard,gatherdata,uploaddata,modelsearch,train,finetune,forecast}
+  {dashboard,gatherdata,uploaddata,modelsearch,train,forecast}
                         Which canswim task to run:
-                        `dashboard` for stock charting and scans of recorded forecasts.
+                        `dashboard` - start Web App service with stock charting and forecast scans.
                         'gatherdata` to gather 3rd party stock market data and save to HF Hub.
                         'uploaddata` upload to HF Hub any interim changes to local data storage.
                         `modelsearch` to find and save optimal hyperparameters for model training.
                         `train` for continuous model training.
-                        `finetune` to fine tune pretrained model on new stock market data. `forecast` to run forecast on stocks and upload dataset to HF Hub.
 
 options:
   -h, --help            show this help message and exit
   --forecast_start_date FORECAST_START_DATE
                         Optional argument for the `forecast` task. Indicate forecast start date in YYYY-MM-DD format. If not specified, forecast will start from the end of the target series.
 
 NOTE: NOT FINANCIAL OR INVESTMENT ADVICE. USE AT YOUR OWN RISK.
 ```
-
-## Interactive Dashboard hosted on Hugging Face Hub
-
-
-https://huggingface.co/spaces/ivelin/canswim_playground
-
-![canswim playground](https://github.com/ivelin/canswim/assets/2234901/26fb1a5d-49e0-4888-bc1b-042800bcef8f)
```

### Comparing `canswim-0.0.8/setup.cfg` & `canswim-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = canswim
-version = 0.0.8
+version = 0.0.9
 author = Ivelin Ivanov
 author_email = ivelin117@gmail.com
 description = "Developer toolkit for IBD CANSLIM practitioners"
 long_description = file: README.md
 keywords = stock market, analytics
 license = Apache-2.0
 classifiers =
```

### Comparing `canswim-0.0.8/setup.py` & `canswim-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `canswim-0.0.8/src/canswim/__main__.py` & `canswim-0.0.9/src/canswim/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,16 +13,21 @@
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 """
 
 import signal
 import sys
-from loguru import logger
 from dotenv import load_dotenv
+
+# load os env vars before loguru import
+# otherwise it won't pickup LOGURU_LEVEL
+load_dotenv(override=True)
+
+from loguru import logger
 import os
 import argparse
 from canswim import dashboard, gather_data, model_search, train, forecast
 from canswim.hfhub import HFHub
 
 # Instantiate the parser
 parser = argparse.ArgumentParser(
@@ -39,25 +44,23 @@
     help="""Which %(prog)s task to run:
         `dashboard` for stock charting and scans of recorded forecasts.
         'gatherdata` to gather 3rd party stock market data and save to HF Hub.
         'downloaddata` download model training and forecast data from HF Hub to local data storage.
         'uploaddata` upload to HF Hub any interim changes to local train and forecast data.
         `modelsearch` to find and save optimal hyperparameters for model training.
         `train` for continuous model training.
-        `finetune` to fine tune pretrained model on new stock market data.
         `forecast` to run forecast on stocks and upload dataset to HF Hub.
         """,
     choices=[
         "dashboard",
         "gatherdata",
         "downloaddata",
         "uploaddata",
         "modelsearch",
         "train",
-        "finetune",
         "forecast",
     ],
 )
 
 parser.add_argument(
     "--forecast_start_date",
     type=str,
@@ -71,15 +74,14 @@
     required=False,
     default=False,
     help="""Optional argument for the `train` task. Whether to train a newly created model or continue training an existing pre-trained model.""",
 )
 
 args = parser.parse_args()
 
-load_dotenv(override=True)
 logging_dir = os.getenv("logging_dir", "tmp")
 logging_path = f"{logging_dir}/canswim.log"
 rot = "24 hours"
 ret = "30 days"
 logger.add(logging_path, rotation=rot, retention=ret)
 
 logger.info(
@@ -112,13 +114,11 @@
         gather_data.main()
     case "downloaddata":
         hfhub.download_data()
     case "uploaddata":
         hfhub.upload_data()
     case "train":
         train.main(new_model=args.new_model)
-    case "finetune":
-        raise NotImplementedError("finetune task not implemented yet")
     case "forecast":
         forecast.main(forecast_start_date=args.forecast_start_date)
     case _:
         logger.error("Unrecognized task argument {m} ", m=args.module)
```

### Comparing `canswim-0.0.8/src/canswim/covariates.py` & `canswim-0.0.9/src/canswim/covariates.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pandas.tseries.offsets import BDay
 import pandas as pd
 from darts import TimeSeries
 from darts.dataprocessing.transformers import MissingValuesFiller
 from typing import Union
 import numpy as np
 from loguru import logger
+import os
 
 fiscal_periods = ["quarter", "annual"]
 fiscal_freq = {"annual": "Y", "quarter": "Q"}
 
 
 # credit for implementation: https://stackoverflow.com/a/39068260/12015435
 def is_business_day(date):
@@ -28,14 +29,16 @@
         return date
 
 
 class Covariates:
     def __init__(self):
         self.past_covariates = {}
         self.future_covariates = {}
+        self.data_dir = os.getenv("data_dir", "data")
+        self.data_3rd_party = os.getenv("data-3rd-party", "data-3rd-party")
 
     @property
     def pyarrow_filters(self):
         return [
             ("Symbol", "in", self.__load_tickers),
             ("Date", ">=", self.__start_date),
         ]
@@ -45,15 +48,15 @@
         # drop columns used in target series
         past_price_covariates = {
             t: stock_price_series[t].drop_columns(col_names=target_columns)
             for t in stock_price_series.keys()
         }
         return past_price_covariates
 
-    # backfill quarterly earnigs and revenue estimates so that the model can see the next quarter's estimates during the previou s quarter days
+    # backfill quarterly earnigs and revenue estimates so that the model can see the next quarter's estimates during the previous quarter days
 
     def back_fill_earn_estimates(self, t_earn=None):
         t_earn["time"] = t_earn["time"].bfill()
         t_earn["epsEstimated"] = t_earn["epsEstimated"].bfill()
         t_earn["revenueEstimated"] = t_earn["revenueEstimated"].bfill()
         t_earn["fiscalDateEnding_day"] = t_earn["fiscalDateEnding_day"].bfill()
         t_earn["fiscalDateEnding_month"] = t_earn["fiscalDateEnding_month"].bfill()
@@ -195,62 +198,60 @@
                 ##static_covs_single = pd.DataFrame(data={"cik": [cik]})
                 # logger.info(f"Company with ticker {t} has cik: {cik}")
                 ts_tmp = TimeSeries.from_dataframe(
                     t_iown, freq="B", fill_missing_dates=True
                 )
                 t_iown = ts_tmp.pd_dataframe()
                 t_iown.ffill(inplace=True)
+                # use 0 as a filler for unknown ownership absolute values and deltas
                 ts = TimeSeries.from_dataframe(t_iown, fillna_value=0)
                 ts_padded = self.pad_covs(
                     cov_series=ts, price_series=prices, fillna_value=0
                 )
-                ##ts_padded = ts_padded.with_static_covariates(
-                ##    covariates=static_covs_single
-                ##)
-                # logger.info(f'kms_ser_padded start time, end time: {kms_ser_padded.start_time()}, {kms_ser_padded.end_time()}')
                 assert (
                     len(ts_padded.gaps()) == 0
                 ), f"found gaps in series: \n{ts_padded.gaps()}"
                 t_inst_ownership_series[t] = ts_padded
-                assert len(ts_padded.gaps()) == 0
-                t_inst_ownership_series[t] = ts_padded
-            except Exception as e:
-                # df1 = (
-                #    t_iown.groupby(t_iown.columns.tolist())
-                #    .apply(lambda x: tuple(x.index))
-                #   .reset_index(name="date")
-                # )
+            except KeyError as e:
+                logger.info(
+                    f"""Skipping {t} from covariates series. 
+                        No institutional ownership data available for {t}, error: {type(e)}, {e}"""
+                )
+            except AssertionError as e:
                 logger.warning(f"Skipping {t} due to error: {type(e)}: {e}")
-                # logger.info(
-                #    f"Duplicated index rows: \n {t_iown.loc[t_iown.index == pd.Timestamp('1987-03-31')]}"
-                #
-                # return t_iown
 
         return t_inst_ownership_series
 
     def stack_covariates(self, old_covs=None, new_covs=None, min_samples=1):
-        logger.info(f"stacking covariates")
+        logger.info(f"stacking covariates.")
         # stack sales and earnigns to past covariates
         stacked_covs = {}
         for t, covs in list(old_covs.items()):
             try:
                 assert (
                     type(new_covs[t]) == TimeSeries
                 ), f"type of {t} is not TimeSeries, but {type(new_covs[t])}"
                 # logger.info(f'stacking future covs for {t}')
                 old_sliced = covs.slice_intersect(new_covs[t])
                 new_sliced = new_covs[t].slice_intersect(old_sliced)
                 stacked = old_sliced.stack(new_sliced)
-                # logger.info(f'past covariates for {t} including earnings calendar: {len(new_past_covs[t].components)}')
-                # logger.info(f'past covariates for {t} start time: {new_past_covs[t].start_time()}, end time: {new_past_covs[t].end_time()}')
-                # logger.info(f'past covariates for {t} sample: \n{new_past_covs[t][0].pd_dataframe()}')
+                # logger.debug(
+                #     f"covariates for {t} start time: {stacked.start_time()}, end time: {stacked.end_time()}"
+                # )
+                # logger.debug(f"covariates for {t} sample: \n{stacked.pd_dataframe()}")
                 if len(stacked) >= min_samples:
                     stacked_covs[t] = stacked
+                else:
+                    logger.info(
+                        f"Skipping {t} due to lack of min {min_samples} samples. Only {len(stacked)} samples available in covs stack."
+                    )
             except KeyError as e:
                 logger.warning(f"Skipping {t} due to error: {type(e)}: {e}")
+        if len(stacked_covs.keys()) > 0:
+            logger.info(f"stacked covariates column count: {len(stacked.columns)}")
         return stacked_covs
 
     def df_index_to_biz_days(self, df=None):
         new_index = df.index.map(lambda x: to_biz_day(date=x))
         df.index = new_index
         return df
 
@@ -365,17 +366,17 @@
         sectors_series = sectors_series.slice(
             train_date_start, sectors_series.end_time()
         )
         filler = MissingValuesFiller(n_jobs=-1)
         series_filled = filler.transform(sectors_series)
         assert len(series_filled.gaps()) == 0
         sectors_series = series_filled
-        logger.info(
-            f"Finished preparing past covariates: market sectors. {len(sectors_series)} records, columns: {sectors_series.columns}"
-        )
+        # logger.debug(
+        #     f"Finished preparing past covariates: market sectors. {len(sectors_series)} records, columns: {sectors_series.columns}"
+        # )
         return sectors_series
 
     def prepare_industry_fund_series(self, train_date_start=None):
         logger.info("preparing past covariates: industry funds")
         industry_funds_df = self.industry_funds_df.copy()
         # flatten column hierarchy so Darts can use as covariate series
         industry_funds_df.columns = [f"{i}_{j}" for i, j in industry_funds_df.columns]
@@ -386,17 +387,17 @@
         industry_funds_series = industry_funds_series.slice(
             train_date_start, industry_funds_series.end_time()
         )
         filler = MissingValuesFiller(n_jobs=-1)
         industry_funds_filled = filler.transform(industry_funds_series)
         assert len(industry_funds_filled.gaps()) == 0
         industry_funds_series = industry_funds_filled
-        logger.info(
-            f"Finished preparing past covariates: industry funds. {len(industry_funds_series.columns)} columns, {len(industry_funds_series)} records,  \ncolumns: \n{industry_funds_series.columns}"
-        )
+        # logger.debug(
+        #     f"Finished preparing past covariates: industry funds. {len(industry_funds_series.columns)} columns, {len(industry_funds_series)} records,  \ncolumns: \n{industry_funds_series.columns}"
+        # )
         return industry_funds_series
 
     def load_data(self, stock_tickers: set = None, start_date: pd.Timestamp = None):
         self.__start_date = start_date
         self.__load_tickers = stock_tickers
         self.load_past_covariates()
         self.load_future_covariates()
@@ -437,14 +438,16 @@
 
     def load_industry_funds(self):
         file = "data/data-3rd-party/industry_funds.parquet"
         self.industry_funds_df = pd.read_parquet(file)
 
     def load_future_covariates(self):
         self.load_estimates()
+        self.load_dividends()
+        self.load_splits()
 
     def prepare_data(
         self,
         stock_price_series: dict = None,
         target_columns: Union[str, list] = None,
         train_date_start: pd.Timestamp = None,
         min_samples: int = None,
@@ -501,25 +504,44 @@
         self.est_loaded_df = {}
         for period in fiscal_periods:
             assert period in fiscal_periods
             est_file = f"data/data-3rd-party/analyst_estimates_{period}.parquet"
             logger.info(f"Loading data from: {est_file}")
             # est_loaded_df = pd.read_csv(est_file)
             est_loaded_df = pd.read_parquet(est_file, filters=self.pyarrow_filters)
+            # drop duplicate index rows
+            est_loaded_df = est_loaded_df[~est_loaded_df.index.duplicated(keep="last")]
             assert est_loaded_df.index.is_unique
-            # logger.info(f'{period} estimates loaded: \n{est_loaded_df}')
-            # est_loaded_df["date"] = pd.to_datetime(est_loaded_df["date"])
-            est_unique = est_loaded_df.drop_duplicates()  # subset=["symbol", "date"])
-            assert not est_unique.duplicated().any()
-            # est_unique = est_unique.set_index(keys=["symbol", "date"])
-            assert est_loaded_df.index.has_duplicates == False
-            assert est_loaded_df.index.is_unique == True
+            est_loaded_df = est_loaded_df.drop_duplicates()
+            assert not est_loaded_df.duplicated().any()
             # logger.info(f'{period} estimates prepared: \n{est_unique}')
             self.est_loaded_df[period] = est_loaded_df
 
+    def load_dividends(self):
+        self.dividends_loaded_df = {}
+        data_file = f"{self.data_dir}/{self.data_3rd_party}/stock_dividends.parquet"
+        logger.info(f"Loading data from: {data_file}")
+        loaded_df = pd.read_parquet(data_file, filters=self.pyarrow_filters)
+        assert loaded_df.index.is_unique
+        loaded_df = loaded_df.drop_duplicates()
+        assert not loaded_df.duplicated().any()
+        # logger.debug(f"Dividends loaded: \n{loaded_df}")
+        self.dividends_loaded_df = loaded_df
+
+    def load_splits(self):
+        self.splits_loaded_df = {}
+        data_file = f"{self.data_dir}/{self.data_3rd_party}/stock_splits.parquet"
+        logger.info(f"Loading data from: {data_file}")
+        loaded_df = pd.read_parquet(data_file, filters=self.pyarrow_filters)
+        assert loaded_df.index.is_unique
+        loaded_df = loaded_df.drop_duplicates()
+        assert not loaded_df.duplicated().any()
+        # logger.debug(f"Splits loaded: \n{loaded_df}")
+        self.splits_loaded_df = loaded_df
+
     def est_add_future_periods(self, est_df=None, n_future_periods=None, period=None):
         """
         Prepare time series with concatenated estimates for n_future_periods
         """
         # new_df = pd.DataFrame(index=est_df.index)
         # logger.info('est_df', est_df)
         # add fiscalDateEnding columns
@@ -598,16 +620,16 @@
                 assert (
                     len(est_padded.gaps()) == 0
                 ), f"found gaps in series: \n{est_padded.gaps()}"
                 t_est_series[t] = est_padded
 
             except KeyError as e:
                 logger.info(
-                    f"Skipping {t} from covariates series. No analyst estimates available for {t}, error:",
-                    e,
+                    f"""Skipping {t} from covariates series. 
+                        No analyst estimates available for {t}, error: {type(e)}, {e}"""
                 )
         return t_est_series
 
     def prepare_analyst_estimates(self, stock_price_series=None):
         logger.info("preparing future covariates: analyst estimates")
         quarter_est_series = self.prepare_est_series(
             all_est_df=self.est_loaded_df["quarter"],
@@ -627,47 +649,54 @@
         self,
         stock_price_series: dict = None,
         target_columns: Union[str, list] = None,
         train_date_start: pd.Timestamp = None,
     ):
         logger.info("preparing past covariates")
         # start with price-volume covariates
-        price_covariates = self.get_price_covariates(
+        past_covariates = self.get_price_covariates(
             stock_price_series=stock_price_series, target_columns=target_columns
         )
         # add revenue and earnings covariates
-        self.earn_covariates = self.prepare_earn_series(
-            tickers=stock_price_series.keys()
-        )
-        self.past_covariates = self.stack_covariates(
-            old_covs=price_covariates, new_covs=self.earn_covariates
+        earn_covariates = self.prepare_earn_series(tickers=stock_price_series.keys())
+        past_covariates = self.stack_covariates(
+            old_covs=past_covariates, new_covs=earn_covariates
         )
         # add key metrics covariates
         kms_series = self.prepare_key_metrics(stock_price_series=stock_price_series)
         past_covariates = self.stack_covariates(
-            old_covs=self.past_covariates, new_covs=kms_series
+            old_covs=past_covariates, new_covs=kms_series
+        )
+        # add historical stock splits covariates
+        stock_split_series = self.prepare_splits(stock_price_series=stock_price_series)
+        past_covariates = self.stack_covariates(
+            old_covs=past_covariates, new_covs=stock_split_series
         )
+        # add stock institutional ownership covariates
         inst_ownership_series = self.prepare_institutional_symbol_ownership_series(
             stock_price_series=stock_price_series
         )
         past_covariates = self.stack_covariates(
             old_covs=past_covariates, new_covs=inst_ownership_series
         )
+        # add broad market covariates
         broad_market_series = self.prepare_broad_market_series(
             train_date_start=train_date_start
         )
         broad_market_dict = {t: broad_market_series for t in stock_price_series.keys()}
         past_covariates = self.stack_covariates(
             old_covs=past_covariates, new_covs=broad_market_dict
         )
+        # add market sectors covariates
         sectors_series = self.prepare_sectors_series(train_date_start=train_date_start)
         sectors_dict = {t: sectors_series for t in stock_price_series.keys()}
         past_covariates = self.stack_covariates(
             old_covs=past_covariates, new_covs=sectors_dict
         )
+        # add industry fund covariates
         industry_funds_series = self.prepare_industry_fund_series(
             train_date_start=train_date_start
         )
         industry_funds_dict = {
             t: industry_funds_series for t in stock_price_series.keys()
         }
         past_covariates = self.stack_covariates(
@@ -706,29 +735,248 @@
                 s_ext = TimeSeries.from_dataframe(df, freq="B", fill_missing_dates=True)
                 new_series[t] = s_ext
                 # logger.info(
                 #     f"{t} series after extension start, end: {s_ext.start_time()}, {s_ext.end_time()}"
                 # )
         return new_series
 
+    def prepare_dividends(self, stock_price_series: dict = None):
+
+        def no_dividends_stock(start_date: pd.Timestamp):
+            """Prepare placeholder dataframe for a stock without any historical dividends"""
+            return pd.DataFrame(
+                {
+                    "dividend": [0],
+                    "recordDate": [start_date],
+                    "paymentDate": [start_date],
+                    "declarationDate": [start_date],
+                }
+            )
+
+        logger.info("preparing future covariates: stock dividends")
+        # convert date strings to numerical representation
+        div_df = self.dividends_loaded_df.copy()
+        # logger.debug(f"div_df sample: \n{div_df}")
+        # logger.debug(f"div_df.columns: {div_df.columns}")
+        # remove adjDividend because it cannot be used as a future covariate
+        # remove label because it is simply another string format for Date,
+        # which does not add unique and useful information to the training data
+        div_df.drop(["adjDividend", "label"], axis="columns", inplace=True)
+        # convert date columns from string to pd.Timestamp
+        for c in ["declarationDate", "paymentDate", "recordDate"]:
+            div_df[c] = pd.to_datetime(div_df[c])
+        # drop rows with null / unknown declarationDate, paymentDate or dividend
+        div_df.dropna(
+            subset=["declarationDate", "paymentDate", "dividend"],
+            how="any",
+            inplace=True,
+        )
+        t_series = {}
+        for t, prices in stock_price_series.items():
+            try:
+                # logger.debug(f"ticker: {t}")
+                try:
+                    t_div = div_df.loc[[t]]
+                except KeyError as e:
+                    # no dividends information available for ticker
+                    # assume stock has never issued dividends
+                    t_div = no_dividends_stock(start_date=prices.start_time())
+                # logger.debug(f"t_div sample for {t}: \n{t_div}")
+                # replace ["Symbol", "Date"] index with declarationDate
+                # simultaneously drop previous ["Symbol", "Date"] multiindex columns
+                t_div = t_div.set_index("declarationDate", drop=True)
+                # logger.debug(f"t_div.columns: {t_div.columns}")
+                # logger.debug(f"t_div sample for {t}: \n{t_div}")
+                t_div.index.name = "Date"
+                # logger.debug(f"t_div sample for {t}: \n{t_div}")
+                # logger.debug(
+                # f"t_div  {t} samples with null index: \n{t_div[t_div.index.isnull()]}"
+                # )
+                assert not t_div.index.isnull().any()
+                date_col_names = ["paymentDate", "recordDate"]
+                for date_col_name in date_col_names:
+                    date_col = t_div[date_col_name]
+                    # date_col = pd.to_datetime(t_div[date_col_name])
+                    date_col_year = date_col.dt.year
+                    date_col_month = date_col.dt.month
+                    date_col_day = date_col.dt.day
+                    div_n_cols = len(t_div.columns)
+                    # add encodings for year, month and day to make it easier for the model to see how far in the future is the next dividends date
+                    # and potentially discover cyclical behavior in stock price movement based on dividends
+                    t_div.insert(
+                        loc=div_n_cols,
+                        column=f"{date_col_name}_day",
+                        value=date_col_day,
+                    )
+                    t_div.insert(
+                        loc=div_n_cols,
+                        column=f"{date_col_name}_month",
+                        value=date_col_month,
+                    )
+                    t_div.insert(
+                        loc=div_n_cols,
+                        column=f"{date_col_name}_year",
+                        value=date_col_year,
+                    )
+                t_div.drop(date_col_names, axis="columns", inplace=True)
+                # logger.debug(f"t_div sample for {t}: \n{t_div}")
+                # logger.debug(f"t_div.index for {t}: \n{t_div.index}")
+                # align declaration dates to the closest business days used in the target timeseries index
+                t_div = self.df_index_to_biz_days(t_div)
+                # drop rows with duplicate datetime index values
+                t_div = t_div[~t_div.index.duplicated(keep="last")]
+                assert (
+                    t_div.index.is_unique
+                ), f"Duplicate index keys found for {t}: {t_div[t_div.index.duplicated()]}"
+                # make sure we don't leak forward dividend declarations
+                # that are not known at prediction time
+                t_div.drop(
+                    index=t_div[t_div.index > prices.end_time()].index, inplace=True
+                )
+                assert not t_div.empty
+                assert (
+                    t_div.index.max() <= prices.end_time()
+                ), f"""Dividend declarations which are not know at prediction time must not leak into future covariates: 
+                    {t} dividends end time {t_div.index.max()} > price target end time {prices.end_time()}"""
+                # logger.debug(f"t_div sample for {t}: \n{t_div}")
+                tmp = TimeSeries.from_dataframe(
+                    t_div, freq="B", fill_missing_dates=True
+                )
+                # logger.debug(
+                #     f"tmp series start time, end time: {tmp.start_time()}, {tmp.end_time()}"
+                # )
+                t_div = tmp.pd_dataframe()
+                t_div.ffill(inplace=True)
+                # Fill empty cells with 0 to indicate to the model unknown dividend
+                ts = TimeSeries.from_dataframe(t_div, freq="B", fillna_value=0)
+                ts_padded = self.pad_covs(
+                    cov_series=ts, price_series=prices, fillna_value=0
+                )
+                assert (
+                    len(ts_padded.gaps()) == 0
+                ), f"Found unexpected gaps in series: \n{ts_padded.gaps()}"
+                # logger.debug(f"ts_padded sample for {t}: \n{ts_padded.pd_dataframe()}")
+                # logger.debug(
+                #     f"ts_padded series start time, end time: {ts_padded.start_time()}, {ts_padded.end_time()}"
+                # )
+                t_series[t] = ts_padded
+            except (KeyError, ValueError, AssertionError) as e:
+                logger.exception(f"Skipping {t} due to error: {type(e)}: {e}")
+
+        # if len(t_series.keys()) > 0:
+        #     logger.debug(f"t_series.columns[{t}]: {t_series[t].columns}")
+        #     logger.debug(f"len(t_series[{t}]): {len(t_series[t])}")
+        #     logger.debug(f"t_series[{t}]: {t_series[t]}")
+        #     logger.debug(
+        #         f"t_series[{t}] start time, end time: {t_series[t].start_time()}, {t_series[t].end_time()}"
+        #     )
+        return t_series
+
+    def prepare_splits(self, stock_price_series: dict = None):
+
+        def no_splits_stock(start_date: pd.Timestamp):
+            """Prepare placeholder dataframe for a stock without any historical splits"""
+            df = pd.DataFrame(
+                {
+                    "Symbol": ["any"],
+                    "Date": [start_date],
+                    "numerator": [1],
+                    "denominator": [1],
+                }
+            )
+            df = df.set_index(keys=["Symbol", "Date"], drop=True)
+            # logger.debug(f"df: \n{df}")
+            return df
+
+        logger.info("preparing past covariates: stock splits")
+        # convert date strings to numerical representation
+        splits_df = self.splits_loaded_df.copy()
+        # logger.debug(f"self.splits_loaded_df.columns: {self.splits_loaded_df.columns}")
+        # remove label because it is simply another string format for Date,
+        # which does not add unique and useful information to the training data
+        splits_df = splits_df.drop(["label"], axis="columns")
+        # logger.debug(f"splits_df.columns {splits_df.columns}")
+        # logger.debug(f"splits_df sample: \n{splits_df}")
+        t_series = {}
+        for t, prices in stock_price_series.items():
+            try:
+                # logger.debug(f"ticker: {t}")
+                try:
+                    t_splits = splits_df.loc[[t]]
+                except KeyError as e:
+                    # no dividends information available for ticker
+                    # assume stock has never issued dividends
+                    t_splits = no_splits_stock(start_date=prices.start_time())
+
+                # logger.debug(f"t_splits sample: \n{t_splits}")
+                t_splits = t_splits.droplevel("Symbol")
+                # t_splits.index = pd.to_datetime(t_splits.index)
+                # logger.debug(f"index type for {t}: {type(t_splits.index)}")
+                assert t_splits.index.is_unique
+                assert not t_splits.index.isnull().any()
+                # align declaration dates to the closest business days used in the target timeseries index
+                t_div = self.df_index_to_biz_days(t_splits)
+                # drop rows with duplicate datetime index values
+                t_splits = t_splits[~t_splits.index.duplicated(keep="last")]
+                # logger.debug(f"t_splits sample for {t}: {t_splits}")
+                tmp = TimeSeries.from_dataframe(
+                    t_splits, freq="B", fill_missing_dates=True
+                )
+                # logger.debug(
+                #     f"tmp series start time, end time: {tmp.start_time()}, {tmp.end_time()}"
+                # )
+                t_splits = tmp.pd_dataframe()
+                # Do not interpolate splits forward, because
+                # the Date index is the date when the split occurs
+                # the model should not be confused as to when exactly
+                # a stock split takes place
+                # --> NO: t_splits.ffill(inplace=True)
+                # fill in empty numerator and denominator values with 1s,
+                # which is equivalent to no stock splits occuring on a given date
+                ts = TimeSeries.from_dataframe(t_div, freq="B", fillna_value=1)
+                ts_padded = self.pad_covs(
+                    cov_series=ts, price_series=prices, fillna_value=1
+                )
+                assert (
+                    len(ts_padded.gaps()) == 0
+                ), f"found gaps in series: \n{ts_padded.gaps()}"
+                # logger.debug(f"ts_padded sample for {t}: {ts_padded.pd_dataframe()}")
+                t_series[t] = ts_padded
+            except (KeyError, ValueError, AssertionError) as e:
+                logger.exception(f"Skipping {t} due to error: {type(e)}: {e}")
+
+        return t_series
+
     def prepare_future_covariates(
-        self, stock_price_series: {} = None, min_samples=None, pred_horizon: int = None
+        self,
+        stock_price_series: dict = None,
+        min_samples=None,
+        pred_horizon: int = None,
     ):
         logger.info("Preparing future covariates")
         # add analyst estimates
         quarter_est_series, annual_est_series = self.prepare_analyst_estimates(
             stock_price_series=stock_price_series
         )
         ## Stack analyst estimates to future covariates
-        stacked_future_covariates = self.stack_covariates(
+        future_covariates = self.stack_covariates(
             old_covs=quarter_est_series,
             new_covs=annual_est_series,
             min_samples=min_samples,
         )
-        future_covariates = stacked_future_covariates
-
+        # add stock dividends covariates
+        # for some stocks there will be dividends declared prior to the forecast date
+        # with known payment dates scheduled into the future
+        dividend_series = self.prepare_dividends(stock_price_series=stock_price_series)
+        future_covariates = self.stack_covariates(
+            old_covs=future_covariates,
+            new_covs=dividend_series,
+            min_samples=min_samples,
+        )
+        # extend covars into forecast horizon future dates
         future_covariates = self.__extend_series(
             n=pred_horizon, series=future_covariates, target=stock_price_series
         )
-
+        # add holidays
         future_covariates = self.__add_holidays(future_covariates)
+        # update covs object state
         self.future_covariates = future_covariates
```

### Comparing `canswim-0.0.8/src/canswim/dashboard/__init__.py` & `canswim-0.0.9/src/canswim/dashboard/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,24 +66,33 @@
             AS SELECT date, symbol, forecast_start_year, forecast_start_month, forecast_start_day, COLUMNS(\"close_quantile_\d+\.\d+\") 
             FROM read_parquet('{self.forecast_path}/**/*.parquet', hive_partitioning = 1) as f
             SEMI JOIN stock_tickers
             ON f.symbol = stock_tickers.symbol;
             """
         )
         duckdb.sql(
-            f"""
-            CREATE VIEW close_price 
-            AS SELECT Date, Symbol, Close 
+            f"""--sql
+            CREATE TABLE latest_forecast AS
+                SELECT symbol, max(make_date(forecast_start_year, forecast_start_month, forecast_start_day)) as date
+                FROM forecast
+                GROUP BY symbol
+                ;
+            """
+        )
+        duckdb.sql(
+            f"""--sql
+            CREATE VIEW close_price
+            AS SELECT Date, Symbol, "{self.canswim_model.target_column}" as Close
             FROM read_parquet('{self.stocks_price_path}') as cp
             SEMI JOIN stock_tickers
             ON cp.symbol = stock_tickers.symbol;
             """
         )
         duckdb.sql(
-            f"""
+            f"""--sql
             CREATE VIEW backtest_error 
             AS SELECT f.symbol, mean(abs(log(greatest(f."close_quantile_0.5", 0.01)/cp.Close))) as mal_error
             FROM forecast as f, close_price as cp
             WHERE cp.symbol = f.symbol AND cp.date = f.date
             GROUP BY f.symbol, cp.symbol
             HAVING cp.symbol = f.symbol
             """
```

### Comparing `canswim-0.0.8/src/canswim/dashboard/advanced.py` & `canswim-0.0.9/src/canswim/dashboard/advanced.py`

 * *Files 12% similar despite different names*

```diff
@@ -61,11 +61,14 @@
             outputs=[self.queryResult],
         )
 
     def scan_forecasts(self, query):
         try:
             # only run select queries
             if query.strip().upper().startswith("SELECT"):
-                return duckdb.sql(query).df()
+                sql_result = duckdb.sql(query)
+                logger.debug(f"SQL Result: \n{sql_result}")
+                df = sql_result.df()
+                return df
         except Exception as e:
             gr.Error("An error occurred while running the query:", e)
             return None
```

### Comparing `canswim-0.0.8/src/canswim/dashboard/charts.py` & `canswim-0.0.9/src/canswim/dashboard/charts.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,33 +84,37 @@
     def get_rr(self, ticker=None, lowq_min=None):
         assert ticker is not None
         assert lowq_min is not None and lowq_min >= 0
         # logger.debug(f"lowq_min: {lowq_min}")
         mean_col = "close_quantile_0.5"
         rr = 1.01  # minimum reward/risk ratio
         reward = 1  # minimum reward percent
-        df = duckdb.sql(
+        sql_result = duckdb.sql(
             f"""--sql
             SELECT 
                 f.symbol, 
                 min(f.date) as forecast_start_date, 
                 arg_max(c.close, c.date) as prior_close_price, 
                 {lowq_min} as forecast_close_low, 
                 max("{mean_col}") as forecast_close_high, 
                 100*(forecast_close_high / prior_close_price - 1) as reward_percent, 
                 (forecast_close_high - prior_close_price)/GREATEST(prior_close_price-forecast_close_low, 0.01) as reward_risk,
                 max(e.mal_error) as backtest_error,
                 max(c.date) as prior_close_date, 
-            FROM forecast f, close_price c, backtest_error as e
-            WHERE f.symbol = '{ticker}' AND f.symbol = c.symbol AND f.symbol = e.symbol
-            GROUP BY f.symbol, f.forecast_start_year, f.forecast_start_month, f.forecast_start_day, c.symbol, e.symbol
-            HAVING prior_close_date < forecast_start_date AND forecast_close_high > prior_close_price 
-            AND reward_risk> {rr} AND reward_percent >= {reward}                
+            FROM forecast f, close_price c, backtest_error as e, latest_forecast as lf
+            WHERE f.symbol = '{ticker}' AND f.symbol = lf.symbol AND 
+                f.symbol = c.symbol AND f.symbol = e.symbol AND c.date < lf.date
+            GROUP BY f.symbol, f.forecast_start_year, f.forecast_start_month, f.forecast_start_day, c.symbol, e.symbol, lf.symbol, lf.date
+            HAVING forecast_close_high > prior_close_price AND
+                make_date(f.forecast_start_year, f.forecast_start_month, f.forecast_start_day) = lf.date AND
+                reward_risk> {rr} AND reward_percent >= {reward}                
             """
-        ).df()
+        )
+        logger.debug(f"sqlresult: \n{sql_result}")
+        df = sql_result.df()
         logger.info(f"rr table df: {df}")
         dateformat = lambda d: d.strftime("%d %b, %Y")
         df_styler = df.style.format(
             {"prior_close_date": dateformat, "forecast_start_date": dateformat},
             precision=2,
             thousands=",",
             decimal=".",
@@ -223,15 +227,15 @@
                     label_to_use = "Value"
                 else:
                     label_to_use = label
             kwargs["label"] = label_to_use
 
             if len(central_series) > 1:
                 p = ax.plot(
-                    df.index.values, central_series.values, "-", *args, **kwargs
+                    df.index.values, central_series.values, "--", *args, **kwargs
                 )
             # empty TimeSeries
             elif len(central_series) == 0:
                 p = ax.plot(
                     [],
                     [],
                     *args,
@@ -340,14 +344,15 @@
         )
         logger.info(f"df columns count: {len(df.columns)}")
         logger.info(f"df row count: {len(df)}")
         logger.info(f"df columns: {df.columns}")
         logger.info(f"df column types: \n{df.dtypes}")
         # logger.debug(f"df row sample: {df}")
         df = df.drop(columns=["symbol"])
+        df.sort_index(ascending=True, inplace=True)
         df_list = []
         for y in df["forecast_start_year"].unique():
             for m in df.loc[df["forecast_start_year"] == y][
                 "forecast_start_month"
             ].unique():
                 for d in df.loc[
                     (df["forecast_start_year"] == y) & (df["forecast_start_month"] == m)
@@ -361,10 +366,12 @@
                         columns=[
                             "forecast_start_year",
                             "forecast_start_month",
                             "forecast_start_day",
                         ]
                     )
                     if not single_forecast.empty:
-                        single_forecast = single_forecast.sort_index()
                         df_list.append(single_forecast)
+                        logger.info(
+                            f"Loaded forecast series with start date: {y}/{m}/{d}"
+                        )
         return df_list
```

### Comparing `canswim-0.0.8/src/canswim/dashboard/scans.py` & `canswim-0.0.9/src/canswim/dashboard/scans.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,33 +41,37 @@
             outputs=[self.scanResult],
         )
 
     def scan_forecasts(self, lowq, reward, rr):
         lq = (100 - lowq) / 100
         low_quantile_col = f"close_quantile_{lq}"
         mean_col = "close_quantile_0.5"
-        df = duckdb.sql(
+        sql_result = duckdb.sql(
             f"""--sql
             SELECT 
                 f.symbol, 
                 min(f.date) as forecast_start_date, 
                 arg_max(c.close, c.date) as prior_close_price, 
                 min("{low_quantile_col}") as forecast_close_low, 
                 max("{mean_col}") as forecast_close_high, 
                 100*(forecast_close_high / prior_close_price - 1) as reward_percent, 
                 (forecast_close_high - prior_close_price)/GREATEST(prior_close_price-forecast_close_low, 0.01) as reward_risk,
                 max(e.mal_error) as backtest_error,
                 max(c.date) as prior_close_date, 
-            FROM forecast f, close_price c, backtest_error as e
-            WHERE f.symbol = c.symbol and f.symbol = e.symbol
-            GROUP BY f.symbol, f.forecast_start_year, f.forecast_start_month, f.forecast_start_day, c.symbol, e.symbol
-            HAVING prior_close_date < forecast_start_date AND forecast_close_high > prior_close_price 
-                AND reward_risk> {rr} AND reward_percent >= {reward}
+            FROM forecast f, close_price c, backtest_error as e, latest_forecast as lf
+            WHERE f.symbol = lf.symbol AND 
+                f.symbol = c.symbol AND f.symbol = e.symbol AND c.date < lf.date
+            GROUP BY f.symbol, f.forecast_start_year, f.forecast_start_month, f.forecast_start_day, c.symbol, e.symbol, lf.symbol, lf.date
+            HAVING forecast_close_high > prior_close_price AND
+                make_date(f.forecast_start_year, f.forecast_start_month, f.forecast_start_day) = lf.date AND
+                reward_risk> {rr} AND reward_percent >= {reward}                
             """
-        ).df()
+        )
+        logger.debug(f"SQL Result: \n{sql_result}")
+        df = sql_result.df()
         dateformat = lambda d: d.strftime("%d %b, %Y")
         df_styler = df.style.format(
             {"prior_close_date": dateformat, "forecast_start_date": dateformat},
             precision=2,
             thousands=",",
             decimal=".",
         )
```

### Comparing `canswim-0.0.8/src/canswim/gather_data.py` & `canswim-0.0.9/src/canswim/gather_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -91,22 +91,25 @@
         self.price_frequency = "1d"  # "1wk"
         self.min_start_date = os.getenv("train_date_start", "1991-01-01")
 
     def gather_stock_tickers(self):
         # Prepare list of stocks for training
         all_stock_set = set()
         stock_files = [
+            # "test_stocks.csv"
             "IBD50.csv",
             "IBD250.csv",
             "ibdlive_picks.csv",
             "russell2000_iwm_holdings.csv",
             "sp500_ivv_holdings.csv",
             "nasdaq100_cndx_holdings.csv",
             "watchlist.csv",
             "vti_total_market_stocks.csv",
+            "ITB_holdings.csv",
+            "IYM_holdings.csv",
             self.all_stocks_file,
         ]
         logger.info(
             "Compiling list of stocks to train on from: {files}", files=stock_files
         )
         for f in stock_files:
             fp = f"data/data-3rd-party/{f}"
@@ -122,51 +125,22 @@
 
         logger.info(f"Total size of stock set: {len(all_stock_set)}")
         # logger.info(f"All stocks set: {all_stock_set}")
         # Drop invalid symbols with more than 10 ticker characters.
         # Almost all stocks have less than 5 characters.
         slist = [x for x in set(all_stock_set) if len(x) < 10]
         self.stocks_ticker_set = set(slist)
-        # drop known junk symbols from the data feed
-        junk_tickers = set(
-            [
-                "MSFUT",
-                "GEFB",
-                "METCV",
-                "SGAFT",
-                "NQH4",
-                "XTSLA",
-                "-",
-                "PDLI",
-                "ADRO",
-                "ICSUAGD",
-                "BFB",
-                "GTXI",
-                "P5N994",
-                "LGFB",
-                "MLIFT",
-                "ESH4",
-                "LGFA",
-                "MOGA",
-                "PBRA",
-                "BRKB",
-                "RTYH4",
-                "\xa0",
-                "CRDA",
-                "GBP",
-                "ESMT",
-                "MRTX",
-                "RAIN",
-                "CAD",
-                "EUR",
-            ]
+        # drop symbols which yfinance does not like
+        junk_tickers = pd.read_csv(
+            f"{self.data_dir}/{self.data_3rd_party}/junk_tickers.csv"
         )
-        self.stocks_ticker_set = self.stocks_ticker_set - junk_tickers
+        junk_tickers = set(junk_tickers["Symbol"])
+        self.stocks_ticker_set = sorted(list(self.stocks_ticker_set - junk_tickers))
         stocks_df = pd.DataFrame()
-        stocks_df["Symbol"] = list(self.stocks_ticker_set)
+        stocks_df["Symbol"] = self.stocks_ticker_set
         stocks_df = stocks_df.set_index(["Symbol"])
         stocks_df.index = stocks_df.index.drop_duplicates()
         stocks_df
         stocks_file = f"data/data-3rd-party/{self.all_stocks_file}"
         stocks_df.to_csv(stocks_file)
         logger.info(f"Saved stock set to {stocks_file}")
 
@@ -193,17 +167,29 @@
 
     def _gather_yfdata_date_index(self, data_file: str = None, tickers: str = None):
         start_date = self.min_start_date
         old_df = None
         try:
             old_df = pd.read_parquet(data_file)
             logger.info("Loaded saved data. Sample: \n{df}", df=old_df)
-            start_date = get_latest_date(old_df.index) - pd.Timedelta(1, "d")
-            logger.info(f"Columns: \n{old_df.columns}")
-            logger.info(f"Latest saved record is after {start_date}")
+            # check if all symbols are represented in the loaded data
+            # if not, then download all historical data from scratch
+            # otherwise, only fetch new data after latest saved date
+            new_tickers = set(tickers) - set(old_df.columns.levels[0])
+            if not new_tickers:
+                start_date = get_latest_date(old_df.index) - pd.Timedelta(1, "d")
+                logger.info(f"Columns: \n{old_df.columns}")
+                logger.info(f"Latest saved record is after {start_date}")
+            else:
+                logger.info(
+                    f"Not all tickers found in saved data. Missing: {new_tickers}"
+                )
+                logger.info(
+                    f"\nTicker set: {tickers}, \nTickers with saved data: {set(old_df.columns.levels[0])}"
+                )
         except Exception as e:
             logger.warning(f"Could not load data from file: {data_file}. Error: {e}")
         new_df = yf.download(tickers, start=start_date, group_by="tickers", period="1d")
         new_df = new_df.dropna(how="all")
         logger.info("New data gathered. Sample: \n{bm}", bm=new_df)
         logger.info(f"Columns: \n{new_df.columns}")
         if old_df is not None:
@@ -216,33 +202,42 @@
         else:
             merged_df = new_df
         logger.info("Updated data ready. Sample: \n{bm}", bm=merged_df)
         assert merged_df.index.is_unique
         merged_df.to_parquet(data_file)
         logger.info(f"Saved data to {data_file}")
         _bm = pd.read_parquet(data_file)
-        assert sorted(_bm.columns) == sorted(merged_df.columns)
-        assert len(_bm) == len(merged_df)
+        pd.testing.assert_frame_equal(_bm, merged_df)
         logger.info(f"Sanity check passed for saved data. Loaded OK from {data_file}")
 
     def gather_broad_market_data(self):
         ## Prepare data for broad market indicies
         # Capture S&P500, NASDAQ100 and Russell 200 indexes and their equal weighted counter parts
         # As well as VIX volatility index, DYX US Dollar index, TNX US 12 Weeks Treasury Yield, 5 Years Treasury Yield and 10 Year Treasuries Yield
-        broad_market_indicies = (
-            "^SPX ^SPXEW ^NDX ^NDXE ^RUT ^R2ESC ^VIX DX-Y.NYB ^IRX ^FVX ^TNX"
-        )
+        broad_market_indicies = [
+            "^SPX",
+            "^SPXEW",
+            "^NDX",
+            "^NDXE",
+            "^RUT",
+            "^R2ESC",
+            "^VIX",
+            "DX-Y.NYB",
+            "^IRX",
+            "^FVX",
+            "^TNX",
+        ]
         data_file = "data/data-3rd-party/broad_market.parquet"
         self._gather_yfdata_date_index(
             data_file=data_file, tickers=broad_market_indicies
         )
 
     def gather_sectors_data(self):
         """Gather historic price and volume data for key market sectors"""
-        sector_indicies = "XLE ^SP500-15 ^SP500-20 ^SP500-25 ^SP500-30 ^SP500-35 ^SP500-40 ^SP500-45 ^SP500-50 ^SP500-55 ^SP500-60"
+        sector_indicies = "XLE ^SP500-15 ^SP500-20 ^SP500-25 ^SP500-30 ^SP500-35 ^SP500-40 ^SP500-45 ^SP500-50 ^SP500-55 ^SP500-60".split()
         data_file = "data/data-3rd-party/sectors.parquet"
         self._gather_yfdata_date_index(data_file=data_file, tickers=sector_indicies)
 
     def gather_industry_fund_data(self):
         """
         Gather historic price and volume data for key industry ETFs.
         The goal of these covariates is to provide the model with a more granural breakdown of stock grouping by industry.
@@ -257,21 +252,35 @@
             f"data/data-3rd-party/all_stocks_price_hist_{self.price_frequency}.parquet"
         )
         start_date = self.min_start_date
         old_df = None
         try:
             old_df = pd.read_parquet(data_file)
             logger.info("Loaded saved data. Sample: \n{df}", df=old_df)
-            start_date = get_latest_date(
-                old_df.index.get_level_values("Date")
-            ) - pd.Timedelta(1, "d")
-            logger.info(f"Columns: \n{old_df.columns}")
-            logger.info(f"Latest saved record is after {start_date}")
+            # check if all symbols are represented in the loaded data
+            # if not, then download all historical data from scratch
+            # otherwise, only fetch new data after latest saved date
+            all_tickers = set(self.stocks_ticker_set)
+            old_tickers = set(old_df.index.get_level_values("Symbol"))
+            new_tickers = all_tickers - old_tickers
+            if not new_tickers:
+                start_date = get_latest_date(
+                    old_df.index.get_level_values("Date")
+                ) - pd.Timedelta(1, "d")
+                logger.info(f"Columns: \n{old_df.columns}")
+                logger.info(f"Latest saved record is after {start_date}")
+            else:
+                logger.info(
+                    f"Not all tickers found in saved data. Missing: {new_tickers}"
+                )
+                logger.info(
+                    f"\nTicker set: {all_tickers}, \nTickers with saved data: {old_tickers}"
+                )
         except Exception as e:
-            logger.exception(f"Could not load data from file: {data_file}. Error: {e}")
+            logger.warning(f"Could not load data from file: {data_file}. Error: {e}")
         new_df = yf.download(
             self.stocks_ticker_set, start=start_date, group_by="tickers"
         )
         new_df = new_df.dropna(how="all")
         new_df = new_df.stack(level=0)
         new_df.index.names = ["Date", "Symbol"]
         new_df.index = new_df.index.swaplevel(0)
@@ -287,42 +296,46 @@
             merged_df = merged_df[~merged_df.index.duplicated(keep="last")]
         else:
             merged_df = new_df
         logger.info("Updated data ready. Sample: \n{df}", df=merged_df)
         # df=merged_df.loc[merged_df.index.get_level_values("Symbol") == 'TEAM'])
         assert merged_df.index.is_unique
         merged_df.to_parquet(data_file)
-        logger.info(f"Saved broad market data to {data_file}")
+        logger.info(f"Saved data to {data_file}")
+        logger.info(f"Verifing saved data...")
         _bm = pd.read_parquet(data_file)
-        assert sorted(_bm.columns) == sorted(merged_df.columns)
-        assert len(_bm) == len(merged_df)
-        logger.info(
-            f"Sanity check passed for broad market data. Loaded OK from {data_file}"
-        )
+        pd.testing.assert_frame_equal(_bm, merged_df)
+        logger.info(f"Sanity check passed. Loaded OK from {data_file}")
 
     def gather_earnings_data(self):
-        logger.info("Gathering  earnings and sales data...")
-        earnings_all_df = (
-            None  # pd.DataFrame() -- Pandas prefers None to empty df in concat
-        )
+        logger.info("Gathering earnings and sales data...")
+        earnings_all_df = None  # Pandas prefers None to empty df in concat
         for ticker in self.stocks_ticker_set:  # ['AAON']: #
             earnings = fmpsdk.historical_earning_calendar(
                 apikey=self.FMP_API_KEY, symbol=ticker, limit=-1
             )
             if earnings is not None and len(earnings) > 0:
-                edf = pd.DataFrame(earnings)
-                edf = edf.dropna(how="all")
-                edf["date"] = pd.to_datetime(edf["date"])
-                edf = edf.set_index(["symbol", "date"])
-                # edf = edf.pivot(columns='symbol')
-                # edf.swaplevel(i=0,j=1, axis=0)
-                # edf.drop(columns=['symbol'])
-                earnings_all_df = pd.concat([earnings_all_df, edf])
-                # n_earnings = len(earnings)
-                # logger.info(f"Total earnings reports for {ticker}: {n_earnings}")
+                try:
+                    edf = pd.DataFrame(earnings)
+                    edf = edf.dropna(how="all")
+                    edf = edf.fillna(-1)
+                    if not edf.empty:
+                        edf["date"] = pd.to_datetime(edf["date"])
+                        edf = edf.set_index(["symbol", "date"])
+                        earnings_all_df = pd.concat([earnings_all_df, edf])
+                        logger.info(f"Total earnings reports for {ticker}: {len(edf)}")
+                    else:
+                        logger.warning(f"Skipping {ticker} due to lack of data")
+                except ValueError as e:
+                    logger.warning(
+                        f"Skipping {ticker} due to error: {type(e)}, {e}, \n{earnings} "
+                    )
+            else:
+                logger.warning(f"Skipping {ticker} due to lack of data")
+
         #    earliest_earn = earnings[-1] if len(earnings > 0 else 'None')
         #    logger.info(f"Earliest earnings report for {ticker}: {earliest_earn}")
 
         logger.info(f"Earnings sample report for {ticker}: \n{earnings}")
         earnings_all_df.index.names = ["Symbol", "Date"]
         earnings_all_df = earnings_all_df.sort_index()
         logger.info(
@@ -333,66 +346,148 @@
             f"len(earnings_all_df.index.levels[0]): \n{len(earnings_all_df.index.levels[0])}"
         )
         earnings_file = "data/data-3rd-party/earnings_calendar.parquet"
         earnings_all_df.to_parquet(earnings_file)
         ### Read back data and verify it
         tmp_earn_df = pd.read_parquet(earnings_file)
         logger.info(f"tmp_earn_df: \n{tmp_earn_df}")
-        assert tmp_earn_df.index.names == ["Symbol", "Date"]
-        assert len(tmp_earn_df) == len(earnings_all_df)
-        assert sorted(tmp_earn_df.columns) == sorted(earnings_all_df.columns)
+        pd.testing.assert_frame_equal(tmp_earn_df, earnings_all_df)
         logger.info(
             f"Sanity check passed for earnings data. Loaded OK from file: {earnings_file}"
         )
 
     def gather_stock_key_metrics(self):
         logger.info("Gathering key metrics data with company fundamentals...")
-        keymetrics_all_df = pd.DataFrame()
+        keymetrics_all_df = None
         for ticker in self.stocks_ticker_set:
             kms = fmpsdk.key_metrics(
                 apikey=self.FMP_API_KEY, symbol=ticker, period="quarter", limit=-1
             )
             if kms is not None and len(kms) > 0:
-                kms_df = pd.DataFrame(kms)
-                kms_df["date"] = pd.to_datetime(kms_df["date"])
-                kms_df = kms_df.set_index(["symbol", "date"])
-                # logger.info(f"Key metrics for {ticker} sample: \n{kms_df.columns}")
-                keymetrics_all_df = pd.concat([keymetrics_all_df, kms_df])
-                # logger.info(f"Key metrics concatenated {ticker}: \n{keymetrics_all_df.columns}")
-                n_kms = len(kms_df)
-                logger.info(f"Total key metrics reports for {ticker}: {n_kms}")
+                try:
+                    kms_df = pd.DataFrame(kms)
+                    kms_df = kms_df.dropna(how="all")
+                    kms_df = kms_df.fillna(-1)
+                    if not kms_df.empty:
+                        kms_df["date"] = pd.to_datetime(kms_df["date"])
+                        kms_df = kms_df.set_index(["symbol", "date"])
+                        # logger.info(f"Key metrics for {ticker} sample: \n{kms_df.columns}")
+                        keymetrics_all_df = pd.concat([keymetrics_all_df, kms_df])
+                        # logger.info(f"Key metrics concatenated {ticker}: \n{keymetrics_all_df.columns}")
+                        n_kms = len(kms_df)
+                        logger.info(f"Total key metrics reports for {ticker}: {n_kms}")
+                    else:
+                        logger.warning(f"Skipping {ticker} due to lack of data")
+                except ValueError as e:
+                    logger.warning(
+                        f"Skipping {ticker} due to error: {type(e)}, {e}, \n{kms} "
+                    )
             else:
                 logger.info(f"No {ticker} key metrics reports: kms={kms}")
 
-        logger.info(f"keymetrics_all_df: \n{keymetrics_all_df}")
-        logger.info(f"keymetrics_all_df.dtypes: \n{keymetrics_all_df.dtypes}")
-        logger.info(f"len(keymetrics_all_df): \n{len(keymetrics_all_df)}")
-        # index, row = next(keymetrics_all_df.iterrows())
-        # row["averagePayables"]
-        # prevent parquet serialization issues
-        keymetrics_all_df["averagePayables"] = pd.to_numeric(
-            keymetrics_all_df["averagePayables"], dtype_backend="pyarrow"
+        logger.debug(f"keymetrics_all_df: \n{keymetrics_all_df}")
+        logger.debug(f"keymetrics_all_df.dtypes: \n{keymetrics_all_df.dtypes}")
+        logger.debug(f"len(keymetrics_all_df): \n{len(keymetrics_all_df)}")
+        # cleanup data types to prevent parquet serialization issues
+        kms_num_cols = list(set(keymetrics_all_df.columns) - {"calendarYear", "period"})
+        keymetrics_all_df[kms_num_cols] = keymetrics_all_df[kms_num_cols].apply(
+            pd.to_numeric, dtype_backend="pyarrow"
         )
         keymetrics_all_df.index.names = ["Symbol", "Date"]
         keymetrics_all_df = keymetrics_all_df.sort_index()
+        logger.debug(
+            f"keymetrics_all_df.dtypes after cleanup: \n{keymetrics_all_df.dtypes}"
+        )
         kms_file = "data/data-3rd-party/keymetrics_history.parquet"
         keymetrics_all_df.to_parquet(kms_file, engine="pyarrow")
         ### Read back data and verify it
         temp_kms_df = pd.read_parquet(kms_file)
         logger.info(f"temp_kms_df: \n{temp_kms_df}")
-        assert temp_kms_df.index.names == ["Symbol", "Date"]
-        assert len(temp_kms_df) == len(keymetrics_all_df)
-        assert sorted(temp_kms_df.columns) == sorted(keymetrics_all_df.columns)
+        pd.testing.assert_frame_equal(temp_kms_df, keymetrics_all_df)
         logger.info(
             f"Sanity check passed for key metrics data. Loaded OK from file: {kms_file}"
         )
 
+    def gather_stock_dividends(self):
+        logger.info("Gathering stock dividends data...")
+        all_df = None
+        for ticker in self.stocks_ticker_set:
+            logger.info(f"Gathering report for {ticker}")
+            raw = fmpsdk.historical_stock_dividend(
+                apikey=self.FMP_API_KEY, symbol=ticker
+            )
+            # skip symbols without any data
+            if raw is not None:
+                raw = raw.get("historical")
+            if raw is not None and len(raw) > 0:
+                # logger.info(f"Sample raw report for {ticker}: \n{raw}")
+                df = pd.DataFrame(raw)
+                # logger.debug(f"df for {ticker}: \n{df}")
+                df = df.dropna(how="all")
+                df["date"] = pd.to_datetime(df["date"])
+                df["symbol"] = ticker
+                df = df.set_index(["symbol", "date"])
+                all_df = pd.concat([all_df, df])
+                logger.debug(f"Total reports for {ticker}: {len(df)}")
+
+        if all_df is not None:
+            logger.debug(f"Sample report for {ticker}: \n{df}")
+            all_df.index.names = ["Symbol", "Date"]
+            all_df = all_df.sort_index()
+            logger.info(f"Total number of records for all stocks: \n{len(all_df)}")
+            logger.debug(f"all_df: \n{all_df}")
+            logger.info(f"len(all_df.index.levels[0]): \n{len(all_df.index.levels[0])}")
+            file = f"{self.data_dir}/{self.data_3rd_party}/stock_dividends.parquet"
+            all_df.to_parquet(file)
+            ### Read back data and verify it
+            tmp_df = pd.read_parquet(file)
+            logger.debug(f"tmp_df: \n{tmp_df}")
+            pd.testing.assert_frame_equal(tmp_df, all_df)
+            logger.info(f"Sanity check passed. Data loaded OK from file: {file}")
+        logger.info("Finished gathering stock dividends data.")
+
+    def gather_stock_splits(self):
+        logger.info("Gathering stock splits data...")
+        all_df = None
+        for ticker in self.stocks_ticker_set:
+            logger.info(f"Gathering report for {ticker}")
+            raw = fmpsdk.historical_stock_split(apikey=self.FMP_API_KEY, symbol=ticker)
+            # skip symbols without any data
+            if raw is not None:
+                raw = raw.get("historical")
+            if raw is not None and len(raw) > 0:
+                # logger.debug(f"Sample raw report for {ticker}: \n{raw}")
+                df = pd.DataFrame(raw)
+                # logger.debug(f"df for {ticker}: \n{df}")
+                df = df.dropna(how="all")
+                df["date"] = pd.to_datetime(df["date"])
+                df["symbol"] = ticker
+                df = df.set_index(["symbol", "date"])
+                all_df = pd.concat([all_df, df])
+                logger.debug(f"Total reports for {ticker}: {len(df)}")
+
+        if all_df is not None:
+            logger.debug(f"Sample report for {ticker}: \n{df}")
+            all_df.index.names = ["Symbol", "Date"]
+            all_df = all_df.sort_index()
+            logger.info(f"Total number of records for all stocks: \n{len(all_df)}")
+            logger.debug(f"all_df: \n{all_df}")
+            logger.info(f"len(all_df.index.levels[0]): \n{len(all_df.index.levels[0])}")
+            file = f"{self.data_dir}/{self.data_3rd_party}/stock_splits.parquet"
+            all_df.to_parquet(file)
+            ### Read back data and verify it
+            tmp_df = pd.read_parquet(file)
+            logger.debug(f"tmp_df: \n{tmp_df}")
+            pd.testing.assert_frame_equal(tmp_df, all_df)
+            logger.info(f"Sanity check passed. Data loaded OK from file: {file}")
+        logger.info("Finished gathering stock splits data.")
+
     def gather_institutional_stock_ownership(self):
         logger.info("Gathering institutional ownership data...")
-        inst_ownership_all_df = pd.DataFrame()
+        inst_ownership_all_df = None
         for ticker in self.stocks_ticker_set:
             inst_ownership = institutional_symbol_ownership(
                 apikey=self.FMP_API_KEY,
                 symbol=ticker,
                 limit=-1,
                 includeCurrentQuarter=False,
             )
@@ -464,42 +559,50 @@
             "data/data-3rd-party/institutional_symbol_ownership.parquet"
         )
         inst_own_df.to_parquet(inst_ownership_file, engine="pyarrow")
 
         ### Read back data and verify it
         tmp_int_own_df = pd.read_parquet(inst_ownership_file)
         logger.info(f"tmp_int_own_df: \n{tmp_int_own_df}")
-        assert tmp_int_own_df.index.names == ["Symbol", "Date"]
-        assert len(tmp_int_own_df) == len(inst_own_df)
-        assert sorted(tmp_int_own_df.columns) == sorted(inst_own_df.columns)
+        pd.testing.assert_frame_equal(tmp_int_own_df, inst_own_df)
         logger.info(
             f"Sanity check passed for institutional ownership data. Loaded OK from file: {inst_ownership_file}"
         )
 
     def gather_analyst_estimates(self):
 
         def _fetch_estimates(period=None):
             assert period in ["quarter", "annual"]
-            estimates_all_df = pd.DataFrame()
+            estimates_all_df = None
             for ticker in self.stocks_ticker_set:  # ['ALTR']:
                 est = analyst_estimates(
                     apikey=self.FMP_API_KEY, symbol=ticker, period=period, limit=-1
                 )
-                # logger.info('est:', est)
                 if est is not None and len(est) > 0:
-                    est_df = pd.DataFrame(est)
-                    est_df["date"] = pd.to_datetime(est_df["date"])
-                    est_df = est_df.set_index(["symbol", "date"])
-                    # logger.info(f"Analyst estimates for {ticker} sample: \n{est_df.columns}")
-                    estimates_all_df = pd.concat([estimates_all_df, est_df])
-                    # logger.info(f"Key metrics concatenated {ticker}: \n{estimates_all_df.columns}")
-                    n_est = len(est_df)
-                    logger.info(
-                        f"{n_est} total {ticker} {period} analyst estimates reports"
-                    )
+                    try:
+                        # logger.debug(f"{ticker} estimates: {est}")
+                        est_df = pd.DataFrame(est)
+                        est_df = est_df.dropna(how="all")
+                        est_df = est_df.fillna(-1)
+                        if not est_df.empty:
+                            est_df["date"] = pd.to_datetime(est_df["date"])
+                            est_df = est_df.set_index(["symbol", "date"])
+                            # logger.info(f"Analyst estimates for {ticker} sample: \n{est_df.columns}")
+                            estimates_all_df = pd.concat([estimates_all_df, est_df])
+                            # logger.info(f"Key metrics concatenated {ticker}: \n{estimates_all_df.columns}")
+                            n_est = len(est_df)
+                            logger.info(
+                                f"{n_est} total {ticker} {period} analyst estimates reports"
+                            )
+                        else:
+                            logger.warning(f"Skipping {ticker} due to lack of data")
+                    except ValueError as e:
+                        logger.warning(
+                            f"Skipping {ticker} due to error: {type(e)}, {e}, \n{est} "
+                        )
                 else:
                     logger.info(
                         f"No {ticker} {period} analyst estimates reports: est={est}"
                     )
 
             return estimates_all_df
 
@@ -513,19 +616,15 @@
             # est_file_name= f'data/analyst_estimates_{p}.csv.bz2'
             # estimates_all_df.to_csv(est_file_name)
             estimates_all_df.to_parquet(est_file_name)
             logger.info(f"Saved analyst estimates to: {est_file_name}")
             logger.info(f"all {p} estimates count: {len(estimates_all_df)}")
             # logger.info(f"{p} estimates sample:\n{estimates_all_df}")
             tmp_est_df = pd.read_parquet(est_file_name)
-            assert tmp_est_df.index.names == ["Symbol", "Date"]
-            assert len(tmp_est_df) == len(estimates_all_df)
-            # logger.info(f"tmp_est_df.columns: {tmp_est_df.columns}")
-            # logger.info(f"estimates_all_df.columns: {estimates_all_df.columns}")
-            assert sorted(tmp_est_df.columns) == sorted(estimates_all_df.columns)
+            pd.testing.assert_frame_equal(tmp_est_df, estimates_all_df)
             logger.info(
                 f"Sanity check passed for analyst estimates data. Loaded OK from file: {est_file_name}"
             )
 
 
 # main function
 def main():
@@ -533,14 +632,16 @@
     hfhub.download_data()
     g = MarketDataGatherer()
     g.gather_broad_market_data()
     g.gather_sectors_data()
     g.gather_industry_fund_data()
     g.gather_stock_tickers()
     g.gather_stock_price_data()
+    g.gather_stock_dividends()
+    g.gather_stock_splits()
     g.gather_earnings_data()
     g.gather_stock_key_metrics()
     g.gather_institutional_stock_ownership()
     g.gather_analyst_estimates()
     hfhub.upload_data()
```

### Comparing `canswim-0.0.8/src/canswim/hfhub.py` & `canswim-0.0.9/src/canswim/hfhub.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import os
 import tempfile
 from typing import Optional
 from darts import TimeSeries
 from darts.models.forecasting.forecasting_model import ForecastingModel
 from huggingface_hub import snapshot_download, upload_folder, create_repo
 import torch
-import canswim
+import tarfile
+import os.path
 
 
 class HFHub:
     """
     HuggingFace Hub integration using official HF API.
     https://huggingface.co/docs/huggingface_hub/v0.20.3/en/guides/integrations
     """
@@ -150,54 +151,73 @@
             return
         if local_dir is not None:
             data_dir = local_dir
         else:
             data_dir = self.data_dir
         if repo_id is None:
             repo_id = self.repo_id
+        logger.info(
+            f"Downloading hf data from {repo_id} to data dir:\n",
+            os.listdir(data_dir),
+        )
         snapshot_download(
             repo_id=repo_id,
             repo_type="dataset",
             local_dir=data_dir,
             token=self.HF_TOKEN,
         )
-        logger.info(
-            f"Downloaded hf dataset files from {repo_id} to data dir:\n",
-            os.listdir(data_dir),
-        )
+        # Unpack forecast parquet files from tar
+        forecast_dir = f"{data_dir}/forecast/"
+        forecast_tar = f"{data_dir}/forecast.tar"
+        with tarfile.open(forecast_tar, "r:gz") as tar:
+            logger.info(f"Extracting {forecast_tar} to folder {forecast_dir}")
+            tar.extractall(path=forecast_dir, filter="data")
 
     def upload_data(
         self, repo_id: str = None, private: bool = True, local_dir: str = None
     ):
         if not self.hfhub_sync:
             logger.info("Local mode selected. Skipping upload.")
             return
         if local_dir is not None:
             data_dir = local_dir
         else:
             data_dir = self.data_dir
-        logger.info(f"Uploading data from directory: {data_dir}")
         if repo_id is None:
             repo_id = self.repo_id
+        logger.info(
+            f"Uploading data from local directory: '{data_dir}' to repo id: '{repo_id}'"
+        )
         ## Upload all gathered data from 3rd party sources to hf hub
         # prefix for HF Hub dataset repo
         # Create repo if not existing yet
         repo_info = create_repo(
             repo_id=repo_id,
             repo_type="dataset",
             private=private,
             exist_ok=True,
             token=self.HF_TOKEN,
         )
         logger.info(
             f"repo_info: {repo_info}",
         )
+        # Compress forecast parquet files to pass hfhub limitation of 25k LFS files
+        forecast_dir = f"{data_dir}/forecast/"
+        forecast_tar = f"{data_dir}/forecast.tar"
+        with tarfile.open(forecast_tar, "w:gz") as tar:
+            logger.info(f"Creating {forecast_tar} from folder {forecast_dir}")
+            tar.add(forecast_dir, arcname=os.path.basename(forecast_dir))
+        # upload select files  to hfhub
+        logger.info(f"uploading folder {data_dir}")
         upload_folder(
             repo_id=repo_id,
             # path_in_repo="data-3rd-party",
             repo_type="dataset",
             folder_path=data_dir,
             token=self.HF_TOKEN,
+            # ignore_patterns=[forecast_dir],
+            # allow_patterns="",
+            # delete_patterns=[forecast_dir],
         )
         logger.info(
             "Upload finished.",
         )
```

### Comparing `canswim-0.0.8/src/canswim/model.py` & `canswim-0.0.9/src/canswim/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         self.val_start = {}
         self.test_start = {}
         self.torch_model: TiDEModel = None
         self.model_name = "canswim_model.pt"
         self.n_plot_samples: int = 4
         self.train_date_start: pd.Timestamp = None
         self.targets = Targets()
+        self.target_column = "Close"
         self.covariates = Covariates()
         self.hfhub = HFHub()
         # use GPU if available
         if torch.cuda.is_available():
             logger.info("Configuring CUDA GPU")
             # utilize CUDA tensor cores with bfloat16
             # https://pytorch.org/docs/stable/generated/torch.set_float32_matmul_precision.html#torch.set_float32_matmul_precision
@@ -101,22 +102,27 @@
                 del self.covariates.past_covariates[t]
                 del self.covariates.future_covariates[t]
                 # logger.info(f'preparing train, val split for {t}')
                 logger.info(f"Removing {t} from training loop. Not enough samples")
         self.targets.target_series = target_series_ok
         # drop tickers that do not have full data sets for training targets, past and future covariates
         target_set = set(self.targets.target_series.keys())
+        # logger.debug(f"Tickers with complete target data: {target_set} ")
         future_set = set(self.covariates.future_covariates.keys())
+        # logger.debug(f"Tickers with complete future covs data: {future_set} ")
         past_set = set(self.covariates.past_covariates.keys())
+        # logger.debug(f"Tickers with complete past covs data: {past_set} ")
         tickers_with_complete_data = target_set & future_set & past_set
         tickers_without_complete_data = (
             target_set | future_set | past_set
         ) - tickers_with_complete_data
         logger.info(
-            f"Removing time series for tickers with incomplete data sets: {tickers_without_complete_data}. Keeping {tickers_with_complete_data} "
+            f"""Removing time series for tickers with incomplete data sets: 
+                \n{tickers_without_complete_data}
+                \nKeeping {tickers_with_complete_data}"""
         )
         new_target_series = {}
         new_future_covariates = {}
         new_past_covariates = {}
         for t in tickers_with_complete_data:
             new_target_series[t] = self.targets.target_series[t]
             new_future_covariates[t] = self.covariates.future_covariates[t]
@@ -325,16 +331,14 @@
 
         self.stock_train_list = os.getenv("stock_tickers_list", "all_stocks.csv")
         logger.info("Stocks train list: {stl}", stl=self.stock_train_list)
 
         self.n_stocks = int(
             os.getenv("n_stocks", 50)
         )  # -1 for all, otherwise a number like 300
-        if self.n_stocks == -1:
-            self.n_stocks = len(self.stock_train_list)
         logger.info("n_stocks: {ns}", ns=self.n_stocks)
 
         # model training epochs
         self.n_epochs = int(os.getenv("n_epochs", 5))
         logger.info("n_epochs: {ne}", ne=self.n_epochs)
 
         # patience for number of epochs without validation loss progress
@@ -350,40 +354,46 @@
         # prepare stock price time series
         ## ticker_train_dict = dict((k, self.ticker_dict[k]) for k in self.stock_tickers)
         self.stock_price_series = self.targets.prepare_stock_price_series(
             train_date_start=start_date
         )
         logger.info(f"Prepared {len(self.stock_price_series)} stock price series")
         # prepare target time series
-        target_columns = ["Close"]
         self.targets.prepare_data(
-            stock_price_series=self.stock_price_series, target_columns=target_columns
+            stock_price_series=self.stock_price_series,
+            target_columns=self.target_column,
         )
         logger.info(f"Prepared {len(self.targets.target_series)} stock targets")
         self.covariates.prepare_data(
             stock_price_series=self.stock_price_series,
-            target_columns=target_columns,
+            target_columns=self.target_column,
             train_date_start=start_date,
             min_samples=self.min_samples,
             pred_horizon=self.pred_horizon,
         )
         self.__align_targets_and_covariates()
         logger.info(
             f"Prepared {len(self.targets.target_series)} stock targets after alignment with covariates"
         )
         # prepare forecast lists as expected by the torch predict method
         self.targets_ticker_list = []
         self.targets_list = []
         self.past_cov_list = []
         self.future_cov_list = []
         for t in sorted(self.targets.target_series.keys()):
-            self.targets_ticker_list.append(t)
-            self.targets_list.append(self.targets.target_series[t])
-            self.past_cov_list.append(self.covariates.past_covariates[t])
-            self.future_cov_list.append(self.covariates.future_covariates[t])
+            n_target_samples = len(self.targets.target_series[t])
+            if n_target_samples >= self.min_samples:
+                self.targets_ticker_list.append(t)
+                self.targets_list.append(self.targets.target_series[t])
+                self.past_cov_list.append(self.covariates.past_covariates[t])
+                self.future_cov_list.append(self.covariates.future_covariates[t])
+            else:
+                logger.info(
+                    f"Skipping {t} due to lack of data. Only {n_target_samples} available"
+                )
         if self.targets_list is not None and len(self.targets_list) > 0:
             logger.info(
                 f"Sample targets columns count: {len(self.targets_list[0].columns)}, {self.targets_list[0].columns}"
             )
             logger.info(
                 f"Sample past covariates columns count: {len(self.past_cov_list[0].columns)}, {self.past_cov_list[0].columns}"
             )
@@ -486,15 +496,17 @@
     def __build_model(self, **kwargs):
         # scaler = Scaler(verbose=True, n_jobs=-1)
         # darts encoder examples: https://unit8co.github.io/darts/generated_api/darts.dataprocessing.encoders.encoders.html#
         # Prepare Encoders that Darts will automatically use for training and inference
 
         encoders = {
             "cyclic": {"future": ["dayofweek", "month", "quarter"]},
-            "datetime_attribute": {"future": ["dayofweek", "month", "quarter", "year"]},
+            "datetime_attribute": {
+                "future": ["dayofweek", "day", "month", "quarter", "year"]
+            },
             "position": {"past": ["relative"], "future": ["relative"]},
             "custom": {
                 "future": [election_year_offset]
             },  # signal proximity to US election years, which is known to have significance to market cycles.
             # "transformer": scaler
         }
         # hyperparamter selection
@@ -573,23 +585,39 @@
         ), "Call build() or load_model() before calling train()."
         # when True, multiple time series are supported
         supports_multi_ts = issubclass(
             self.torch_model.__class__, GlobalForecastingModel
         )
         assert supports_multi_ts is True
         # train model
-        # for i in range(100):
         logger.info("Starting model training...")
+        assert (
+            self.target_train_list is not None and len(self.target_train_list) > 0
+        ), "Targets train list must not be empty"
+        assert len(self.target_train_list) == len(
+            self.past_cov_list
+        ), f"""Past covs series list must be the exact same length as targets list
+            {len(self.target_train_list)} != {len(self.past_cov_list)}
+            """
+        assert len(self.target_train_list) == len(
+            self.future_cov_list
+        ), f"""Future covs series list must be the exact same length as targets list
+            {len(self.target_train_list)} != {len(self.future_cov_list)}
+            """
+        assert len(self.target_train_list) == len(
+            self.future_cov_list
+        ), f"""Validation series list must be the exact same length as targets list
+            {len(self.target_train_list)} != {len(self.target_val_list)}
+            """
         self.torch_model.fit(
             self.target_train_list,
             epochs=self.n_epochs,
             past_covariates=self.past_cov_list,
             future_covariates=self.future_cov_list,
             val_series=self.target_val_list,
-            ##val_past_covariates=self.past_cov_val_list,
             val_past_covariates=self.past_cov_list,
             val_future_covariates=self.future_cov_list,
             verbose=True,
             num_loader_workers=4,  # num_loader_workers recommended at 4*n_GPUs
         )
         logger.info("Model training finished.")
         # load best checkpoint
@@ -610,33 +638,35 @@
         fig, axes = plt.subplots(nrows=self.n_plot_samples, ncols=1, figsize=(20, 20))
         axes2 = {}
         for i in range(self.n_plot_samples):
             axes2[i] = axes[i].twinx()
         for i, t in enumerate(self.train_series.keys()):
             if i > self.n_plot_samples - 1:
                 break
-            self.train_series[t]["Close"].plot(
+            self.train_series[t][self.target_column].plot(
                 label=f"ticker {t} Close train", ax=axes[i]
             )
             #    train_series[t]['Volume'].plot(label=f'ticker {t} Volume train', ax=axes2[i])
-            self.val_series[t]["Close"].plot(label=f"ticker {t} Close val", ax=axes[i])
+            self.val_series[t][self.target_column].plot(
+                label=f"ticker {t} Close val", ax=axes[i]
+            )
             #    val_series[t]['Volume'].plot(label=f'ticker {t} Volume val', ax=axes2[i])
-            self.test_series[t]["Close"].plot(
+            self.test_series[t][self.target_column].plot(
                 label=f"ticker {t} Close test", ax=axes[i]
             )
         #    test_series[t]['Volume'].plot(label=f'ticker {t} Volume test', ax=axes2[i])
         axes[0].set_ylabel("Target Series")
 
     def plot_seasonality(self):
         # plot sample of target series
         fig, axes = plt.subplots(nrows=1, ncols=self.n_plot_samples, figsize=(12, 4))
         for i, t in enumerate(self.train_series.keys()):
             if i >= self.n_plot_samples:
                 break
-            plot_acf(self.train_series[t]["Close"], alpha=0.05, axis=axes[i])
+            plot_acf(self.train_series[t][self.target_column], alpha=0.05, axis=axes[i])
 
         axes[0].set_ylabel("Seasonality")
 
     def save_model(self):
         self.torch_model.save(self.model_name)
 
     def upload_model(self, repo_id: str = None):
@@ -665,15 +695,18 @@
         else:
             all_stock_tickers = pd.read_csv(
                 f"data/data-3rd-party/{self.stock_train_list}"
             )
             logger.info(f"Loaded {len(all_stock_tickers)} symbols in total")
             stock_set = list(set(all_stock_tickers["Symbol"]))
             # reduce ticker set to a workable sample size for one training loop
-            self.__stock_tickers = random.sample(stock_set, self.n_stocks)
+            if self.n_stocks > 0 and self.n_stocks < len(stock_set):
+                self.__stock_tickers = random.sample(stock_set, self.n_stocks)
+            else:
+                self.__stock_tickers = stock_set
         logger.info(
             f"Training loop stock subset has {len(self.stock_tickers)} tickers: ",
             self.stock_tickers,
         )
         self.targets.load_data(
             stock_tickers=self.stock_tickers,
             min_samples=self.min_samples,
@@ -771,28 +804,28 @@
 
         def plot_actual():
             for i, t in enumerate(sorted(self.train_series.keys())):
                 if i < self.n_plot_samples:
                     target = self.targets.target_series[t]
                     actual[t] = target.slice(self.val_start[t], target.end_time())
                     # ax = actual[t]['Open'].plot(label='actual Open', linewidth=1, ax=axes[i])
-                    ax = actual[t]["Close"].plot(
+                    ax = actual[t][self.target_column].plot(
                         label="actual Close", linewidth=1, ax=axes[i]
                     )
                     vol = self.covariates.past_covariates[t]["Volume"].slice(
                         self.val_start[t], target.end_time()
                     )
                     vol.plot(label="actual Volume", linewidth=1, ax=axes2[i])
 
         def plot_pred(pred_out=None, past_cov_list=None):
             # pred2 = model.predict(pred_horizon, series=pred2_series, past_covariates=past_covariates, future_covariates=future_covariates, mc_dropout=True, num_samples=500) #   len(val))
             for i, t in enumerate(sorted(self.train_series.keys())):
                 if i < self.n_plot_samples:
                     # ax = pred_out[i]['Open'].plot(label=f'forecast Open', linewidth=2, ax=axes[i])
-                    ax = pred_out[i]["Close"].plot(
+                    ax = pred_out[i][self.target_column].plot(
                         label="forecast Close", linewidth=2, ax=axes[i]
                     )
                     plt.legend()
                     # Major ticks every half year, minor ticks every month,
                     ax.xaxis.set_major_locator(dates.MonthLocator(bymonth=range(13)))
                     ax.xaxis.set_minor_locator(dates.MonthLocator())
                     ax.grid(True)
@@ -861,26 +894,28 @@
         # logger.info(f"backtest series: \n{backtest}")
         # loss = quantile_loss(target, backtest, n_jobs=-1, verbose=True)
         return backtest  # , loss
 
     def plot_backtest_results(
         self,
         target: TimeSeries = None,
-        backtest: [TimeSeries] = None,
+        backtest: List[TimeSeries] = None,
         start: pd.Timestamp = None,
         forecast_horizon: int = None,
     ):
         fig, axes = plt.subplots(figsize=(20, 12))
         # axes2 = axes.twinx()
 
         actual_sliced = target.slice(
             start - pd.Timedelta(days=self.train_history),
             target.end_time(),
         )
-        ax = actual_sliced["Close"].plot(label="actual Close", linewidth=2, ax=axes)
+        ax = actual_sliced[self.target_column].plot(
+            label="actual Close", linewidth=2, ax=axes
+        )
         # past_cov_list[i]['Volume'].plot(label='actual Volume', ax=axes2)
 
         # Major ticks every half year, minor ticks every month,
         ax.xaxis.set_major_locator(dates.MonthLocator(bymonth=range(13), interval=1))
         ax.xaxis.set_minor_locator(dates.MonthLocator())
         ax.grid(True)
```

### Comparing `canswim-0.0.8/src/canswim/model_search.py` & `canswim-0.0.9/src/canswim/model_search.py`

 * *Files identical despite different names*

### Comparing `canswim-0.0.8/src/canswim/targets.py` & `canswim-0.0.9/src/canswim/targets.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,19 +48,20 @@
         # stock_tickers = self.__get_stock_tickers(stocks_df)
         tickers = list(stocks_df.index.levels[0])
         logger.info(f"price history loaded for {len(tickers)} stocks: \n{tickers}")
         for t in tickers:
             # logger.info(f"validating price data for {t}")
             stock_full_hist = stocks_df.loc[[t]]
             if len(stock_full_hist.index) >= self.min_samples:
-                # UPDATE: Do not drop Close as it carries unique information about the relationships between OHLC and Adj Close
-                # We also keep Adj Close which takes into account dividends and splits
                 stock_full_hist = stock_full_hist.droplevel("Symbol")
                 stock_full_hist.index = pd.to_datetime(stock_full_hist.index)
-                stock_price_dict[t] = stock_full_hist  # .drop(columns=['Close'])
+                # Drop Adj Close because yfiance changes its values retroactively at future dates
+                # after stock dividend or split dates, which makes training data less stable
+                # Ref: https://help.yahoo.com/kb/adjusted-close-sln28256.html
+                stock_price_dict[t] = stock_full_hist.drop(columns=["Adj Close"])
                 # logger.info(f'ticker: {t}')
                 # logger.info(f'ticker historic data: {ticker_dict[t]}')
             else:
                 logger.info(
                     f"Skipping {t} from price series. Not enough samples for model training."
                 )
         self.stock_price_dict = stock_price_dict
@@ -92,15 +93,17 @@
                 t: drop_non_target_columns(s) for t, s in stock_price_series.items()
             }
             logger.info(f"Preparing multivariate target series: {target_columns}")
         self.target_series = target_series
 
     def prepare_stock_price_series(self, train_date_start: pd.Timestamp = None):
         loaded_tickers = self.stock_price_dict.keys()
-        logger.info(f"Preparing ticker series for {len(loaded_tickers)} stocks.")
+        logger.info(
+            f"Preparing ticker series for {len(loaded_tickers)} stocks: \n{loaded_tickers}"
+        )
         stock_price_series = {
             t: TimeSeries.from_dataframe(self.stock_price_dict[t], freq="B")
             for t in loaded_tickers
         }
         logger.info("Ticker series dict created.")
         filler = MissingValuesFiller()
         for t, series in stock_price_series.items():
```

### Comparing `canswim-0.0.8/src/canswim/train.py` & `canswim-0.0.9/src/canswim/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self.canswim_model.prepare_data()
         self.canswim_model.plot_splits()
         self.canswim_model.plot_seasonality()
 
     def build_new_model(self):
         """Build a new model using known optimal hyperparameters"""
         self.canswim_model.build(
-            input_chunk_length=168,
+            input_chunk_length=252,
             output_chunk_length=42,
             hidden_size=2048,
             num_encoder_layers=3,
             num_decoder_layers=2,
             decoder_output_dim=8,
             temporal_decoder_hidden=80,
             use_layer_norm=True,
```

### Comparing `canswim-0.0.8/src/canswim.egg-info/PKG-INFO` & `canswim-0.0.9/src/canswim.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canswim
-Version: 0.0.8
+Version: 0.0.9
 Summary: "Developer toolkit for IBD CANSLIM practitioners"
 Author: Ivelin Ivanov
 Author-email: ivelin117@gmail.com
 License: Apache-2.0
 Keywords: stock market,analytics
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -42,30 +42,22 @@
 ```
 $ python -m canswim -h
 usage: canswim [-h] {dashboard,train}
 
 CANSWIM is a toolkit for CANSLIM style investors. Aims to complement the Simple Moving Average and other technical indicators.
 
 positional arguments:
-  {dashboard,gatherdata,uploaddata,modelsearch,train,finetune,forecast}
+  {dashboard,gatherdata,uploaddata,modelsearch,train,forecast}
                         Which canswim task to run:
-                        `dashboard` for stock charting and scans of recorded forecasts.
+                        `dashboard` - start Web App service with stock charting and forecast scans.
                         'gatherdata` to gather 3rd party stock market data and save to HF Hub.
                         'uploaddata` upload to HF Hub any interim changes to local data storage.
                         `modelsearch` to find and save optimal hyperparameters for model training.
                         `train` for continuous model training.
-                        `finetune` to fine tune pretrained model on new stock market data. `forecast` to run forecast on stocks and upload dataset to HF Hub.
 
 options:
   -h, --help            show this help message and exit
   --forecast_start_date FORECAST_START_DATE
                         Optional argument for the `forecast` task. Indicate forecast start date in YYYY-MM-DD format. If not specified, forecast will start from the end of the target series.
 
 NOTE: NOT FINANCIAL OR INVESTMENT ADVICE. USE AT YOUR OWN RISK.
 ```
-
-## Interactive Dashboard hosted on Hugging Face Hub
-
-
-https://huggingface.co/spaces/ivelin/canswim_playground
-
-![canswim playground](https://github.com/ivelin/canswim/assets/2234901/26fb1a5d-49e0-4888-bc1b-042800bcef8f)
```

### Comparing `canswim-0.0.8/src/canswim.egg-info/SOURCES.txt` & `canswim-0.0.9/src/canswim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

