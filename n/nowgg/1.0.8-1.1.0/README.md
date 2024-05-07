# Comparing `tmp/nowgg-1.0.8.tar.gz` & `tmp/nowgg-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nowgg-1.0.8.tar", last modified: Fri Apr 12 10:20:34 2024, max compression
+gzip compressed data, was "nowgg-1.1.0.tar", last modified: Tue May  7 05:43:21 2024, max compression
```

## Comparing `nowgg-1.0.8.tar` & `nowgg-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-12 10:20:34.409798 nowgg-1.0.8/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1576 2024-04-12 10:20:34.409798 nowgg-1.0.8/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1380 2024-04-12 10:20:32.000000 nowgg-1.0.8/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-12 10:20:34.409798 nowgg-1.0.8/nowgg.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1576 2024-04-12 10:20:34.000000 nowgg-1.0.8/nowgg.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      203 2024-04-12 10:20:34.000000 nowgg-1.0.8/nowgg.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-12 10:20:34.000000 nowgg-1.0.8/nowgg.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-12 10:20:34.000000 nowgg-1.0.8/nowgg.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-12 10:20:34.000000 nowgg-1.0.8/nowgg.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-12 10:20:34.000000 nowgg-1.0.8/nowgg.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10284 2024-04-12 10:20:32.000000 nowgg-1.0.8/nowgg.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-12 10:20:34.409798 nowgg-1.0.8/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      516 2024-04-12 10:20:34.000000 nowgg-1.0.8/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 05:43:21.403078 nowgg-1.1.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2126 2024-05-07 05:43:21.403078 nowgg-1.1.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1930 2024-05-07 05:43:20.000000 nowgg-1.1.0/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 05:43:21.403078 nowgg-1.1.0/nowgg.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2126 2024-05-07 05:43:21.000000 nowgg-1.1.0/nowgg.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      203 2024-05-07 05:43:21.000000 nowgg-1.1.0/nowgg.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-07 05:43:21.000000 nowgg-1.1.0/nowgg.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-07 05:43:21.000000 nowgg-1.1.0/nowgg.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-05-07 05:43:21.000000 nowgg-1.1.0/nowgg.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-07 05:43:21.000000 nowgg-1.1.0/nowgg.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12438 2024-05-07 05:43:20.000000 nowgg-1.1.0/nowgg.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-07 05:43:21.403078 nowgg-1.1.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      516 2024-05-07 05:43:21.000000 nowgg-1.1.0/setup.py
```

### Comparing `nowgg-1.0.8/PKG-INFO` & `nowgg-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowgg
-Version: 1.0.8
+Version: 1.1.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author-email: cloudmaster@now.gg
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
@@ -23,28 +23,44 @@
     * Used to identify the publisher company.
     * Your Publisher token is available under the [Account Information](https://docs.now.gg/nowstudio/start-using-nowstudio#ac-info) section of nowStudio.
 
 ## Using nowgg CLI
 
 Open any terminal on macOS or Windows.
 
-Install nowgg CLI tool
+### Install nowgg CLI tool
 ```bash
   pip install nowgg
 ```
-Initialize nowgg CLI
+### Initialize nowgg CLI
 ```bash
   nowgg init --token "<your_publisherToken_from_nowStudio>"
 ```
-Upload App to nowStudio
+
+## Upload app using nowgg CLI to NowStudio
+
+### Upload App
+
 ```bash
   nowgg upload --app_id <your_app_id> --file_path "/directory/sample.apk" --apk_version <apk_version> --version_code <app_version_code>
+```
+
+#### add to test track after upload
+To create a draft on a test track, simply suffix the track id to the app_id, for example if your app_id is 1234, and you want to create draft on t1, provide app_id as 1234_t1
 
+### Upload App to a Test Track and trigger deployment
+providing the --deploy flag, will trigger a deployment on the test track. 
+
+```bash
+  nowgg upload --app_id <your_app_id> --file_path "/directory/sample.apk" --apk_version <apk_version> --version_code <app_version_code> --deploy
 ```
-For Help
+
+
+## For Help
+
 ```bash
   nowgg -h
   nowgg init -h
   nowgg upload -h
 ```  
 
 **Note**: Your app will be uploaded to the App Library within nowStudio.
```

### Comparing `nowgg-1.0.8/README.md` & `nowgg-1.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -13,28 +13,44 @@
     * Used to identify the publisher company.
     * Your Publisher token is available under the [Account Information](https://docs.now.gg/nowstudio/start-using-nowstudio#ac-info) section of nowStudio.
 
 ## Using nowgg CLI
 
 Open any terminal on macOS or Windows.
 
-Install nowgg CLI tool
+### Install nowgg CLI tool
 ```bash
   pip install nowgg
 ```
-Initialize nowgg CLI
+### Initialize nowgg CLI
 ```bash
   nowgg init --token "<your_publisherToken_from_nowStudio>"
 ```
-Upload App to nowStudio
+
+## Upload app using nowgg CLI to NowStudio
+
+### Upload App
+
 ```bash
   nowgg upload --app_id <your_app_id> --file_path "/directory/sample.apk" --apk_version <apk_version> --version_code <app_version_code>
+```
+
+#### add to test track after upload
+To create a draft on a test track, simply suffix the track id to the app_id, for example if your app_id is 1234, and you want to create draft on t1, provide app_id as 1234_t1
 
+### Upload App to a Test Track and trigger deployment
+providing the --deploy flag, will trigger a deployment on the test track. 
+
+```bash
+  nowgg upload --app_id <your_app_id> --file_path "/directory/sample.apk" --apk_version <apk_version> --version_code <app_version_code> --deploy
 ```
-For Help
+
+
+## For Help
+
 ```bash
   nowgg -h
   nowgg init -h
   nowgg upload -h
 ```  
 
 **Note**: Your app will be uploaded to the App Library within nowStudio.
```

### Comparing `nowgg-1.0.8/nowgg.egg-info/PKG-INFO` & `nowgg-1.1.0/nowgg.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowgg
-Version: 1.0.8
+Version: 1.1.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author-email: cloudmaster@now.gg
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
@@ -23,28 +23,44 @@
     * Used to identify the publisher company.
     * Your Publisher token is available under the [Account Information](https://docs.now.gg/nowstudio/start-using-nowstudio#ac-info) section of nowStudio.
 
 ## Using nowgg CLI
 
 Open any terminal on macOS or Windows.
 
-Install nowgg CLI tool
+### Install nowgg CLI tool
 ```bash
   pip install nowgg
 ```
-Initialize nowgg CLI
+### Initialize nowgg CLI
 ```bash
   nowgg init --token "<your_publisherToken_from_nowStudio>"
 ```
-Upload App to nowStudio
+
+## Upload app using nowgg CLI to NowStudio
+
+### Upload App
+
 ```bash
   nowgg upload --app_id <your_app_id> --file_path "/directory/sample.apk" --apk_version <apk_version> --version_code <app_version_code>
+```
+
+#### add to test track after upload
+To create a draft on a test track, simply suffix the track id to the app_id, for example if your app_id is 1234, and you want to create draft on t1, provide app_id as 1234_t1
 
+### Upload App to a Test Track and trigger deployment
+providing the --deploy flag, will trigger a deployment on the test track. 
+
+```bash
+  nowgg upload --app_id <your_app_id> --file_path "/directory/sample.apk" --apk_version <apk_version> --version_code <app_version_code> --deploy
 ```
-For Help
+
+
+## For Help
+
 ```bash
   nowgg -h
   nowgg init -h
   nowgg upload -h
 ```  
 
 **Note**: Your app will be uploaded to the App Library within nowStudio.
```

### Comparing `nowgg-1.0.8/nowgg.py` & `nowgg-1.1.0/nowgg.py`

 * *Files 15% similar despite different names*

```diff
@@ -92,16 +92,56 @@
                     "Error occurred during part upload. Please retry after some time.")
                 executor.shutdown(wait=False)
                 os.kill(process_id, signal.SIGINT)
     if event.is_set():
         return []
     return promises_array
 
+def save_to_app_track(file_url, app_id, token, app_version, app_version_code, upload_type, no_code, track_suffix, deploy):
+    json_to_send = {
+                      "upload_url": file_url,
+                      "app_version": app_version,
+                      "app_version_code": app_version_code,
+                      "game_id": app_id,
+                      "upload_type": upload_type,
+                      "track_suffix": track_suffix,
+                      "is_deploy": deploy
+                    }
+    headers = {"publisher_token": token}
+    response = requests.post(
+                f"{get_host()}/v2/publisher/test-track",
+                json=json_to_send, headers=headers)
+    if response.status_code in OK_STATUS:
+        if deploy:
+            logger.info("Successfully Saved to your Test Track and Triggered a Deployment!")
+        else:
+            logger.info("Successfully Saved to your Test Track!")
+    else:
+        logger.error(response.json().get('message', response.reason))
 
-def upload_file(file_path, game_id, token, app_version, app_version_code, no_code):
+def save_to_app_library(file_url, app_id, token, app_version, app_version_code, upload_type, no_code):
+    json_to_send = {
+                      "upload_url": file_url,
+                      "app_version": app_version,
+                      "app_version_code": app_version_code,
+                      "game_id": app_id,
+                      "upload_type": upload_type,
+                      "is_no_code_payment": True if no_code else False
+                    }
+    headers = {"publisher_token": token}
+    response = requests.post(
+                f"{get_host()}/v2/publisher/apk-library",
+                json=json_to_send, headers=headers)
+    if response.status_code in OK_STATUS:
+        logger.info("Successfully uploaded to your App Library!")
+    else:
+        logger.error(response.json().get('message', response.reason))
+
+
+def upload_file(file_path, app_id, token, app_version, app_version_code, no_code, track_suffix=None, deploy=False):
     if not (file_path.endswith(".zip") or file_path.endswith(".apk")):
         logging.error(
             "Invalid file type. Only .zip or .apk files are allowed.")
         return
     
     try:
         file_name = os.path.basename(file_path)
@@ -110,15 +150,15 @@
         headers = {"publisher_token": token}
 
         file_size = os.path.getsize(file_path)
         chunks_count = int((file_size // UPLOAD_CHUNK_SIZE) + 1)
 
         # Initialize multipart upload
         response = requests.post(f"{get_host()}/v2/publisher/asset/mutipart_upload/start",
-                                 params={"file_name": file_name, "game_id": game_id,
+                                 params={"file_name": file_name, "game_id": app_id,
                                          "parts_count": chunks_count},
                                  headers=headers)
         if response.status_code not in OK_STATUS:
             logger.error(response.json().get('message', response.reason))
             return
         data = response.json().get('data', {})
         upload_id = data.get('upload_id', "")
@@ -144,28 +184,17 @@
         response = requests.post(f"{get_host()}/v2/publisher/asset/mutipart_upload/end", json={
             "upload_id": upload_id, "parts_info": sorted_upload_parts_array,
                                     "s3_file_path": s3_file_path}, headers=headers)
         response.raise_for_status
         if response.status_code in OK_STATUS:
             logger.info("Upload completed.")
             file_url = f"https://cdn.now.gg/{s3_file_path}"
-            json_to_send = {"upload_url": file_url,
-                      "app_version": app_version,
-                      "app_version_code": app_version_code,
-                      "game_id": game_id,
-                      "upload_type": upload_type,
-                      "is_no_code_payment": True if no_code else False}
-            
-            response = requests.post(
-                f"{get_host()}/v2/publisher/apk-library",
-                json=json_to_send, headers=headers)
-            if response.status_code in OK_STATUS:
-                logger.info("Successfully uploaded to your Apk Library!")
-            else:
-                logger.error(response.json().get('message', response.reason))
+            save_to_app_library(file_url, app_id, token, app_version, app_version_code,upload_type, no_code)
+            if track_suffix:
+                save_to_app_track(file_url, app_id, token, app_version, app_version_code, upload_type, no_code, track_suffix, deploy)
         else:
             logger.error(response.json().get('message', response.reason))
 
     except Exception as e:
         logger.error(f"Error: {e}")
 
 
@@ -193,27 +222,27 @@
         if response.status_code not in OK_STATUS:
             logger.error(response.json().get('message', response.reason))
             return
         
         cache['token'] = token
         logger.info("init successful!")
 
-    def upload(self, app_id, app_file_path, app_version, app_version_code, no_code=0):
+    def upload(self, app_id, app_file_path, app_version, app_version_code, no_code=0, track_suffix=None, deploy=False):
         """Upload utility
 
         Args:
             app_id (str): required parameter app_id
             app_file_path (str): required parameter app_file_path
             app_version (str): required parameter app_version
             app_version_code (int): required parameter app_version_code
 
         """
         token = cache.get('token')
         if token:
-            return upload_file(app_file_path, app_id, token, app_version, app_version_code, no_code)
+            return upload_file(app_file_path, app_id, token, app_version, app_version_code, no_code, track_suffix, deploy)
         else:
             logger.error(
                 "Please init first with token. nowgg init -t <your-token>")
 
 
 set_log_level()
 
@@ -243,28 +272,44 @@
         '-f', '--file_path', type=str, help='File Path', required=True)
     upload_parser.add_argument(
         '-av', '--apk_version', type=str, help='apk version name', required=True)
     upload_parser.add_argument(
         '-vc', '--version_code', type=int, help='apk version code', required=True)
     upload_parser.add_argument(
         '-nc', '--no_code', action="store_true", help=argparse.SUPPRESS, required=False)
+    upload_parser.add_argument(
+        '-d', '--deploy', action="store_true", help='trigger deployment for the uploaded file to a specified test track', required=False) 
 
     config_parser = subparsers.add_parser('config')
     config_parser.add_argument(
         '-hn', '--host_name', help=argparse.SUPPRESS, required=False)
     
     args = parser.parse_args()
     if args.verbose:
         set_log_level(logging.DEBUG)
 
     if args.command == 'init':
         nowgg.init(args.token)
     elif args.command == 'upload':
-        nowgg.upload(args.app_id, args.file_path,
-                     args.apk_version, args.version_code, args.no_code)
+        app_id = args.app_id
+        track_suffix = None
+        deploy = False
+        if "_" in app_id:
+            app_id, track_suffix = app_id.split("_")
+            track_suffix = f"_{track_suffix}"
+        
+        if args.deploy:
+            if not track_suffix:
+                logger.error("--deploy can only be used when uploading to a track. Please provide a track suffix with the app_id.")
+                return
+            else:
+                deploy = True
+          
+        nowgg.upload(app_id, args.file_path,
+               args.apk_version, args.version_code, args.no_code, track_suffix, deploy)
     elif args.command == 'config':
         nowgg.config(args.host_name)
     else:
         parser.print_help()
 
 
 class CustomHelpFormatter(argparse.HelpFormatter):
```

### Comparing `nowgg-1.0.8/setup.py` & `nowgg-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from pathlib import Path
 import os
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(
     name='nowgg',
-    version='1.0.8',
+    version='1.1.0',
     scripts=['nowgg.py'],
     author_email='cloudmaster@now.gg',
     install_requires=[
         'requests'
     ],
     long_description=long_description,
     long_description_content_type='text/markdown',
```

