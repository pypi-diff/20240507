# Comparing `tmp/pyxui-0.0.9.tar.gz` & `tmp/pyxui-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxui-0.0.9.tar", last modified: Thu Jul  6 08:33:52 2023, max compression
+gzip compressed data, was "pyxui-1.0.1.tar", last modified: Tue May  7 20:36:14 2024, max compression
```

## Comparing `pyxui-0.0.9.tar` & `pyxui-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 08:33:52.555309 pyxui-0.0.9/
--rw-rw-rw-   0        0        0     1070 2023-07-06 08:30:19.000000 pyxui-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     6043 2023-07-06 08:33:52.554312 pyxui-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     5411 2023-07-06 08:30:19.000000 pyxui-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 08:33:52.487572 pyxui-0.0.9/pyxui/
--rw-rw-rw-   0        0        0       26 2023-07-06 08:30:19.000000 pyxui-0.0.9/pyxui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 08:33:52.509795 pyxui-0.0.9/pyxui/config_gen/
--rw-rw-rw-   0        0        0      441 2023-07-06 08:30:19.000000 pyxui-0.0.9/pyxui/config_gen/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 08:33:52.516535 pyxui-0.0.9/pyxui/errors/
--rw-rw-rw-   0        0        0      884 2023-07-06 08:30:19.000000 pyxui-0.0.9/pyxui/errors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 08:33:52.553314 pyxui-0.0.9/pyxui/methods/
--rw-rw-rw-   0        0        0      235 2023-07-06 08:30:19.000000 pyxui-0.0.9/pyxui/methods/__init__.py
--rw-rw-rw-   0        0        0     1612 2023-07-06 08:30:19.000000 pyxui-0.0.9/pyxui/methods/base.py
--rw-rw-rw-   0        0        0     7953 2023-07-06 08:30:19.000000 pyxui-0.0.9/pyxui/methods/clients.py
--rw-rw-rw-   0        0        0     1190 2023-07-06 08:30:19.000000 pyxui-0.0.9/pyxui/methods/inbounds.py
--rw-rw-rw-   0        0        0     1077 2023-07-06 08:30:19.000000 pyxui-0.0.9/pyxui/methods/login.py
--rw-rw-rw-   0        0        0      573 2023-07-06 08:30:19.000000 pyxui-0.0.9/pyxui/xui.py
-drwxrwxrwx   0        0        0        0 2023-07-06 08:33:52.502531 pyxui-0.0.9/pyxui.egg-info/
--rw-rw-rw-   0        0        0     6043 2023-07-06 08:33:52.000000 pyxui-0.0.9/pyxui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-07-06 08:33:52.000000 pyxui-0.0.9/pyxui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 08:33:52.000000 pyxui-0.0.9/pyxui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-06 08:33:52.000000 pyxui-0.0.9/pyxui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-06 08:33:52.000000 pyxui-0.0.9/pyxui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 08:33:52.555309 pyxui-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      707 2023-07-06 08:32:01.000000 pyxui-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 20:36:14.620338 pyxui-1.0.1/
+-rw-rw-rw-   0        0        0     1070 2023-07-06 08:30:19.000000 pyxui-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     6069 2024-05-07 20:36:14.619341 pyxui-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5629 2024-05-07 20:18:32.000000 pyxui-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 20:36:14.593100 pyxui-1.0.1/pyxui/
+-rw-rw-rw-   0        0        0       26 2023-07-22 18:08:28.000000 pyxui-1.0.1/pyxui/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 20:36:14.609862 pyxui-1.0.1/pyxui/config_gen/
+-rw-rw-rw-   0        0        0      441 2023-07-22 18:08:28.000000 pyxui-1.0.1/pyxui/config_gen/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 20:36:14.610860 pyxui-1.0.1/pyxui/errors/
+-rw-rw-rw-   0        0        0      884 2023-07-22 18:08:28.000000 pyxui-1.0.1/pyxui/errors/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 20:36:14.617343 pyxui-1.0.1/pyxui/methods/
+-rw-rw-rw-   0        0        0      235 2023-07-22 18:08:28.000000 pyxui-1.0.1/pyxui/methods/__init__.py
+-rw-rw-rw-   0        0        0     1619 2024-05-07 20:20:04.000000 pyxui-1.0.1/pyxui/methods/base.py
+-rw-rw-rw-   0        0        0     7953 2023-07-22 18:08:28.000000 pyxui-1.0.1/pyxui/methods/clients.py
+-rw-rw-rw-   0        0        0     1190 2023-07-22 18:08:28.000000 pyxui-1.0.1/pyxui/methods/inbounds.py
+-rw-rw-rw-   0        0        0     1020 2024-05-07 20:20:11.000000 pyxui-1.0.1/pyxui/methods/login.py
+-rw-rw-rw-   0        0        0      623 2024-05-07 20:19:46.000000 pyxui-1.0.1/pyxui/xui.py
+drwxrwxrwx   0        0        0        0 2024-05-07 20:36:14.618343 pyxui-1.0.1/pyxui.egg-info/
+-rw-rw-rw-   0        0        0     6069 2024-05-07 20:36:14.000000 pyxui-1.0.1/pyxui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2024-05-07 20:36:14.000000 pyxui-1.0.1/pyxui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 20:36:14.000000 pyxui-1.0.1/pyxui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-07 20:36:14.000000 pyxui-1.0.1/pyxui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-07 20:36:14.000000 pyxui-1.0.1/pyxui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 20:36:14.620338 pyxui-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      707 2024-05-07 20:36:07.000000 pyxui-1.0.1/setup.py
```

### Comparing `pyxui-0.0.9/LICENSE` & `pyxui-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxui-0.0.9/PKG-INFO` & `pyxui-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pyxui
-Version: 0.0.9
+Version: 1.0.1
 Summary: An application with python that allows you to modify your xui panel
 Home-page: https://github.com/staliox/pyxui
 Author: Staliox
 License: MIT
 Keywords: pyxui,xui,xui python,xui panel
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
 
 # PyXUI 
 An application with python that allows you to modify your xui panel ([alireza0 x-ui](https://github.com/alireza0/x-ui)) ([Sanaeii 3x-ui](https://github.com/MHSanaei/3x-ui)) 
 
 ## How To Install
 ```
 pip install pyxui
@@ -30,15 +31,15 @@
     panel="alireza", # Your panel name, "alireza" or "sanaei"
 )
 
 # Advanced:
 xui = XUI(
     full_address="http://staliox.site:2087",
     panel="alireza", # Your panel name, "alireza" or "sanaei"
-    https=False # Make note if you don't use https set False else set True
+    https=False, # Make note if you don't use https set False else set True
     session_string=... # If you have session cookie to use panel without login
 )
 ```
 
 - Login in your panel
 ```python
 from pyxui.errors import BadLogin
```

### Comparing `pyxui-0.0.9/pyxui/errors/__init__.py` & `pyxui-1.0.1/pyxui/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxui-0.0.9/pyxui/methods/base.py` & `pyxui-1.0.1/pyxui/methods/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         
         if path == "login":
             url = f"{self.full_address}/login"
         else:
             url = f"{self.full_address}/{self.api_path}/inbounds/{path}"
 
         if self.session_string:
-            cookie = {'session': self.session_string}
+            cookie = {self.cookie_name: self.session_string}
         else:
             cookie = None
 
         if method == "GET":
             response = requests.get(url, cookies=cookie, verify=self.https)
         elif method == "POST":
             response = requests.post(url, cookies=cookie, data=params, verify=self.https)
```

### Comparing `pyxui-0.0.9/pyxui/methods/clients.py` & `pyxui-1.0.1/pyxui/methods/clients.py`

 * *Files identical despite different names*

### Comparing `pyxui-0.0.9/pyxui/methods/inbounds.py` & `pyxui-1.0.1/pyxui/methods/inbounds.py`

 * *Files identical despite different names*

### Comparing `pyxui-0.0.9/pyxui/methods/login.py` & `pyxui-1.0.1/pyxui/methods/login.py`

 * *Files 25% similar despite different names*

```diff
@@ -31,16 +31,13 @@
             params={
                 'username': username,
                 'password': password
             }
         )
 
         if send_request.status_code == 200:
-            self.session_string = send_request.cookies.get("session")
+            self.session_string = send_request.cookies.get(self.cookie_name)
 
             if self.session_string:
                 return True
-            else:
-                raise errors.BadLogin()
-
-        else:
-            raise errors.BadLogin()
+            
+        raise errors.BadLogin()
```

### Comparing `pyxui-0.0.9/pyxui/xui.py` & `pyxui-1.0.1/pyxui/xui.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     ) -> None:
         super().__init__()
 
         self.full_address = full_address
         self.panel = panel
         self.https = https
         self.session_string = session_string
-        self.api_path = None
 
         if self.panel == "alireza":
             self.api_path = "xui/API"
+            self.cookie_name = "x-ui"
             
         elif self.panel == "sanaei":
-            self.api_path = "panel/api"
+            self.api_path = "panel/api"
+            self.cookie_name = "session"
```

### Comparing `pyxui-0.0.9/pyxui.egg-info/PKG-INFO` & `pyxui-1.0.1/pyxui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pyxui
-Version: 0.0.9
+Version: 1.0.1
 Summary: An application with python that allows you to modify your xui panel
 Home-page: https://github.com/staliox/pyxui
 Author: Staliox
 License: MIT
 Keywords: pyxui,xui,xui python,xui panel
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
 
 # PyXUI 
 An application with python that allows you to modify your xui panel ([alireza0 x-ui](https://github.com/alireza0/x-ui)) ([Sanaeii 3x-ui](https://github.com/MHSanaei/3x-ui)) 
 
 ## How To Install
 ```
 pip install pyxui
@@ -30,15 +31,15 @@
     panel="alireza", # Your panel name, "alireza" or "sanaei"
 )
 
 # Advanced:
 xui = XUI(
     full_address="http://staliox.site:2087",
     panel="alireza", # Your panel name, "alireza" or "sanaei"
-    https=False # Make note if you don't use https set False else set True
+    https=False, # Make note if you don't use https set False else set True
     session_string=... # If you have session cookie to use panel without login
 )
 ```
 
 - Login in your panel
 ```python
 from pyxui.errors import BadLogin
```

### Comparing `pyxui-0.0.9/setup.py` & `pyxui-1.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
     
-VERSION = "0.0.9"
+VERSION = "1.0.1"
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name="pyxui",
     version=VERSION,
```

