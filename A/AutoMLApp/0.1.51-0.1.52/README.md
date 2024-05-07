# Comparing `tmp/automlapp-0.1.51.tar.gz` & `tmp/automlapp-0.1.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automlapp-0.1.51.tar", last modified: Tue May  7 11:10:14 2024, max compression
+gzip compressed data, was "automlapp-0.1.52.tar", last modified: Tue May  7 11:18:23 2024, max compression
```

## Comparing `automlapp-0.1.51.tar` & `automlapp-0.1.52.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 11:10:14.369929 automlapp-0.1.51/
-drwxrwxrwx   0        0        0        0 2024-05-07 11:10:14.367886 automlapp-0.1.51/AutoMLApp.egg-info/
--rw-rw-rw-   0        0        0     5052 2024-05-07 11:10:14.000000 automlapp-0.1.51/AutoMLApp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      786 2024-05-07 11:10:14.000000 automlapp-0.1.51/AutoMLApp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 11:10:14.000000 automlapp-0.1.51/AutoMLApp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-05-07 11:10:14.000000 automlapp-0.1.51/AutoMLApp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      268 2024-05-07 11:10:14.000000 automlapp-0.1.51/AutoMLApp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-07 11:10:14.000000 automlapp-0.1.51/AutoMLApp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-05-03 11:39:36.000000 automlapp-0.1.51/LICENSE
--rw-rw-rw-   0        0        0     5052 2024-05-07 11:10:14.369310 automlapp-0.1.51/PKG-INFO
--rw-rw-rw-   0        0        0     3993 2024-04-12 09:40:36.000000 automlapp-0.1.51/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 11:10:14.352454 automlapp-0.1.51/automlapp/
--rw-rw-rw-   0        0        0       44 2024-05-07 10:07:08.000000 automlapp-0.1.51/automlapp/__init__.py
--rw-rw-rw-   0        0        0    60999 2024-05-07 10:10:10.000000 automlapp-0.1.51/automlapp/app.py
--rw-rw-rw-   0        0        0      405 2024-05-07 09:49:38.000000 automlapp-0.1.51/automlapp/launcher.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:10:14.362787 automlapp-0.1.51/automlapp/modules/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:09:32.000000 automlapp-0.1.51/automlapp/modules/__init__.py
--rw-rw-rw-   0        0        0     5467 2024-04-12 09:40:36.000000 automlapp-0.1.51/automlapp/modules/data_cleaning.py
--rw-rw-rw-   0        0        0     2509 2024-04-12 09:40:36.000000 automlapp-0.1.51/automlapp/modules/data_input.py
--rw-rw-rw-   0        0        0     3330 2024-04-12 09:40:36.000000 automlapp-0.1.51/automlapp/modules/data_preprocessing.py
--rw-rw-rw-   0        0        0     1072 2024-04-12 09:40:36.000000 automlapp-0.1.51/automlapp/modules/data_summarization.py
--rw-rw-rw-   0        0        0     3431 2024-04-12 09:40:36.000000 automlapp-0.1.51/automlapp/modules/data_visualization.py
--rw-rw-rw-   0        0        0     3648 2024-03-11 09:12:37.000000 automlapp-0.1.51/automlapp/modules/data_woeiv.py
--rw-rw-rw-   0        0        0     9479 2024-04-30 03:54:14.000000 automlapp-0.1.51/automlapp/modules/hyperparameter_tuning.py
--rw-rw-rw-   0        0        0    14621 2024-04-12 09:40:36.000000 automlapp-0.1.51/automlapp/modules/model_evaluation.py
--rw-rw-rw-   0        0        0     5532 2024-04-30 03:54:14.000000 automlapp-0.1.51/automlapp/modules/model_training.py
--rw-rw-rw-   0        0        0     6453 2024-04-12 09:40:36.000000 automlapp-0.1.51/automlapp/modules/train_user_params.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:10:14.365909 automlapp-0.1.51/automlapp/utils/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:09:13.000000 automlapp-0.1.51/automlapp/utils/__init__.py
--rw-rw-rw-   0        0        0      197 2024-04-12 09:40:36.000000 automlapp-0.1.51/automlapp/utils/print_utils.py
--rw-rw-rw-   0        0        0      857 2024-02-14 07:42:28.000000 automlapp-0.1.51/automlapp/utils/streamlit_utils.py
--rw-rw-rw-   0        0        0       42 2024-05-07 11:10:14.371146 automlapp-0.1.51/setup.cfg
--rw-rw-rw-   0        0        0     1493 2024-05-07 10:58:50.000000 automlapp-0.1.51/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:18:23.367214 automlapp-0.1.52/
+drwxrwxrwx   0        0        0        0 2024-05-07 11:18:23.364353 automlapp-0.1.52/AutoMLApp.egg-info/
+-rw-rw-rw-   0        0        0     5052 2024-05-07 11:18:23.000000 automlapp-0.1.52/AutoMLApp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      786 2024-05-07 11:18:23.000000 automlapp-0.1.52/AutoMLApp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 11:18:23.000000 automlapp-0.1.52/AutoMLApp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-05-07 11:18:23.000000 automlapp-0.1.52/AutoMLApp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      268 2024-05-07 11:18:23.000000 automlapp-0.1.52/AutoMLApp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-07 11:18:23.000000 automlapp-0.1.52/AutoMLApp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-05-03 11:39:36.000000 automlapp-0.1.52/LICENSE
+-rw-rw-rw-   0        0        0     5052 2024-05-07 11:18:23.367214 automlapp-0.1.52/PKG-INFO
+-rw-rw-rw-   0        0        0     3993 2024-04-12 09:40:36.000000 automlapp-0.1.52/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 11:18:23.344912 automlapp-0.1.52/automlapp/
+-rw-rw-rw-   0        0        0       44 2024-05-07 10:07:08.000000 automlapp-0.1.52/automlapp/__init__.py
+-rw-rw-rw-   0        0        0    61011 2024-05-07 11:18:08.000000 automlapp-0.1.52/automlapp/app.py
+-rw-rw-rw-   0        0        0      405 2024-05-07 09:49:38.000000 automlapp-0.1.52/automlapp/launcher.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:18:23.361610 automlapp-0.1.52/automlapp/modules/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:09:32.000000 automlapp-0.1.52/automlapp/modules/__init__.py
+-rw-rw-rw-   0        0        0     5467 2024-04-12 09:40:36.000000 automlapp-0.1.52/automlapp/modules/data_cleaning.py
+-rw-rw-rw-   0        0        0     2509 2024-04-12 09:40:36.000000 automlapp-0.1.52/automlapp/modules/data_input.py
+-rw-rw-rw-   0        0        0     3330 2024-04-12 09:40:36.000000 automlapp-0.1.52/automlapp/modules/data_preprocessing.py
+-rw-rw-rw-   0        0        0     1072 2024-04-12 09:40:36.000000 automlapp-0.1.52/automlapp/modules/data_summarization.py
+-rw-rw-rw-   0        0        0     3431 2024-04-12 09:40:36.000000 automlapp-0.1.52/automlapp/modules/data_visualization.py
+-rw-rw-rw-   0        0        0     3648 2024-03-11 09:12:37.000000 automlapp-0.1.52/automlapp/modules/data_woeiv.py
+-rw-rw-rw-   0        0        0     9479 2024-04-30 03:54:14.000000 automlapp-0.1.52/automlapp/modules/hyperparameter_tuning.py
+-rw-rw-rw-   0        0        0    14621 2024-04-12 09:40:36.000000 automlapp-0.1.52/automlapp/modules/model_evaluation.py
+-rw-rw-rw-   0        0        0     5532 2024-04-30 03:54:14.000000 automlapp-0.1.52/automlapp/modules/model_training.py
+-rw-rw-rw-   0        0        0     6453 2024-04-12 09:40:36.000000 automlapp-0.1.52/automlapp/modules/train_user_params.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:18:23.364353 automlapp-0.1.52/automlapp/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:09:13.000000 automlapp-0.1.52/automlapp/utils/__init__.py
+-rw-rw-rw-   0        0        0      197 2024-04-12 09:40:36.000000 automlapp-0.1.52/automlapp/utils/print_utils.py
+-rw-rw-rw-   0        0        0      857 2024-02-14 07:42:28.000000 automlapp-0.1.52/automlapp/utils/streamlit_utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 11:18:23.367214 automlapp-0.1.52/setup.cfg
+-rw-rw-rw-   0        0        0     1493 2024-05-07 11:18:17.000000 automlapp-0.1.52/setup.py
```

### Comparing `automlapp-0.1.51/AutoMLApp.egg-info/PKG-INFO` & `automlapp-0.1.52/AutoMLApp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoMLApp
-Version: 0.1.51
+Version: 0.1.52
 Summary: An automated machine learning application designed for efficient model training, evaluation, and hyperparameter tuning.
 Author: Shivam Nikam
 Author-email: shivam.nikam@think360.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `automlapp-0.1.51/AutoMLApp.egg-info/SOURCES.txt` & `automlapp-0.1.52/AutoMLApp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.51/LICENSE` & `automlapp-0.1.52/LICENSE`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.51/PKG-INFO` & `automlapp-0.1.52/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoMLApp
-Version: 0.1.51
+Version: 0.1.52
 Summary: An automated machine learning application designed for efficient model training, evaluation, and hyperparameter tuning.
 Author: Shivam Nikam
 Author-email: shivam.nikam@think360.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `automlapp-0.1.51/README.md` & `automlapp-0.1.52/README.md`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.51/automlapp/app.py` & `automlapp-0.1.52/automlapp/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from streamlit_extras.colored_header import colored_header
 import pandas as pd
 import plotly.express as px
 from scipy.stats import skew
 from sklearn.decomposition import PCA
 from sklearn.model_selection import train_test_split
-from utils.streamlit_utils import hide_icons, remove_whitespaces, st
-from utils.print_utils import print_shape
+from .utils.streamlit_utils import hide_icons, remove_whitespaces, st
+from .utils.print_utils import print_shape
 from streamlit_modal import Modal
 import pickle
 import os, warnings, zipfile
 
-from modules.data_input import DataInput
-from modules.data_summarization import DataSummarization
-from modules.data_cleaning import DataCleaning
-from modules.data_visualization import DataVisualization
-from modules.data_woeiv import DataWOEIV
-from modules.data_preprocessing import DataPreprocessing
-from modules.model_training import ModelTraining
-from modules.model_evaluation import ModelEvaluation
-from modules.hyperparameter_tuning import HyperparameterTuning
-from modules.train_user_params import ModelTrainingWithUserParams
+from .modules.data_input import DataInput
+from .modules.data_summarization import DataSummarization
+from .modules.data_cleaning import DataCleaning
+from .modules.data_visualization import DataVisualization
+from .modules.data_woeiv import DataWOEIV
+from .modules.data_preprocessing import DataPreprocessing
+from .modules.model_training import ModelTraining
+from .modules.model_evaluation import ModelEvaluation
+from .modules.hyperparameter_tuning import HyperparameterTuning
+from .modules.train_user_params import ModelTrainingWithUserParams
 from launcher import launch_streamlit
 
 warnings.filterwarnings("ignore")
 
 plot_colors = px.colors.sequential.Blues[::-2]
 
 st.set_page_config(layout="wide")
```

### Comparing `automlapp-0.1.51/automlapp/modules/data_cleaning.py` & `automlapp-0.1.52/automlapp/modules/data_cleaning.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.51/automlapp/modules/data_input.py` & `automlapp-0.1.52/automlapp/modules/data_input.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.51/automlapp/modules/data_preprocessing.py` & `automlapp-0.1.52/automlapp/modules/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.51/automlapp/modules/data_summarization.py` & `automlapp-0.1.52/automlapp/modules/data_summarization.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.51/automlapp/modules/data_visualization.py` & `automlapp-0.1.52/automlapp/modules/data_visualization.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.51/automlapp/modules/data_woeiv.py` & `automlapp-0.1.52/automlapp/modules/data_woeiv.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.51/automlapp/modules/hyperparameter_tuning.py` & `automlapp-0.1.52/automlapp/modules/hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.51/automlapp/modules/model_evaluation.py` & `automlapp-0.1.52/automlapp/modules/model_evaluation.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.51/automlapp/modules/model_training.py` & `automlapp-0.1.52/automlapp/modules/model_training.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.51/automlapp/modules/train_user_params.py` & `automlapp-0.1.52/automlapp/modules/train_user_params.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.51/automlapp/utils/streamlit_utils.py` & `automlapp-0.1.52/automlapp/utils/streamlit_utils.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.51/setup.py` & `automlapp-0.1.52/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="AutoMLApp",
-    version="0.1.51",
+    version="0.1.52",
     author="Shivam Nikam",
     author_email="shivam.nikam@think360.ai",
     description="An automated machine learning application designed for efficient model training, evaluation, and hyperparameter tuning.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     #url="https://github.com/YourGithub/AutoMLApp",
     packages=find_packages(),
```

