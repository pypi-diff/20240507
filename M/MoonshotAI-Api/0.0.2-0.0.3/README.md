# Comparing `tmp/MoonshotAI_Api-0.0.2.tar.gz` & `tmp/MoonshotAI_Api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MoonshotAI_Api-0.0.2.tar", last modified: Thu May  2 13:13:13 2024, max compression
+gzip compressed data, was "MoonshotAI_Api-0.0.3.tar", last modified: Tue May  7 07:17:52 2024, max compression
```

## Comparing `MoonshotAI_Api-0.0.2.tar` & `MoonshotAI_Api-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 tomerefroni   (501) staff       (20)        0 2024-05-02 13:13:13.494614 MoonshotAI_Api-0.0.2/
-drwxr-xr-x   0 tomerefroni   (501) staff       (20)        0 2024-05-02 13:13:13.488815 MoonshotAI_Api-0.0.2/MoonshotAI_Api/
--rw-r--r--   0 tomerefroni   (501) staff       (20)     1066 2024-04-22 09:05:33.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api/LICENSE
--rw-r--r--   0 tomerefroni   (501) staff       (20)       13 2024-04-08 13:04:59.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api/README.md
--rw-r--r--   0 tomerefroni   (501) staff       (20)        0 2022-07-04 11:50:12.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api/__init__.py
--rw-r--r--   0 tomerefroni   (501) staff       (20)     5352 2024-04-24 12:26:17.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api/ltv_client.py
-drwxr-xr-x   0 tomerefroni   (501) staff       (20)        0 2024-05-02 13:13:13.493091 MoonshotAI_Api-0.0.2/MoonshotAI_Api/utils/
--rw-r--r--   0 tomerefroni   (501) staff       (20)      652 2024-05-02 10:52:05.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api/utils/consts.py
--rw-r--r--   0 tomerefroni   (501) staff       (20)       88 2024-04-21 08:43:57.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api/utils/output_enum.py
--rw-r--r--   0 tomerefroni   (501) staff       (20)     1032 2024-04-21 09:33:40.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api/utils/utils.py
-drwxr-xr-x   0 tomerefroni   (501) staff       (20)        0 2024-05-02 13:13:13.491562 MoonshotAI_Api-0.0.2/MoonshotAI_Api.egg-info/
--rw-r--r--   0 tomerefroni   (501) staff       (20)      190 2024-05-02 13:13:13.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api.egg-info/PKG-INFO
--rw-r--r--   0 tomerefroni   (501) staff       (20)      445 2024-05-02 13:13:13.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api.egg-info/SOURCES.txt
--rw-r--r--   0 tomerefroni   (501) staff       (20)        1 2024-05-02 13:13:13.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api.egg-info/dependency_links.txt
--rw-r--r--   0 tomerefroni   (501) staff       (20)        1 2024-04-24 12:32:27.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api.egg-info/not-zip-safe
--rw-r--r--   0 tomerefroni   (501) staff       (20)       17 2024-05-02 13:13:13.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api.egg-info/requires.txt
--rw-r--r--   0 tomerefroni   (501) staff       (20)       15 2024-05-02 13:13:13.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api.egg-info/top_level.txt
--rw-r--r--   0 tomerefroni   (501) staff       (20)      190 2024-05-02 13:13:13.494195 MoonshotAI_Api-0.0.2/PKG-INFO
--rw-r--r--   0 tomerefroni   (501) staff       (20)       13 2024-04-08 13:04:59.000000 MoonshotAI_Api-0.0.2/README.md
--rw-r--r--   0 tomerefroni   (501) staff       (20)       38 2024-05-02 13:13:13.494733 MoonshotAI_Api-0.0.2/setup.cfg
--rw-r--r--   0 tomerefroni   (501) staff       (20)      385 2024-05-02 13:11:16.000000 MoonshotAI_Api-0.0.2/setup.py
+drwxr-xr-x   0 moshe      (502) staff       (20)        0 2024-05-07 07:17:52.900403 MoonshotAI_Api-0.0.3/
+-rw-r--r--   0 moshe      (502) staff       (20)     1066 2024-05-07 06:26:25.000000 MoonshotAI_Api-0.0.3/LICENSE.md
+drwxr-xr-x   0 moshe      (502) staff       (20)        0 2024-05-07 07:17:52.898543 MoonshotAI_Api-0.0.3/MoonshotAI_Api/
+-rw-r--r--   0 moshe      (502) staff       (20)     1066 2024-05-07 06:26:25.000000 MoonshotAI_Api-0.0.3/MoonshotAI_Api/LICENSE
+-rw-r--r--   0 moshe      (502) staff       (20)       13 2024-05-07 06:26:25.000000 MoonshotAI_Api-0.0.3/MoonshotAI_Api/README.md
+-rw-r--r--   0 moshe      (502) staff       (20)        0 2024-05-07 06:26:25.000000 MoonshotAI_Api-0.0.3/MoonshotAI_Api/__init__.py
+-rw-r--r--   0 moshe      (502) staff       (20)     5397 2024-05-07 07:08:57.000000 MoonshotAI_Api-0.0.3/MoonshotAI_Api/ltv_client.py
+drwxr-xr-x   0 moshe      (502) staff       (20)        0 2024-05-07 07:17:52.899780 MoonshotAI_Api-0.0.3/MoonshotAI_Api/utils/
+-rw-r--r--   0 moshe      (502) staff       (20)      652 2024-05-07 06:26:25.000000 MoonshotAI_Api-0.0.3/MoonshotAI_Api/utils/consts.py
+-rw-r--r--   0 moshe      (502) staff       (20)       88 2024-05-07 06:26:25.000000 MoonshotAI_Api-0.0.3/MoonshotAI_Api/utils/output_enum.py
+-rw-r--r--   0 moshe      (502) staff       (20)     1293 2024-05-07 07:04:39.000000 MoonshotAI_Api-0.0.3/MoonshotAI_Api/utils/utils.py
+drwxr-xr-x   0 moshe      (502) staff       (20)        0 2024-05-07 07:17:52.899384 MoonshotAI_Api-0.0.3/MoonshotAI_Api.egg-info/
+-rw-r--r--   0 moshe      (502) staff       (20)      167 2024-05-07 07:17:52.000000 MoonshotAI_Api-0.0.3/MoonshotAI_Api.egg-info/PKG-INFO
+-rw-r--r--   0 moshe      (502) staff       (20)      470 2024-05-07 07:17:52.000000 MoonshotAI_Api-0.0.3/MoonshotAI_Api.egg-info/SOURCES.txt
+-rw-r--r--   0 moshe      (502) staff       (20)        1 2024-05-07 07:17:52.000000 MoonshotAI_Api-0.0.3/MoonshotAI_Api.egg-info/dependency_links.txt
+-rw-r--r--   0 moshe      (502) staff       (20)        1 2024-05-07 06:27:43.000000 MoonshotAI_Api-0.0.3/MoonshotAI_Api.egg-info/not-zip-safe
+-rw-r--r--   0 moshe      (502) staff       (20)       17 2024-05-07 07:17:52.000000 MoonshotAI_Api-0.0.3/MoonshotAI_Api.egg-info/requires.txt
+-rw-r--r--   0 moshe      (502) staff       (20)       15 2024-05-07 07:17:52.000000 MoonshotAI_Api-0.0.3/MoonshotAI_Api.egg-info/top_level.txt
+-rw-r--r--   0 moshe      (502) staff       (20)      167 2024-05-07 07:17:52.900199 MoonshotAI_Api-0.0.3/PKG-INFO
+-rw-r--r--   0 moshe      (502) staff       (20)       13 2024-05-07 06:26:25.000000 MoonshotAI_Api-0.0.3/README.md
+-rw-r--r--   0 moshe      (502) staff       (20)       38 2024-05-07 07:17:52.900445 MoonshotAI_Api-0.0.3/setup.cfg
+-rw-r--r--   0 moshe      (502) staff       (20)      385 2024-05-07 07:17:35.000000 MoonshotAI_Api-0.0.3/setup.py
+drwxr-xr-x   0 moshe      (502) staff       (20)        0 2024-05-07 07:17:52.899893 MoonshotAI_Api-0.0.3/tests/
+-rw-r--r--   0 moshe      (502) staff       (20)     1128 2024-05-07 07:16:10.000000 MoonshotAI_Api-0.0.3/tests/test.py
```

### Comparing `MoonshotAI_Api-0.0.2/MoonshotAI_Api/LICENSE` & `MoonshotAI_Api-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `MoonshotAI_Api-0.0.2/MoonshotAI_Api/ltv_client.py` & `MoonshotAI_Api-0.0.3/MoonshotAI_Api/ltv_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,19 @@
     def __init__(self, profile, token, default=False):
         self.profile = profile
         self._account_name = profile
         self.token = token
         self.default = default
 
     # Default output format - CSV filename
-    def fetch_data(self, kpi, pred_time, start_date, end_date, date_type, output_format=OutputFormat.CSV.value):
+    def fetch_data(self, kpi, pred_time, start_date, end_date,output_path, date_type='lead', output_format=OutputFormat.CSV.value):
 
         # Querying data
         query_id = self.__query_data(kpi=kpi, pred_time=pred_time, start_date=start_date, end_date=end_date,
-                                     date_type=date_type)
+                                     date_type=date_type,)
 
         # Add wait mechanic to make sure the data is ready
         status = None
         for idx in range(1, MAX_RETRIES):
             status = self.__check_status(query_id=query_id)
             if status == SUCCESS:
                 break
@@ -32,15 +32,15 @@
 
         if status != SUCCESS:
             raise Exception(f"Error getting data with given query id. Query execution status: {status}")
 
         # Getting data
         url = self.__get_data(query_id=query_id)
 
-        csv_data = download_file(url=url, output_format=output_format)
+        csv_data = download_file(url=url, output_format=output_format, output_path=output_path)
 
         # Returning data as stream / CSV filename depends on the output format
         return csv_data
 
     def __query_data(self, kpi, pred_time, start_date, end_date, date_type):
         headers = {
             "token": self.token,
```

### Comparing `MoonshotAI_Api-0.0.2/MoonshotAI_Api/utils/consts.py` & `MoonshotAI_Api-0.0.3/MoonshotAI_Api/utils/consts.py`

 * *Files identical despite different names*

