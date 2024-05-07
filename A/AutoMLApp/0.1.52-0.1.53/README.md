# Comparing `tmp/automlapp-0.1.52.tar.gz` & `tmp/automlapp-0.1.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automlapp-0.1.52.tar", last modified: Tue May  7 11:18:23 2024, max compression
+gzip compressed data, was "automlapp-0.1.53.tar", last modified: Tue May  7 11:26:49 2024, max compression
```

## Comparing `automlapp-0.1.52.tar` & `automlapp-0.1.53.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 11:18:23.367214 automlapp-0.1.52/
-drwxrwxrwx   0        0        0        0 2024-05-07 11:18:23.364353 automlapp-0.1.52/AutoMLApp.egg-info/
--rw-rw-rw-   0        0        0     5052 2024-05-07 11:18:23.000000 automlapp-0.1.52/AutoMLApp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      786 2024-05-07 11:18:23.000000 automlapp-0.1.52/AutoMLApp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 11:18:23.000000 automlapp-0.1.52/AutoMLApp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-05-07 11:18:23.000000 automlapp-0.1.52/AutoMLApp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      268 2024-05-07 11:18:23.000000 automlapp-0.1.52/AutoMLApp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-07 11:18:23.000000 automlapp-0.1.52/AutoMLApp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-05-03 11:39:36.000000 automlapp-0.1.52/LICENSE
--rw-rw-rw-   0        0        0     5052 2024-05-07 11:18:23.367214 automlapp-0.1.52/PKG-INFO
--rw-rw-rw-   0        0        0     3993 2024-04-12 09:40:36.000000 automlapp-0.1.52/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 11:18:23.344912 automlapp-0.1.52/automlapp/
--rw-rw-rw-   0        0        0       44 2024-05-07 10:07:08.000000 automlapp-0.1.52/automlapp/__init__.py
--rw-rw-rw-   0        0        0    61011 2024-05-07 11:18:08.000000 automlapp-0.1.52/automlapp/app.py
--rw-rw-rw-   0        0        0      405 2024-05-07 09:49:38.000000 automlapp-0.1.52/automlapp/launcher.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:18:23.361610 automlapp-0.1.52/automlapp/modules/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:09:32.000000 automlapp-0.1.52/automlapp/modules/__init__.py
--rw-rw-rw-   0        0        0     5467 2024-04-12 09:40:36.000000 automlapp-0.1.52/automlapp/modules/data_cleaning.py
--rw-rw-rw-   0        0        0     2509 2024-04-12 09:40:36.000000 automlapp-0.1.52/automlapp/modules/data_input.py
--rw-rw-rw-   0        0        0     3330 2024-04-12 09:40:36.000000 automlapp-0.1.52/automlapp/modules/data_preprocessing.py
--rw-rw-rw-   0        0        0     1072 2024-04-12 09:40:36.000000 automlapp-0.1.52/automlapp/modules/data_summarization.py
--rw-rw-rw-   0        0        0     3431 2024-04-12 09:40:36.000000 automlapp-0.1.52/automlapp/modules/data_visualization.py
--rw-rw-rw-   0        0        0     3648 2024-03-11 09:12:37.000000 automlapp-0.1.52/automlapp/modules/data_woeiv.py
--rw-rw-rw-   0        0        0     9479 2024-04-30 03:54:14.000000 automlapp-0.1.52/automlapp/modules/hyperparameter_tuning.py
--rw-rw-rw-   0        0        0    14621 2024-04-12 09:40:36.000000 automlapp-0.1.52/automlapp/modules/model_evaluation.py
--rw-rw-rw-   0        0        0     5532 2024-04-30 03:54:14.000000 automlapp-0.1.52/automlapp/modules/model_training.py
--rw-rw-rw-   0        0        0     6453 2024-04-12 09:40:36.000000 automlapp-0.1.52/automlapp/modules/train_user_params.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:18:23.364353 automlapp-0.1.52/automlapp/utils/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:09:13.000000 automlapp-0.1.52/automlapp/utils/__init__.py
--rw-rw-rw-   0        0        0      197 2024-04-12 09:40:36.000000 automlapp-0.1.52/automlapp/utils/print_utils.py
--rw-rw-rw-   0        0        0      857 2024-02-14 07:42:28.000000 automlapp-0.1.52/automlapp/utils/streamlit_utils.py
--rw-rw-rw-   0        0        0       42 2024-05-07 11:18:23.367214 automlapp-0.1.52/setup.cfg
--rw-rw-rw-   0        0        0     1493 2024-05-07 11:18:17.000000 automlapp-0.1.52/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:26:49.824471 automlapp-0.1.53/
+drwxrwxrwx   0        0        0        0 2024-05-07 11:26:49.824471 automlapp-0.1.53/AutoMLApp.egg-info/
+-rw-rw-rw-   0        0        0     5052 2024-05-07 11:26:49.000000 automlapp-0.1.53/AutoMLApp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      747 2024-05-07 11:26:49.000000 automlapp-0.1.53/AutoMLApp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 11:26:49.000000 automlapp-0.1.53/AutoMLApp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-05-07 11:26:49.000000 automlapp-0.1.53/AutoMLApp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      268 2024-05-07 11:26:49.000000 automlapp-0.1.53/AutoMLApp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-07 11:26:49.000000 automlapp-0.1.53/AutoMLApp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-05-03 11:39:36.000000 automlapp-0.1.53/LICENSE
+-rw-rw-rw-   0        0        0     5052 2024-05-07 11:26:49.824471 automlapp-0.1.53/PKG-INFO
+-rw-rw-rw-   0        0        0     3993 2024-04-12 09:40:36.000000 automlapp-0.1.53/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 11:26:49.672494 automlapp-0.1.53/automlapp/
+-rw-rw-rw-   0        0        0       44 2024-05-07 10:07:08.000000 automlapp-0.1.53/automlapp/__init__.py
+-rw-rw-rw-   0        0        0    61011 2024-05-07 11:18:08.000000 automlapp-0.1.53/automlapp/app.py
+-rw-rw-rw-   0        0        0      405 2024-05-07 09:49:38.000000 automlapp-0.1.53/automlapp/launcher.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:26:49.804791 automlapp-0.1.53/automlapp/modules/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:09:32.000000 automlapp-0.1.53/automlapp/modules/__init__.py
+-rw-rw-rw-   0        0        0     5469 2024-05-07 11:23:48.000000 automlapp-0.1.53/automlapp/modules/data_cleaning.py
+-rw-rw-rw-   0        0        0     2511 2024-05-07 11:23:57.000000 automlapp-0.1.53/automlapp/modules/data_input.py
+-rw-rw-rw-   0        0        0     3332 2024-05-07 11:24:04.000000 automlapp-0.1.53/automlapp/modules/data_preprocessing.py
+-rw-rw-rw-   0        0        0     1074 2024-05-07 11:24:45.000000 automlapp-0.1.53/automlapp/modules/data_summarization.py
+-rw-rw-rw-   0        0        0     3433 2024-05-07 11:24:56.000000 automlapp-0.1.53/automlapp/modules/data_visualization.py
+-rw-rw-rw-   0        0        0     3650 2024-05-07 11:25:02.000000 automlapp-0.1.53/automlapp/modules/data_woeiv.py
+-rw-rw-rw-   0        0        0     9481 2024-05-07 11:25:23.000000 automlapp-0.1.53/automlapp/modules/hyperparameter_tuning.py
+-rw-rw-rw-   0        0        0    14623 2024-05-07 11:26:02.000000 automlapp-0.1.53/automlapp/modules/model_evaluation.py
+-rw-rw-rw-   0        0        0     5534 2024-05-07 11:26:09.000000 automlapp-0.1.53/automlapp/modules/model_training.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:26:49.815918 automlapp-0.1.53/automlapp/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:09:13.000000 automlapp-0.1.53/automlapp/utils/__init__.py
+-rw-rw-rw-   0        0        0      191 2024-05-07 11:20:36.000000 automlapp-0.1.53/automlapp/utils/print_utils.py
+-rw-rw-rw-   0        0        0      857 2024-02-14 07:42:28.000000 automlapp-0.1.53/automlapp/utils/streamlit_utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 11:26:49.824471 automlapp-0.1.53/setup.cfg
+-rw-rw-rw-   0        0        0     1493 2024-05-07 11:26:46.000000 automlapp-0.1.53/setup.py
```

### Comparing `automlapp-0.1.52/AutoMLApp.egg-info/PKG-INFO` & `automlapp-0.1.53/AutoMLApp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoMLApp
-Version: 0.1.52
+Version: 0.1.53
 Summary: An automated machine learning application designed for efficient model training, evaluation, and hyperparameter tuning.
 Author: Shivam Nikam
 Author-email: shivam.nikam@think360.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `automlapp-0.1.52/AutoMLApp.egg-info/SOURCES.txt` & `automlapp-0.1.53/AutoMLApp.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,11 +16,10 @@
 automlapp/modules/data_preprocessing.py
 automlapp/modules/data_summarization.py
 automlapp/modules/data_visualization.py
 automlapp/modules/data_woeiv.py
 automlapp/modules/hyperparameter_tuning.py
 automlapp/modules/model_evaluation.py
 automlapp/modules/model_training.py
-automlapp/modules/train_user_params.py
 automlapp/utils/__init__.py
 automlapp/utils/print_utils.py
 automlapp/utils/streamlit_utils.py
```

### Comparing `automlapp-0.1.52/LICENSE` & `automlapp-0.1.53/LICENSE`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.52/PKG-INFO` & `automlapp-0.1.53/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoMLApp
-Version: 0.1.52
+Version: 0.1.53
 Summary: An automated machine learning application designed for efficient model training, evaluation, and hyperparameter tuning.
 Author: Shivam Nikam
 Author-email: shivam.nikam@think360.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `automlapp-0.1.52/README.md` & `automlapp-0.1.53/README.md`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.52/automlapp/app.py` & `automlapp-0.1.53/automlapp/app.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.52/automlapp/modules/data_cleaning.py` & `automlapp-0.1.53/automlapp/modules/data_cleaning.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import pandas as pd
-from utils.streamlit_utils import hide_icons, remove_whitespaces, st
+from ..utils.streamlit_utils import hide_icons, remove_whitespaces, st
 
 class DataCleaning:
     def __init__(_self, df):
         _self.df = df.copy()
 
     def detect_outliers(_self, lower_percentile=5, upper_percentile=95):
         lower_bound, upper_bound = _self.df.quantile(lower_percentile/100), _self.df.quantile(upper_percentile/100)
```

### Comparing `automlapp-0.1.52/automlapp/modules/data_input.py` & `automlapp-0.1.53/automlapp/modules/data_input.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from utils.streamlit_utils import st
+from ..utils.streamlit_utils import st
 import os, io
 import pandas as pd
 import zipfile
 
 class DataInput:
     def __init__(_self, uploaded_file, key_suffix = None):
         _self.uploaded_file = uploaded_file
```

### Comparing `automlapp-0.1.52/automlapp/modules/data_preprocessing.py` & `automlapp-0.1.53/automlapp/modules/data_preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from utils.streamlit_utils import st
+from ..utils.streamlit_utils import st
 import pandas as pd
 import numpy as np
 from scipy.stats import skew, boxcox
 from imblearn.over_sampling import RandomOverSampler
 from imblearn.under_sampling import RandomUnderSampler
 from imblearn.combine import SMOTEENN
 from sklearn.preprocessing import StandardScaler, MinMaxScaler, RobustScaler
```

### Comparing `automlapp-0.1.52/automlapp/modules/data_summarization.py` & `automlapp-0.1.53/automlapp/modules/data_summarization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from utils.streamlit_utils import st
+from ..utils.streamlit_utils import st
 
 class DataSummarization:
     def __init__(_self, df):
         _self.df = df
 
     def summarize(_self):
         if _self.df is not None:
```

### Comparing `automlapp-0.1.52/automlapp/modules/data_visualization.py` & `automlapp-0.1.53/automlapp/modules/data_visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from utils.streamlit_utils import st
+from ..utils.streamlit_utils import st
 import plotly.express as px
 
 class DataVisualization:
     def __init__(self, df):
         self.df = df
         self.plot_colors = px.colors.sequential.YlOrRd[::-2]
```

### Comparing `automlapp-0.1.52/automlapp/modules/data_woeiv.py` & `automlapp-0.1.53/automlapp/modules/data_woeiv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from utils.streamlit_utils import st
+from ..utils.streamlit_utils import st
 import pandas as pd
 import numpy as np
 import scorecardpy as sc
 import io
 
 class DataWOEIV:
     def __init__(_self, df):
```

### Comparing `automlapp-0.1.52/automlapp/modules/hyperparameter_tuning.py` & `automlapp-0.1.53/automlapp/modules/hyperparameter_tuning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from utils.streamlit_utils import st
+from ..utils.streamlit_utils import st
 import pandas as pd
 from sklearn.linear_model import LogisticRegression
 from sklearn.tree import DecisionTreeClassifier
 from sklearn.ensemble import RandomForestClassifier, AdaBoostClassifier
 from xgboost import XGBClassifier
 from lightgbm import LGBMClassifier
 from sklearn.model_selection import GridSearchCV, RandomizedSearchCV
```

### Comparing `automlapp-0.1.52/automlapp/modules/model_evaluation.py` & `automlapp-0.1.53/automlapp/modules/model_evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from utils.streamlit_utils import st
+from ..utils.streamlit_utils import st
 import pandas as pd
 import numpy as np
 import plotly.express as px
 from sklearn.metrics import confusion_matrix, accuracy_score, confusion_matrix, precision_score, recall_score, f1_score, auc, roc_curve
 from sklearn.metrics import ConfusionMatrixDisplay
 
 class ModelEvaluation:
```

### Comparing `automlapp-0.1.52/automlapp/modules/model_training.py` & `automlapp-0.1.53/automlapp/modules/model_training.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from utils.streamlit_utils import st
+from ..utils.streamlit_utils import st
 import pandas as pd
 from sklearn.linear_model import LogisticRegression
 from sklearn.tree import DecisionTreeClassifier
 from sklearn.ensemble import RandomForestClassifier, AdaBoostClassifier
 from xgboost import XGBClassifier
 from lightgbm import LGBMClassifier
```

### Comparing `automlapp-0.1.52/automlapp/utils/streamlit_utils.py` & `automlapp-0.1.53/automlapp/utils/streamlit_utils.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.52/setup.py` & `automlapp-0.1.53/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="AutoMLApp",
-    version="0.1.52",
+    version="0.1.53",
     author="Shivam Nikam",
     author_email="shivam.nikam@think360.ai",
     description="An automated machine learning application designed for efficient model training, evaluation, and hyperparameter tuning.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     #url="https://github.com/YourGithub/AutoMLApp",
     packages=find_packages(),
```

