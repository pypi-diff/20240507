# Comparing `tmp/sparkhistogram-0.3.tar.gz` & `tmp/sparkhistogram-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkhistogram-0.3.tar", last modified: Fri May 20 12:07:39 2022, max compression
+gzip compressed data, was "sparkhistogram-0.4.tar", last modified: Tue May  7 15:14:59 2024, max compression
```

## Comparing `sparkhistogram-0.3.tar` & `sparkhistogram-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2022-05-20 12:07:39.180108 sparkhistogram-0.3/
--rw-r--r--   0 luca      (1000) luca      (1000)     3028 2022-05-20 12:07:39.180108 sparkhistogram-0.3/PKG-INFO
--rw-r--r--   0 luca      (1000) luca      (1000)       67 2022-05-20 12:07:39.180108 sparkhistogram-0.3/setup.cfg
--rw-r--r--   0 luca      (1000) luca      (1000)     3316 2022-05-19 19:55:14.000000 sparkhistogram-0.3/setup.py
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2022-05-20 12:07:39.179108 sparkhistogram-0.3/sparkhistogram/
--rw-r--r--   0 luca      (1000) luca      (1000)      141 2022-05-17 12:24:11.000000 sparkhistogram-0.3/sparkhistogram/__init__.py
--rw-r--r--   0 luca      (1000) luca      (1000)     4004 2022-05-20 12:04:16.000000 sparkhistogram-0.3/sparkhistogram/histogram.py
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2022-05-20 12:07:39.179108 sparkhistogram-0.3/sparkhistogram.egg-info/
--rw-r--r--   0 luca      (1000) luca      (1000)     3028 2022-05-20 12:07:38.000000 sparkhistogram-0.3/sparkhistogram.egg-info/PKG-INFO
--rw-r--r--   0 luca      (1000) luca      (1000)      262 2022-05-20 12:07:39.000000 sparkhistogram-0.3/sparkhistogram.egg-info/SOURCES.txt
--rw-r--r--   0 luca      (1000) luca      (1000)        1 2022-05-20 12:07:38.000000 sparkhistogram-0.3/sparkhistogram.egg-info/dependency_links.txt
--rw-r--r--   0 luca      (1000) luca      (1000)        1 2022-05-20 12:07:38.000000 sparkhistogram-0.3/sparkhistogram.egg-info/not-zip-safe
--rw-r--r--   0 luca      (1000) luca      (1000)       15 2022-05-20 12:07:39.000000 sparkhistogram-0.3/sparkhistogram.egg-info/top_level.txt
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-07 15:14:59.218605 sparkhistogram-0.4/
+-rw-r--r--   0 luca      (1000) luca      (1000)     3008 2024-05-07 15:14:59.218605 sparkhistogram-0.4/PKG-INFO
+-rw-r--r--   0 luca      (1000) luca      (1000)       67 2024-05-07 15:14:59.218605 sparkhistogram-0.4/setup.cfg
+-rw-r--r--   0 luca      (1000) luca      (1000)     3316 2024-05-07 15:13:10.000000 sparkhistogram-0.4/setup.py
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-07 15:14:59.217605 sparkhistogram-0.4/sparkhistogram/
+-rw-r--r--   0 luca      (1000) luca      (1000)      141 2022-05-17 12:24:11.000000 sparkhistogram-0.4/sparkhistogram/__init__.py
+-rw-r--r--   0 luca      (1000) luca      (1000)     4891 2024-05-07 15:13:10.000000 sparkhistogram-0.4/sparkhistogram/histogram.py
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-07 15:14:59.218605 sparkhistogram-0.4/sparkhistogram.egg-info/
+-rw-r--r--   0 luca      (1000) luca      (1000)     3008 2024-05-07 15:14:59.000000 sparkhistogram-0.4/sparkhistogram.egg-info/PKG-INFO
+-rw-r--r--   0 luca      (1000) luca      (1000)      262 2024-05-07 15:14:59.000000 sparkhistogram-0.4/sparkhistogram.egg-info/SOURCES.txt
+-rw-r--r--   0 luca      (1000) luca      (1000)        1 2024-05-07 15:14:59.000000 sparkhistogram-0.4/sparkhistogram.egg-info/dependency_links.txt
+-rw-r--r--   0 luca      (1000) luca      (1000)        1 2024-05-07 15:14:59.000000 sparkhistogram-0.4/sparkhistogram.egg-info/not-zip-safe
+-rw-r--r--   0 luca      (1000) luca      (1000)       15 2024-05-07 15:14:59.000000 sparkhistogram-0.4/sparkhistogram.egg-info/top_level.txt
```

### Comparing `sparkhistogram-0.3/PKG-INFO` & `sparkhistogram-0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: sparkhistogram
-Version: 0.3
+Version: 0.4
 Summary: Sparkhistogram contains helper functions for generating data histograms with the Spark DataFrame API.
 Home-page: https://github.com/LucaCanali/Miscellaneous/blob/master/Spark_Notes/Spark_DataFrame_Histograms.md
 Author: Luca Canali
 Author-email: luca.canali@cern.ch
 License: Apache License, Version 2.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -81,9 +80,7 @@
 |    10| 75.0|   16|
 |    11| 85.0|    7|
 +------+-----+-----+
 ```
 
 More details and notebooks with matplotlib visualization of the histograms at:  
 https://github.com/LucaCanali/Miscellaneous/blob/master/Spark_Notes/Spark_DataFrame_Histograms.md
-
-
```

### Comparing `sparkhistogram-0.3/setup.py` & `sparkhistogram-0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 ```
 
 More details and notebooks with matplotlib visualization of the histograms at:  
 https://github.com/LucaCanali/Miscellaneous/blob/master/Spark_Notes/Spark_DataFrame_Histograms.md
 """
 
 setup(name='sparkhistogram',
-    version='0.3',
+    version='0.4',
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Luca Canali',
     author_email='luca.canali@cern.ch',
     url='https://github.com/LucaCanali/Miscellaneous/blob/master/Spark_Notes/Spark_DataFrame_Histograms.md',
     license='Apache License, Version 2.0',
```

### Comparing `sparkhistogram-0.3/sparkhistogram/histogram.py` & `sparkhistogram-0.4/sparkhistogram/histogram.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,28 +21,40 @@
         
         Output DataFrame
         ----------------
         bucket: the bucket number, range from 1 to bins (included)
         value: midpoint value of the given bucket
         count: number of values in the bucket        
     """
+    # Compute the step size for the histogram
     step = (max_val - min_val) / bins
-    # this will be used to fill in for missing buckets, i.e. buckets with no corresponding values
+
+    # Get the Spark Session handle
     spark = SparkSession.getActiveSession()
-    df_buckets = spark.sql(f"select id+1 as bucket from range({bins})")
-    histdf = (df
-              .selectExpr(f"width_bucket({value_col}, {min_val}, {max_val}, {bins}) as bucket")
-              .groupBy("bucket")
-              .count()
-              .join(df_buckets, "bucket", "right_outer") # add missing buckets and remove buckets out of range
-              .selectExpr("bucket", f"{min_val} + (bucket - 0.5) * {step} as value",  # use center value of the buckets
-                          "nvl(count, 0) as count") # buckets with no values will have a count of 0
-              .orderBy("bucket")
-             )
-    return histdf
+
+    # df_buckets is the range of {bins} buckets as requested by the user
+    # It will be used to fill in for missing buckets, i.e. buckets with no corresponding values
+    df_buckets = spark.range(bins).selectExpr("id + 1 as bucket")
+
+    # Group user data into buckets and count their population count
+    df_grouped = (df
+                   .selectExpr(f"width_bucket({value_col}, {min_val}, {max_val}, {bins}) as bucket")
+                   .groupBy("bucket")
+                   .count()
+                 )
+
+    # Join df_buckets with the grouped data to fill in missing buckets
+    df_hist = (df_buckets # note this will be typically broadcasted, the order of the join is important
+               .join(df_grouped, "bucket", "left_outer") # add missing buckets and remove buckets out of range
+               .selectExpr("bucket", f"{min_val} + (bucket - 0.5) * {step} as value",  # use center value of the buckets
+                           "nvl(count, 0) as count") # buckets with no values will have a count of 0
+               .orderBy("bucket")
+              )
+
+    return df_hist
 
 
 def computeWeightedHistogram(df: "DataFrame", value_col: str, weight_col: str,
                              min_val: float, max_val: float, bins: int) -> "DataFrame":
     """ This is a dataframe function to compute the weighted histogram of a DataFrame column.
         A weighted histogram is a generalization of a frequency histogram.
 
@@ -58,23 +70,35 @@
         max_val: maximum value in the histogram
         bins: number of histogram buckets to compute
 
         Output DataFrame
         ----------------
         bucket: the bucket number, range from 1 to bins (included)
         value: midpoint value of the given bucket
-        count: weighted sum of the number of values in the bucket
+        weighted_sum: weighted sum of the number of values in the bucket
     """
+    # Compute the step size for the histogram
     step = (max_val - min_val) / bins
-    # this will be used to fill in for missing buckets, i.e. buckets with no corresponding values
+
+    # Get the Spark Session handle
     spark = SparkSession.getActiveSession()
-    df_buckets = spark.sql(f"select id+1 as bucket from range({bins})")
-    histdf = (df
-              .selectExpr(f"width_bucket({value_col}, {min_val}, {max_val}, {bins}) as bucket", f"{weight_col}")
-              .groupBy("bucket")
-              .agg(sum(f"{weight_col}").alias("weighted_sum"))  # sum the weights on the weight_col
-              .join(df_buckets, "bucket", "right_outer") # add missing buckets and remove buckets out of range
-              .selectExpr("bucket", f"{min_val} + (bucket - 0.5) * {step} as value",  # use center value of the buckets
-                          "nvl(weighted_sum, 0) as weighted_sum") # buckets with no values will have a sum of 0
-              .orderBy("bucket")
-              )
-    return histdf
+
+    # df_buckets is the range of {bins} buckets as requested by the user
+    # It will be used to fill in for missing buckets, i.e. buckets with no corresponding values
+    df_buckets = spark.range(bins).selectExpr("id + 1 as bucket")
+
+    # Group user data into buckets and compute a weighted sum of the values
+    df_grouped = (df
+                  .selectExpr(f"width_bucket({value_col}, {min_val}, {max_val}, {bins}) as bucket", f"{weight_col}")
+                  .groupBy("bucket")
+                  .agg(sum(f"{weight_col}").alias("weighted_sum"))  # sum the weights on the weight_col
+                 )
+
+    # Join df_buckets with the grouped data to fill in missing buckets
+    df_hist = (df_buckets # note this will be typically broadcasted, the order of the join is important
+               .join(df_grouped, "bucket", "left_outer") # add missing buckets and remove buckets out of range
+               .selectExpr("bucket", f"{min_val} + (bucket - 0.5) * {step} as value",  # use center value of the buckets
+                           "nvl(weighted_sum, 0) as weighted_sum")  # buckets with no values will have a sum of 0
+               .orderBy("bucket")
+               )
+
+    return df_hist
```

### Comparing `sparkhistogram-0.3/sparkhistogram.egg-info/PKG-INFO` & `sparkhistogram-0.4/sparkhistogram.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: sparkhistogram
-Version: 0.3
+Version: 0.4
 Summary: Sparkhistogram contains helper functions for generating data histograms with the Spark DataFrame API.
 Home-page: https://github.com/LucaCanali/Miscellaneous/blob/master/Spark_Notes/Spark_DataFrame_Histograms.md
 Author: Luca Canali
 Author-email: luca.canali@cern.ch
 License: Apache License, Version 2.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -81,9 +80,7 @@
 |    10| 75.0|   16|
 |    11| 85.0|    7|
 +------+-----+-----+
 ```
 
 More details and notebooks with matplotlib visualization of the histograms at:  
 https://github.com/LucaCanali/Miscellaneous/blob/master/Spark_Notes/Spark_DataFrame_Histograms.md
-
-
```

