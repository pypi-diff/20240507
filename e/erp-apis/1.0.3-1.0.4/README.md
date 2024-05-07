# Comparing `tmp/erp_apis-1.0.3-py3-none-any.whl.zip` & `tmp/erp_apis-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -4,12 +4,12 @@
 -rw-rw-rw-  2.0 fat      141 b- defN 24-Apr-29 06:37 erp_apis/apis/__init__.py
 -rw-rw-rw-  2.0 fat     2566 b- defN 24-May-07 01:25 erp_apis/apis/afterSales.py
 -rw-rw-rw-  2.0 fat     1517 b- defN 24-May-07 02:48 erp_apis/apis/goods.py
 -rw-rw-rw-  2.0 fat     1010 b- defN 24-Apr-30 10:14 erp_apis/apis/inventory.py
 -rw-rw-rw-  2.0 fat     3680 b- defN 24-May-05 08:01 erp_apis/apis/order.py
 -rw-rw-rw-  2.0 fat     1953 b- defN 24-May-07 02:48 erp_apis/apis/test.py
 -rw-rw-rw-  2.0 fat      777 b- defN 24-Apr-30 11:33 erp_apis/apis/user.py
--rw-rw-rw-  2.0 fat     1580 b- defN 24-May-07 02:49 erp_apis-1.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 02:49 erp_apis-1.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 24-May-07 02:49 erp_apis-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1013 b- defN 24-May-07 02:49 erp_apis-1.0.3.dist-info/RECORD
+-rw-rw-rw-  2.0 fat     1580 b- defN 24-May-07 03:01 erp_apis-1.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 03:01 erp_apis-1.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 24-May-07 03:01 erp_apis-1.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1013 b- defN 24-May-07 03:01 erp_apis-1.0.4.dist-info/RECORD
 13 files, 18247 bytes uncompressed, 7923 bytes compressed:  56.6%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: erp_apis/apis/test.py
 Comment: 
 
 Filename: erp_apis/apis/user.py
 Comment: 
 
-Filename: erp_apis-1.0.3.dist-info/METADATA
+Filename: erp_apis-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: erp_apis-1.0.3.dist-info/WHEEL
+Filename: erp_apis-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: erp_apis-1.0.3.dist-info/top_level.txt
+Filename: erp_apis-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: erp_apis-1.0.3.dist-info/RECORD
+Filename: erp_apis-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `erp_apis-1.0.3.dist-info/METADATA` & `erp_apis-1.0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erp-apis
-Version: 1.0.3
+Version: 1.0.4
 Summary: erp_apis
 Home-page: https://gitee.com/li_fucheng/erp_sdk_python
 Author: 李福成
 Author-email: lfct@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://gitee.com/li_fucheng/erp_sdk_python/issues
 Project-URL: Documentation, https://gitee.com/li_fucheng/erp_sdk_python
```

## Comparing `erp_apis-1.0.3.dist-info/RECORD` & `erp_apis-1.0.4.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -3,11 +3,11 @@
 erp_apis/apis/__init__.py,sha256=mP4VQl6EDhiYFTvOeAO7G4N6a5xtWXrXG5gRyW4HfQg,141
 erp_apis/apis/afterSales.py,sha256=zLQPY_P4D7rot_NxkSk845pBru1qGfbxOdbDo4qf84o,2566
 erp_apis/apis/goods.py,sha256=JggkrGbgSeVZQ1N9I56xBIs1LqBZVVssUpC4-CTF_Qk,1517
 erp_apis/apis/inventory.py,sha256=sLPIvOdKHIdfC0lAxtoK3ey8-n5OEbUsjFPX-_c6yY4,1010
 erp_apis/apis/order.py,sha256=6Z9HEfYeomktbIqGmQgEFYADa-XkBZEcVIeR-eLudco,3680
 erp_apis/apis/test.py,sha256=7xg6YNGhwp6UJiXCkL_KKnILyy9-WotbUnoYvHl8sp0,1953
 erp_apis/apis/user.py,sha256=Wcqqb8YWG7XsWWaTzSmF-N4FDO98L_Z4ECXSeWhKf_8,777
-erp_apis-1.0.3.dist-info/METADATA,sha256=3saNeaxT8ucgiahQTpdUzN3ptveCJmgUaehSgSZNxKk,1580
-erp_apis-1.0.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-erp_apis-1.0.3.dist-info/top_level.txt,sha256=i_r33fdpLh_LFdzZEdgEk4155_iw3lEof10yhsc5_MA,23
-erp_apis-1.0.3.dist-info/RECORD,,
+erp_apis-1.0.4.dist-info/METADATA,sha256=874D-ogXx8lG38CuHjuBbubWG_-GAgDjFXyTold1PZ8,1580
+erp_apis-1.0.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+erp_apis-1.0.4.dist-info/top_level.txt,sha256=i_r33fdpLh_LFdzZEdgEk4155_iw3lEof10yhsc5_MA,23
+erp_apis-1.0.4.dist-info/RECORD,,
```

