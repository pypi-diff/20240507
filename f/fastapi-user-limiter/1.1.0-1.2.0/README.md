# Comparing `tmp/fastapi_user_limiter-1.1.0.tar.gz` & `tmp/fastapi_user_limiter-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_user_limiter-1.1.0.tar", last modified: Mon May  6 12:04:45 2024, max compression
+gzip compressed data, was "fastapi_user_limiter-1.2.0.tar", last modified: Mon May  6 12:25:25 2024, max compression
```

## Comparing `fastapi_user_limiter-1.1.0.tar` & `fastapi_user_limiter-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:04:45.537661 fastapi_user_limiter-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-06 12:04:45.537661 fastapi_user_limiter-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-06 12:04:29.000000 fastapi_user_limiter-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-06 12:04:29.000000 fastapi_user_limiter-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 12:04:45.537661 fastapi_user_limiter-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:04:45.537661 fastapi_user_limiter-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:04:45.537661 fastapi_user_limiter-1.1.0/src/fastapi_user_limiter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:04:29.000000 fastapi_user_limiter-1.1.0/src/fastapi_user_limiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-05-06 12:04:29.000000 fastapi_user_limiter-1.1.0/src/fastapi_user_limiter/limiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:04:45.537661 fastapi_user_limiter-1.1.0/src/fastapi_user_limiter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-06 12:04:45.000000 fastapi_user_limiter-1.1.0/src/fastapi_user_limiter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-06 12:04:45.000000 fastapi_user_limiter-1.1.0/src/fastapi_user_limiter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 12:04:45.000000 fastapi_user_limiter-1.1.0/src/fastapi_user_limiter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-06 12:04:45.000000 fastapi_user_limiter-1.1.0/src/fastapi_user_limiter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-06 12:04:45.000000 fastapi_user_limiter-1.1.0/src/fastapi_user_limiter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:25:25.202324 fastapi_user_limiter-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-05-06 12:25:25.198324 fastapi_user_limiter-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-06 12:25:20.000000 fastapi_user_limiter-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-06 12:25:20.000000 fastapi_user_limiter-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 12:25:25.202324 fastapi_user_limiter-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:25:25.198324 fastapi_user_limiter-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:25:25.198324 fastapi_user_limiter-1.2.0/src/fastapi_user_limiter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:25:20.000000 fastapi_user_limiter-1.2.0/src/fastapi_user_limiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-05-06 12:25:20.000000 fastapi_user_limiter-1.2.0/src/fastapi_user_limiter/limiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:25:25.198324 fastapi_user_limiter-1.2.0/src/fastapi_user_limiter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-05-06 12:25:25.000000 fastapi_user_limiter-1.2.0/src/fastapi_user_limiter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-06 12:25:25.000000 fastapi_user_limiter-1.2.0/src/fastapi_user_limiter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 12:25:25.000000 fastapi_user_limiter-1.2.0/src/fastapi_user_limiter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-06 12:25:25.000000 fastapi_user_limiter-1.2.0/src/fastapi_user_limiter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-06 12:25:25.000000 fastapi_user_limiter-1.2.0/src/fastapi_user_limiter.egg-info/top_level.txt
```

### Comparing `fastapi_user_limiter-1.1.0/PKG-INFO` & `fastapi_user_limiter-1.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: fastapi_user_limiter
-Version: 1.1.0
-Summary: Rate-limiter for FastAPI with the possibility of user-based rate limits
-Author-email: Ramtin Yazdanian <ramtin.yazdanian@epfl.ch>
-Project-URL: Homepage, https://github.com/epflgraph/fastapi-user-limiter
-Project-URL: Bug Tracker, https://github.com/epflgraph/fastapi-user-limiter/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-Requires-Dist: fastapi[all]
-Requires-Dist: redis
-
 # FastAPI rate limiter
 
 This package adds a rate limiter to FastAPI using Redis.
 
 ## Installation
 
 First install Redis, then install the package using:
@@ -115,11 +100,49 @@
 @app.post("/auth",
           dependencies=[Depends(rate_limiter(3, 20,
                                              user=get_user))])
 async def read_with_auth(data: dict):
     return {'input': data}
 ```
 
-## Future features
+#### User-based rate limit overrides
+The async callable introduced above can be used to override `max_requests`
+and/or `window` values for specific users by returning a `dict` instead of
+a `str`. In the example below, the callable overrides and increases the 
+value of `max_requests` for the user `"admin"` and for the endpoint
+`/auth`:
+
+
+```python
+from fastapi_user_limiter.limiter import rate_limiter
+from fastapi import Depends, FastAPI
+from starlette.datastructures import Headers, URL
+
+
+app = FastAPI()
+
+
+# The user callable can return either of these two:
+# A. One single string containing the username
+# B. A dictionary that maps the key "username" to the username (obligatory), plus two optional keys:
+#     i. "max_requests": overriding the endpoint's original max_requests value for this particular user
+#     ii. "window": overriding the endpoint's original window value for this particular user
+# Provide a None to "max_requests" or "window" in order to disable rate limiting (for the given
+# user and endpoint).
+# If a dictionary without a "username" key is provided, an AssertionError is raised.
+
+async def get_user_with_override(headers: Headers, url: URL):
+    # This user callable returns a dictionary and overrides max_requests for the user "admin"
+    # when the endpoint's URL is '/auth'.
+    username = headers['authorization'].replace('Bearer ', '')
+    result_dict = {"username": username}
+    if username == 'admin' and url.path == '/auth':
+        result_dict['max_requests'] = 7
+    return result_dict
 
-The package will soon have the additional feature of allowing each user account to have a different window size and max 
-request count for each endpoint.
+# 3 requests max per 20 seconds, per user
+@app.post("/auth",
+          dependencies=[Depends(rate_limiter(3, 20,
+                                             user=get_user_with_override))])
+async def read_with_auth(data: dict):
+    return {'input': data}
+```
```

### Comparing `fastapi_user_limiter-1.1.0/pyproject.toml` & `fastapi_user_limiter-1.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastapi_user_limiter"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="Ramtin Yazdanian", email="ramtin.yazdanian@epfl.ch" }
 ]
 description = "Rate-limiter for FastAPI with the possibility of user-based rate limits"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `fastapi_user_limiter-1.1.0/src/fastapi_user_limiter/limiter.py` & `fastapi_user_limiter-1.2.0/src/fastapi_user_limiter/limiter.py`

 * *Files identical despite different names*

