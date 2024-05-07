# Comparing `tmp/joker-clients-0.2.4.tar.gz` & `tmp/joker-clients-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joker-clients-0.2.4.tar", last modified: Wed Apr 24 01:01:04 2024, max compression
+gzip compressed data, was "joker-clients-0.3.0.tar", last modified: Tue May  7 08:05:32 2024, max compression
```

## Comparing `joker-clients-0.2.4.tar` & `joker-clients-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-24 01:01:04.795645 joker-clients-0.2.4/
--rw-r--r--   0 Hailong    (502) staff       (20)    35149 2022-11-02 01:25:38.000000 joker-clients-0.2.4/LICENSE
--rw-r--r--   0 Hailong    (502) staff       (20)       24 2022-11-02 01:25:38.000000 joker-clients-0.2.4/MANIFEST.in
--rw-r--r--   0 Hailong    (502) staff       (20)     1422 2024-04-24 01:01:04.795366 joker-clients-0.2.4/PKG-INFO
--rw-r--r--   0 Hailong    (502) staff       (20)      533 2022-11-02 08:02:40.000000 joker-clients-0.2.4/README.md
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-24 01:01:04.786518 joker-clients-0.2.4/joker/
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-24 01:01:04.792232 joker-clients-0.2.4/joker/clients/
--rw-r--r--   0 Hailong    (502) staff       (20)      333 2024-04-24 01:00:09.000000 joker-clients-0.2.4/joker/clients/__init__.py
--rw-r--r--   0 Hailong    (502) staff       (20)     2372 2024-04-24 00:59:51.000000 joker-clients-0.2.4/joker/clients/cas.py
--rw-r--r--   0 Hailong    (502) staff       (20)     3366 2024-03-22 07:54:34.000000 joker-clients-0.2.4/joker/clients/email.py
--rw-r--r--   0 Hailong    (502) staff       (20)      386 2024-03-22 07:54:34.000000 joker-clients-0.2.4/joker/clients/files.py
--rw-r--r--   0 Hailong    (502) staff       (20)     3044 2024-03-22 08:21:27.000000 joker-clients-0.2.4/joker/clients/http.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1316 2024-03-22 07:54:34.000000 joker-clients-0.2.4/joker/clients/monolog.py
--rw-r--r--   0 Hailong    (502) staff       (20)     4058 2024-04-24 00:59:55.000000 joker-clients-0.2.4/joker/clients/printable.py
--rw-r--r--   0 Hailong    (502) staff       (20)     3832 2024-04-24 00:59:51.000000 joker-clients-0.2.4/joker/clients/utils.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-24 01:01:04.794911 joker-clients-0.2.4/joker_clients.egg-info/
--rw-r--r--   0 Hailong    (502) staff       (20)     1422 2024-04-24 01:01:04.000000 joker-clients-0.2.4/joker_clients.egg-info/PKG-INFO
--rw-r--r--   0 Hailong    (502) staff       (20)      511 2024-04-24 01:01:04.000000 joker-clients-0.2.4/joker_clients.egg-info/SOURCES.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        1 2024-04-24 01:01:04.000000 joker-clients-0.2.4/joker_clients.egg-info/dependency_links.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        6 2024-04-24 01:01:04.000000 joker-clients-0.2.4/joker_clients.egg-info/namespace_packages.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        1 2023-07-25 09:13:10.000000 joker-clients-0.2.4/joker_clients.egg-info/not-zip-safe
--rw-r--r--   0 Hailong    (502) staff       (20)       52 2024-04-24 01:01:04.000000 joker-clients-0.2.4/joker_clients.egg-info/requires.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        6 2024-04-24 01:01:04.000000 joker-clients-0.2.4/joker_clients.egg-info/top_level.txt
--rw-r--r--   0 Hailong    (502) staff       (20)       51 2024-03-21 10:39:12.000000 joker-clients-0.2.4/requirements.txt
--rw-r--r--   0 Hailong    (502) staff       (20)       38 2024-04-24 01:01:04.795776 joker-clients-0.2.4/setup.cfg
--rw-r--r--   0 Hailong    (502) staff       (20)     2087 2024-03-22 08:23:35.000000 joker-clients-0.2.4/setup.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-05-07 08:05:32.355369 joker-clients-0.3.0/
+-rw-r--r--   0 Hailong    (502) staff       (20)    35149 2022-11-02 01:25:38.000000 joker-clients-0.3.0/LICENSE
+-rw-r--r--   0 Hailong    (502) staff       (20)       24 2022-11-02 01:25:38.000000 joker-clients-0.3.0/MANIFEST.in
+-rw-r--r--   0 Hailong    (502) staff       (20)     1422 2024-05-07 08:05:32.354961 joker-clients-0.3.0/PKG-INFO
+-rw-r--r--   0 Hailong    (502) staff       (20)      533 2022-11-02 08:02:40.000000 joker-clients-0.3.0/README.md
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-05-07 08:05:32.344445 joker-clients-0.3.0/joker/
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-05-07 08:05:32.351076 joker-clients-0.3.0/joker/clients/
+-rw-r--r--   0 Hailong    (502) staff       (20)      333 2024-05-07 08:04:05.000000 joker-clients-0.3.0/joker/clients/__init__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     2229 2024-05-07 08:01:44.000000 joker-clients-0.3.0/joker/clients/cas.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     3366 2024-03-22 07:54:34.000000 joker-clients-0.3.0/joker/clients/email.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      386 2024-03-22 07:54:34.000000 joker-clients-0.3.0/joker/clients/files.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     3044 2024-03-22 08:21:27.000000 joker-clients-0.3.0/joker/clients/http.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1316 2024-03-22 07:54:34.000000 joker-clients-0.3.0/joker/clients/monolog.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     4058 2024-05-07 08:01:42.000000 joker-clients-0.3.0/joker/clients/printable.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     3826 2024-05-07 08:01:44.000000 joker-clients-0.3.0/joker/clients/utils.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-05-07 08:05:32.354387 joker-clients-0.3.0/joker_clients.egg-info/
+-rw-r--r--   0 Hailong    (502) staff       (20)     1422 2024-05-07 08:05:32.000000 joker-clients-0.3.0/joker_clients.egg-info/PKG-INFO
+-rw-r--r--   0 Hailong    (502) staff       (20)      511 2024-05-07 08:05:32.000000 joker-clients-0.3.0/joker_clients.egg-info/SOURCES.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        1 2024-05-07 08:05:32.000000 joker-clients-0.3.0/joker_clients.egg-info/dependency_links.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        6 2024-05-07 08:05:32.000000 joker-clients-0.3.0/joker_clients.egg-info/namespace_packages.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        1 2023-07-25 09:13:10.000000 joker-clients-0.3.0/joker_clients.egg-info/not-zip-safe
+-rw-r--r--   0 Hailong    (502) staff       (20)       52 2024-05-07 08:05:32.000000 joker-clients-0.3.0/joker_clients.egg-info/requires.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        6 2024-05-07 08:05:32.000000 joker-clients-0.3.0/joker_clients.egg-info/top_level.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)       51 2024-03-21 10:39:12.000000 joker-clients-0.3.0/requirements.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)       38 2024-05-07 08:05:32.355498 joker-clients-0.3.0/setup.cfg
+-rw-r--r--   0 Hailong    (502) staff       (20)     2087 2024-03-22 08:23:35.000000 joker-clients-0.3.0/setup.py
```

### Comparing `joker-clients-0.2.4/LICENSE` & `joker-clients-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `joker-clients-0.2.4/PKG-INFO` & `joker-clients-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joker-clients
-Version: 0.2.4
+Version: 0.3.0
 Summary: simple clients for simple and dedicated services
 Home-page: https://github.com/frozflame/joker-clients
 Author: frozflame
 Author-email: frozflame@outlook.com
 License: GNU General Public License (GPL)
 Keywords: joker
 Classifier: Programming Language :: Python
```

### Comparing `joker-clients-0.2.4/README.md` & `joker-clients-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `joker-clients-0.2.4/joker/clients/email.py` & `joker-clients-0.3.0/joker/clients/email.py`

 * *Files identical despite different names*

### Comparing `joker-clients-0.2.4/joker/clients/http.py` & `joker-clients-0.3.0/joker/clients/http.py`

 * *Files identical despite different names*

### Comparing `joker-clients-0.2.4/joker/clients/monolog.py` & `joker-clients-0.3.0/joker/clients/monolog.py`

 * *Files identical despite different names*

### Comparing `joker-clients-0.2.4/joker/clients/printable.py` & `joker-clients-0.3.0/joker/clients/printable.py`

 * *Files identical despite different names*

### Comparing `joker-clients-0.2.4/joker/clients/utils.py` & `joker-clients-0.3.0/joker/clients/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 _logger = logging.getLogger(__name__)
 Pathlike = typing.Union[str, os.PathLike]
 
 
 class ResponseDict(dict):
     @property
     def code(self) -> int:
-        return self.get("code", 3)
+        return self.get("code", 0)
 
     @property
     def data(self):
         return self.get("data")
 
     @property
     def message(self):
-        return self.get("message", "OK")
+        return self.get("message")
 
 
 def dump_json_request_to_curl(method: str, url: str, data=None, aslist=False):
     method = method.upper()
     if method == "GET":
         parts = ["curl", url]
     else:
```

### Comparing `joker-clients-0.2.4/joker_clients.egg-info/PKG-INFO` & `joker-clients-0.3.0/joker_clients.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joker-clients
-Version: 0.2.4
+Version: 0.3.0
 Summary: simple clients for simple and dedicated services
 Home-page: https://github.com/frozflame/joker-clients
 Author: frozflame
 Author-email: frozflame@outlook.com
 License: GNU General Public License (GPL)
 Keywords: joker
 Classifier: Programming Language :: Python
```

### Comparing `joker-clients-0.2.4/setup.py` & `joker-clients-0.3.0/setup.py`

 * *Files identical despite different names*

