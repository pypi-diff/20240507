# Comparing `tmp/heartbeat_library-0.0.8.tar.gz` & `tmp/heartbeat_library-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heartbeat_library-0.0.8.tar", last modified: Mon May  6 18:38:43 2024, max compression
+gzip compressed data, was "heartbeat_library-0.0.9.tar", last modified: Tue May  7 12:03:05 2024, max compression
```

## Comparing `heartbeat_library-0.0.8.tar` & `heartbeat_library-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 18:38:43.350232 heartbeat_library-0.0.8/
--rw-rw-rw-   0        0        0     1104 2024-05-03 19:24:03.000000 heartbeat_library-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     2057 2024-05-06 18:38:43.349233 heartbeat_library-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1270 2024-05-06 13:42:31.000000 heartbeat_library-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 18:38:43.343229 heartbeat_library-0.0.8/heartbeat-library/
--rw-rw-rw-   0        0        0       65 2024-05-06 17:58:23.000000 heartbeat_library-0.0.8/heartbeat-library/__init__.py
--rw-rw-rw-   0        0        0     3416 2024-05-06 17:50:42.000000 heartbeat_library-0.0.8/heartbeat-library/heartbeat_library.py
-drwxrwxrwx   0        0        0        0 2024-05-06 18:38:43.348231 heartbeat_library-0.0.8/heartbeat_library.egg-info/
--rw-rw-rw-   0        0        0     2057 2024-05-06 18:38:43.000000 heartbeat_library-0.0.8/heartbeat_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2024-05-06 18:38:43.000000 heartbeat_library-0.0.8/heartbeat_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 18:38:43.000000 heartbeat_library-0.0.8/heartbeat_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-06 18:02:12.000000 heartbeat_library-0.0.8/heartbeat_library.egg-info/requirements.txt
--rw-rw-rw-   0        0        0       18 2024-05-06 18:38:43.000000 heartbeat_library-0.0.8/heartbeat_library.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 18:38:43.350232 heartbeat_library-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1019 2024-05-06 18:38:29.000000 heartbeat_library-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:03:05.987429 heartbeat_library-0.0.9/
+-rw-rw-rw-   0        0        0     1104 2024-05-03 19:24:03.000000 heartbeat_library-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     2108 2024-05-07 12:03:05.985417 heartbeat_library-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1270 2024-05-06 13:42:31.000000 heartbeat_library-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 12:03:05.964409 heartbeat_library-0.0.9/heartbeat-library/
+-rw-rw-rw-   0        0        0       65 2024-05-06 17:58:23.000000 heartbeat_library-0.0.9/heartbeat-library/__init__.py
+-rw-rw-rw-   0        0        0     3416 2024-05-06 17:50:42.000000 heartbeat_library-0.0.9/heartbeat-library/heartbeat_library.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:03:05.974936 heartbeat_library-0.0.9/heartbeat_library.egg-info/
+-rw-rw-rw-   0        0        0     2108 2024-05-07 12:03:05.000000 heartbeat_library-0.0.9/heartbeat_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2024-05-07 12:03:05.000000 heartbeat_library-0.0.9/heartbeat_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 12:03:05.000000 heartbeat_library-0.0.9/heartbeat_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-07 12:03:05.000000 heartbeat_library-0.0.9/heartbeat_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-07 12:03:05.000000 heartbeat_library-0.0.9/heartbeat_library.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 12:03:05.988432 heartbeat_library-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1067 2024-05-07 12:03:00.000000 heartbeat_library-0.0.9/setup.py
```

### Comparing `heartbeat_library-0.0.8/LICENSE` & `heartbeat_library-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `heartbeat_library-0.0.8/PKG-INFO` & `heartbeat_library-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: heartbeat-library
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library for sending pulses to a process monitoring server
 Author: Pedro Ferreira Braz
 Author-email: pbraz.pedrof@gmail.com
 License: MIT License
 Keywords: heartbeat,heartbeat-library,heartbeat-api,heartbeat-wrapper,heartbeat-python,heartbeat-python-wrapper,heartbeat-python-api,heartbeat-python-wrapper-api,heartbeat-python-api-wrapper,multithreading,threading,requests,python-requests,python-threading,python-multithreading,python-heartbeat,python-heartbeat-api,python-heartbeat-wrapper,python-heartbeat-python,python-heartbeat-python-wrapper,python-heartbeat-python-api,python-heartbeat-python-wrapper-api,python-heartbeat-python-api-wrapper
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: threading
 
 # Python Heartbeat Library
 
 The Python Heartbeat Library is a simple utility that allows you to send regular "pulses" to a specific endpoint. These pulses serve as confirmation that your main script is functioning correctly. If the main script stops for any reason, the heartbeat will also cease, indicating that something went wrong.
 
 # Installation
```

### Comparing `heartbeat_library-0.0.8/README.md` & `heartbeat_library-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `heartbeat_library-0.0.8/heartbeat-library/heartbeat_library.py` & `heartbeat_library-0.0.9/heartbeat-library/heartbeat_library.py`

 * *Files identical despite different names*

### Comparing `heartbeat_library-0.0.8/heartbeat_library.egg-info/PKG-INFO` & `heartbeat_library-0.0.9/heartbeat_library.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: heartbeat-library
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library for sending pulses to a process monitoring server
 Author: Pedro Ferreira Braz
 Author-email: pbraz.pedrof@gmail.com
 License: MIT License
 Keywords: heartbeat,heartbeat-library,heartbeat-api,heartbeat-wrapper,heartbeat-python,heartbeat-python-wrapper,heartbeat-python-api,heartbeat-python-wrapper-api,heartbeat-python-api-wrapper,multithreading,threading,requests,python-requests,python-threading,python-multithreading,python-heartbeat,python-heartbeat-api,python-heartbeat-wrapper,python-heartbeat-python,python-heartbeat-python-wrapper,python-heartbeat-python-api,python-heartbeat-python-wrapper-api,python-heartbeat-python-api-wrapper
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: threading
 
 # Python Heartbeat Library
 
 The Python Heartbeat Library is a simple utility that allows you to send regular "pulses" to a specific endpoint. These pulses serve as confirmation that your main script is functioning correctly. If the main script stops for any reason, the heartbeat will also cease, indicating that something went wrong.
 
 # Installation
```

### Comparing `heartbeat_library-0.0.8/setup.py` & `heartbeat_library-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='heartbeat-library',
-    version='0.0.8',
+    version='0.0.9',
     license='MIT License',
     author='Pedro Ferreira Braz',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='pbraz.pedrof@gmail.com',
     keywords='heartbeat, heartbeat-library, heartbeat-api, heartbeat-wrapper, heartbeat-python, heartbeat-python-wrapper, heartbeat-python-api, heartbeat-python-wrapper-api, heartbeat-python-api-wrapper, multithreading, threading, requests, python-requests, python-threading, python-multithreading, python-heartbeat, python-heartbeat-api, python-heartbeat-wrapper, python-heartbeat-python, python-heartbeat-python-wrapper, python-heartbeat-python-api, python-heartbeat-python-wrapper-api, python-heartbeat-python-api-wrapper',
     description=u'Library for sending pulses to a process monitoring server',
     packages=find_packages(),
-    install_requires=[])
+    install_requires=[
+        'requests',
+        'threading'
+    ])
```

