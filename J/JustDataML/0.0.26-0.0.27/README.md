# Comparing `tmp/JustDataML-0.0.26.tar.gz` & `tmp/JustDataML-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/JustDataML-0.0.26.tar", last modified: Sat Mar 30 12:56:10 2024, max compression
+gzip compressed data, was "dist/JustDataML-0.0.27.tar", last modified: Tue May  7 10:36:30 2024, max compression
```

## Comparing `JustDataML-0.0.26.tar` & `JustDataML-0.0.27.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)        0 2024-03-30 12:56:10.119458 JustDataML-0.0.26/
-drwxrwxr-x   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)        0 2024-03-30 12:56:10.115458 JustDataML-0.0.26/JDML/
--rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)     6736 2024-03-30 11:11:31.000000 JustDataML-0.0.26/JDML/JDML.py
--rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)        8 2024-03-24 08:48:59.000000 JustDataML-0.0.26/JDML/__init__.py
-drwxrwxr-x   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)        0 2024-03-30 12:56:10.119458 JustDataML-0.0.26/JDML/source/
--rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)     2596 2024-03-30 11:11:27.000000 JustDataML-0.0.26/JDML/source/Configuration.py
--rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)      636 2024-03-25 13:04:26.000000 JustDataML-0.0.26/JDML/source/Exception.py
--rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)      474 2024-03-24 08:49:58.000000 JustDataML-0.0.26/JDML/source/Logger.py
-drwxrwxr-x   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)        0 2024-03-30 12:56:10.119458 JustDataML-0.0.26/JDML/source/Pipeline/
--rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)    86942 2024-03-30 11:24:00.000000 JustDataML-0.0.26/JDML/source/Pipeline/Predict_Pipeline.py
--rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)     1935 2024-03-30 11:25:20.000000 JustDataML-0.0.26/JDML/source/Pipeline/Train_Pipeline.py
--rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)        0 2024-03-24 08:49:58.000000 JustDataML-0.0.26/JDML/source/Pipeline/__init__.py
--rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)    13717 2024-03-30 11:14:49.000000 JustDataML-0.0.26/JDML/source/Utils.py
--rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)        0 2024-03-24 08:49:58.000000 JustDataML-0.0.26/JDML/source/__init__.py
-drwxrwxr-x   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)        0 2024-03-30 12:56:10.119458 JustDataML-0.0.26/JDML/source/components/
--rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)     6604 2024-03-30 11:21:01.000000 JustDataML-0.0.26/JDML/source/components/Data_Transformation.py
--rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)     1916 2024-03-30 11:21:13.000000 JustDataML-0.0.26/JDML/source/components/Data_ingestion.py
--rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)     4028 2024-03-30 11:22:22.000000 JustDataML-0.0.26/JDML/source/components/Model_Trainer.py
--rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)        0 2024-03-24 08:49:58.000000 JustDataML-0.0.26/JDML/source/components/__init__.py
-drwxrwxr-x   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)        0 2024-03-30 12:56:10.119458 JustDataML-0.0.26/JustDataML.egg-info/
--rw-r--r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)    10934 2024-03-30 12:56:10.000000 JustDataML-0.0.26/JustDataML.egg-info/PKG-INFO
--rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)      650 2024-03-30 12:56:10.000000 JustDataML-0.0.26/JustDataML.egg-info/SOURCES.txt
--rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)        1 2024-03-30 12:56:10.000000 JustDataML-0.0.26/JustDataML.egg-info/dependency_links.txt
--rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)       42 2024-03-30 12:56:10.000000 JustDataML-0.0.26/JustDataML.egg-info/entry_points.txt
--rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)       64 2024-03-30 12:56:10.000000 JustDataML-0.0.26/JustDataML.egg-info/requires.txt
--rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)        5 2024-03-30 12:56:10.000000 JustDataML-0.0.26/JustDataML.egg-info/top_level.txt
--rw-r--r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)    10934 2024-03-30 12:56:10.119458 JustDataML-0.0.26/PKG-INFO
--rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)    10238 2024-03-30 12:55:44.000000 JustDataML-0.0.26/README.md
--rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)       38 2024-03-30 12:56:10.119458 JustDataML-0.0.26/setup.cfg
--rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)     1537 2024-03-30 12:51:31.000000 JustDataML-0.0.26/setup.py
+drwxrwxr-x   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)        0 2024-05-07 10:36:30.688300 JustDataML-0.0.27/
+drwxrwxr-x   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)        0 2024-05-07 10:36:30.684300 JustDataML-0.0.27/JDML/
+-rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)     9024 2024-04-21 18:18:16.000000 JustDataML-0.0.27/JDML/JDML.py
+-rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)        8 2024-03-24 08:48:59.000000 JustDataML-0.0.27/JDML/__init__.py
+drwxrwxr-x   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)        0 2024-05-07 10:36:30.684300 JustDataML-0.0.27/JDML/source/
+-rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)     2596 2024-03-30 11:11:27.000000 JustDataML-0.0.27/JDML/source/Configuration.py
+-rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)      636 2024-03-25 13:04:26.000000 JustDataML-0.0.27/JDML/source/Exception.py
+-rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)      474 2024-03-24 08:49:58.000000 JustDataML-0.0.27/JDML/source/Logger.py
+drwxrwxr-x   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)        0 2024-05-07 10:36:30.684300 JustDataML-0.0.27/JDML/source/Pipeline/
+-rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)    86942 2024-03-30 11:24:00.000000 JustDataML-0.0.27/JDML/source/Pipeline/Predict_Pipeline.py
+-rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)     1935 2024-03-30 11:25:20.000000 JustDataML-0.0.27/JDML/source/Pipeline/Train_Pipeline.py
+-rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)        0 2024-03-24 08:49:58.000000 JustDataML-0.0.27/JDML/source/Pipeline/__init__.py
+-rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)    13717 2024-03-30 11:14:49.000000 JustDataML-0.0.27/JDML/source/Utils.py
+-rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)        0 2024-03-24 08:49:58.000000 JustDataML-0.0.27/JDML/source/__init__.py
+drwxrwxr-x   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)        0 2024-05-07 10:36:30.688300 JustDataML-0.0.27/JDML/source/components/
+-rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)     6604 2024-03-30 11:21:01.000000 JustDataML-0.0.27/JDML/source/components/Data_Transformation.py
+-rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)     1916 2024-03-30 11:21:13.000000 JustDataML-0.0.27/JDML/source/components/Data_ingestion.py
+-rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)     4028 2024-03-30 11:22:22.000000 JustDataML-0.0.27/JDML/source/components/Model_Trainer.py
+-rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)        0 2024-03-24 08:49:58.000000 JustDataML-0.0.27/JDML/source/components/__init__.py
+drwxrwxr-x   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)        0 2024-05-07 10:36:30.688300 JustDataML-0.0.27/JustDataML.egg-info/
+-rw-r--r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)    13096 2024-05-07 10:36:30.000000 JustDataML-0.0.27/JustDataML.egg-info/PKG-INFO
+-rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)      650 2024-05-07 10:36:30.000000 JustDataML-0.0.27/JustDataML.egg-info/SOURCES.txt
+-rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)        1 2024-05-07 10:36:30.000000 JustDataML-0.0.27/JustDataML.egg-info/dependency_links.txt
+-rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)       42 2024-05-07 10:36:30.000000 JustDataML-0.0.27/JustDataML.egg-info/entry_points.txt
+-rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)       64 2024-05-07 10:36:30.000000 JustDataML-0.0.27/JustDataML.egg-info/requires.txt
+-rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)        5 2024-05-07 10:36:30.000000 JustDataML-0.0.27/JustDataML.egg-info/top_level.txt
+-rw-r--r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)    13096 2024-05-07 10:36:30.688300 JustDataML-0.0.27/PKG-INFO
+-rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)    12455 2024-05-07 10:32:20.000000 JustDataML-0.0.27/README.md
+-rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)       38 2024-05-07 10:36:30.688300 JustDataML-0.0.27/setup.cfg
+-rw-rw-r--   0 jaideepsinh.dabhi  (1001) jaideepsinh.dabhi  (1001)     1482 2024-05-07 10:34:48.000000 JustDataML-0.0.27/setup.py
```

### Comparing `JustDataML-0.0.26/JDML/source/Configuration.py` & `JustDataML-0.0.27/JDML/source/Configuration.py`

 * *Files identical despite different names*

### Comparing `JustDataML-0.0.26/JDML/source/Exception.py` & `JustDataML-0.0.27/JDML/source/Exception.py`

 * *Files identical despite different names*

### Comparing `JustDataML-0.0.26/JDML/source/Pipeline/Predict_Pipeline.py` & `JustDataML-0.0.27/JDML/source/Pipeline/Predict_Pipeline.py`

 * *Files identical despite different names*

### Comparing `JustDataML-0.0.26/JDML/source/Pipeline/Train_Pipeline.py` & `JustDataML-0.0.27/JDML/source/Pipeline/Train_Pipeline.py`

 * *Files identical despite different names*

### Comparing `JustDataML-0.0.26/JDML/source/Utils.py` & `JustDataML-0.0.27/JDML/source/Utils.py`

 * *Files identical despite different names*

### Comparing `JustDataML-0.0.26/JDML/source/components/Data_Transformation.py` & `JustDataML-0.0.27/JDML/source/components/Data_Transformation.py`

 * *Files identical despite different names*

### Comparing `JustDataML-0.0.26/JDML/source/components/Data_ingestion.py` & `JustDataML-0.0.27/JDML/source/components/Data_ingestion.py`

 * *Files identical despite different names*

### Comparing `JustDataML-0.0.26/JDML/source/components/Model_Trainer.py` & `JustDataML-0.0.27/JDML/source/components/Model_Trainer.py`

 * *Files identical despite different names*

### Comparing `JustDataML-0.0.26/JustDataML.egg-info/PKG-INFO` & `JustDataML-0.0.27/JustDataML.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: JustDataML
-Version: 0.0.26
-Summary: This is a Machine Learning Tool Developed to Help Non Tech Students and Non Coders to try ML for there Data
+Version: 0.0.27
+Summary: JustDataML :Simplified Machine Learning for Everyone
 Home-page: https://github.com/jaideepsinhdabhi/JustDataML
 Author: Jaideepsinh Dabhi
 Author-email: jadieep.dabhi7603@gmail.com
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
@@ -42,15 +42,15 @@
 
 to Run this Tool you will Require
 Below this thing to do
 
 
 ## Installation
 
-Suggestion: Please Use a Virtual env for this to succesfully run it 
+Suggestion: Use a Virtual env for this to succesfully run it 
 
 1. Install my Application with pip install
 
 ```bash
   pip install JustDataML
 
 ```
@@ -78,68 +78,114 @@
 ## Usage/Examples CLI Tool
 
 ```bash
 python JDML/JDML.py -- Config <Data Config File> --Train --Predict <test.csv> --Output <Output Name>
 
 ```
 ### Arguments
-- `-C, --Config`: [Compulsory] You need to provide a configuration file to obtain all the necessary arguments.
+- `-C, --Config`: You need to provide a configuration file to obtain all the necessary arguments.
 
     Note: Make sure you give proper argument mentioned in the Document.
 
 - `-T, --Train`: [Optional] If provided, it initiates model training based on the specified data_config file. 
 
     Note : Ensure that the Data files are available in the "Data" folder.
 
 - `-P, --Predict`: [Optional] If provided, performs prediction using the trained model. Make sure not to delete or modify the artifact folder to get the results.
 
 - `-O, --Output`: [Required with -P (--Predict)] Specifies the output name for the predicted dataframe generated from the test data.
     Note: it will also generate Model_summary file and if Hyperparameter is given Yes in Config file then it will generate stats file for that too
 
 
 
-## Usage/Examples Python
+## Usage/Examples as a Python library
 
 we can also use this tool as a python library
+
+First we will import required libraries
 ```python
-from JDML.JDML import Just_Data_ML
-import argparse
+
+import pandas as pd # to read our data
+from JDML.JDML import Just_Data_ML # to train , predict using JDML tool
+
+
+# we will also import Libraries that we will use in our models
+
+# for Normalization we can use other also
+from sklearn.preprocessing import StandardScaler
+
+# here for example we will use Random Forest and linear regression
+from sklearn.ensemble import RandomForestRegressor 
+from sklearn.linear_model import LinearRegression
 
 ```
-Import the Tool
+we have create a instance to use jdml
 
 ```python
+jdml_in = Just_Data_ML()
 
-arguments = argparse.Namespace(Config="Data_Config.csv",Train=True,Predict="Test.csv", Output="Output.csv")
 ```
-Yes we need to give arguments like this (will fix thsi issue in next release)
+Lets Read the Data
+
+Here we are using a bioinformatics data (KEGG Metabolic Reaction Network (Undirected)) and we will predict e for our example.
+
+you can find Data [Here](https://archive.ics.uci.edu/dataset/221/kegg+metabolic+reaction+network+undirected)
+
 
 ```python
-jdml=Just_Data_ML(arguments)
+data_df = pd.read_csv("Data/Reaction Network (Undirected).csv",index_col=False)
 
 ```
-parsing the arugments
+Let's Assign Target_Col and Features for our task
 
 ```python
-jdml.Data_df
+Feature_Kegg = ["Connected Components","Diameter","Radius","Centralization","Shortest Path","Characteristic Path","Avg.num.Neighbours","Density","Heterogeneity","Isolated Nodes","Number of Self Loops","Multi-edge Node Pair","NeighborhoodConnectivity","NumberOfDirectedEdges","Stress","SelfLoops",
+"Partner Of MultiEdged NodePairs","Degree","TopologicalCoefficient","BetweennessCentrality","Radiality","Eccentricity","NumberOfUndirectedEdges","ClosenessCentrality","AverageShortestPathLength","ClusteringCoefficient","nodeCount"]
+
+
+target_col = ['edgeCount']
 ```
-For checking the DataFrame you provided 
+we have consider all columns as feature but we can do a feature selection and train your model for those selected features. for now we will use all the features and predict `edgeCount` as Target.
 
+Now we also need to assign few other paramters and arguments for our tool
 ```python
-jdml.Data_train()
+Problem_Objective = 'Regression'   #task to choose between regresison and classification
+Normalization = StandardScaler()  # Normalization technique our data
+
+Models_to_train = {'Random Forest':RandomForestRegressor(n_jobs=-1), 'Linear Regression':LinearRegression()}   # we have select our models and parse it as dict to work.
 ```
 For Model Training 
 
 ```python
-jdml.Predict_test()
+jdml_in.Data_Train(Feature_Kegg,data_df,target_col,Models_to_train,    
+    Problem_Objective,HyperParamter_Yes_or_No='Yes',  #by default it will be 'No'
+    Normalization_tech=Normalization)
 
 ```
-For Predicting the Test gvien
 
-Voila You will have the Prediction file (Column `Target_Out`) in the Output Folder.
+You will have your model trained now its time for prediction
+
+
+```python
+# importing test csv as DataFrame
+test_df = pd.read_csv("test.csv")
+
+```
+note: Yes, you do not need to preprocess test file it will be handled by tool itself.
+
+Now we need to do prediction from our test file.
+
+```python
+predictions = jdml_in.Predict_test(Problem_Objective,Feature_Kegg,test_df)
+
+```
+
+Voila You will have the Prediction file (Column `Target_Out`) in the Output DataFrame.
+
+
 
 ## Data Configuration File Example
 
 This is an example of a data configuration file (`Data_Config.csv`) used with the JustData_ML (JDML) tool. This file specifies the necessary information for training and predicting with machine learning models.
 
 ### CSV Structure:
 
@@ -152,15 +198,15 @@
 - **Normalization_tech:** Normalization technique to be applied (`StandardScaler`, `MinMaxScaler`, etc.).
 - **Model_to_include:** Models to include in the training process (`ALL` or specific models). (below Listed for Models)
 - **HyperParamter_Yes_or_No:** Indicates whether hyperparameter tuning should be performed (`Yes` or `No`).
 
 
     #####   A sample csv file and some Data are there in Data Folder for a demo Run
 
-    #### Note : It will also generate logs into a logs folder for every run please check for every Run to get more idea on that.
+    #### Note : It will also generate logs into a logs folder for every run check for every Run to get more idea on that.
 
 ## Available Models for Regression and Classification
 
 ### Regression Models:
 
 1. **Random Forest**
    - Description: Random Forest is an ensemble learning method that operates by constructing multiple decision trees during training and outputting the mean prediction of the individual trees.
```

### Comparing `JustDataML-0.0.26/JustDataML.egg-info/SOURCES.txt` & `JustDataML-0.0.27/JustDataML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JustDataML-0.0.26/PKG-INFO` & `JustDataML-0.0.27/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: JustDataML
-Version: 0.0.26
-Summary: This is a Machine Learning Tool Developed to Help Non Tech Students and Non Coders to try ML for there Data
+Version: 0.0.27
+Summary: JustDataML :Simplified Machine Learning for Everyone
 Home-page: https://github.com/jaideepsinhdabhi/JustDataML
 Author: Jaideepsinh Dabhi
 Author-email: jadieep.dabhi7603@gmail.com
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
@@ -42,15 +42,15 @@
 
 to Run this Tool you will Require
 Below this thing to do
 
 
 ## Installation
 
-Suggestion: Please Use a Virtual env for this to succesfully run it 
+Suggestion: Use a Virtual env for this to succesfully run it 
 
 1. Install my Application with pip install
 
 ```bash
   pip install JustDataML
 
 ```
@@ -78,68 +78,114 @@
 ## Usage/Examples CLI Tool
 
 ```bash
 python JDML/JDML.py -- Config <Data Config File> --Train --Predict <test.csv> --Output <Output Name>
 
 ```
 ### Arguments
-- `-C, --Config`: [Compulsory] You need to provide a configuration file to obtain all the necessary arguments.
+- `-C, --Config`: You need to provide a configuration file to obtain all the necessary arguments.
 
     Note: Make sure you give proper argument mentioned in the Document.
 
 - `-T, --Train`: [Optional] If provided, it initiates model training based on the specified data_config file. 
 
     Note : Ensure that the Data files are available in the "Data" folder.
 
 - `-P, --Predict`: [Optional] If provided, performs prediction using the trained model. Make sure not to delete or modify the artifact folder to get the results.
 
 - `-O, --Output`: [Required with -P (--Predict)] Specifies the output name for the predicted dataframe generated from the test data.
     Note: it will also generate Model_summary file and if Hyperparameter is given Yes in Config file then it will generate stats file for that too
 
 
 
-## Usage/Examples Python
+## Usage/Examples as a Python library
 
 we can also use this tool as a python library
+
+First we will import required libraries
 ```python
-from JDML.JDML import Just_Data_ML
-import argparse
+
+import pandas as pd # to read our data
+from JDML.JDML import Just_Data_ML # to train , predict using JDML tool
+
+
+# we will also import Libraries that we will use in our models
+
+# for Normalization we can use other also
+from sklearn.preprocessing import StandardScaler
+
+# here for example we will use Random Forest and linear regression
+from sklearn.ensemble import RandomForestRegressor 
+from sklearn.linear_model import LinearRegression
 
 ```
-Import the Tool
+we have create a instance to use jdml
 
 ```python
+jdml_in = Just_Data_ML()
 
-arguments = argparse.Namespace(Config="Data_Config.csv",Train=True,Predict="Test.csv", Output="Output.csv")
 ```
-Yes we need to give arguments like this (will fix thsi issue in next release)
+Lets Read the Data
+
+Here we are using a bioinformatics data (KEGG Metabolic Reaction Network (Undirected)) and we will predict e for our example.
+
+you can find Data [Here](https://archive.ics.uci.edu/dataset/221/kegg+metabolic+reaction+network+undirected)
+
 
 ```python
-jdml=Just_Data_ML(arguments)
+data_df = pd.read_csv("Data/Reaction Network (Undirected).csv",index_col=False)
 
 ```
-parsing the arugments
+Let's Assign Target_Col and Features for our task
 
 ```python
-jdml.Data_df
+Feature_Kegg = ["Connected Components","Diameter","Radius","Centralization","Shortest Path","Characteristic Path","Avg.num.Neighbours","Density","Heterogeneity","Isolated Nodes","Number of Self Loops","Multi-edge Node Pair","NeighborhoodConnectivity","NumberOfDirectedEdges","Stress","SelfLoops",
+"Partner Of MultiEdged NodePairs","Degree","TopologicalCoefficient","BetweennessCentrality","Radiality","Eccentricity","NumberOfUndirectedEdges","ClosenessCentrality","AverageShortestPathLength","ClusteringCoefficient","nodeCount"]
+
+
+target_col = ['edgeCount']
 ```
-For checking the DataFrame you provided 
+we have consider all columns as feature but we can do a feature selection and train your model for those selected features. for now we will use all the features and predict `edgeCount` as Target.
 
+Now we also need to assign few other paramters and arguments for our tool
 ```python
-jdml.Data_train()
+Problem_Objective = 'Regression'   #task to choose between regresison and classification
+Normalization = StandardScaler()  # Normalization technique our data
+
+Models_to_train = {'Random Forest':RandomForestRegressor(n_jobs=-1), 'Linear Regression':LinearRegression()}   # we have select our models and parse it as dict to work.
 ```
 For Model Training 
 
 ```python
-jdml.Predict_test()
+jdml_in.Data_Train(Feature_Kegg,data_df,target_col,Models_to_train,    
+    Problem_Objective,HyperParamter_Yes_or_No='Yes',  #by default it will be 'No'
+    Normalization_tech=Normalization)
 
 ```
-For Predicting the Test gvien
 
-Voila You will have the Prediction file (Column `Target_Out`) in the Output Folder.
+You will have your model trained now its time for prediction
+
+
+```python
+# importing test csv as DataFrame
+test_df = pd.read_csv("test.csv")
+
+```
+note: Yes, you do not need to preprocess test file it will be handled by tool itself.
+
+Now we need to do prediction from our test file.
+
+```python
+predictions = jdml_in.Predict_test(Problem_Objective,Feature_Kegg,test_df)
+
+```
+
+Voila You will have the Prediction file (Column `Target_Out`) in the Output DataFrame.
+
+
 
 ## Data Configuration File Example
 
 This is an example of a data configuration file (`Data_Config.csv`) used with the JustData_ML (JDML) tool. This file specifies the necessary information for training and predicting with machine learning models.
 
 ### CSV Structure:
 
@@ -152,15 +198,15 @@
 - **Normalization_tech:** Normalization technique to be applied (`StandardScaler`, `MinMaxScaler`, etc.).
 - **Model_to_include:** Models to include in the training process (`ALL` or specific models). (below Listed for Models)
 - **HyperParamter_Yes_or_No:** Indicates whether hyperparameter tuning should be performed (`Yes` or `No`).
 
 
     #####   A sample csv file and some Data are there in Data Folder for a demo Run
 
-    #### Note : It will also generate logs into a logs folder for every run please check for every Run to get more idea on that.
+    #### Note : It will also generate logs into a logs folder for every run check for every Run to get more idea on that.
 
 ## Available Models for Regression and Classification
 
 ### Regression Models:
 
 1. **Random Forest**
    - Description: Random Forest is an ensemble learning method that operates by constructing multiple decision trees during training and outputting the mean prediction of the individual trees.
```

### Comparing `JustDataML-0.0.26/README.md` & `JustDataML-0.0.27/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 to Run this Tool you will Require
 Below this thing to do
 
 
 ## Installation
 
-Suggestion: Please Use a Virtual env for this to succesfully run it 
+Suggestion: Use a Virtual env for this to succesfully run it 
 
 1. Install my Application with pip install
 
 ```bash
   pip install JustDataML
 
 ```
@@ -58,68 +58,114 @@
 ## Usage/Examples CLI Tool
 
 ```bash
 python JDML/JDML.py -- Config <Data Config File> --Train --Predict <test.csv> --Output <Output Name>
 
 ```
 ### Arguments
-- `-C, --Config`: [Compulsory] You need to provide a configuration file to obtain all the necessary arguments.
+- `-C, --Config`: You need to provide a configuration file to obtain all the necessary arguments.
 
     Note: Make sure you give proper argument mentioned in the Document.
 
 - `-T, --Train`: [Optional] If provided, it initiates model training based on the specified data_config file. 
 
     Note : Ensure that the Data files are available in the "Data" folder.
 
 - `-P, --Predict`: [Optional] If provided, performs prediction using the trained model. Make sure not to delete or modify the artifact folder to get the results.
 
 - `-O, --Output`: [Required with -P (--Predict)] Specifies the output name for the predicted dataframe generated from the test data.
     Note: it will also generate Model_summary file and if Hyperparameter is given Yes in Config file then it will generate stats file for that too
 
 
 
-## Usage/Examples Python
+## Usage/Examples as a Python library
 
 we can also use this tool as a python library
+
+First we will import required libraries
 ```python
-from JDML.JDML import Just_Data_ML
-import argparse
+
+import pandas as pd # to read our data
+from JDML.JDML import Just_Data_ML # to train , predict using JDML tool
+
+
+# we will also import Libraries that we will use in our models
+
+# for Normalization we can use other also
+from sklearn.preprocessing import StandardScaler
+
+# here for example we will use Random Forest and linear regression
+from sklearn.ensemble import RandomForestRegressor 
+from sklearn.linear_model import LinearRegression
 
 ```
-Import the Tool
+we have create a instance to use jdml
 
 ```python
+jdml_in = Just_Data_ML()
 
-arguments = argparse.Namespace(Config="Data_Config.csv",Train=True,Predict="Test.csv", Output="Output.csv")
 ```
-Yes we need to give arguments like this (will fix thsi issue in next release)
+Lets Read the Data
+
+Here we are using a bioinformatics data (KEGG Metabolic Reaction Network (Undirected)) and we will predict e for our example.
+
+you can find Data [Here](https://archive.ics.uci.edu/dataset/221/kegg+metabolic+reaction+network+undirected)
+
 
 ```python
-jdml=Just_Data_ML(arguments)
+data_df = pd.read_csv("Data/Reaction Network (Undirected).csv",index_col=False)
 
 ```
-parsing the arugments
+Let's Assign Target_Col and Features for our task
 
 ```python
-jdml.Data_df
+Feature_Kegg = ["Connected Components","Diameter","Radius","Centralization","Shortest Path","Characteristic Path","Avg.num.Neighbours","Density","Heterogeneity","Isolated Nodes","Number of Self Loops","Multi-edge Node Pair","NeighborhoodConnectivity","NumberOfDirectedEdges","Stress","SelfLoops",
+"Partner Of MultiEdged NodePairs","Degree","TopologicalCoefficient","BetweennessCentrality","Radiality","Eccentricity","NumberOfUndirectedEdges","ClosenessCentrality","AverageShortestPathLength","ClusteringCoefficient","nodeCount"]
+
+
+target_col = ['edgeCount']
 ```
-For checking the DataFrame you provided 
+we have consider all columns as feature but we can do a feature selection and train your model for those selected features. for now we will use all the features and predict `edgeCount` as Target.
 
+Now we also need to assign few other paramters and arguments for our tool
 ```python
-jdml.Data_train()
+Problem_Objective = 'Regression'   #task to choose between regresison and classification
+Normalization = StandardScaler()  # Normalization technique our data
+
+Models_to_train = {'Random Forest':RandomForestRegressor(n_jobs=-1), 'Linear Regression':LinearRegression()}   # we have select our models and parse it as dict to work.
 ```
 For Model Training 
 
 ```python
-jdml.Predict_test()
+jdml_in.Data_Train(Feature_Kegg,data_df,target_col,Models_to_train,    
+    Problem_Objective,HyperParamter_Yes_or_No='Yes',  #by default it will be 'No'
+    Normalization_tech=Normalization)
 
 ```
-For Predicting the Test gvien
 
-Voila You will have the Prediction file (Column `Target_Out`) in the Output Folder.
+You will have your model trained now its time for prediction
+
+
+```python
+# importing test csv as DataFrame
+test_df = pd.read_csv("test.csv")
+
+```
+note: Yes, you do not need to preprocess test file it will be handled by tool itself.
+
+Now we need to do prediction from our test file.
+
+```python
+predictions = jdml_in.Predict_test(Problem_Objective,Feature_Kegg,test_df)
+
+```
+
+Voila You will have the Prediction file (Column `Target_Out`) in the Output DataFrame.
+
+
 
 ## Data Configuration File Example
 
 This is an example of a data configuration file (`Data_Config.csv`) used with the JustData_ML (JDML) tool. This file specifies the necessary information for training and predicting with machine learning models.
 
 ### CSV Structure:
 
@@ -132,15 +178,15 @@
 - **Normalization_tech:** Normalization technique to be applied (`StandardScaler`, `MinMaxScaler`, etc.).
 - **Model_to_include:** Models to include in the training process (`ALL` or specific models). (below Listed for Models)
 - **HyperParamter_Yes_or_No:** Indicates whether hyperparameter tuning should be performed (`Yes` or `No`).
 
 
     #####   A sample csv file and some Data are there in Data Folder for a demo Run
 
-    #### Note : It will also generate logs into a logs folder for every run please check for every Run to get more idea on that.
+    #### Note : It will also generate logs into a logs folder for every run check for every Run to get more idea on that.
 
 ## Available Models for Regression and Classification
 
 ### Regression Models:
 
 1. **Random Forest**
    - Description: Random Forest is an ensemble learning method that operates by constructing multiple decision trees during training and outputting the mean prediction of the individual trees.
```

### Comparing `JustDataML-0.0.26/setup.py` & `JustDataML-0.0.27/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 with open("README.md", "r") as f:
     long_description = f.read()
 
 #print(get_requirements('requirements.txt'))
 
 setup(
     name="JustDataML",
-    version="0.0.26",
+    version="0.0.27",
     author="Jaideepsinh Dabhi",
     author_email="jadieep.dabhi7603@gmail.com",
-    description="This is a Machine Learning Tool Developed to Help Non Tech Students and Non Coders to try ML for there Data",
+    description="JustDataML :Simplified Machine Learning for Everyone",
     #package_dir={"":"JDML"},
     #packages=find_packages(where="JDML"),
     packages=find_packages(),
     #packages=find_packages(include=[".", "source.*"]),
     url="https://github.com/jaideepsinhdabhi/JustDataML",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

