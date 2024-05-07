# Comparing `tmp/xwl-1.0.0.tar.gz` & `tmp/xwl-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xwl-1.0.0.tar", last modified: Mon Mar  4 10:52:30 2024, max compression
+gzip compressed data, was "xwl-1.0.1.tar", last modified: Tue May  7 09:56:36 2024, max compression
```

## Comparing `xwl-1.0.0.tar` & `xwl-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,33 @@
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-03-04 10:52:30.488045 xwl-1.0.0/
--rw-r--r--   0 xju       (1001) xju       (1001)     2153 2024-03-04 10:52:30.484045 xwl-1.0.0/PKG-INFO
--rw-r--r--   0 xju       (1001) xju       (1001)      617 2024-03-04 10:52:29.000000 xwl-1.0.0/README.rst
--rw-r--r--   0 xju       (1001) xju       (1001)     1060 2024-03-04 10:52:29.000000 xwl-1.0.0/pyproject.toml
--rw-r--r--   0 xju       (1001) xju       (1001)       38 2024-03-04 10:52:30.488045 xwl-1.0.0/setup.cfg
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-03-04 10:52:30.484045 xwl-1.0.0/src/
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-03-04 10:52:30.484045 xwl-1.0.0/src/xwl/
--rw-r--r--   0 xju       (1001) xju       (1001)     8102 2024-03-03 04:27:40.000000 xwl-1.0.0/src/xwl/__init__.py
--rw-r--r--   0 xju       (1001) xju       (1001)    10161 2024-03-04 10:49:55.000000 xwl-1.0.0/src/xwl/dispatcher.py
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-03-04 10:52:30.484045 xwl-1.0.0/src/xwl/example/
--rw-r--r--   0 xju       (1001) xju       (1001)     3928 2024-03-04 10:50:36.000000 xwl-1.0.0/src/xwl/example/app.py
--rwxr-xr-x   0 xju       (1001) xju       (1001)     1359 2024-03-04 10:50:31.000000 xwl-1.0.0/src/xwl/example/mt-server.py
--rwxr-xr-x   0 xju       (1001) xju       (1001)     1288 2024-03-04 10:50:49.000000 xwl-1.0.0/src/xwl/example/server.py
--rw-r--r--   0 xju       (1001) xju       (1001)      870 2024-03-04 10:50:19.000000 xwl-1.0.0/src/xwl/example/submodule.py
--rwxr-xr-x   0 xju       (1001) xju       (1001)     7863 2024-03-04 10:49:38.000000 xwl-1.0.0/src/xwl/example.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     7874 2024-03-03 04:00:45.000000 xwl-1.0.0/src/xwl/wsgi.py
--rw-r--r--   0 xju       (1001) xju       (1001)     2380 2024-03-04 10:49:47.000000 xwl-1.0.0/src/xwl/wsgi.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2349 2024-03-04 10:52:27.000000 xwl-1.0.0/src/xwl/xwl.py.test
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-03-04 10:52:30.484045 xwl-1.0.0/src/xwl.egg-info/
--rw-r--r--   0 xju       (1001) xju       (1001)     2153 2024-03-04 10:52:30.000000 xwl-1.0.0/src/xwl.egg-info/PKG-INFO
--rw-r--r--   0 xju       (1001) xju       (1001)      409 2024-03-04 10:52:30.000000 xwl-1.0.0/src/xwl.egg-info/SOURCES.txt
--rw-r--r--   0 xju       (1001) xju       (1001)        1 2024-03-04 10:52:30.000000 xwl-1.0.0/src/xwl.egg-info/dependency_links.txt
--rw-r--r--   0 xju       (1001) xju       (1001)        7 2024-03-04 10:52:30.000000 xwl-1.0.0/src/xwl.egg-info/requires.txt
--rw-r--r--   0 xju       (1001) xju       (1001)        4 2024-03-04 10:52:30.000000 xwl-1.0.0/src/xwl.egg-info/top_level.txt
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-05-07 09:56:36.932978 xwl-1.0.1/
+-rw-r--r--   0 xju       (1001) xju       (1001)     1064 2024-05-07 09:56:35.000000 xwl-1.0.1/MIT-LICENCE
+-rw-r--r--   0 xju       (1001) xju       (1001)     2279 2024-05-07 09:56:36.932978 xwl-1.0.1/PKG-INFO
+-rw-r--r--   0 xju       (1001) xju       (1001)      721 2024-05-07 09:56:35.000000 xwl-1.0.1/README.rst
+-rw-r--r--   0 xju       (1001) xju       (1001)     1088 2024-05-07 09:56:35.000000 xwl-1.0.1/pyproject.toml
+-rw-r--r--   0 xju       (1001) xju       (1001)       38 2024-05-07 09:56:36.932978 xwl-1.0.1/setup.cfg
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-05-07 09:56:36.928978 xwl-1.0.1/src/
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-05-07 09:56:36.928978 xwl-1.0.1/src/xwl/
+-rw-r--r--   0 xju       (1001) xju       (1001)     8102 2024-03-03 04:27:40.000000 xwl-1.0.1/src/xwl/__init__.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    10114 2024-03-12 21:51:46.000000 xwl-1.0.1/src/xwl/dispatcher.py
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-05-07 09:56:36.928978 xwl-1.0.1/src/xwl/example/
+-rw-r--r--   0 xju       (1001) xju       (1001)     1002 2024-03-03 04:37:21.000000 xwl-1.0.1/src/xwl/example/1.svg.gz
+-rw-r--r--   0 xju       (1001) xju       (1001)     3928 2024-03-04 10:50:36.000000 xwl-1.0.1/src/xwl/example/app.py
+-rwxr-xr-x   0 xju       (1001) xju       (1001)     1359 2024-03-04 10:50:31.000000 xwl-1.0.1/src/xwl/example/mt-server.py
+-rwxr-xr-x   0 xju       (1001) xju       (1001)     1288 2024-03-04 10:50:49.000000 xwl-1.0.1/src/xwl/example/server.py
+-rw-r--r--   0 xju       (1001) xju       (1001)      870 2024-03-04 10:50:19.000000 xwl-1.0.1/src/xwl/example/submodule.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     2872 2024-03-04 10:50:55.000000 xwl-1.0.1/src/xwl/example/test.html
+-rw-r--r--   0 xju       (1001) xju       (1001)     4857 2024-03-04 10:51:01.000000 xwl-1.0.1/src/xwl/example/test.js
+-rw-r--r--   0 xju       (1001) xju       (1001)     1263 2024-03-04 10:50:44.000000 xwl-1.0.1/src/xwl/example/test2.html
+-rw-r--r--   0 xju       (1001) xju       (1001)     1920 2024-03-04 10:50:24.000000 xwl-1.0.1/src/xwl/example/test2.js
+-rw-r--r--   0 xju       (1001) xju       (1001)    33381 2024-03-04 10:51:08.000000 xwl-1.0.1/src/xwl/example/xwl.js
+-rwxr-xr-x   0 xju       (1001) xju       (1001)     7863 2024-03-04 10:49:38.000000 xwl-1.0.1/src/xwl/example.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)        0 2024-05-07 09:56:35.000000 xwl-1.0.1/src/xwl/py.typed
+-rw-r--r--   0 xju       (1001) xju       (1001)     7874 2024-03-03 04:00:45.000000 xwl-1.0.1/src/xwl/wsgi.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     2380 2024-03-04 10:49:47.000000 xwl-1.0.1/src/xwl/wsgi.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    33381 2024-03-04 10:51:08.000000 xwl-1.0.1/src/xwl/xwl.js
+-rw-r--r--   0 xju       (1001) xju       (1001)     2349 2024-03-04 10:52:27.000000 xwl-1.0.1/src/xwl/xwl.py.test
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-05-07 09:56:36.928978 xwl-1.0.1/src/xwl.egg-info/
+-rw-r--r--   0 xju       (1001) xju       (1001)     2279 2024-05-07 09:56:36.000000 xwl-1.0.1/src/xwl.egg-info/PKG-INFO
+-rw-r--r--   0 xju       (1001) xju       (1001)      603 2024-05-07 09:56:36.000000 xwl-1.0.1/src/xwl.egg-info/SOURCES.txt
+-rw-r--r--   0 xju       (1001) xju       (1001)        1 2024-05-07 09:56:36.000000 xwl-1.0.1/src/xwl.egg-info/dependency_links.txt
+-rw-r--r--   0 xju       (1001) xju       (1001)        7 2024-05-07 09:56:36.000000 xwl-1.0.1/src/xwl.egg-info/requires.txt
+-rw-r--r--   0 xju       (1001) xju       (1001)        4 2024-05-07 09:56:36.000000 xwl-1.0.1/src/xwl.egg-info/top_level.txt
```

### Comparing `xwl-1.0.0/PKG-INFO` & `xwl-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xwl
-Version: 1.0.0
+Version: 1.0.1
 Summary: xwl library
 Author: Trevor Taylor
 License: Copyright © 2022 Trevor Taylor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -14,24 +14,31 @@
 Project-URL: Homepage, https://github.com/urnest/urnest
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
+Requires-Dist: xju>=2
 
 xwl python library
 ------------------
 
 WSGI dispatcher that maps HTTP requests to python functions of same/similar name.
 
 * function params taken from query string and/or POST content
 * function access control via python decorators
 * JSON support for parameters and responses
 * small javascript library with convenience async postToServer
 * and getFromServer functions
 
+(see the bottom of this readme for release history)
+
 see `xwl.example <xwl/example>`_ which implements a HTTP
 `server.py <xwl/example/server.py>`_ using
 `dispatcher.py <xwl/dispatcher.py>`_ to map HTTP requests to
 `app <xwl/example/app.py>`_ and
 `app.submodule <xwl/example.submodule.py>`_ functions
+
+Release History
+
+- 1.0.1 add missing files to whl
```

### Comparing `xwl-1.0.0/README.rst` & `xwl-1.0.1/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -5,12 +5,18 @@
 
 * function params taken from query string and/or POST content
 * function access control via python decorators
 * JSON support for parameters and responses
 * small javascript library with convenience async postToServer
 * and getFromServer functions
 
+(see the bottom of this readme for release history)
+
 see `xwl.example <xwl/example>`_ which implements a HTTP
 `server.py <xwl/example/server.py>`_ using
 `dispatcher.py <xwl/dispatcher.py>`_ to map HTTP requests to
 `app <xwl/example/app.py>`_ and
 `app.submodule <xwl/example.submodule.py>`_ functions
+
+Release History
+
+- 1.0.1 add missing files to whl
```

### Comparing `xwl-1.0.0/pyproject.toml` & `xwl-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "xwl"
-version = "1.0.0"
+version = "1.0.1"
 description = "xwl library"
 readme = "README.rst"
 authors = [{ name = "Trevor Taylor"}]
 license = { file = "MIT-LICENCE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -20,8 +20,8 @@
 Homepage = "https://github.com/urnest/urnest"
 [tool.setuptools.packages.find]
 where = ["src"]  # list of folders that contain the packages (["."] by default)
 include = ["xwl","xwl.*","xwl.example.*"]  # package names should match these glob patterns (["*"] by default)
 exclude = []  # exclude packages matching these glob patterns (empty by default)
 namespaces = true  # to disable scanning PEP 420 namespaces (true by default)
 [tool.setuptools.package-data]
-xwl = [ "./example.py.test","./wsgi.py.test","./xwl.py.test", "py.typed"]
+xwl = [ "./example.py.test","./wsgi.py.test","./xwl.py.test", "./py.typed", "example/*", "./xwl.js" ]
```

### Comparing `xwl-1.0.0/src/xwl/__init__.py` & `xwl-1.0.1/src/xwl/__init__.py`

 * *Files identical despite different names*

### Comparing `xwl-1.0.0/src/xwl/dispatcher.py` & `xwl-1.0.1/src/xwl/dispatcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         request_param_names=request_params.keys()
         request_attr_names=request_attrs.keys()
         param_default_names=param_defaults.keys()
         raise in_context('get value of %(param_name)s from params supplied as json-encoded "json_params" HTTP param (%(json_param_names)s), HTTP params (%(request_param_names)s), webapp2 request attributes (%(request_attr_names)s) or function paramter defaults (%(param_default_names)s)'%vars()) from None
     pass
 
 def makeParams(remote_addr,method,headers,params,url,referer,cookies,f):
-    'make dictionary of params for calling function %(f)s, getting them from remote_addr, method, headers, GET/POST params, url, cookies'''
+    '''make dictionary of params for calling function %(f)s, getting them from remote_addr, method, headers, GET/POST params, url, cookies'''
     try:
         json_params=fromJson(params.get('json_params','{}'))
         param_names=f.__code__.co_varnames[0:f.__code__.co_argcount]
         func_defaults=f.__defaults__ or []
         no_default_params=len(param_names)-len(func_defaults)
         param_defaults=dict([ (param_name,default_value) for param_name,default_value in zip(param_names[no_default_params:],func_defaults)])
         #request.__dict__ does not give us anything useful
@@ -167,18 +167,16 @@
             self.log('INFO: {name} used {mod.__name__}.{fname}()'.format(**vars()))
             result=promoteContent(result)
             headers=result.cookieHeaders()
             if result.location:
                 headers.append( ('Location',result.location) )
                 start_response('303 See Other',headers)
                 return [''.encode('utf-8')]
-            headers.extend([(n,v) for n,v in result.headers
-                            if not n in ('Content-Type','Content-Encoding')])
-            c=dict([ (n,v) for n,v in result.headers
-                     if n in ('Content-Type','Content-Encoding')])
+            headers.extend([(n,v) for n,v in result.headers if not n in ('Content-Type','Content-Encoding')])
+            c=dict([ (n,v) for n,v in result.headers if n in ('Content-Type','Content-Encoding')])
             if result.contentType: c['Content-Type']=result.contentType
             if result.contentEncoding: c['Content-Encoding']=result.contentEncoding
             headers.extend(c.items())
             start_response('200 OK',headers)
             return [result.content]
         except:
             raise in_context(l1(Dispatcher.dispatchToFunction.__doc__).format(
```

### Comparing `xwl-1.0.0/src/xwl/example/app.py` & `xwl-1.0.1/src/xwl/example/app.py`

 * *Files identical despite different names*

### Comparing `xwl-1.0.0/src/xwl/example/mt-server.py` & `xwl-1.0.1/src/xwl/example/mt-server.py`

 * *Files identical despite different names*

### Comparing `xwl-1.0.0/src/xwl/example/server.py` & `xwl-1.0.1/src/xwl/example/server.py`

 * *Files identical despite different names*

### Comparing `xwl-1.0.0/src/xwl/example/submodule.py` & `xwl-1.0.1/src/xwl/example/submodule.py`

 * *Files identical despite different names*

### Comparing `xwl-1.0.0/src/xwl/example.py.test` & `xwl-1.0.1/src/xwl/example.py.test`

 * *Files identical despite different names*

### Comparing `xwl-1.0.0/src/xwl/wsgi.py` & `xwl-1.0.1/src/xwl/wsgi.py`

 * *Files identical despite different names*

### Comparing `xwl-1.0.0/src/xwl/wsgi.py.test` & `xwl-1.0.1/src/xwl/wsgi.py.test`

 * *Files identical despite different names*

### Comparing `xwl-1.0.0/src/xwl/xwl.py.test` & `xwl-1.0.1/src/xwl/xwl.py.test`

 * *Files identical despite different names*

### Comparing `xwl-1.0.0/src/xwl.egg-info/PKG-INFO` & `xwl-1.0.1/src/xwl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xwl
-Version: 1.0.0
+Version: 1.0.1
 Summary: xwl library
 Author: Trevor Taylor
 License: Copyright © 2022 Trevor Taylor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -14,24 +14,31 @@
 Project-URL: Homepage, https://github.com/urnest/urnest
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
+Requires-Dist: xju>=2
 
 xwl python library
 ------------------
 
 WSGI dispatcher that maps HTTP requests to python functions of same/similar name.
 
 * function params taken from query string and/or POST content
 * function access control via python decorators
 * JSON support for parameters and responses
 * small javascript library with convenience async postToServer
 * and getFromServer functions
 
+(see the bottom of this readme for release history)
+
 see `xwl.example <xwl/example>`_ which implements a HTTP
 `server.py <xwl/example/server.py>`_ using
 `dispatcher.py <xwl/dispatcher.py>`_ to map HTTP requests to
 `app <xwl/example/app.py>`_ and
 `app.submodule <xwl/example.submodule.py>`_ functions
+
+Release History
+
+- 1.0.1 add missing files to whl
```

