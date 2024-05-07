# Comparing `tmp/ratelimitedqueues-0.0.1a7.tar.gz` & `tmp/ratelimitedqueues-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratelimitedqueues-0.0.1a7.tar", last modified: Mon Apr 29 10:38:49 2024, max compression
+gzip compressed data, was "ratelimitedqueues-0.0.2.tar", last modified: Tue May  7 21:35:42 2024, max compression
```

## Comparing `ratelimitedqueues-0.0.1a7.tar` & `ratelimitedqueues-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:38:49.890217 ratelimitedqueues-0.0.1a7/
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-29 10:38:49.890217 ratelimitedqueues-0.0.1a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-29 10:38:38.000000 ratelimitedqueues-0.0.1a7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-29 10:38:38.000000 ratelimitedqueues-0.0.1a7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:38:49.890217 ratelimitedqueues-0.0.1a7/rateLimitedQueues.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-29 10:38:49.000000 ratelimitedqueues-0.0.1a7/rateLimitedQueues.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-29 10:38:49.000000 ratelimitedqueues-0.0.1a7/rateLimitedQueues.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:38:49.000000 ratelimitedqueues-0.0.1a7/rateLimitedQueues.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 10:38:49.000000 ratelimitedqueues-0.0.1a7/rateLimitedQueues.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-04-29 10:38:38.000000 ratelimitedqueues-0.0.1a7/rateLimitedQueues.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 10:38:49.890217 ratelimitedqueues-0.0.1a7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:35:42.590344 ratelimitedqueues-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-07 21:35:42.590344 ratelimitedqueues-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-07 21:35:38.000000 ratelimitedqueues-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-07 21:35:38.000000 ratelimitedqueues-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:35:42.590344 ratelimitedqueues-0.0.2/rateLimitedQueues.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-07 21:35:42.000000 ratelimitedqueues-0.0.2/rateLimitedQueues.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-07 21:35:42.000000 ratelimitedqueues-0.0.2/rateLimitedQueues.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 21:35:42.000000 ratelimitedqueues-0.0.2/rateLimitedQueues.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 21:35:42.000000 ratelimitedqueues-0.0.2/rateLimitedQueues.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-07 21:35:38.000000 ratelimitedqueues-0.0.2/rateLimitedQueues.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 21:35:42.590344 ratelimitedqueues-0.0.2/setup.cfg
```

### Comparing `ratelimitedqueues-0.0.1a7/PKG-INFO` & `ratelimitedqueues-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: rateLimitedQueues
-Version: 0.0.1a7
+Version: 0.0.2
 Summary: A well maintained program to execute functions in queue as if only 1 worker is executing them one by one (High priority first). Works wonders when a series of time consuming tasks has to be performed but they need to be in sequence.
 Maintainer-email: Bhindi <bhaskarpanja93@gmail.com>
 Project-URL: Homepage, https://github.com/BhaskarPanja93/rateLimitedQueues
 Keywords: thread,threaded,task,threaded task,queue,queues,queued tasks
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# rateLimitedQueues v0.0.1a7
+# rateLimitedQueues v0.0.2
 
 ```pip install rateLimitedQueues --upgrade```
 
 
 ###### <br>A well maintained program to execute functions in queue as if only 1 worker is executing them one by one (High priority first). Works wonders when a series of time consuming tasks has to be performed but they need to be in sequence.
 
 <br>To install: 
@@ -27,21 +27,24 @@
 ```
 
 
 #### <br><br>Using this program is as simple as:
 ```
 from rateLimitedQueues import Manager
 
-rateLimiter = Manager()
+rateLimiter = Manager(timeBetweenExecution=1, smallestWaitTime=0)
 
-def functionToCall(a, b, c, d, *args, **kwargs):
-    sleep(2)
-    print(a, b, c, d, args, kwargs)
+def mainFunction(url, headers, json, *args, **kwargs):
+    sleep(1)
+    print(args, kwargs)
 
 
 for _ in range(10):
-    rateLimiter.queueAction(functionToCall, randrange(1,5), True, 1, 2, 3, 4, 5, c=10, d=12, e=60)
-
+    rateLimiter.queueAction(mainFunction, postFunction=functionToCallAfterMainFunction, postKwArgs={"kwarg1":True, "kwarg2": 20},
+                            executePriority=3, executeThreaded=False,
+                            'https://www.google.com',
+                            headers={'Authorization': "Bearer 1234"},
+                            json={})
 ```
 
 
 ###### <br>This project is always open to suggestions and feature requests.
```

### Comparing `ratelimitedqueues-0.0.1a7/README.md` & `ratelimitedqueues-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# rateLimitedQueues v0.0.1a7
+# rateLimitedQueues v0.0.2
 
 ```pip install rateLimitedQueues --upgrade```
 
 
 ###### <br>A well maintained program to execute functions in queue as if only 1 worker is executing them one by one (High priority first). Works wonders when a series of time consuming tasks has to be performed but they need to be in sequence.
 
 <br>To install: 
@@ -14,21 +14,24 @@
 ```
 
 
 #### <br><br>Using this program is as simple as:
 ```
 from rateLimitedQueues import Manager
 
-rateLimiter = Manager()
+rateLimiter = Manager(timeBetweenExecution=1, smallestWaitTime=0)
 
-def functionToCall(a, b, c, d, *args, **kwargs):
-    sleep(2)
-    print(a, b, c, d, args, kwargs)
+def mainFunction(url, headers, json, *args, **kwargs):
+    sleep(1)
+    print(args, kwargs)
 
 
 for _ in range(10):
-    rateLimiter.queueAction(functionToCall, randrange(1,5), True, 1, 2, 3, 4, 5, c=10, d=12, e=60)
-
+    rateLimiter.queueAction(mainFunction, postFunction=functionToCallAfterMainFunction, postKwArgs={"kwarg1":True, "kwarg2": 20},
+                            executePriority=3, executeThreaded=False,
+                            'https://www.google.com',
+                            headers={'Authorization': "Bearer 1234"},
+                            json={})
 ```
 
 
 ###### <br>This project is always open to suggestions and feature requests.
```

### Comparing `ratelimitedqueues-0.0.1a7/pyproject.toml` & `ratelimitedqueues-0.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rateLimitedQueues"
-version = "0.0.1a7"
+version = "0.0.2"
 description = "A well maintained program to execute functions in queue as if only 1 worker is executing them one by one (High priority first). Works wonders when a series of time consuming tasks has to be performed but they need to be in sequence."
 readme = "README.md"
 maintainers = [{ name = "Bhindi", email = "bhaskarpanja93@gmail.com" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `ratelimitedqueues-0.0.1a7/rateLimitedQueues.egg-info/PKG-INFO` & `ratelimitedqueues-0.0.2/rateLimitedQueues.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: rateLimitedQueues
-Version: 0.0.1a7
+Version: 0.0.2
 Summary: A well maintained program to execute functions in queue as if only 1 worker is executing them one by one (High priority first). Works wonders when a series of time consuming tasks has to be performed but they need to be in sequence.
 Maintainer-email: Bhindi <bhaskarpanja93@gmail.com>
 Project-URL: Homepage, https://github.com/BhaskarPanja93/rateLimitedQueues
 Keywords: thread,threaded,task,threaded task,queue,queues,queued tasks
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# rateLimitedQueues v0.0.1a7
+# rateLimitedQueues v0.0.2
 
 ```pip install rateLimitedQueues --upgrade```
 
 
 ###### <br>A well maintained program to execute functions in queue as if only 1 worker is executing them one by one (High priority first). Works wonders when a series of time consuming tasks has to be performed but they need to be in sequence.
 
 <br>To install: 
@@ -27,21 +27,24 @@
 ```
 
 
 #### <br><br>Using this program is as simple as:
 ```
 from rateLimitedQueues import Manager
 
-rateLimiter = Manager()
+rateLimiter = Manager(timeBetweenExecution=1, smallestWaitTime=0)
 
-def functionToCall(a, b, c, d, *args, **kwargs):
-    sleep(2)
-    print(a, b, c, d, args, kwargs)
+def mainFunction(url, headers, json, *args, **kwargs):
+    sleep(1)
+    print(args, kwargs)
 
 
 for _ in range(10):
-    rateLimiter.queueAction(functionToCall, randrange(1,5), True, 1, 2, 3, 4, 5, c=10, d=12, e=60)
-
+    rateLimiter.queueAction(mainFunction, postFunction=functionToCallAfterMainFunction, postKwArgs={"kwarg1":True, "kwarg2": 20},
+                            executePriority=3, executeThreaded=False,
+                            'https://www.google.com',
+                            headers={'Authorization': "Bearer 1234"},
+                            json={})
 ```
 
 
 ###### <br>This project is always open to suggestions and feature requests.
```

