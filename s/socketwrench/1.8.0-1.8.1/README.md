# Comparing `tmp/socketwrench-1.8.0.tar.gz` & `tmp/socketwrench-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketwrench-1.8.0.tar", last modified: Fri May  3 02:49:14 2024, max compression
+gzip compressed data, was "socketwrench-1.8.1.tar", last modified: Tue May  7 19:02:27 2024, max compression
```

## Comparing `socketwrench-1.8.0.tar` & `socketwrench-1.8.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:49:14.751569 socketwrench-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-03 02:49:08.000000 socketwrench-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-03 02:49:08.000000 socketwrench-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10918 2024-05-03 02:49:14.751569 socketwrench-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9039 2024-05-03 02:49:08.000000 socketwrench-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-03 02:49:08.000000 socketwrench-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 02:49:14.751569 socketwrench-1.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:49:14.743569 socketwrench-1.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:49:14.747569 socketwrench-1.8.0/src/socketwrench/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20975 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/openapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:49:14.747569 socketwrench-1.8.0/src/socketwrench/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/resources/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:49:14.747569 socketwrench-1.8.0/src/socketwrench/resources/playground/
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/resources/playground/panels.js
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/resources/playground/playground.html
--rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/resources/playground/playground.js
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/resources/swagger.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:49:14.751569 socketwrench-1.8.0/src/socketwrench/samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/samples/file_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/samples/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    10313 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    21106 2024-05-03 02:49:08.000000 socketwrench-1.8.0/src/socketwrench/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:49:14.751569 socketwrench-1.8.0/src/socketwrench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10918 2024-05-03 02:49:14.000000 socketwrench-1.8.0/src/socketwrench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-03 02:49:14.000000 socketwrench-1.8.0/src/socketwrench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 02:49:14.000000 socketwrench-1.8.0/src/socketwrench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 02:49:14.000000 socketwrench-1.8.0/src/socketwrench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:02:27.365853 socketwrench-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-07 19:02:22.000000 socketwrench-1.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-07 19:02:22.000000 socketwrench-1.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-07 19:02:27.365853 socketwrench-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-05-07 19:02:22.000000 socketwrench-1.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-07 19:02:22.000000 socketwrench-1.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 19:02:27.365853 socketwrench-1.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:02:27.357853 socketwrench-1.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:02:27.361853 socketwrench-1.8.1/src/socketwrench/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20975 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/openapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:02:27.365853 socketwrench-1.8.1/src/socketwrench/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/resources/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:02:27.365853 socketwrench-1.8.1/src/socketwrench/resources/playground/
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/resources/playground/panels.js
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/resources/playground/playground.html
+-rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/resources/playground/playground.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/resources/swagger.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:02:27.365853 socketwrench-1.8.1/src/socketwrench/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/samples/file_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/samples/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10313 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21106 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:02:27.365853 socketwrench-1.8.1/src/socketwrench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-07 19:02:27.000000 socketwrench-1.8.1/src/socketwrench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-07 19:02:27.000000 socketwrench-1.8.1/src/socketwrench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:02:27.000000 socketwrench-1.8.1/src/socketwrench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 19:02:27.000000 socketwrench-1.8.1/src/socketwrench.egg-info/top_level.txt
```

### Comparing `socketwrench-1.8.0/LICENSE` & `socketwrench-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.0/PKG-INFO` & `socketwrench-1.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.8.0
+Version: 1.8.1
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -34,14 +34,24 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # socketwrench
 A webserver based on `socket.socket` with no dependencies other than the standard library.
 Provides a lightweight quickstart to make an API which supports OpenAPI, Swagger, and more.
 
+## NOTE:
+this is **not** a production-ready web server. It is a learning tool and a lightweight way to make a simple API. While I attempted to reduce overhead in calls, I haven't taken time to thoroughly optimize, and I have not implemented any complex features to deal with security, performance, or scalability.
+
+## Project Goals
+Part of the goal of this project was to understand how web servers work and to make a simple web server that is easy to use and understand.
+As learning progressed, features were added, but the code became a bit more complex.
+To learn more about the basics of web servers and how to develop one from scratch, see [learning.md](./learning.md) or jump straight into the 
+building blocks of source code in [simplestsocketwrench.py](./src/simplestsocketwrench.py) => [simplesocketwrench.py](./src/simplesocketwrench.py) => [socketwrench](./src/socketwrench).
+If you would prefer to use this library, read on!
+
 # Quickstart
 ### Install
 ```bash
 pip install socketwrench
 ```
 
 ### Serve a class
```

### Comparing `socketwrench-1.8.0/README.md` & `socketwrench-1.8.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 # socketwrench
 A webserver based on `socket.socket` with no dependencies other than the standard library.
 Provides a lightweight quickstart to make an API which supports OpenAPI, Swagger, and more.
 
+## NOTE:
+this is **not** a production-ready web server. It is a learning tool and a lightweight way to make a simple API. While I attempted to reduce overhead in calls, I haven't taken time to thoroughly optimize, and I have not implemented any complex features to deal with security, performance, or scalability.
+
+## Project Goals
+Part of the goal of this project was to understand how web servers work and to make a simple web server that is easy to use and understand.
+As learning progressed, features were added, but the code became a bit more complex.
+To learn more about the basics of web servers and how to develop one from scratch, see [learning.md](./learning.md) or jump straight into the 
+building blocks of source code in [simplestsocketwrench.py](./src/simplestsocketwrench.py) => [simplesocketwrench.py](./src/simplesocketwrench.py) => [socketwrench](./src/socketwrench).
+If you would prefer to use this library, read on!
+
 # Quickstart
 ### Install
 ```bash
 pip install socketwrench
 ```
 
 ### Serve a class
```

### Comparing `socketwrench-1.8.0/pyproject.toml` & `socketwrench-1.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketwrench"
-version = "1.8.0"
+version = "1.8.1"
 description = "A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger."
 readme = "README.md"
 authors = [{ name = "Torin Halsted", email = "modularizer@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
```

### Comparing `socketwrench-1.8.0/src/socketwrench/__init__.py` & `socketwrench-1.8.1/src/socketwrench/__init__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.0/src/socketwrench/__main__.py` & `socketwrench-1.8.1/src/socketwrench/__main__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.0/src/socketwrench/connection.py` & `socketwrench-1.8.1/src/socketwrench/connection.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.0/src/socketwrench/handlers.py` & `socketwrench-1.8.1/src/socketwrench/handlers.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.0/src/socketwrench/openapi.py` & `socketwrench-1.8.1/src/socketwrench/openapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,15 +77,26 @@
                                 module = __import__("socketwrench.types", fromlist=[class_name])
                                 return_type = getattr(module, class_name)
                             except:
                                 return_type = Response
                 except:
                     pass
             if return_type is not inspect._empty:
-                if return_type is Path or issubclass(return_type, Path) or return_type is FileResponse or issubclass(return_type, FileResponse):
+                if return_type is None:
+                    route_info["responses"] = {
+                        "200": {
+                            "description": "Success",
+                            "content": {
+                                "application/json": {
+                                    "schema": {"type": "object"}
+                                }
+                            }
+                        }
+                    }
+                elif return_type is Path or issubclass(return_type, Path) or return_type is FileResponse or issubclass(return_type, FileResponse):
                     content_type = getattr(return_type, "default_content_type", "application/octet-stream")
                     route_info["responses"] = {
                         "200": {
                             "description": "File response",
                             "content": {
                                 content_type: {
                                     "schema": {"type": "string", "format": "binary"}
@@ -145,8 +156,8 @@
             if gettag(func, "do_not_serve", False):
                 tags.append("private")
             route_info["tags"] = tags
 
         openapi["paths"][route_name] = {}
         for method in allowed_methods:
             openapi["paths"][route_name][method.lower()] = route_info
-    return openapi
+    return openapi
```

### Comparing `socketwrench-1.8.0/src/socketwrench/resources/favicon.ico` & `socketwrench-1.8.1/src/socketwrench/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.0/src/socketwrench/resources/playground/panels.js` & `socketwrench-1.8.1/src/socketwrench/resources/playground/panels.js`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.0/src/socketwrench/resources/playground/playground.html` & `socketwrench-1.8.1/src/socketwrench/resources/playground/playground.html`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.0/src/socketwrench/resources/playground/playground.js` & `socketwrench-1.8.1/src/socketwrench/resources/playground/playground.js`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.0/src/socketwrench/resources/swagger.html` & `socketwrench-1.8.1/src/socketwrench/resources/swagger.html`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.0/src/socketwrench/samples/file_sample.py` & `socketwrench-1.8.1/src/socketwrench/samples/file_sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.0/src/socketwrench/samples/sample.py` & `socketwrench-1.8.1/src/socketwrench/samples/sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.0/src/socketwrench/server.py` & `socketwrench-1.8.1/src/socketwrench/server.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.0/src/socketwrench/tags.py` & `socketwrench-1.8.1/src/socketwrench/tags.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.0/src/socketwrench/types.py` & `socketwrench-1.8.1/src/socketwrench/types.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.0/src/socketwrench.egg-info/PKG-INFO` & `socketwrench-1.8.1/src/socketwrench.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.8.0
+Version: 1.8.1
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -34,14 +34,24 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # socketwrench
 A webserver based on `socket.socket` with no dependencies other than the standard library.
 Provides a lightweight quickstart to make an API which supports OpenAPI, Swagger, and more.
 
+## NOTE:
+this is **not** a production-ready web server. It is a learning tool and a lightweight way to make a simple API. While I attempted to reduce overhead in calls, I haven't taken time to thoroughly optimize, and I have not implemented any complex features to deal with security, performance, or scalability.
+
+## Project Goals
+Part of the goal of this project was to understand how web servers work and to make a simple web server that is easy to use and understand.
+As learning progressed, features were added, but the code became a bit more complex.
+To learn more about the basics of web servers and how to develop one from scratch, see [learning.md](./learning.md) or jump straight into the 
+building blocks of source code in [simplestsocketwrench.py](./src/simplestsocketwrench.py) => [simplesocketwrench.py](./src/simplesocketwrench.py) => [socketwrench](./src/socketwrench).
+If you would prefer to use this library, read on!
+
 # Quickstart
 ### Install
 ```bash
 pip install socketwrench
 ```
 
 ### Serve a class
```

### Comparing `socketwrench-1.8.0/src/socketwrench.egg-info/SOURCES.txt` & `socketwrench-1.8.1/src/socketwrench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

