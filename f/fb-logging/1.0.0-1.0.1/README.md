# Comparing `tmp/fb_logging-1.0.0.tar.gz` & `tmp/fb_logging-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fb_logging-1.0.0.tar", last modified: Sun Feb  4 13:46:51 2024, max compression
+gzip compressed data, was "fb_logging-1.0.1.tar", last modified: Tue May  7 10:04:38 2024, max compression
```

## Comparing `fb_logging-1.0.0.tar` & `fb_logging-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 13:46:51.574422 fb_logging-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-02-04 13:46:47.000000 fb_logging-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-04 13:46:47.000000 fb_logging-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-02-04 13:46:51.574422 fb_logging-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-04 13:46:47.000000 fb_logging-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 13:46:51.570422 fb_logging-1.0.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)    14653 2024-02-04 13:46:47.000000 fb_logging-1.0.0/bin/dch2speclog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 13:46:51.570422 fb_logging-1.0.0/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 13:46:51.574422 fb_logging-1.0.0/lib/fb_logging/
--rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-02-04 13:46:47.000000 fb_logging-1.0.0/lib/fb_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16513 2024-02-04 13:46:47.000000 fb_logging-1.0.0/lib/fb_logging/colored.py
--rw-r--r--   0 runner    (1001) docker     (127)    42932 2024-02-04 13:46:47.000000 fb_logging-1.0.0/lib/fb_logging/deb_changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)    12290 2024-02-04 13:46:47.000000 fb_logging-1.0.0/lib/fb_logging/deb_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-04 13:46:51.000000 fb_logging-1.0.0/lib/fb_logging/local_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-02-04 13:46:47.000000 fb_logging-1.0.0/lib/fb_logging/syslog_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-02-04 13:46:47.000000 fb_logging-1.0.0/lib/fb_logging/unix_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 13:46:51.574422 fb_logging-1.0.0/lib/fb_logging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-02-04 13:46:51.000000 fb_logging-1.0.0/lib/fb_logging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-02-04 13:46:51.000000 fb_logging-1.0.0/lib/fb_logging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-04 13:46:51.000000 fb_logging-1.0.0/lib/fb_logging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-04 13:46:51.000000 fb_logging-1.0.0/lib/fb_logging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-02-04 13:46:51.574422 fb_logging-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-02-04 13:46:47.000000 fb_logging-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 13:46:51.574422 fb_logging-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-02-04 13:46:47.000000 fb_logging-1.0.0/test/general.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8967 2024-02-04 13:46:47.000000 fb_logging-1.0.0/test/test_colored.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10982 2024-02-04 13:46:47.000000 fb_logging-1.0.0/test/test_fb_logging.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6751 2024-02-04 13:46:47.000000 fb_logging-1.0.0/test/test_syslog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:04:38.370543 fb_logging-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-07 10:04:33.000000 fb_logging-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-07 10:04:33.000000 fb_logging-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-07 10:04:38.370543 fb_logging-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 10:04:33.000000 fb_logging-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:04:38.370543 fb_logging-1.0.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14653 2024-05-07 10:04:33.000000 fb_logging-1.0.1/bin/dch2speclog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:04:38.370543 fb_logging-1.0.1/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:04:38.370543 fb_logging-1.0.1/lib/fb_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-05-07 10:04:33.000000 fb_logging-1.0.1/lib/fb_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16513 2024-05-07 10:04:33.000000 fb_logging-1.0.1/lib/fb_logging/colored.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42932 2024-05-07 10:04:33.000000 fb_logging-1.0.1/lib/fb_logging/deb_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12290 2024-05-07 10:04:33.000000 fb_logging-1.0.1/lib/fb_logging/deb_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-07 10:04:38.000000 fb_logging-1.0.1/lib/fb_logging/local_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-07 10:04:33.000000 fb_logging-1.0.1/lib/fb_logging/syslog_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-05-07 10:04:33.000000 fb_logging-1.0.1/lib/fb_logging/unix_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:04:38.370543 fb_logging-1.0.1/lib/fb_logging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-07 10:04:38.000000 fb_logging-1.0.1/lib/fb_logging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-07 10:04:38.000000 fb_logging-1.0.1/lib/fb_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 10:04:38.000000 fb_logging-1.0.1/lib/fb_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 10:04:38.000000 fb_logging-1.0.1/lib/fb_logging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-07 10:04:38.374543 fb_logging-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-05-07 10:04:33.000000 fb_logging-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:04:38.370543 fb_logging-1.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-07 10:04:33.000000 fb_logging-1.0.1/test/general.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8967 2024-05-07 10:04:33.000000 fb_logging-1.0.1/test/test_colored.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10982 2024-05-07 10:04:33.000000 fb_logging-1.0.1/test/test_fb_logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6751 2024-05-07 10:04:33.000000 fb_logging-1.0.1/test/test_syslog.py
```

### Comparing `fb_logging-1.0.0/LICENSE` & `fb_logging-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fb_logging-1.0.0/PKG-INFO` & `fb_logging-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb_logging
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python modules to extend the logging mechanism in Python.
 Home-page: https://github.com/fbrehm/fb-logging
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fb_logging-1.0.0/bin/dch2speclog` & `fb_logging-1.0.1/bin/dch2speclog`

 * *Files identical despite different names*

### Comparing `fb_logging-1.0.0/lib/fb_logging/__init__.py` & `fb_logging-1.0.1/lib/fb_logging/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 @contact: frank@brehm-online.com
 @copyright: © 2024 by Frank Brehm, Berlin
 """
 
 __author__ = 'Frank Brehm <frank@brehm-online.com>'
 __copyright__ = '(C) 2024 by Frank Brehm, Berlin'
 __contact__ = 'frank@brehm-online.com'
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 __license__ = 'LGPL-3'
 
 # Standard modules
 import copy
 import logging
 import logging.handlers
 import os
```

### Comparing `fb_logging-1.0.0/lib/fb_logging/colored.py` & `fb_logging-1.0.1/lib/fb_logging/colored.py`

 * *Files identical despite different names*

### Comparing `fb_logging-1.0.0/lib/fb_logging/deb_changelog.py` & `fb_logging-1.0.1/lib/fb_logging/deb_changelog.py`

 * *Files identical despite different names*

### Comparing `fb_logging-1.0.0/lib/fb_logging/deb_version.py` & `fb_logging-1.0.1/lib/fb_logging/deb_version.py`

 * *Files identical despite different names*

### Comparing `fb_logging-1.0.0/lib/fb_logging/syslog_handler.py` & `fb_logging-1.0.1/lib/fb_logging/syslog_handler.py`

 * *Files identical despite different names*

### Comparing `fb_logging-1.0.0/lib/fb_logging/unix_handler.py` & `fb_logging-1.0.1/lib/fb_logging/unix_handler.py`

 * *Files identical despite different names*

### Comparing `fb_logging-1.0.0/lib/fb_logging.egg-info/PKG-INFO` & `fb_logging-1.0.1/lib/fb_logging.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb-logging
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python modules to extend the logging mechanism in Python.
 Home-page: https://github.com/fbrehm/fb-logging
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fb_logging-1.0.0/setup.cfg` & `fb_logging-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `fb_logging-1.0.0/setup.py` & `fb_logging-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `fb_logging-1.0.0/test/general.py` & `fb_logging-1.0.1/test/general.py`

 * *Files identical despite different names*

### Comparing `fb_logging-1.0.0/test/test_colored.py` & `fb_logging-1.0.1/test/test_colored.py`

 * *Files identical despite different names*

### Comparing `fb_logging-1.0.0/test/test_fb_logging.py` & `fb_logging-1.0.1/test/test_fb_logging.py`

 * *Files identical despite different names*

### Comparing `fb_logging-1.0.0/test/test_syslog.py` & `fb_logging-1.0.1/test/test_syslog.py`

 * *Files identical despite different names*

