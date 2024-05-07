# Comparing `tmp/threed_optix-5.0.5.tar.gz` & `tmp/threed_optix-5.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threed_optix-5.0.5.tar", last modified: Tue May  7 07:35:27 2024, max compression
+gzip compressed data, was "threed_optix-5.0.6.tar", last modified: Tue May  7 09:41:08 2024, max compression
```

## Comparing `threed_optix-5.0.5.tar` & `threed_optix-5.0.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-07 07:35:27.593617 threed_optix-5.0.5/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      148 2024-03-24 13:38:50.000000 threed_optix-5.0.5/.gitignore
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1064 2024-02-20 12:16:48.000000 threed_optix-5.0.5/LICENSE.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2377 2024-05-07 07:35:27.593617 threed_optix-5.0.5/PKG-INFO
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2077 2024-03-24 13:38:50.000000 threed_optix-5.0.5/README.md
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-07 07:35:27.593617 threed_optix-5.0.5/help/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43940 2024-05-06 11:41:26.000000 threed_optix-5.0.5/help/SDK help text.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43940 2024-05-06 11:41:26.000000 threed_optix-5.0.5/help/SDK help.md
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      107 2024-05-07 07:35:27.593617 threed_optix-5.0.5/setup.cfg
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1222 2024-05-06 11:41:26.000000 threed_optix-5.0.5/setup.py
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-07 07:35:27.593617 threed_optix-5.0.5/src/
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-07 07:35:27.593617 threed_optix-5.0.5/src/threed_optix/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      844 2024-05-06 11:41:26.000000 threed_optix-5.0.5/src/threed_optix/__init__.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    23949 2024-05-07 07:32:41.000000 threed_optix-5.0.5/src/threed_optix/analyses.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     4172 2024-03-24 13:38:50.000000 threed_optix-5.0.5/src/threed_optix/beams.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43648 2024-05-07 07:32:41.000000 threed_optix-5.0.5/src/threed_optix/client.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)       29 2024-03-24 13:38:50.000000 threed_optix-5.0.5/src/threed_optix/optimize.py
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-07 07:35:27.593617 threed_optix-5.0.5/src/threed_optix/package_utils/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)       16 2024-03-24 13:38:50.000000 threed_optix-5.0.5/src/threed_optix/package_utils/__init__.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    15563 2024-05-01 11:13:46.000000 threed_optix-5.0.5/src/threed_optix/package_utils/api.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     3248 2024-05-07 07:32:41.000000 threed_optix-5.0.5/src/threed_optix/package_utils/general.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1582 2024-05-01 11:13:46.000000 threed_optix-5.0.5/src/threed_optix/package_utils/math.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)       70 2024-03-24 13:38:50.000000 threed_optix-5.0.5/src/threed_optix/package_utils/matlab.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    19129 2024-05-07 07:32:41.000000 threed_optix-5.0.5/src/threed_optix/package_utils/vars.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    61029 2024-05-07 07:32:32.000000 threed_optix-5.0.5/src/threed_optix/parts.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    15046 2024-05-06 11:41:26.000000 threed_optix-5.0.5/src/threed_optix/simulations.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     4719 2024-05-07 07:32:41.000000 threed_optix-5.0.5/src/threed_optix/utils.py
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-07 07:35:27.593617 threed_optix-5.0.5/src/threed_optix.egg-info/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2377 2024-05-07 07:35:27.000000 threed_optix-5.0.5/src/threed_optix.egg-info/PKG-INFO
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      756 2024-05-07 07:35:27.000000 threed_optix-5.0.5/src/threed_optix.egg-info/SOURCES.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)        1 2024-05-07 07:35:27.000000 threed_optix-5.0.5/src/threed_optix.egg-info/dependency_links.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      107 2024-05-07 07:35:27.000000 threed_optix-5.0.5/src/threed_optix.egg-info/requires.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)       13 2024-05-07 07:35:27.000000 threed_optix-5.0.5/src/threed_optix.egg-info/top_level.txt
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-07 09:41:08.373030 threed_optix-5.0.6/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      148 2024-03-24 13:38:50.000000 threed_optix-5.0.6/.gitignore
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1064 2024-02-20 12:16:48.000000 threed_optix-5.0.6/LICENSE.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2377 2024-05-07 09:41:08.373030 threed_optix-5.0.6/PKG-INFO
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2077 2024-03-24 13:38:50.000000 threed_optix-5.0.6/README.md
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-07 09:41:08.373030 threed_optix-5.0.6/help/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43940 2024-05-06 11:41:26.000000 threed_optix-5.0.6/help/SDK help text.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43940 2024-05-06 11:41:26.000000 threed_optix-5.0.6/help/SDK help.md
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      107 2024-05-07 09:41:08.373030 threed_optix-5.0.6/setup.cfg
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1222 2024-05-06 11:41:26.000000 threed_optix-5.0.6/setup.py
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-07 09:41:08.373030 threed_optix-5.0.6/src/
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-07 09:41:08.373030 threed_optix-5.0.6/src/threed_optix/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      844 2024-05-06 11:41:26.000000 threed_optix-5.0.6/src/threed_optix/__init__.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    23949 2024-05-07 07:32:41.000000 threed_optix-5.0.6/src/threed_optix/analyses.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     4172 2024-03-24 13:38:50.000000 threed_optix-5.0.6/src/threed_optix/beams.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43648 2024-05-07 07:32:41.000000 threed_optix-5.0.6/src/threed_optix/client.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)       29 2024-03-24 13:38:50.000000 threed_optix-5.0.6/src/threed_optix/optimize.py
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-07 09:41:08.373030 threed_optix-5.0.6/src/threed_optix/package_utils/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)       16 2024-03-24 13:38:50.000000 threed_optix-5.0.6/src/threed_optix/package_utils/__init__.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    15738 2024-05-07 09:40:04.000000 threed_optix-5.0.6/src/threed_optix/package_utils/api.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     3248 2024-05-07 07:32:41.000000 threed_optix-5.0.6/src/threed_optix/package_utils/general.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1582 2024-05-01 11:13:46.000000 threed_optix-5.0.6/src/threed_optix/package_utils/math.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)       70 2024-03-24 13:38:50.000000 threed_optix-5.0.6/src/threed_optix/package_utils/matlab.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    19175 2024-05-07 09:40:59.000000 threed_optix-5.0.6/src/threed_optix/package_utils/vars.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    61029 2024-05-07 07:32:32.000000 threed_optix-5.0.6/src/threed_optix/parts.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    15046 2024-05-06 11:41:26.000000 threed_optix-5.0.6/src/threed_optix/simulations.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     4719 2024-05-07 07:32:41.000000 threed_optix-5.0.6/src/threed_optix/utils.py
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-07 09:41:08.373030 threed_optix-5.0.6/src/threed_optix.egg-info/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2377 2024-05-07 09:41:08.000000 threed_optix-5.0.6/src/threed_optix.egg-info/PKG-INFO
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      756 2024-05-07 09:41:08.000000 threed_optix-5.0.6/src/threed_optix.egg-info/SOURCES.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)        1 2024-05-07 09:41:08.000000 threed_optix-5.0.6/src/threed_optix.egg-info/dependency_links.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      107 2024-05-07 09:41:08.000000 threed_optix-5.0.6/src/threed_optix.egg-info/requires.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)       13 2024-05-07 09:41:08.000000 threed_optix-5.0.6/src/threed_optix.egg-info/top_level.txt
```

### Comparing `threed_optix-5.0.5/LICENSE.txt` & `threed_optix-5.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.5/PKG-INFO` & `threed_optix-5.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threed_optix
-Version: 5.0.5
+Version: 5.0.6
 Home-page: https://3doptix.com
 Author: 3DOptix
 Author-email: ereztep@3doptix.com
 License: MIT
 Keywords: Optics,Optical Design,Optical Simulation,Optical Design Software,3DOptix
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `threed_optix-5.0.5/README.md` & `threed_optix-5.0.6/README.md`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.5/help/SDK help text.txt` & `threed_optix-5.0.6/help/SDK help text.txt`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.5/help/SDK help.md` & `threed_optix-5.0.6/help/SDK help.md`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.5/setup.py` & `threed_optix-5.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.5/src/threed_optix/__init__.py` & `threed_optix-5.0.6/src/threed_optix/__init__.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.5/src/threed_optix/analyses.py` & `threed_optix-5.0.6/src/threed_optix/analyses.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.5/src/threed_optix/beams.py` & `threed_optix-5.0.6/src/threed_optix/beams.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.5/src/threed_optix/client.py` & `threed_optix-5.0.6/src/threed_optix/client.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.5/src/threed_optix/package_utils/api.py` & `threed_optix-5.0.6/src/threed_optix/package_utils/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,16 @@
     Returns:
         tuple: The data and message from the response.
     """
 
     url = f'{v.API_URL}/{endpoint}'
     headers = {'X-API-KEY': api_key,
                'Content-Type': 'application/json',
-               "sdk-version": v.VERSION}
+               "sdk-version": v.VERSION,
+               'origin': v.ORIGIN}
 
     if v.DEBUG:
         print(f'GET {url}')
         print(f'Headers: {headers}')
 
     r = requests.get(url, headers=headers)
     verify_response(r)
@@ -76,17 +77,19 @@
         json_data (dict): The JSON payload for the request.
         api_key (str): The API key.
 
     Returns:
         tuple: The data and message from the response.
     """
     url = f'{v.API_URL}/{endpoint}'
-    headers =  {'X-API-KEY': api_key,
+    headers = {'X-API-KEY': api_key,
                'Content-Type': 'application/json',
-               "sdk-version": v.VERSION}
+               "sdk-version": v.VERSION,
+               'origin': v.ORIGIN}
+
 
     if v.DEBUG:
         print(f'PUT {url}')
         print(f'Headers: {headers}')
         print(f'Payload: {json_data}')
 
     r = requests.put(url, headers=headers, json=json_data)
@@ -109,17 +112,19 @@
         data (dict): The data to send.
         api_key (str): The API key.
 
     Returns:
         tuple: The data and message from the response.
     '''
     url = f'{v.API_URL}/{endpoint}'
-    headers =  {'X-API-KEY': api_key,
+    headers = {'X-API-KEY': api_key,
                'Content-Type': 'application/json',
-               "sdk-version": v.VERSION}
+               "sdk-version": v.VERSION,
+               'origin': v.ORIGIN}
+
 
     if v.DEBUG:
         print(f'SET {url}')
         print(f'Headers: {headers}')
         print(f'Payload: {data}')
 
 
@@ -142,17 +147,19 @@
         data (dict): The data to send.
         api_key (str): The API key.
 
     Returns:
         tuple: The status, message, and data from the response.
     '''
     url = f'{v.API_URL}/{endpoint}'
-    headers =  {'X-API-KEY': api_key,
+    headers = {'X-API-KEY': api_key,
                'Content-Type': 'application/json',
-               "sdk-version": v.VERSION}
+               "sdk-version": v.VERSION,
+               'origin': v.ORIGIN}
+
 
     if v.DEBUG:
         print(f'POST {url}')
         print(f'Headers: {headers}')
         print(f'Payload: {data}')
 
     r = requests.post(url, headers=headers, json=data)
@@ -172,17 +179,19 @@
         endpoint (str): The endpoint to send the request to.
         api_key (str): The API key.
 
     Returns:
         tuple: The status and message from the response.
     '''
     url = f'{v.API_URL}/{endpoint}'
-    headers =  {'X-API-KEY': api_key,
+    headers = {'X-API-KEY': api_key,
                'Content-Type': 'application/json',
-               "sdk-version": v.VERSION}
+               "sdk-version": v.VERSION,
+               'origin': v.ORIGIN}
+
 
     if v.DEBUG:
         print(f'DELETE {url}')
         print(f'Headers: {headers}')
 
     r = requests.delete(url, headers=headers)
     verify_response(r)
```

### Comparing `threed_optix-5.0.5/src/threed_optix/package_utils/general.py` & `threed_optix-5.0.6/src/threed_optix/package_utils/general.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.5/src/threed_optix/package_utils/math.py` & `threed_optix-5.0.6/src/threed_optix/package_utils/math.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.5/src/threed_optix/package_utils/vars.py` & `threed_optix-5.0.6/src/threed_optix/package_utils/vars.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import numpy as np
 import re
 
 DEBUG = False
 BASE_BACKUP = 'DEFAULT'
 VALID_RESPONSE_CODES = [200, 201, 202, 204]
 # Take the version of the package
-VERSION = "5.0.5"
+VERSION = "5.0.6"
 
 
 #Base API URL
 API_URL = "https://api.3doptix.com/v1"
+ORIGIN = 0 #0 for origin that is a human user
 
 class Surfaces:
     DETECTOR_FRONT = 'front'
 
 class Analyses:
     DEFAULT_NUM_RAYS = 30
```

### Comparing `threed_optix-5.0.5/src/threed_optix/parts.py` & `threed_optix-5.0.6/src/threed_optix/parts.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.5/src/threed_optix/simulations.py` & `threed_optix-5.0.6/src/threed_optix/simulations.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.5/src/threed_optix/utils.py` & `threed_optix-5.0.6/src/threed_optix/utils.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.5/src/threed_optix.egg-info/PKG-INFO` & `threed_optix-5.0.6/src/threed_optix.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threed-optix
-Version: 5.0.5
+Version: 5.0.6
 Home-page: https://3doptix.com
 Author: 3DOptix
 Author-email: ereztep@3doptix.com
 License: MIT
 Keywords: Optics,Optical Design,Optical Simulation,Optical Design Software,3DOptix
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `threed_optix-5.0.5/src/threed_optix.egg-info/SOURCES.txt` & `threed_optix-5.0.6/src/threed_optix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

