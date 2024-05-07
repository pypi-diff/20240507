# Comparing `tmp/mlimputer-1.0.65-py3-none-any.whl.zip` & `tmp/mlimputer-1.0.66-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 13216 bytes, number of entries: 10
+Zip file size: 13213 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Jan-02 00:48 mlimputer/__init__.py
 -rw-rw-rw-  2.0 fat     5174 b- defN 24-Jan-02 00:54 mlimputer/imputation.py
 -rw-rw-rw-  2.0 fat     6482 b- defN 24-Apr-20 22:10 mlimputer/model_selection.py
 -rw-rw-rw-  2.0 fat    21184 b- defN 24-Apr-20 22:05 mlimputer/models_imputation.py
 -rw-rw-rw-  2.0 fat     2801 b- defN 24-Apr-20 22:18 mlimputer/parameters.py
--rw-rw-rw-  2.0 fat     1090 b- defN 24-Apr-20 22:18 mlimputer-1.0.65.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     7026 b- defN 24-Apr-20 22:18 mlimputer-1.0.65.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-20 22:18 mlimputer-1.0.65.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-Apr-20 22:18 mlimputer-1.0.65.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      809 b- defN 24-Apr-20 22:18 mlimputer-1.0.65.dist-info/RECORD
-10 files, 44668 bytes uncompressed, 11836 bytes compressed:  73.5%
+-rw-rw-rw-  2.0 fat     1090 b- defN 24-May-07 21:34 mlimputer-1.0.66.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     7038 b- defN 24-May-07 21:34 mlimputer-1.0.66.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 21:34 mlimputer-1.0.66.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-May-07 21:34 mlimputer-1.0.66.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      809 b- defN 24-May-07 21:34 mlimputer-1.0.66.dist-info/RECORD
+10 files, 44680 bytes uncompressed, 11833 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: mlimputer/models_imputation.py
 Comment: 
 
 Filename: mlimputer/parameters.py
 Comment: 
 
-Filename: mlimputer-1.0.65.dist-info/LICENSE
+Filename: mlimputer-1.0.66.dist-info/LICENSE
 Comment: 
 
-Filename: mlimputer-1.0.65.dist-info/METADATA
+Filename: mlimputer-1.0.66.dist-info/METADATA
 Comment: 
 
-Filename: mlimputer-1.0.65.dist-info/WHEEL
+Filename: mlimputer-1.0.66.dist-info/WHEEL
 Comment: 
 
-Filename: mlimputer-1.0.65.dist-info/top_level.txt
+Filename: mlimputer-1.0.66.dist-info/top_level.txt
 Comment: 
 
-Filename: mlimputer-1.0.65.dist-info/RECORD
+Filename: mlimputer-1.0.66.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mlimputer-1.0.65.dist-info/LICENSE` & `mlimputer-1.0.66.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mlimputer-1.0.65.dist-info/METADATA` & `mlimputer-1.0.66.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mlimputer
-Version: 1.0.65
-Summary: MLimputer - Null Imputation Framework for Supervised Machine Learning
+Version: 1.0.66
+Summary: MLimputer - Missing Data Imputation Framework for Supervised Machine Learning
 Home-page: https://github.com/TsLu1s/MLimputer
 Author: Luís Santos
 Author-email: luisf_ssantos@hotmail.com
 License: MIT
 Keywords: data science,machine learning,data preprecessing,null imputation,missing data imputation,predictive null imputation,multiple null imputation,automated machine learning
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
@@ -27,15 +27,15 @@
 Requires-Dist: atlantic (>=1.1.25)
 Requires-Dist: catboost (>=1.1.1)
 Requires-Dist: xgboost (>=1.7.3)
 Requires-Dist: lightgbm (>=3.3.5)
 
 <br>
 <p align="center">
-  <h2 align="center"> MLimputer - Null Imputation Framework for Supervised Machine Learning
+  <h2 align="center"> MLimputer - Missing Data Imputation Framework for Supervised Machine Learning
   <br>
   
 ## Framework Contextualization <a name = "ta"></a>
 
 The `MLimputer` project constitutes an complete and integrated pipeline to automate the handling of missing values in datasets through regression prediction and aims at reducing bias and increase the precision of imputation results when compared to more classic imputation methods.
 This package provides multiple algorithm options to impute your data, in which every observed data column with existing missing values is fitted with a robust preprocessing approach and subsequently predicted.
 
@@ -149,12 +149,12 @@
 output = open("imputer_rf.pkl", 'wb')
 pickle.dump(mli_rf, output)
 
 ```  
     
 ## License
 
-Distributed under the MIT License. See [LICENSE](https://github.com/TsLu1s/TSForecasting/blob/main/LICENSE) for more information.
+Distributed under the MIT License. See [LICENSE](https://github.com/TsLu1s/MLimputer/blob/main/LICENSE) for more information.
 
 ## Contact 
  
 Luis Santos - [LinkedIn](https://www.linkedin.com/in/lu%C3%ADsfssantos/)
```

