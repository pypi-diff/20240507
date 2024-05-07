# Comparing `tmp/ofunctions.platform-1.5.0.tar.gz` & `tmp/ofunctions.platform-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofunctions.platform-1.5.0.tar", last modified: Fri Jan  5 14:07:35 2024, max compression
+gzip compressed data, was "ofunctions.platform-1.5.1.tar", last modified: Tue May  7 08:18:31 2024, max compression
```

## Comparing `ofunctions.platform-1.5.0.tar` & `ofunctions.platform-1.5.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-01-05 14:07:35.407324 ofunctions.platform-1.5.0/
--rw-rw-rw-   0        0        0     1590 2023-09-30 16:02:47.000000 ofunctions.platform-1.5.0/LICENSE
--rw-rw-rw-   0        0        0    17696 2024-01-05 14:07:35.407324 ofunctions.platform-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0    16468 2024-01-05 13:37:33.000000 ofunctions.platform-1.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-01-05 14:07:35.265153 ofunctions.platform-1.5.0/ofunctions/
-drwxrwxrwx   0        0        0        0 2024-01-05 14:07:35.344670 ofunctions.platform-1.5.0/ofunctions/platform/
--rw-rw-rw-   0        0        0     2853 2024-01-05 13:39:38.000000 ofunctions.platform-1.5.0/ofunctions/platform/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-05 14:07:35.344670 ofunctions.platform-1.5.0/ofunctions.platform.egg-info/
--rw-rw-rw-   0        0        0    17696 2024-01-05 14:07:35.000000 ofunctions.platform-1.5.0/ofunctions.platform.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      722 2024-01-05 14:07:35.000000 ofunctions.platform-1.5.0/ofunctions.platform.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-05 14:07:35.000000 ofunctions.platform-1.5.0/ofunctions.platform.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-01-05 14:07:35.000000 ofunctions.platform-1.5.0/ofunctions.platform.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0        2 2023-10-06 16:15:00.000000 ofunctions.platform-1.5.0/ofunctions.platform.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-01-05 14:07:35.000000 ofunctions.platform-1.5.0/ofunctions.platform.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-05 14:07:35.407324 ofunctions.platform-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     7685 2023-09-30 20:53:03.000000 ofunctions.platform-1.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-05 14:07:35.407324 ofunctions.platform-1.5.0/tests/
--rw-rw-rw-   0        0        0     5866 2023-09-30 16:02:47.000000 ofunctions.platform-1.5.0/tests/test_bisection.py
--rw-rw-rw-   0        0        0     3374 2023-09-30 16:02:47.000000 ofunctions.platform-1.5.0/tests/test_checksums.py
--rw-rw-rw-   0        0        0     2037 2023-09-30 20:53:02.000000 ofunctions.platform-1.5.0/tests/test_csv.py
--rw-rw-rw-   0        0        0     1037 2023-09-30 20:53:02.000000 ofunctions.platform-1.5.0/tests/test_delayed_keyboardinterrupt.py
--rw-rw-rw-   0        0        0     8438 2023-09-30 16:02:47.000000 ofunctions.platform-1.5.0/tests/test_file_utils.py
--rw-rw-rw-   0        0        0     1023 2023-09-30 16:02:47.000000 ofunctions.platform-1.5.0/tests/test_json_sanitize.py
--rw-rw-rw-   0        0        0     3308 2023-09-30 20:53:03.000000 ofunctions.platform-1.5.0/tests/test_logger_utils.py
--rw-rw-rw-   0        0        0     1616 2023-09-30 16:02:47.000000 ofunctions.platform-1.5.0/tests/test_mailer.py
--rw-rw-rw-   0        0        0     3566 2024-01-05 13:38:01.000000 ofunctions.platform-1.5.0/tests/test_misc.py
--rw-rw-rw-   0        0        0     6659 2024-01-01 21:08:53.000000 ofunctions.platform-1.5.0/tests/test_network.py
--rw-rw-rw-   0        0        0     1188 2023-09-30 16:02:47.000000 ofunctions.platform-1.5.0/tests/test_platform.py
--rw-rw-rw-   0        0        0     4242 2023-12-30 23:40:58.000000 ofunctions.platform-1.5.0/tests/test_process.py
--rw-rw-rw-   0        0        0      940 2023-09-30 16:02:47.000000 ofunctions.platform-1.5.0/tests/test_random.py
--rw-rw-rw-   0        0        0     2426 2023-09-30 16:02:47.000000 ofunctions.platform-1.5.0/tests/test_service_control.py
--rw-rw-rw-   0        0        0     2215 2023-09-30 20:53:03.000000 ofunctions.platform-1.5.0/tests/test_string_handling.py
--rw-rw-rw-   0        0        0     3778 2023-09-30 16:02:47.000000 ofunctions.platform-1.5.0/tests/test_threading.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:18:31.948305 ofunctions.platform-1.5.1/
+-rw-rw-rw-   0        0        0     1590 2023-09-30 16:02:48.000000 ofunctions.platform-1.5.1/LICENSE
+-rw-rw-rw-   0        0        0    18188 2024-05-07 08:18:31.948305 ofunctions.platform-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0    16960 2024-04-25 10:07:07.000000 ofunctions.platform-1.5.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 08:18:31.853531 ofunctions.platform-1.5.1/ofunctions/
+drwxrwxrwx   0        0        0        0 2024-05-07 08:18:31.901309 ofunctions.platform-1.5.1/ofunctions/platform/
+-rw-rw-rw-   0        0        0     3058 2024-05-07 08:16:59.000000 ofunctions.platform-1.5.1/ofunctions/platform/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:18:31.945298 ofunctions.platform-1.5.1/ofunctions.platform.egg-info/
+-rw-rw-rw-   0        0        0    18188 2024-05-07 08:18:31.000000 ofunctions.platform-1.5.1/ofunctions.platform.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      722 2024-05-07 08:18:31.000000 ofunctions.platform-1.5.1/ofunctions.platform.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 08:18:31.000000 ofunctions.platform-1.5.1/ofunctions.platform.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-07 08:18:31.000000 ofunctions.platform-1.5.1/ofunctions.platform.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0        2 2023-10-06 16:15:02.000000 ofunctions.platform-1.5.1/ofunctions.platform.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-07 08:18:31.000000 ofunctions.platform-1.5.1/ofunctions.platform.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 08:18:31.948305 ofunctions.platform-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     7685 2023-09-30 20:53:04.000000 ofunctions.platform-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:18:31.944791 ofunctions.platform-1.5.1/tests/
+-rw-rw-rw-   0        0        0     5866 2023-09-30 16:02:48.000000 ofunctions.platform-1.5.1/tests/test_bisection.py
+-rw-rw-rw-   0        0        0     3374 2023-09-30 16:02:48.000000 ofunctions.platform-1.5.1/tests/test_checksums.py
+-rw-rw-rw-   0        0        0     2037 2023-09-30 20:53:04.000000 ofunctions.platform-1.5.1/tests/test_csv.py
+-rw-rw-rw-   0        0        0     1037 2023-09-30 20:53:04.000000 ofunctions.platform-1.5.1/tests/test_delayed_keyboardinterrupt.py
+-rw-rw-rw-   0        0        0     8438 2023-09-30 16:02:48.000000 ofunctions.platform-1.5.1/tests/test_file_utils.py
+-rw-rw-rw-   0        0        0     1023 2023-09-30 16:02:48.000000 ofunctions.platform-1.5.1/tests/test_json_sanitize.py
+-rw-rw-rw-   0        0        0     3308 2023-09-30 20:53:04.000000 ofunctions.platform-1.5.1/tests/test_logger_utils.py
+-rw-rw-rw-   0        0        0     1616 2023-09-30 16:02:48.000000 ofunctions.platform-1.5.1/tests/test_mailer.py
+-rw-rw-rw-   0        0        0     3566 2024-01-05 13:38:02.000000 ofunctions.platform-1.5.1/tests/test_misc.py
+-rw-rw-rw-   0        0        0     6659 2024-01-01 21:08:54.000000 ofunctions.platform-1.5.1/tests/test_network.py
+-rw-rw-rw-   0        0        0     1188 2023-09-30 16:02:48.000000 ofunctions.platform-1.5.1/tests/test_platform.py
+-rw-rw-rw-   0        0        0     4242 2023-12-30 23:41:00.000000 ofunctions.platform-1.5.1/tests/test_process.py
+-rw-rw-rw-   0        0        0      940 2023-09-30 16:02:48.000000 ofunctions.platform-1.5.1/tests/test_random.py
+-rw-rw-rw-   0        0        0     2426 2023-09-30 16:02:48.000000 ofunctions.platform-1.5.1/tests/test_service_control.py
+-rw-rw-rw-   0        0        0     2215 2023-09-30 20:53:04.000000 ofunctions.platform-1.5.1/tests/test_string_handling.py
+-rw-rw-rw-   0        0        0     8291 2024-01-09 19:54:48.000000 ofunctions.platform-1.5.1/tests/test_threading.py
```

### Comparing `ofunctions.platform-1.5.0/LICENSE` & `ofunctions.platform-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ofunctions.platform-1.5.0/PKG-INFO` & `ofunctions.platform-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofunctions.platform
-Version: 1.5.0
+Version: 1.5.1
 Summary: Very basic platform identification
 Home-page: https://github.com/netinvent/ofunctions
 Author: NetInvent - Orsiris de Jong
 Author-email: contact@netinvent.fr
 Keywords: network,bisection,logging
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -250,14 +250,22 @@
 mailer.send_email(subject='test', sender_mail='me@example.com', recipient_mails='them@example.com', body='some body just told me', attachment=attachment, filename='My Attachment File.txt')
 ```
 
 ## misc Usage
 
 Misc is a collection of somehow useful functions.
 
+### fn_name
+
+Get the caller function name of current context.
+```
+print(fn_name()) will show current caller function name
+print(fn_name(2)) will show parent of current caller function name
+```
+
 ### BytesConverter
 
 BytesConverter is that little tool that you want when handling bits and byte units.
 Internally, BytesConverter always represents data an int number of bytes.
 BytesConverter will return a float or a str if human output is requested.
 
 Example (output is shown as comment):
@@ -314,14 +322,26 @@
 ofunctions.network is a collection of various tools making network diag / mapping easier.
 
 Setup:
 ```commandline
 pip install ofunctions.network
 ```
 
+### get_public_ip()
+
+Easy way to find Public IPv4 or IPv6 using multiple online services
+
+```
+from ofunctions.netowrk import get_public_ip
+
+print("My IP is", get_public_ip())
+print("My IPv4 is", get_public_ip(ip_version=4))
+print("My IPv6 is", get_public_ip(ip_version=6))
+```
+
 ### IOCounters
 
 IOCounters is a class that will log instant sent/received bytes as well as total sent/received bytes.
 Once an instance is created, logging begins as a thread.
 You may specify which interfaces to track at which resolution.
 If none is given, all interfaces are tracked every second.
```

### Comparing `ofunctions.platform-1.5.0/README.md` & `ofunctions.platform-1.5.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -221,14 +221,22 @@
 mailer.send_email(subject='test', sender_mail='me@example.com', recipient_mails='them@example.com', body='some body just told me', attachment=attachment, filename='My Attachment File.txt')
 ```
 
 ## misc Usage
 
 Misc is a collection of somehow useful functions.
 
+### fn_name
+
+Get the caller function name of current context.
+```
+print(fn_name()) will show current caller function name
+print(fn_name(2)) will show parent of current caller function name
+```
+
 ### BytesConverter
 
 BytesConverter is that little tool that you want when handling bits and byte units.
 Internally, BytesConverter always represents data an int number of bytes.
 BytesConverter will return a float or a str if human output is requested.
 
 Example (output is shown as comment):
@@ -285,14 +293,26 @@
 ofunctions.network is a collection of various tools making network diag / mapping easier.
 
 Setup:
 ```commandline
 pip install ofunctions.network
 ```
 
+### get_public_ip()
+
+Easy way to find Public IPv4 or IPv6 using multiple online services
+
+```
+from ofunctions.netowrk import get_public_ip
+
+print("My IP is", get_public_ip())
+print("My IPv4 is", get_public_ip(ip_version=4))
+print("My IPv6 is", get_public_ip(ip_version=6))
+```
+
 ### IOCounters
 
 IOCounters is a class that will log instant sent/received bytes as well as total sent/received bytes.
 Once an instance is created, logging begins as a thread.
 You may specify which interfaces to track at which resolution.
 If none is given, all interfaces are tracked every second.
```

### Comparing `ofunctions.platform-1.5.0/ofunctions/platform/__init__.py` & `ofunctions.platform-1.5.1/ofunctions/platform/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 """
 
 __intname__ = "ofunctions.platform"
 __author__ = "Orsiris de Jong"
 __copyright__ = "Copyright (C) 2014-2024 Orsiris de Jong"
 __description__ = "Very basic platform identification"
 __licence__ = "BSD 3 Clause"
-__version__ = "1.5.0"
-__build__ = "2024010301"
+__version__ = "1.5.1"
+__build__ = "2024050701"
 __compat__ = "python2.7+"
 
 import os
 import sys
 import platform
 
 
@@ -109,12 +109,24 @@
 
 
 def get_os_identifier():
     # type: () -> dict
     """
     Returns a dict of os info
     """
+
+    platform = "Unknown"
+    version = "Unknown"
+    try:
+        platform = platform.platform()
+    except Exception:
+        pass
+    try:
+        version = platform.version()
+    except Exception:
+        pass
+
     return {
         "type": get_os(),
-        "platform": platform.platform(),
-        "version": platform.version(),
+        "platform": platform,
+        "version": version,
     }
```

### Comparing `ofunctions.platform-1.5.0/ofunctions.platform.egg-info/PKG-INFO` & `ofunctions.platform-1.5.1/ofunctions.platform.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofunctions.platform
-Version: 1.5.0
+Version: 1.5.1
 Summary: Very basic platform identification
 Home-page: https://github.com/netinvent/ofunctions
 Author: NetInvent - Orsiris de Jong
 Author-email: contact@netinvent.fr
 Keywords: network,bisection,logging
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -250,14 +250,22 @@
 mailer.send_email(subject='test', sender_mail='me@example.com', recipient_mails='them@example.com', body='some body just told me', attachment=attachment, filename='My Attachment File.txt')
 ```
 
 ## misc Usage
 
 Misc is a collection of somehow useful functions.
 
+### fn_name
+
+Get the caller function name of current context.
+```
+print(fn_name()) will show current caller function name
+print(fn_name(2)) will show parent of current caller function name
+```
+
 ### BytesConverter
 
 BytesConverter is that little tool that you want when handling bits and byte units.
 Internally, BytesConverter always represents data an int number of bytes.
 BytesConverter will return a float or a str if human output is requested.
 
 Example (output is shown as comment):
@@ -314,14 +322,26 @@
 ofunctions.network is a collection of various tools making network diag / mapping easier.
 
 Setup:
 ```commandline
 pip install ofunctions.network
 ```
 
+### get_public_ip()
+
+Easy way to find Public IPv4 or IPv6 using multiple online services
+
+```
+from ofunctions.netowrk import get_public_ip
+
+print("My IP is", get_public_ip())
+print("My IPv4 is", get_public_ip(ip_version=4))
+print("My IPv6 is", get_public_ip(ip_version=6))
+```
+
 ### IOCounters
 
 IOCounters is a class that will log instant sent/received bytes as well as total sent/received bytes.
 Once an instance is created, logging begins as a thread.
 You may specify which interfaces to track at which resolution.
 If none is given, all interfaces are tracked every second.
```

### Comparing `ofunctions.platform-1.5.0/ofunctions.platform.egg-info/SOURCES.txt` & `ofunctions.platform-1.5.1/ofunctions.platform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ofunctions.platform-1.5.0/setup.py` & `ofunctions.platform-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `ofunctions.platform-1.5.0/tests/test_bisection.py` & `ofunctions.platform-1.5.1/tests/test_bisection.py`

 * *Files identical despite different names*

### Comparing `ofunctions.platform-1.5.0/tests/test_checksums.py` & `ofunctions.platform-1.5.1/tests/test_checksums.py`

 * *Files identical despite different names*

### Comparing `ofunctions.platform-1.5.0/tests/test_csv.py` & `ofunctions.platform-1.5.1/tests/test_csv.py`

 * *Files identical despite different names*

### Comparing `ofunctions.platform-1.5.0/tests/test_delayed_keyboardinterrupt.py` & `ofunctions.platform-1.5.1/tests/test_delayed_keyboardinterrupt.py`

 * *Files identical despite different names*

### Comparing `ofunctions.platform-1.5.0/tests/test_file_utils.py` & `ofunctions.platform-1.5.1/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `ofunctions.platform-1.5.0/tests/test_json_sanitize.py` & `ofunctions.platform-1.5.1/tests/test_json_sanitize.py`

 * *Files identical despite different names*

### Comparing `ofunctions.platform-1.5.0/tests/test_logger_utils.py` & `ofunctions.platform-1.5.1/tests/test_logger_utils.py`

 * *Files identical despite different names*

### Comparing `ofunctions.platform-1.5.0/tests/test_mailer.py` & `ofunctions.platform-1.5.1/tests/test_mailer.py`

 * *Files identical despite different names*

### Comparing `ofunctions.platform-1.5.0/tests/test_misc.py` & `ofunctions.platform-1.5.1/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `ofunctions.platform-1.5.0/tests/test_network.py` & `ofunctions.platform-1.5.1/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `ofunctions.platform-1.5.0/tests/test_platform.py` & `ofunctions.platform-1.5.1/tests/test_platform.py`

 * *Files identical despite different names*

### Comparing `ofunctions.platform-1.5.0/tests/test_process.py` & `ofunctions.platform-1.5.1/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `ofunctions.platform-1.5.0/tests/test_random.py` & `ofunctions.platform-1.5.1/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `ofunctions.platform-1.5.0/tests/test_service_control.py` & `ofunctions.platform-1.5.1/tests/test_service_control.py`

 * *Files identical despite different names*

### Comparing `ofunctions.platform-1.5.0/tests/test_string_handling.py` & `ofunctions.platform-1.5.1/tests/test_string_handling.py`

 * *Files identical despite different names*

