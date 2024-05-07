# Comparing `tmp/increff_runner-3.2.1-py3-none-any.whl.zip` & `tmp/increff_runner-3.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 13295 bytes, number of entries: 16
+Zip file size: 13321 bytes, number of entries: 16
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-05 05:14 increff_runner/__init__.py
 -rw-r--r--  2.0 unx     9762 b- defN 24-Apr-30 04:29 increff_runner/function.py
 -rw-r--r--  2.0 unx     4143 b- defN 24-Feb-22 04:41 increff_runner/commons/algo_block_downloader.py
--rw-r--r--  2.0 unx     2993 b- defN 24-May-03 10:36 increff_runner/commons/callback_helper.py
+-rw-r--r--  2.0 unx     3105 b- defN 24-May-07 02:58 increff_runner/commons/callback_helper.py
 -rw-r--r--  2.0 unx      351 b- defN 24-Feb-15 07:21 increff_runner/commons/constants.py
 -rw-r--r--  2.0 unx     3520 b- defN 24-May-03 10:42 increff_runner/commons/db_helper.py
 -rw-r--r--  2.0 unx      905 b- defN 24-Feb-22 04:41 increff_runner/commons/db_service.py
 -rw-r--r--  2.0 unx      349 b- defN 24-Apr-30 04:29 increff_runner/commons/event_helper.py
 -rw-r--r--  2.0 unx     8405 b- defN 24-May-03 10:38 increff_runner/commons/graphdb_helper.py
 -rw-r--r--  2.0 unx     4177 b- defN 24-May-02 06:39 increff_runner/commons/mse_helper.py
 -rw-r--r--  2.0 unx      687 b- defN 24-Feb-22 04:41 increff_runner/commons/setup.py
 -rw-r--r--  2.0 unx     2104 b- defN 24-Feb-22 04:41 increff_runner/commons/utils.py
--rw-r--r--  2.0 unx      612 b- defN 24-May-03 10:51 increff_runner-3.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-03 10:51 increff_runner-3.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 24-May-03 10:51 increff_runner-3.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1424 b- defN 24-May-03 10:51 increff_runner-3.2.1.dist-info/RECORD
-16 files, 39539 bytes uncompressed, 10901 bytes compressed:  72.4%
+-rw-r--r--  2.0 unx      612 b- defN 24-May-07 03:00 increff_runner-3.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-07 03:00 increff_runner-3.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 24-May-07 03:00 increff_runner-3.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1424 b- defN 24-May-07 03:00 increff_runner-3.2.2.dist-info/RECORD
+16 files, 39651 bytes uncompressed, 10927 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: increff_runner/commons/setup.py
 Comment: 
 
 Filename: increff_runner/commons/utils.py
 Comment: 
 
-Filename: increff_runner-3.2.1.dist-info/METADATA
+Filename: increff_runner-3.2.2.dist-info/METADATA
 Comment: 
 
-Filename: increff_runner-3.2.1.dist-info/WHEEL
+Filename: increff_runner-3.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: increff_runner-3.2.1.dist-info/top_level.txt
+Filename: increff_runner-3.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: increff_runner-3.2.1.dist-info/RECORD
+Filename: increff_runner-3.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## increff_runner/commons/callback_helper.py

```diff
@@ -65,10 +65,12 @@
     }
     add_info_logs(job["id"], f" failure message -> {str(data)}")
     job["webhook_status"] = 400
     update_job(job)
     
     # TODO @jaynit ensure that they are not moved to Success again #cr1_unni
     # TODO @jaynit kill the kube jobs also if it is running #cr1_unni
+
+    change_status_of_task_node(job["data"]["algo_name"], job["data"]["task_id"], job["data"]["level"], FAILED)
     mark_dependant_as_failed(task_id,job["data"]["webHookUri"])
     response = requests.put(url, params=data,headers=headers)
     add_info_logs(job["id"], f"Failure Webhook Response -> {response.status_code}")
```

## Comparing `increff_runner-3.2.1.dist-info/METADATA` & `increff_runner-3.2.2.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: increff-runner
-Version: 3.2.1
+Version: 3.2.2
 Summary: Algo Runner For Increff CaaS
 Author: Jaynit Patel
 Author-email: jaynitpatel11062001@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: pytz ==2023.3.post1
 Requires-Dist: requests ==2.31.0
 Requires-Dist: azure-functions ==1.12.0
```

## Comparing `increff_runner-3.2.1.dist-info/RECORD` & `increff_runner-3.2.2.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 increff_runner/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 increff_runner/function.py,sha256=Kk2mSezi3ypvYkjbSrMtxXoO5qwc29uYHAoTk_-W_Yo,9762
 increff_runner/commons/algo_block_downloader.py,sha256=JSZLYpIuWhybRD13sHPu_05X4KoeMApa5qELLkqA9R4,4143
-increff_runner/commons/callback_helper.py,sha256=7cLwpZxIICos6soH7gQWOr4WCjiE-ywwnB88QSpjWek,2993
+increff_runner/commons/callback_helper.py,sha256=G36Y_HjoRpZdGLgdUveL6H-nyyPuWsdLtmRZRg7rYa8,3105
 increff_runner/commons/constants.py,sha256=dJRawPQQduTe1BqN6SrLYYpzI5bVqS6AbuYwj6Qa6is,351
 increff_runner/commons/db_helper.py,sha256=CmLWncHnvo0AS_cVlC5m6_FqwPLeqBvpEI40a7lyJKY,3520
 increff_runner/commons/db_service.py,sha256=5PtU_AQCwm5FVmRXjJprysNoIy_vKt06vN1IlnxuH-c,905
 increff_runner/commons/event_helper.py,sha256=MN1XR6yielNYXLbLxi3uuiDyXZ-lmVKszL9DOL4swBY,349
 increff_runner/commons/graphdb_helper.py,sha256=c6cnD2He-xMer4dejiFKvAvM1qsbPlDoNqNKkz1mtZE,8405
 increff_runner/commons/mse_helper.py,sha256=m2JNRs72goahs3s3OSwwWvsoP_SWjRbOPfW-MEBP4lA,4177
 increff_runner/commons/setup.py,sha256=iwg58X1DKaSP8hKlXLvH5OXSEW8N_UuRMDb2CocaAfY,687
 increff_runner/commons/utils.py,sha256=PUKWRMYzTTWK7pTK2S5DM0szru4zGmmVKfPpXhnmPUM,2104
-increff_runner-3.2.1.dist-info/METADATA,sha256=qWOFyjxCIBBmZJ8Xd0BEA05Hfhq5m8UIsrBNzpRgLwE,612
-increff_runner-3.2.1.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-increff_runner-3.2.1.dist-info/top_level.txt,sha256=pL8Rxzd3TVe5jhZdPB1tmORoBiwmdtiDgfNAvJtCl1s,15
-increff_runner-3.2.1.dist-info/RECORD,,
+increff_runner-3.2.2.dist-info/METADATA,sha256=oL6QtcJFuELnGRsn4iAV5BRs1EL0bALCdwRbBw0gvDw,612
+increff_runner-3.2.2.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+increff_runner-3.2.2.dist-info/top_level.txt,sha256=pL8Rxzd3TVe5jhZdPB1tmORoBiwmdtiDgfNAvJtCl1s,15
+increff_runner-3.2.2.dist-info/RECORD,,
```

