# Comparing `tmp/ln-markets-2.0.5.tar.gz` & `tmp/ln_markets-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ln-markets-2.0.5.tar", last modified: Tue Jan  2 15:18:16 2024, max compression
+gzip compressed data, was "ln_markets-2.0.6.tar", last modified: Tue May  7 16:29:45 2024, max compression
```

## Comparing `ln-markets-2.0.5.tar` & `ln_markets-2.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2024-01-02 15:18:16.399321 ln-markets-2.0.5/
--rw-r--r--   0 romain     (501) staff       (20)     1067 2023-12-19 14:58:01.000000 ln-markets-2.0.5/LICENSE
--rw-r--r--   0 romain     (501) staff       (20)    14929 2024-01-02 15:18:16.399109 ln-markets-2.0.5/PKG-INFO
--rw-r--r--   0 romain     (501) staff       (20)    14036 2023-12-19 14:58:01.000000 ln-markets-2.0.5/README.md
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2024-01-02 15:18:16.398916 ln-markets-2.0.5/ln_markets.egg-info/
--rw-r--r--   0 romain     (501) staff       (20)    14929 2024-01-02 15:18:16.000000 ln-markets-2.0.5/ln_markets.egg-info/PKG-INFO
--rw-r--r--   0 romain     (501) staff       (20)      309 2024-01-02 15:18:16.000000 ln-markets-2.0.5/ln_markets.egg-info/SOURCES.txt
--rw-r--r--   0 romain     (501) staff       (20)        1 2024-01-02 15:18:16.000000 ln-markets-2.0.5/ln_markets.egg-info/dependency_links.txt
--rw-r--r--   0 romain     (501) staff       (20)       26 2024-01-02 15:18:16.000000 ln-markets-2.0.5/ln_markets.egg-info/requires.txt
--rw-r--r--   0 romain     (501) staff       (20)       10 2024-01-02 15:18:16.000000 ln-markets-2.0.5/ln_markets.egg-info/top_level.txt
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2024-01-02 15:18:16.398639 ln-markets-2.0.5/lnmarkets/
--rw-r--r--   0 romain     (501) staff       (20)        1 2023-12-19 14:58:01.000000 ln-markets-2.0.5/lnmarkets/__init__.py
--rw-r--r--   0 romain     (501) staff       (20)    13719 2024-01-02 15:17:54.000000 ln-markets-2.0.5/lnmarkets/rest.py
--rw-r--r--   0 romain     (501) staff       (20)     2359 2023-12-19 14:58:01.000000 ln-markets-2.0.5/lnmarkets/websockets.py
--rw-r--r--   0 romain     (501) staff       (20)      104 2023-12-19 14:58:01.000000 ln-markets-2.0.5/pyproject.toml
--rw-r--r--   0 romain     (501) staff       (20)       89 2024-01-02 15:18:16.399482 ln-markets-2.0.5/setup.cfg
--rw-r--r--   0 romain     (501) staff       (20)     1192 2024-01-02 15:17:54.000000 ln-markets-2.0.5/setup.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2024-01-02 15:18:16.398760 ln-markets-2.0.5/tests/
--rw-r--r--   0 romain     (501) staff       (20)        1 2023-12-19 14:58:01.000000 ln-markets-2.0.5/tests/test_node_state.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2024-05-07 16:29:45.937348 ln_markets-2.0.6/
+-rw-r--r--   0 romain     (501) staff       (20)     1067 2023-12-19 14:58:01.000000 ln_markets-2.0.6/LICENSE
+-rw-r--r--   0 romain     (501) staff       (20)    14919 2024-05-07 16:29:45.937222 ln_markets-2.0.6/PKG-INFO
+-rw-r--r--   0 romain     (501) staff       (20)    14026 2024-05-07 16:29:24.000000 ln_markets-2.0.6/README.md
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2024-05-07 16:29:45.936995 ln_markets-2.0.6/ln_markets.egg-info/
+-rw-r--r--   0 romain     (501) staff       (20)    14919 2024-05-07 16:29:45.000000 ln_markets-2.0.6/ln_markets.egg-info/PKG-INFO
+-rw-r--r--   0 romain     (501) staff       (20)      309 2024-05-07 16:29:45.000000 ln_markets-2.0.6/ln_markets.egg-info/SOURCES.txt
+-rw-r--r--   0 romain     (501) staff       (20)        1 2024-05-07 16:29:45.000000 ln_markets-2.0.6/ln_markets.egg-info/dependency_links.txt
+-rw-r--r--   0 romain     (501) staff       (20)       26 2024-05-07 16:29:45.000000 ln_markets-2.0.6/ln_markets.egg-info/requires.txt
+-rw-r--r--   0 romain     (501) staff       (20)       10 2024-05-07 16:29:45.000000 ln_markets-2.0.6/ln_markets.egg-info/top_level.txt
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2024-05-07 16:29:45.936687 ln_markets-2.0.6/lnmarkets/
+-rw-r--r--   0 romain     (501) staff       (20)        1 2023-12-19 14:58:01.000000 ln_markets-2.0.6/lnmarkets/__init__.py
+-rw-r--r--   0 romain     (501) staff       (20)    13721 2024-05-07 16:29:24.000000 ln_markets-2.0.6/lnmarkets/rest.py
+-rw-r--r--   0 romain     (501) staff       (20)     2359 2023-12-19 14:58:01.000000 ln_markets-2.0.6/lnmarkets/websockets.py
+-rw-r--r--   0 romain     (501) staff       (20)      104 2023-12-19 14:58:01.000000 ln_markets-2.0.6/pyproject.toml
+-rw-r--r--   0 romain     (501) staff       (20)       89 2024-05-07 16:29:45.937525 ln_markets-2.0.6/setup.cfg
+-rw-r--r--   0 romain     (501) staff       (20)     1192 2024-05-07 16:29:24.000000 ln_markets-2.0.6/setup.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2024-05-07 16:29:45.936812 ln_markets-2.0.6/tests/
+-rw-r--r--   0 romain     (501) staff       (20)        1 2023-12-19 14:58:01.000000 ln_markets-2.0.6/tests/test_node_state.py
```

### Comparing `ln-markets-2.0.5/LICENSE` & `ln_markets-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ln-markets-2.0.5/PKG-INFO` & `ln_markets-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ln-markets
-Version: 2.0.5
+Version: 2.0.6
 Summary: LN Markets API python implementation
 Home-page: https://github.com/ln-markets/api-python
 Author: Romain ROUPHAEL
 License: MIT
 Keywords: lnmarkets trading rest api bitcoin lightning network futures options
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -220,15 +220,15 @@
 ```
 # No parameters
 ```
 
 Example:
 
 ```python
-lnm.futures_close_all_positions()
+lnm.futures_close_all()
 ```
 
 [`DELETE /futures/all/close`](https://docs.lnmarkets.com/api/v2) documentation for more details.
 
 ### futures_cancel
 
 Cancel a specific trade for this user.
```

### Comparing `ln-markets-2.0.5/README.md` & `ln_markets-2.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
 ```
 # No parameters
 ```
 
 Example:
 
 ```python
-lnm.futures_close_all_positions()
+lnm.futures_close_all()
 ```
 
 [`DELETE /futures/all/close`](https://docs.lnmarkets.com/api/v2) documentation for more details.
 
 ### futures_cancel
 
 Cancel a specific trade for this user.
```

### Comparing `ln-markets-2.0.5/ln_markets.egg-info/PKG-INFO` & `ln_markets-2.0.6/ln_markets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ln-markets
-Version: 2.0.5
+Version: 2.0.6
 Summary: LN Markets API python implementation
 Home-page: https://github.com/ln-markets/api-python
 Author: Romain ROUPHAEL
 License: MIT
 Keywords: lnmarkets trading rest api bitcoin lightning network futures options
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -220,15 +220,15 @@
 ```
 # No parameters
 ```
 
 Example:
 
 ```python
-lnm.futures_close_all_positions()
+lnm.futures_close_all()
 ```
 
 [`DELETE /futures/all/close`](https://docs.lnmarkets.com/api/v2) documentation for more details.
 
 ### futures_cancel
 
 Cancel a specific trade for this user.
```

### Comparing `ln-markets-2.0.5/lnmarkets/rest.py` & `ln_markets-2.0.6/lnmarkets/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
         return self.before_request_api(method, path, params, credentials)
     
     
     def futures_get_trade(self, params):
         method = 'GET'
         trade_id = params.get('id')  
         path = f'/futures/trades/{trade_id}'
-        credentials = False
+        credentials = True
 
         return self.before_request_api(method, path, params, credentials)
 
     
 
 
     ## Options
@@ -432,15 +432,15 @@
         path = '/user/notifications'
         credentials = True
         params = {}
         
         return self.before_request_api(method, path, params, credentials)
     
     def mark_notifications_read(self):
-        method = 'PUT'
+        method = 'DELETE'
         path = '/user/notifications/all'
         credentials = True
         params = {}
         
         return self.before_request_api(method, path, params, credentials)
```

### Comparing `ln-markets-2.0.5/lnmarkets/websockets.py` & `ln_markets-2.0.6/lnmarkets/websockets.py`

 * *Files identical despite different names*

### Comparing `ln-markets-2.0.5/setup.py` & `ln_markets-2.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='ln-markets',
-    version='2.0.5',
+    version='2.0.6',
     packages=['lnmarkets'],
     description='LN Markets API python implementation',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ln-markets/api-python',
     author='Romain ROUPHAEL',
     license='MIT',
```

