# Comparing `tmp/tsforecasting-1.2.76-py3-none-any.whl.zip` & `tmp/tsforecasting-1.2.85-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,7 @@
-Zip file size: 16329 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat      391 b- defN 23-Nov-12 12:08 tsforecasting/__init__.py
--rw-rw-rw-  2.0 fat     3314 b- defN 23-Nov-19 01:20 tsforecasting/evaluation.py
--rw-rw-rw-  2.0 fat     7032 b- defN 23-Nov-19 18:53 tsforecasting/forecasting.py
--rw-rw-rw-  2.0 fat     1685 b- defN 23-Nov-20 22:15 tsforecasting/parameters.py
--rw-rw-rw-  2.0 fat    12591 b- defN 23-Nov-19 18:05 tsforecasting/treatment.py
--rw-rw-rw-  2.0 fat    13651 b- defN 23-Nov-19 18:53 tsforecasting/variational.py
--rw-rw-rw-  2.0 fat     1078 b- defN 23-Nov-27 22:14 tsforecasting-1.2.76.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9479 b- defN 23-Nov-27 22:14 tsforecasting-1.2.76.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Nov-27 22:14 tsforecasting-1.2.76.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Nov-27 22:14 tsforecasting-1.2.76.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      925 b- defN 23-Nov-27 22:14 tsforecasting-1.2.76.dist-info/RECORD
-11 files, 50252 bytes uncompressed, 14761 bytes compressed:  70.6%
+Zip file size: 5621 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     1078 b- defN 24-May-06 22:01 tsforecasting-1.2.85.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9798 b- defN 24-May-06 22:01 tsforecasting-1.2.85.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-06 22:01 tsforecasting-1.2.85.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 24-May-06 22:01 tsforecasting-1.2.85.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      421 b- defN 24-May-06 22:01 tsforecasting-1.2.85.dist-info/RECORD
+5 files, 11403 bytes uncompressed, 4831 bytes compressed:  57.6%
```

## zipnote {}

```diff
@@ -1,34 +1,16 @@
-Filename: tsforecasting/__init__.py
+Filename: tsforecasting-1.2.85.dist-info/LICENSE
 Comment: 
 
-Filename: tsforecasting/evaluation.py
+Filename: tsforecasting-1.2.85.dist-info/METADATA
 Comment: 
 
-Filename: tsforecasting/forecasting.py
+Filename: tsforecasting-1.2.85.dist-info/WHEEL
 Comment: 
 
-Filename: tsforecasting/parameters.py
+Filename: tsforecasting-1.2.85.dist-info/top_level.txt
 Comment: 
 
-Filename: tsforecasting/treatment.py
-Comment: 
-
-Filename: tsforecasting/variational.py
-Comment: 
-
-Filename: tsforecasting-1.2.76.dist-info/LICENSE
-Comment: 
-
-Filename: tsforecasting-1.2.76.dist-info/METADATA
-Comment: 
-
-Filename: tsforecasting-1.2.76.dist-info/WHEEL
-Comment: 
-
-Filename: tsforecasting-1.2.76.dist-info/top_level.txt
-Comment: 
-
-Filename: tsforecasting-1.2.76.dist-info/RECORD
+Filename: tsforecasting-1.2.85.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `tsforecasting-1.2.76.dist-info/LICENSE` & `tsforecasting-1.2.85.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tsforecasting-1.2.76.dist-info/METADATA` & `tsforecasting-1.2.85.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsforecasting
-Version: 1.2.76
+Version: 1.2.85
 Summary: TSForecasting is an Automated Time Series Forecasting Framework
 Home-page: https://github.com/TsLu1s/TSForecasting
 Author: Luís Santos
 Author-email: luisf_ssantos@hotmail.com
 License: MIT
 Keywords: data science,machine learning,time series forecasting,automated time series,multivariate time series,univariate time series,automated machine learning,automl
 Classifier: Intended Audience :: Education
@@ -23,27 +23,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas (>=1.4.4)
 Requires-Dist: numpy (>=1.23.5)
 Requires-Dist: python-dateutil (>=2.8.2)
 Requires-Dist: scikit-learn (>=1.2.2)
-Requires-Dist: pmdarima (>=2.0.1)
+Requires-Dist: autogluon (>=1.1.0)
+Requires-Dist: lightgbm (>=4.3.0)
 Requires-Dist: xgboost (>=1.7.4)
-Requires-Dist: h2o (>=3.44.0.1)
-Requires-Dist: prophet (>=1.1.2)
+Requires-Dist: catboost (>=1.2.2)
+Requires-Dist: tqdm (>=4.65.2)
 
 <br>
 <p align="center">
   <h2 align="center"> TSForecasting - Automated Time Series Forecasting Framework
   <br>
   
 ## Framework Contextualization <a name = "ta"></a>
 
-The `TSForecasting` project constitutes an complete and integrated pipeline to Automate Time Series Forecasting applications through the implementation of multivariate approaches integrating regression models referring to modules such as `SKLearn`, `H2O.ai`, `XGBoost` and also univariate approaches of more classics methods such as `Prophet` and `AutoArima`, this following an 'Expanding Window' performance evaluation.
+The `TSForecasting` project offers a comprehensive and integrated pipeline designed to Automate Time Series Forecasting applications. By implementing multivariate approaches that incorporate multiple regression models, it combines multiple relevant modules such as `SKLearn`, `AutoGluon`, `CatBoost` and `XGBoost`, following an `Expanding Window` structured approach for performance evaluation ensuring a robust, scalable and optimized forecasting solution.
 
 The architecture design includes five main sections, these being: data preprocessing, feature engineering, hyperparameter optimization, forecast ensembling and forecasting method selection which are organized and customizable in a pipeline structure.
 
 This project aims at providing the following application capabilities:
 
 * General applicability on tabular datasets: The developed forecasting procedures are applicable on any data table associated with any Time Series Forecasting scopes.
 
@@ -52,18 +53,19 @@
 * Robustness and improvement of predictive results: The implementation of the TSForecasting pipeline aims to improve the predictive performance directly associated with the application of the best performing forecasting method. 
    
 #### Main Development Tools <a name = "pre1"></a>
 
 Major frameworks used to built this project: 
 
 * [Sklearn](https://scikit-learn.org/stable/)
-* [H2O.ai](https://docs.h2o.ai/h2o/latest-stable/h2o-docs/automl.html)
+* [AutoGluon](https://auto.gluon.ai/stable/index.html)
+* [CatBoost](https://catboost.ai/)
 * [XGBoost](https://xgboost.readthedocs.io/en/stable/)
-* [AutoArima](https://alkaline-ml.com/pmdarima/modules/generated/pmdarima.arima.auto_arima.html)
-* [Prophet](https://facebook.github.io/prophet/docs/quick_start.html#python-api)
+* [LightGBM](https://lightgbm.readthedocs.io/en/latest/Installation-Guide.html)
+
     
 ## Performance Evaluation Structure <a name = "ta"></a>
 
 <p align="center">
   <img src="https://i.ibb.co/ctYj6tt/Expanding-Window-TSF.png" align="center" width="450" height="350" />
 </p>  
     
@@ -90,102 +92,103 @@
 
 # Usage Examples
     
 ## 1. TSForecasting - Automated Time Series Forecasting
     
 The first needed step after importing the package is to load a dataset and define your DataTime (`datetime64[ns]` type) and Target column to be predicted, then rename them to `Date` and `y`, respectively.
 The following step is to define your future running pipeline parameters variables, these being:
-* train_size: Length of Train data in which will be applied the first Expanding Window iteration;  
-* forecast_size: Full length of test/future ahead predictions;
-* sliding_size: Length of sliding window, sliding_size>=forecast_size is suggested;
-* models: Select all the models intented to ensemble to evaluation. To fit and compare predictive performance of available models set them in paramater `models:list`, options are the following:
+* train_size: Length of Train data in which will be applied the first Expanding Window iteration;
+* lags: The number of time steps in each window, indicating how many past observations each input sample includes;
+* horizon: Full length of test/future ahead predictions;
+* sliding_size: Length of sliding window, sliding_size>=horizon is suggested;
+* models: All selected models intented to be ensembled for evaluation. To fit and compare predictive performance of available models set them in paramater `models:list`, options are the following:
   * `RandomForest`
   * `ExtraTrees`
   * `GBR`
   * `KNN`
   * `GeneralizedLR`
   * `XGBoost`
-  * `H2O_AutoML`
-  * `AutoArima`
-  * `Prophet`
+  * `LightGBM`
+  * `Catboost`
+  * `AutoGluon`
+
 * hparameters: Nested dictionary in which are contained all models and specific hyperparameters configurations. Feel free to customize each model as you see fit (customization example shown bellow); 
 * granularity: Valid interval of periods correlated to data -> 1m,30m,1h,1d,1wk,1mo (default='1d');
 * metric: Default predictive evaluation metric is `MAE` (Mean Absolute Error), other options are `MAPE` (Mean Absolute Percentage Error) and `MSE`
 (Mean Squared Error);
  
-The `fit_forecast` method set the default parameters for fitting and comparison of all segmented windows for each selected and configurated model. After implementation, the `history` method agregates the returning variables `fit_performance` containing every detailed measure of each `window` iteration predicted value and `fit_predictions` measuring all segmented `window` iterations performance.
+The `fit_forecast` method set the default parameters for fitting and comparison of all segmented windows for each selected and configurated model. After implementation, the `history` method agregates the returning the variable `fit_performance` containing the detailed measures of each window iteration forecasted value and all segmented iterations performance.
 
 The `forecast` method forecasts the future values based on the previously predefined best performing model.
         
 ```py
 
-from tsforecasting.forecasting import TSForecasting
-from tsforecasting.parameters import model_configurations
+from tsforecasting.forecasting import (TSForecasting,
+                                       model_configurations)
 import pandas as pd
 import warnings
 warnings.filterwarnings("ignore", category=Warning) #-> For a clean console
-import h2o
-
-h2o.init() # -> Run only if using H2O_AutoML models   
 
 ## Dataframe Loading
 data = pd.read_csv('csv_directory_path') 
 data = data.rename(columns={'DateTime_Column': 'Date','Target_Name_Column':'y'})
 data = data[['Date',"y"]]
     
 ## Get Models Hyperparameters Configurations
 parameters = model_configurations()
 print(parameters)
 
 # Customization Hyperparameters Example
-parameters["RandomForest"]["n_estimators"] = 200
-parameters["KNN"]["n_neighbors"] = 5
-parameters["Prophet"]["seasonality_mode"] = 'multiplicative'
-parameters["H2O_AutoML"]["max_runtime_secs"] = 90
+hparameters["RandomForest"]["n_estimators"] = 50
+hparameters["KNN"]["n_neighbors"] = 5
+hparameters["Catboost"]["iterations"] = 150
+hparameters["AutoGluon"]["time_limit"] = 50
 
 ## Fit Forecasting Evaluation
-tsf = TSForecasting(train_size = 0.95,
-                    forecast_size = 15,
-                    sliding_size = 15,
-                    models = ['RandomForest','ExtraTrees', 'GBR', 'KNN', 'GeneralizedLR',
-                              'XGBoost', 'AutoArima','Prophet','H2O_AutoML'],
-                    hparameters = parameters,
-                    granularity = "1h", # 1m,30m,1h,1d,1wk,1mo
-                    metric = "MAE"      # MAPE, MSE
+tsf = TSForecasting(train_size = 0.90,
+                    lags = 10,
+                    horizon = 10,
+                    sliding_size = 30,
+                    models = ['RandomForest', 'GeneralizedLR', 'GBR', 'KNN', 'GeneralizedLR',
+                              'XGBoost', 'LightGBM', 'Catboost', 'AutoGluon'],
+                    hparameters = hparameters,
+                    granularity = '1h',
+                    metric = 'MAE'
                     )
 tsf = tsf.fit_forecast(dataset = data)
 
 # Get Fit History
-fit_predictions, fit_performance = tsf.history()
+fit_performance = tsf.history()
 
 ## Forecast
 forecast = tsf.forecast()
 
 ```  
 
 ## 2. TSForecasting - Extra Auxiliar Methods
-    
-The `engin_date` method converts and transforms columns of Datetime type into additional columns (Year, Day of the  Year, Season, Month, Day of the month, Day of the week, Weekend, Hour, Minute, Second) which will be added by association to the input dataset and subsequently deletes the original column if parameter `drop`=`True`.
 
-The `multivariable_lag` method creats all the past lags related to the target `y` feature automatically (in accordance to `range_lags` parameter) and adds each constructed column into the dataset.
+The `make_timeseries` method transforms a DataFrame into a format ready for time series analysis. This transformation prepares data sets for forecasting future values based on historical data, optimizing the input for subsequent model training and analysis, taking into consideration both the recency of data and the horizon of the prediction.
+
+* window_size: Determinates how many past observations each sample in the DataFrame should include. This creates a basis for learning from historical data.
+* horizon: Defines the number of future time steps to forecast. This addition provides direct targets for prediction models.
+* granularity: Adjusts the temporal detail from minutes to months, making the method suitable for diverse time series datasets (options -> 1m,30m,1h,1d,1wk,1mo).
+* datetime_engineering: When activated enriches the dataset with extra date-time features, such as year, month, and day of the week, potentialy enhancing the predictive capabilities of the model.
  
 ```py   
 
-# Feature Engineering 
-
-from tsforecasting.treatment import Treatment
+from tsforecasting.forecasting import Processing
 
-tr = Treatment()
+pr = Processing()
 
-data = tr.engin_date(dataset = data,
-                     drop = False) 
+data = pr.make_timeseries(dataset = data,
+				  window_size = 10, 
+				  horizon = 2, 
+				  granularity = '1h',
+				  datetime_engineering = True)
 
-data = tr.multivariable_lag(dataset = data,
-                            range_lags = [1,10],
-                            drop_na = True)    
 ```
     
 ## License
 
 Distributed under the MIT License. See [LICENSE](https://github.com/TsLu1s/TSForecasting/blob/main/LICENSE) for more information.
 
 ## Contact
```

