# Comparing `tmp/AppAuthN-0.0.16.tar.gz` & `tmp/AppAuthN-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AppAuthN-0.0.16.tar", last modified: Mon May  6 15:15:10 2024, max compression
+gzip compressed data, was "AppAuthN-0.0.17.tar", last modified: Tue May  7 04:09:27 2024, max compression
```

## Comparing `AppAuthN-0.0.16.tar` & `AppAuthN-0.0.17.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 15:15:10.822464 AppAuthN-0.0.16/
--rw-rw-rw-   0        0        0     1091 2024-02-26 10:52:10.000000 AppAuthN-0.0.16/LICENSE
--rw-rw-rw-   0        0        0      101 2024-05-06 15:15:10.819465 AppAuthN-0.0.16/PKG-INFO
--rw-rw-rw-   0        0        0     1075 2024-05-01 06:59:51.000000 AppAuthN-0.0.16/README.md
--rw-rw-rw-   0        0        0       42 2024-05-06 15:15:10.822464 AppAuthN-0.0.16/setup.cfg
--rw-rw-rw-   0        0        0      452 2024-05-06 15:14:05.000000 AppAuthN-0.0.16/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 15:15:10.743510 AppAuthN-0.0.16/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 15:15:10.791484 AppAuthN-0.0.16/src/AppAuthN/
--rw-rw-rw-   0        0        0     4489 2024-05-06 15:08:54.000000 AppAuthN-0.0.16/src/AppAuthN/CertificationReceiver.py
--rw-rw-rw-   0        0        0     1755 2024-05-06 15:13:50.000000 AppAuthN-0.0.16/src/AppAuthN/CloseLoopCounter.py
--rw-rw-rw-   0        0        0     2662 2024-05-06 15:10:45.000000 AppAuthN-0.0.16/src/AppAuthN/InferenceResult.py
--rw-rw-rw-   0        0        0        0 2024-02-26 10:52:10.000000 AppAuthN-0.0.16/src/AppAuthN/__init__.py
--rw-rw-rw-   0        0        0      638 2024-05-06 15:13:33.000000 AppAuthN-0.0.16/src/AppAuthN/config.json
-drwxrwxrwx   0        0        0        0 2024-05-06 15:15:10.815468 AppAuthN-0.0.16/src/AppAuthN.egg-info/
--rw-rw-rw-   0        0        0      101 2024-05-06 15:15:10.000000 AppAuthN-0.0.16/src/AppAuthN.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2024-05-06 15:15:10.000000 AppAuthN-0.0.16/src/AppAuthN.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 15:15:10.000000 AppAuthN-0.0.16/src/AppAuthN.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-06 15:15:10.000000 AppAuthN-0.0.16/src/AppAuthN.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-06 15:15:10.000000 AppAuthN-0.0.16/src/AppAuthN.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 04:09:27.267331 AppAuthN-0.0.17/
+-rw-rw-rw-   0        0        0     1091 2024-02-26 10:52:10.000000 AppAuthN-0.0.17/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-05-07 04:09:27.263206 AppAuthN-0.0.17/PKG-INFO
+-rw-rw-rw-   0        0        0     1075 2024-05-01 06:59:51.000000 AppAuthN-0.0.17/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-07 04:09:27.268331 AppAuthN-0.0.17/setup.cfg
+-rw-rw-rw-   0        0        0      452 2024-05-07 04:08:56.000000 AppAuthN-0.0.17/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 04:09:27.138856 AppAuthN-0.0.17/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 04:09:27.213569 AppAuthN-0.0.17/src/AppAuthN/
+-rw-rw-rw-   0        0        0     4469 2024-05-07 04:08:25.000000 AppAuthN-0.0.17/src/AppAuthN/CertificationReceiver.py
+-rw-rw-rw-   0        0        0     1815 2024-05-07 04:07:23.000000 AppAuthN-0.0.17/src/AppAuthN/CloseLoopCounter.py
+-rw-rw-rw-   0        0        0     2893 2024-05-07 04:05:40.000000 AppAuthN-0.0.17/src/AppAuthN/InferenceResult.py
+-rw-rw-rw-   0        0        0        0 2024-02-26 10:52:10.000000 AppAuthN-0.0.17/src/AppAuthN/__init__.py
+-rw-rw-rw-   0        0        0      662 2024-05-07 04:02:40.000000 AppAuthN-0.0.17/src/AppAuthN/config.json
+drwxrwxrwx   0        0        0        0 2024-05-07 04:09:27.258212 AppAuthN-0.0.17/src/AppAuthN.egg-info/
+-rw-rw-rw-   0        0        0      101 2024-05-07 04:09:26.000000 AppAuthN-0.0.17/src/AppAuthN.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2024-05-07 04:09:26.000000 AppAuthN-0.0.17/src/AppAuthN.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 04:09:26.000000 AppAuthN-0.0.17/src/AppAuthN.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-07 04:09:26.000000 AppAuthN-0.0.17/src/AppAuthN.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-07 04:09:26.000000 AppAuthN-0.0.17/src/AppAuthN.egg-info/top_level.txt
```

### Comparing `AppAuthN-0.0.16/LICENSE` & `AppAuthN-0.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `AppAuthN-0.0.16/README.md` & `AppAuthN-0.0.17/README.md`

 * *Files identical despite different names*

### Comparing `AppAuthN-0.0.16/src/AppAuthN/CertificationReceiver.py` & `AppAuthN-0.0.17/src/AppAuthN/CertificationReceiver.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,31 +82,25 @@
 
 
 ## 驗證certificate是否有效
 def check_identity(data):
     if data["certificate_receiver"]["status"] == "success":
         if data["certificate_receiver"]["certificate"][:64] == generate_hash(data):
             if int(data["certificate_receiver"]["certificate"][64:]) >=  int(time.time()):
-                print("certificate is vaild")
+                print("certificate is valid")
                 # print("the diff between timeout_timestamp and current_time:", int(data["certificate_receiver"]["certificate"][64:]) - int(time.time()))
             else:
-                print("Timeout, certificate is invaild")
+                print("Timeout, certificate is invalid")
                 data["certificate_receiver"]["status"] = "error"
                 #print("the diff between timeout_timestamp and current_time:", int(data["certificate_receiver"]["certificate"][64:]) - int(time.time()))
                 #要測試過期後可不可以自己重新登入
                 send_register_request(data["register"])
         else:
-            print("Invaild hash, certificate is invaild")
+            print("Invalid hash, certificate is invalid")
             data["certificate_receiver"]["status"] = "error"
     else:
         print("unregister, status error")
         data["certificate_receiver"]["status"] = "error"
     return data
 
 
 data_mgt = Data_mgt()
-    
-    
-
-
-
-
```

### Comparing `AppAuthN-0.0.16/src/AppAuthN/CloseLoopCounter.py` & `AppAuthN-0.0.17/src/AppAuthN/CloseLoopCounter.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,28 +24,28 @@
 
     data["closed_loop"]["value"] = global_counter.get_value()
     payload = {
         "application_uid": data["closed_loop"]["application_uid"],
         "position_uid": data["closed_loop"]["position_uid"],
         "packet_uid": data["closed_loop"]["packet_uid"],
         "inference_client_name": data["closed_loop"]["inference_client_name"],
+        "multi_input": data["closed_loop"]["multi_input"],
         "value": data["closed_loop"]["value"]
     }
     # print("Data to be sent:")
     # print(json.dumps(payload, indent=2))
 
     try:
         # Make the POST request
         response = requests.post(closed_loop_endpoint, json=payload)
         access_data = response.json()
-        print("response_payload:", access_data)
+        # print("response_payload:", access_data)
 
         # Check the response status code
         if response.status_code == 200:
             print("status:", response.status_code, "<closed_loop_data>/<ClosedLoopHandler>/<closed_loop_data_receiving>")
         else:
             print("ERROR", response.status_code, "<closed_loop_data_receiving>")
 
     except Exception as e:
         print(f"Error during registration: {e}")
     return data
-
```

### Comparing `AppAuthN-0.0.16/src/AppAuthN/InferenceResult.py` & `AppAuthN-0.0.17/src/AppAuthN/InferenceResult.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 ## send rawdata to inference layer for receiving inference result
 def send_rawdata(rawdata):
     data = data_mgt.read_json()
     check_identity(data)
     data["raw_data"]["application_uid"] = rawdata["application_uid"]
     data["raw_data"]["position_uid"] = rawdata["position_uid"]
     data["raw_data"]["inference_client_name"] = rawdata["inference_client_name"]
+    data["raw_data"]["multi_input"] = rawdata["multi_input"]
     data["raw_data"]["value"] = rawdata["value"]
  
 
     # API endpoint for inference_service
     inference_service_endpoint = f"""{data["api_url_with_I"]}/inference-service-{data["raw_data"]["position_uid"]}"""
     
     if (data["raw_data"]["packet_uid"]  == ""):
@@ -20,30 +21,32 @@
     else:
         data["raw_data"]["packet_uid"] = str(int(data["raw_data"]["packet_uid"])+1)
     payload = {
         "application_uid": data["raw_data"]["application_uid"],
         "position_uid": data["raw_data"]["position_uid"],
         "packet_uid": data["raw_data"]["packet_uid"],
         "inference_client_name": data["raw_data"]["inference_client_name"],
+        "multi_input": data["raw_data"]["multi_input"],
         "value": data["raw_data"]["value"]
     }
     data["closed_loop"]["application_uid"] = data["raw_data"]["application_uid"]
     data["closed_loop"]["position_uid"] = data["raw_data"]["position_uid"]
     data["closed_loop"]["packet_uid"] = data["raw_data"]["packet_uid"]
+    data["closed_loop"]["multi_input"] = data["raw_data"]["multi_input"]
     data["closed_loop"]["inference_client_name"] = data["raw_data"]["inference_client_name"]
     # print("Data to be sent:")
     # print(json.dumps(payload, indent=2))
 
     try:
         # Make the POST request
         global_counter.reset()
         response = requests.post(inference_service_endpoint, json=payload)
         # start a timer
         access_data = response.json()
-        print("inference_result:", access_data)
+        # print("inference_result:", access_data)
 
         # Check the response status code
         if response.status_code == 200:
             data = send_closed_loop(data)
             print("status:", response.status_code, "<inference_exe>/<InferenceServiceHandler>/<inference_service>")
             data["result_receiver"]["status"] = access_data.get('status')
             data["result_receiver"]["value"] = access_data.get('data')
@@ -52,7 +55,8 @@
             # 拿掉，這樣失效的時候才可以重新註冊
             # data["certificate_receiver"]["status"] = "error"
 
     except Exception as e:
         print(f"Error during registration: {e}")
 
     data_mgt.write_json(data)
+    return data["result_receiver"]
```

### Comparing `AppAuthN-0.0.16/src/AppAuthN/config.json` & `AppAuthN-0.0.17/src/AppAuthN/config.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9880952380952381%*

 * *Differences: {"'raw_data'": "{'multi_input': ''}"}*

```diff
@@ -11,14 +11,15 @@
         "packet_uid": "",
         "position_uid": "",
         "value": ""
     },
     "raw_data": {
         "application_uid": "",
         "inference_client_name": "",
+        "multi_input": "",
         "packet_uid": "",
         "position_uid": "",
         "value": ""
     },
     "register": {
         "application_token": "",
         "application_uid": "",
```

