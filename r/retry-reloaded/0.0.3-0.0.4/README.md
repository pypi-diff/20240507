# Comparing `tmp/retry-reloaded-0.0.3.tar.gz` & `tmp/retry_reloaded-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retry-reloaded-0.0.3.tar", last modified: Sun Apr  7 16:14:33 2024, max compression
+gzip compressed data, was "retry_reloaded-0.0.4.tar", last modified: Tue May  7 10:47:32 2024, max compression
```

## Comparing `retry-reloaded-0.0.3.tar` & `retry_reloaded-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:14:33.116637 retry-reloaded-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-07 16:14:33.116637 retry-reloaded-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:14:33.112636 retry-reloaded-0.0.3/retry_reloaded/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/retry_reloaded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/retry_reloaded/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/retry_reloaded/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/retry_reloaded/_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/retry_reloaded/backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/retry_reloaded/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/retry_reloaded/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:14:33.116637 retry-reloaded-0.0.3/retry_reloaded.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-07 16:14:33.000000 retry-reloaded-0.0.3/retry_reloaded.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-07 16:14:33.000000 retry-reloaded-0.0.3/retry_reloaded.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 16:14:33.000000 retry-reloaded-0.0.3/retry_reloaded.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 16:14:33.000000 retry-reloaded-0.0.3/retry_reloaded.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 16:14:33.116637 retry-reloaded-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:14:33.116637 retry-reloaded-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/tests/test_backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/tests/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/tests/test_retry_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:47:32.452273 retry_reloaded-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-05-07 10:47:32.448273 retry_reloaded-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:47:32.448273 retry_reloaded-0.0.4/retry_reloaded/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/retry_reloaded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/retry_reloaded/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/retry_reloaded/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/retry_reloaded/_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/retry_reloaded/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/retry_reloaded/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/retry_reloaded/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:47:32.448273 retry_reloaded-0.0.4/retry_reloaded.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-05-07 10:47:32.000000 retry_reloaded-0.0.4/retry_reloaded.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-07 10:47:32.000000 retry_reloaded-0.0.4/retry_reloaded.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 10:47:32.000000 retry_reloaded-0.0.4/retry_reloaded.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-07 10:47:32.000000 retry_reloaded-0.0.4/retry_reloaded.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 10:47:32.452273 retry_reloaded-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:47:32.448273 retry_reloaded-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/tests/test_backoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/tests/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/tests/test_retry_args.py
```

### Comparing `retry-reloaded-0.0.3/LICENSE` & `retry_reloaded-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `retry-reloaded-0.0.3/PKG-INFO` & `retry_reloaded-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retry-reloaded
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple Python library for retrying functions         with various backoff and callback strategies.
 Home-page: https://github.com/chrisK824/retry
 Author: Chris Karvouniaris
 Author-email: christos.karvouniaris247@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 
 
 ## Install
 `pip install retry-reloaded`
 
 ## Features:
 
-- **Exception Handling**: Retry based on specific exceptions.
+- **Exception Handling**: Retry based on specific exceptions. If not specified then the default behaviour is to retry on all exceptions.
 - **Maximum Retries**: Set the maximum number of retry attempts.
 - **Timeout**: Specify the maximum time in seconds to spend on retries. Timeout check happens right before retry execution of the wrapped function.
 - **Deadline**: Define a deadline in seconds for retries to complete. Deadline check happens right after the retry execution of the wrapped function.
 - **Backoff Strategies**: Choose from various backoff strategies: fixed, exponential, linear, random
 - **Retry Callback**: Execute a callback function between retry attempts.
 - **Successful Retry Callback**: Perform an action after a successful retry.
 - **Failure Callback**: Define a callback function after failing all retries.
```

### Comparing `retry-reloaded-0.0.3/README.md` & `retry_reloaded-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 ## Install
 `pip install retry-reloaded`
 
 ## Features:
 
-- **Exception Handling**: Retry based on specific exceptions.
+- **Exception Handling**: Retry based on specific exceptions. If not specified then the default behaviour is to retry on all exceptions.
 - **Maximum Retries**: Set the maximum number of retry attempts.
 - **Timeout**: Specify the maximum time in seconds to spend on retries. Timeout check happens right before retry execution of the wrapped function.
 - **Deadline**: Define a deadline in seconds for retries to complete. Deadline check happens right after the retry execution of the wrapped function.
 - **Backoff Strategies**: Choose from various backoff strategies: fixed, exponential, linear, random
 - **Retry Callback**: Execute a callback function between retry attempts.
 - **Successful Retry Callback**: Perform an action after a successful retry.
 - **Failure Callback**: Define a callback function after failing all retries.
@@ -144,8 +144,8 @@
 @retry(
         max_retries=3,
         backoff=LinearBackOff(base_delay=0.1, step=0.1),
         failure_callback=failure_callback_
 )
 def fail_with_callback():
     raise ValueError
-```
+```
```

### Comparing `retry-reloaded-0.0.3/retry_reloaded/__init__.py` & `retry_reloaded-0.0.4/retry_reloaded/__init__.py`

 * *Files identical despite different names*

### Comparing `retry-reloaded-0.0.3/retry_reloaded/_exceptions.py` & `retry_reloaded-0.0.4/retry_reloaded/_exceptions.py`

 * *Files identical despite different names*

### Comparing `retry-reloaded-0.0.3/retry_reloaded/_logging.py` & `retry_reloaded-0.0.4/retry_reloaded/_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     console_handler = logging.StreamHandler()
     console_handler.setLevel(logging.DEBUG)
     formatter = logging.Formatter(
         "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
     )
     console_handler.setFormatter(formatter)
     _retry_logger.addHandler(console_handler)
+    _retry_logger.propagate = False
     return _retry_logger
 
 
 def _log_retry(
     logger: logging.Logger,
     fname: str,
     max_retries: Union[int, None],
```

### Comparing `retry-reloaded-0.0.3/retry_reloaded/_validate.py` & `retry_reloaded-0.0.4/retry_reloaded/_validate.py`

 * *Files identical despite different names*

### Comparing `retry-reloaded-0.0.3/retry_reloaded/backoff.py` & `retry_reloaded-0.0.4/retry_reloaded/backoff.py`

 * *Files identical despite different names*

### Comparing `retry-reloaded-0.0.3/retry_reloaded/callback.py` & `retry_reloaded-0.0.4/retry_reloaded/callback.py`

 * *Files identical despite different names*

### Comparing `retry-reloaded-0.0.3/retry_reloaded/retry.py` & `retry_reloaded-0.0.4/retry_reloaded/retry.py`

 * *Files identical despite different names*

### Comparing `retry-reloaded-0.0.3/retry_reloaded.egg-info/PKG-INFO` & `retry_reloaded-0.0.4/retry_reloaded.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retry-reloaded
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple Python library for retrying functions         with various backoff and callback strategies.
 Home-page: https://github.com/chrisK824/retry
 Author: Chris Karvouniaris
 Author-email: christos.karvouniaris247@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 
 
 ## Install
 `pip install retry-reloaded`
 
 ## Features:
 
-- **Exception Handling**: Retry based on specific exceptions.
+- **Exception Handling**: Retry based on specific exceptions. If not specified then the default behaviour is to retry on all exceptions.
 - **Maximum Retries**: Set the maximum number of retry attempts.
 - **Timeout**: Specify the maximum time in seconds to spend on retries. Timeout check happens right before retry execution of the wrapped function.
 - **Deadline**: Define a deadline in seconds for retries to complete. Deadline check happens right after the retry execution of the wrapped function.
 - **Backoff Strategies**: Choose from various backoff strategies: fixed, exponential, linear, random
 - **Retry Callback**: Execute a callback function between retry attempts.
 - **Successful Retry Callback**: Perform an action after a successful retry.
 - **Failure Callback**: Define a callback function after failing all retries.
```

### Comparing `retry-reloaded-0.0.3/setup.py` & `retry_reloaded-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="retry-reloaded",
-    version="0.0.3",
+    version="0.0.4",
     description="A simple Python library for retrying functions \
         with various backoff and callback strategies.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/chrisK824/retry",
     author="Chris Karvouniaris",
     author_email="christos.karvouniaris247@gmail.com",
```

### Comparing `retry-reloaded-0.0.3/tests/test_backoff.py` & `retry_reloaded-0.0.4/tests/test_backoff.py`

 * *Files identical despite different names*

### Comparing `retry-reloaded-0.0.3/tests/test_callback.py` & `retry_reloaded-0.0.4/tests/test_callback.py`

 * *Files identical despite different names*

### Comparing `retry-reloaded-0.0.3/tests/test_retry.py` & `retry_reloaded-0.0.4/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `retry-reloaded-0.0.3/tests/test_retry_args.py` & `retry_reloaded-0.0.4/tests/test_retry_args.py`

 * *Files identical despite different names*

