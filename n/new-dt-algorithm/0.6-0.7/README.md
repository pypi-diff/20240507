# Comparing `tmp/new_dt_algorithm-0.6.tar.gz` & `tmp/new_dt_algorithm-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new_dt_algorithm-0.6.tar", last modified: Tue May  7 12:09:41 2024, max compression
+gzip compressed data, was "new_dt_algorithm-0.7.tar", last modified: Tue May  7 12:18:49 2024, max compression
```

## Comparing `new_dt_algorithm-0.6.tar` & `new_dt_algorithm-0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 12:09:41.478942 new_dt_algorithm-0.6/
--rw-rw-rw-   0        0        0      214 2024-05-07 12:09:41.478942 new_dt_algorithm-0.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-07 11:26:56.000000 new_dt_algorithm-0.6/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 12:09:41.478942 new_dt_algorithm-0.6/new_dt_algorithm.egg-info/
--rw-rw-rw-   0        0        0      214 2024-05-07 12:09:41.000000 new_dt_algorithm-0.6/new_dt_algorithm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-05-07 12:09:41.000000 new_dt_algorithm-0.6/new_dt_algorithm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 12:09:41.000000 new_dt_algorithm-0.6/new_dt_algorithm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-07 12:09:41.000000 new_dt_algorithm-0.6/new_dt_algorithm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    21662 2024-05-07 12:08:49.000000 new_dt_algorithm-0.6/new_dt_algorithm.py
--rw-rw-rw-   0        0        0       42 2024-05-07 12:09:41.478942 new_dt_algorithm-0.6/setup.cfg
--rw-rw-rw-   0        0        0      443 2024-05-07 12:09:25.000000 new_dt_algorithm-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:18:49.632838 new_dt_algorithm-0.7/
+-rw-rw-rw-   0        0        0      214 2024-05-07 12:18:49.632838 new_dt_algorithm-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:26:56.000000 new_dt_algorithm-0.7/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:18:49.632838 new_dt_algorithm-0.7/new_dt_algorithm.egg-info/
+-rw-rw-rw-   0        0        0      214 2024-05-07 12:18:49.000000 new_dt_algorithm-0.7/new_dt_algorithm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-07 12:18:49.000000 new_dt_algorithm-0.7/new_dt_algorithm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 12:18:49.000000 new_dt_algorithm-0.7/new_dt_algorithm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-07 12:18:49.000000 new_dt_algorithm-0.7/new_dt_algorithm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    21851 2024-05-07 12:18:08.000000 new_dt_algorithm-0.7/new_dt_algorithm.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 12:18:49.632838 new_dt_algorithm-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      443 2024-05-07 12:18:41.000000 new_dt_algorithm-0.7/setup.py
```

### Comparing `new_dt_algorithm-0.6/new_dt_algorithm.py` & `new_dt_algorithm-0.7/new_dt_algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -328,16 +328,19 @@
             def custom_sum_product(group):
                 return pd.Series({'Pop%': group['dummy'].sum() / X_t_test.shape[0],
                                   'bad_rate': (group[self.Target].sum() / group['dummy'].sum())})
 
             X_t_test = X_t_test.groupby('predict_prob').apply(custom_sum_product).reset_index()
 
             # Calculate bad difference value
-            bad_diff = abs((X_t_test['predict_prob'] - X_t_test['bad_rate']) * X_t_test['Pop%']).sum()
-            bad_diff_value.append(bad_diff)
+            if (X_t_test.reset_index()['Pop%'].max()<=max_pop_per)&(X_t_test.reset_index()['Pop%'].min()>=min_pop_per):
+                bad_diff = abs((X_t_test['predict_prob'] - X_t_test['bad_rate']) * X_t_test['Pop%']).sum()
+                bad_diff_value.append(bad_diff)
+            else:
+                bad_diff_value.append(100)
             random_st.append(i)
 
         # Find the random state with the lowest bad difference value
         results = pd.DataFrame({'random_state': random_st, 'bad_diff': bad_diff_value})
         results = results[results['bad_diff'] == results['bad_diff'].min()]
 
         # Handle multiple best results
```

