# Comparing `tmp/new_dt_algorithm-0.5.tar.gz` & `tmp/new_dt_algorithm-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new_dt_algorithm-0.5.tar", last modified: Tue May  7 12:00:30 2024, max compression
+gzip compressed data, was "new_dt_algorithm-0.6.tar", last modified: Tue May  7 12:09:41 2024, max compression
```

## Comparing `new_dt_algorithm-0.5.tar` & `new_dt_algorithm-0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 12:00:30.550313 new_dt_algorithm-0.5/
--rw-rw-rw-   0        0        0      214 2024-05-07 12:00:30.550313 new_dt_algorithm-0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-07 11:26:56.000000 new_dt_algorithm-0.5/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 12:00:30.550313 new_dt_algorithm-0.5/new_dt_algorithm.egg-info/
--rw-rw-rw-   0        0        0      214 2024-05-07 12:00:30.000000 new_dt_algorithm-0.5/new_dt_algorithm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-05-07 12:00:30.000000 new_dt_algorithm-0.5/new_dt_algorithm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 12:00:30.000000 new_dt_algorithm-0.5/new_dt_algorithm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-07 12:00:30.000000 new_dt_algorithm-0.5/new_dt_algorithm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    21648 2024-05-07 11:56:18.000000 new_dt_algorithm-0.5/new_dt_algorithm.py
--rw-rw-rw-   0        0        0       42 2024-05-07 12:00:30.550313 new_dt_algorithm-0.5/setup.cfg
--rw-rw-rw-   0        0        0      443 2024-05-07 11:59:49.000000 new_dt_algorithm-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:09:41.478942 new_dt_algorithm-0.6/
+-rw-rw-rw-   0        0        0      214 2024-05-07 12:09:41.478942 new_dt_algorithm-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:26:56.000000 new_dt_algorithm-0.6/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:09:41.478942 new_dt_algorithm-0.6/new_dt_algorithm.egg-info/
+-rw-rw-rw-   0        0        0      214 2024-05-07 12:09:41.000000 new_dt_algorithm-0.6/new_dt_algorithm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-07 12:09:41.000000 new_dt_algorithm-0.6/new_dt_algorithm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 12:09:41.000000 new_dt_algorithm-0.6/new_dt_algorithm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-07 12:09:41.000000 new_dt_algorithm-0.6/new_dt_algorithm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    21662 2024-05-07 12:08:49.000000 new_dt_algorithm-0.6/new_dt_algorithm.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 12:09:41.478942 new_dt_algorithm-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      443 2024-05-07 12:09:25.000000 new_dt_algorithm-0.6/setup.py
```

### Comparing `new_dt_algorithm-0.5/new_dt_algorithm.py` & `new_dt_algorithm-0.6/new_dt_algorithm.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,28 +419,28 @@
         if self.model is None:
             print('Please train the model first.')
         else:
             # Performance evaluation on training data
             import pandas as pd
             import matplotlib.pyplot as plt
             from sklearn.tree import plot_tree
-            train_data = self.train_data
+            train_data = self.train_data.copy()
             train_data['predict_prob'] = self.model.predict_proba(train_data.drop([self.Target], axis=1))[:, 1]
             train_data['dummy'] = 1
 
             def custom_sum_product(group):
                 return pd.Series({'Pop%': group['dummy'].sum() / train_data.shape[0],
                                   'bad_rate': (group[self.Target].sum() / group['dummy'].sum())})
 
             train_result = train_data.groupby('predict_prob').apply(custom_sum_product)
             print("Training Data:")
             print(train_result)
 
             # Performance evaluation on test data
-            test_data = self.test_data
+            test_data = self.test_data.copy()
             test_data['predict_prob'] = self.model.predict_proba(test_data.drop([self.Target], axis=1))[:, 1]
             test_data['dummy'] = 1
 
             def custom_sum_product(group):
                 return pd.Series({'Pop%': group['dummy'].sum() / test_data.shape[0],
                                   'bad_rate': (group[self.Target].sum() / group['dummy'].sum())})
```

