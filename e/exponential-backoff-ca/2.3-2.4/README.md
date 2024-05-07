# Comparing `tmp/exponential_backoff_ca-2.3.tar.gz` & `tmp/exponential_backoff_ca-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exponential_backoff_ca-2.3.tar", last modified: Thu Apr  4 23:25:04 2024, max compression
+gzip compressed data, was "exponential_backoff_ca-2.4.tar", last modified: Tue May  7 17:31:58 2024, max compression
```

## Comparing `exponential_backoff_ca-2.3.tar` & `exponential_backoff_ca-2.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:25:04.091077 exponential_backoff_ca-2.3/
--rw-r--r--   0 root         (0) root         (0)     5233 2024-04-04 23:25:04.091077 exponential_backoff_ca-2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4842 2024-04-04 23:24:52.000000 exponential_backoff_ca-2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:25:04.087077 exponential_backoff_ca-2.3/exponential_backoff_ca/
--rw-r--r--   0 root         (0) root         (0)     4064 2024-04-04 23:24:52.000000 exponential_backoff_ca-2.3/exponential_backoff_ca/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 23:24:52.000000 exponential_backoff_ca-2.3/exponential_backoff_ca/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:25:04.091077 exponential_backoff_ca-2.3/exponential_backoff_ca.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5233 2024-04-04 23:25:04.000000 exponential_backoff_ca-2.3/exponential_backoff_ca.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      275 2024-04-04 23:25:04.000000 exponential_backoff_ca-2.3/exponential_backoff_ca.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 23:25:04.000000 exponential_backoff_ca-2.3/exponential_backoff_ca.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-04 23:25:04.000000 exponential_backoff_ca-2.3/exponential_backoff_ca.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      626 2024-04-04 23:24:52.000000 exponential_backoff_ca-2.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 23:25:04.091077 exponential_backoff_ca-2.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 17:31:57.995356 exponential_backoff_ca-2.4/
+-rw-r--r--   0 root         (0) root         (0)     6181 2024-05-07 17:31:57.995356 exponential_backoff_ca-2.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5790 2024-05-07 17:31:45.000000 exponential_backoff_ca-2.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 17:31:57.995356 exponential_backoff_ca-2.4/exponential_backoff_ca/
+-rw-r--r--   0 root         (0) root         (0)     4170 2024-05-07 17:31:45.000000 exponential_backoff_ca-2.4/exponential_backoff_ca/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 17:31:45.000000 exponential_backoff_ca-2.4/exponential_backoff_ca/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 17:31:57.995356 exponential_backoff_ca-2.4/exponential_backoff_ca.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6181 2024-05-07 17:31:57.000000 exponential_backoff_ca-2.4/exponential_backoff_ca.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      275 2024-05-07 17:31:57.000000 exponential_backoff_ca-2.4/exponential_backoff_ca.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 17:31:57.000000 exponential_backoff_ca-2.4/exponential_backoff_ca.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-07 17:31:57.000000 exponential_backoff_ca-2.4/exponential_backoff_ca.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      626 2024-05-07 17:31:45.000000 exponential_backoff_ca-2.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 17:31:57.995356 exponential_backoff_ca-2.4/setup.cfg
```

### Comparing `exponential_backoff_ca-2.3/PKG-INFO` & `exponential_backoff_ca-2.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: exponential_backoff_ca
-Version: 2.3
-Summary: An exponential backoff iterator with collision avoidance.
-Author: IEDO Team
-Project-URL: Repository, https://github.com/macrotex/python-exponential-backoff-ca
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
 # Exponential Backoff with Collision Avoidance
 
 This module defines a Python iterator implementing exponential backoff
 with collision avoidance. See
 https://en.wikipedia.org/wiki/Exponential_backoff#Collision_avoidance for
 a complete explanation of the algorithm.
 
@@ -79,14 +68,46 @@
 number of times going through loop: 1
 number of times going through loop: 2
 number of times going through loop: 3
 number of times going through loop: 4
 number of times going through loop: 5
 ```
 
+To reuse the iterator you need to reset the counter back to zero. You do this 
+via the `reset()` method:
+
+```
+from exponential_backoff_ca import ExponentialBackoff
+
+time_slot_secs = 2.0
+num_iterations = 5
+
+exp_boff = ExponentialBackoff(time_slot_secs, num_iterations)
+
+for interval in exp_boff:
+    print(f"number of times going through loop: {exp_boff.counter}")
+
+exp.boff.reset()
+for interval in exp_boff:
+    print(f"number of times going through loop (take two): {exp_boff.counter}")
+```
+Will output
+```
+number of times going through loop: 1
+number of times going through loop: 2
+number of times going through loop: 3
+number of times going through loop: 4
+number of times going through loop: 5
+number of times going through loop (take two): 1
+number of times going through loop (take two): 2
+number of times going through loop (take two): 3
+number of times going through loop (take two): 4
+number of times going through loop (take two): 5
+```
+
 To limit the maxiumum number of available slots use the optional `max_slots` parameter:
 
 ```
 from exponential_backoff_ca import ExponentialBackoff
 
 time_slot_secs = 2.0 # The number of seconds in each time slot.
 num_iterations = 10  # The number of iterations.
```

### Comparing `exponential_backoff_ca-2.3/exponential_backoff_ca/__init__.py` & `exponential_backoff_ca-2.4/exponential_backoff_ca/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,7 +113,12 @@
                 msg =f"limit value exceeded; returning limit of {self.limit_value}"
                 self.progress(msg)
                 wait_time = self.limit_value
 
             return wait_time
 
         raise StopIteration
+
+    def reset(self) -> None:
+        """Rest counter to zero."""
+        self.counter = 0
+        return
```

### Comparing `exponential_backoff_ca-2.3/exponential_backoff_ca.egg-info/PKG-INFO` & `exponential_backoff_ca-2.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exponential_backoff_ca
-Version: 2.3
+Version: 2.4
 Summary: An exponential backoff iterator with collision avoidance.
 Author: IEDO Team
 Project-URL: Repository, https://github.com/macrotex/python-exponential-backoff-ca
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -79,14 +79,46 @@
 number of times going through loop: 1
 number of times going through loop: 2
 number of times going through loop: 3
 number of times going through loop: 4
 number of times going through loop: 5
 ```
 
+To reuse the iterator you need to reset the counter back to zero. You do this 
+via the `reset()` method:
+
+```
+from exponential_backoff_ca import ExponentialBackoff
+
+time_slot_secs = 2.0
+num_iterations = 5
+
+exp_boff = ExponentialBackoff(time_slot_secs, num_iterations)
+
+for interval in exp_boff:
+    print(f"number of times going through loop: {exp_boff.counter}")
+
+exp.boff.reset()
+for interval in exp_boff:
+    print(f"number of times going through loop (take two): {exp_boff.counter}")
+```
+Will output
+```
+number of times going through loop: 1
+number of times going through loop: 2
+number of times going through loop: 3
+number of times going through loop: 4
+number of times going through loop: 5
+number of times going through loop (take two): 1
+number of times going through loop (take two): 2
+number of times going through loop (take two): 3
+number of times going through loop (take two): 4
+number of times going through loop (take two): 5
+```
+
 To limit the maxiumum number of available slots use the optional `max_slots` parameter:
 
 ```
 from exponential_backoff_ca import ExponentialBackoff
 
 time_slot_secs = 2.0 # The number of seconds in each time slot.
 num_iterations = 10  # The number of iterations.
```

### Comparing `exponential_backoff_ca-2.3/pyproject.toml` & `exponential_backoff_ca-2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 68.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "exponential_backoff_ca"
-version = "2.3"
+version = "2.4"
 description = "An exponential backoff iterator with collision avoidance."
 readme = "README.md"
 requires-python = ">= 3.9"
 authors = [
   {name = "IEDO Team"},
 ]
 classifiers = [
```

