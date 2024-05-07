# Comparing `tmp/tmticket-0.1.0.tar.gz` & `tmp/tmticket-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmticket-0.1.0.tar", last modified: Fri May  3 20:55:49 2024, max compression
+gzip compressed data, was "tmticket-0.1.8.tar", last modified: Tue May  7 21:09:18 2024, max compression
```

## Comparing `tmticket-0.1.0.tar` & `tmticket-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:55:49.001499 tmticket-0.1.0/
--rw-r--r--   0 root         (0) root         (0)      282 2024-05-03 20:55:49.001499 tmticket-0.1.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:55:48.998499 tmticket-0.1.0/pytmtickets/
--rw-r--r--   0 root         (0) root         (0)      363 2024-04-04 21:21:50.000000 tmticket-0.1.0/pytmtickets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5702 2024-05-02 02:38:59.000000 tmticket-0.1.0/pytmtickets/client.py
--rw-r--r--   0 root         (0) root         (0)    13241 2024-04-04 23:36:56.000000 tmticket-0.1.0/pytmtickets/model.py
--rw-r--r--   0 root         (0) root         (0)     4525 2024-04-07 01:34:01.000000 tmticket-0.1.0/pytmtickets/query.py
--rw-r--r--   0 root         (0) root         (0)      511 2024-04-26 23:49:15.000000 tmticket-0.1.0/pytmtickets/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-03 20:55:49.002499 tmticket-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      542 2024-05-03 20:55:42.000000 tmticket-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 20:55:49.000499 tmticket-0.1.0/tmticket.egg-info/
--rw-r--r--   0 root         (0) root         (0)      282 2024-05-03 20:55:48.000000 tmticket-0.1.0/tmticket.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      276 2024-05-03 20:55:48.000000 tmticket-0.1.0/tmticket.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 20:55:48.000000 tmticket-0.1.0/tmticket.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-03 20:55:48.000000 tmticket-0.1.0/tmticket.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-05-03 20:55:48.000000 tmticket-0.1.0/tmticket.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 21:09:18.404718 tmticket-0.1.8/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-05-07 21:08:23.000000 tmticket-0.1.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      736 2024-05-07 21:09:18.403718 tmticket-0.1.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-07 21:08:23.000000 tmticket-0.1.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 21:09:18.404718 tmticket-0.1.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      968 2024-05-07 21:08:23.000000 tmticket-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 21:09:18.401718 tmticket-0.1.8/tmticket/
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-07 21:08:23.000000 tmticket-0.1.8/tmticket/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5702 2024-05-07 21:08:23.000000 tmticket-0.1.8/tmticket/client.py
+-rw-r--r--   0 root         (0) root         (0)    13241 2024-05-07 21:08:23.000000 tmticket-0.1.8/tmticket/model.py
+-rw-r--r--   0 root         (0) root         (0)     4525 2024-05-07 21:08:23.000000 tmticket-0.1.8/tmticket/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 21:09:18.403718 tmticket-0.1.8/tmticket.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      736 2024-05-07 21:09:17.000000 tmticket-0.1.8/tmticket.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      261 2024-05-07 21:09:18.000000 tmticket-0.1.8/tmticket.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 21:09:17.000000 tmticket-0.1.8/tmticket.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 21:09:17.000000 tmticket-0.1.8/tmticket.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-07 21:09:17.000000 tmticket-0.1.8/tmticket.egg-info/top_level.txt
```

### Comparing `tmticket-0.1.0/pytmtickets/client.py` & `tmticket-0.1.8/tmticket/client.py`

 * *Files identical despite different names*

### Comparing `tmticket-0.1.0/pytmtickets/model.py` & `tmticket-0.1.8/tmticket/model.py`

 * *Files identical despite different names*

### Comparing `tmticket-0.1.0/pytmtickets/query.py` & `tmticket-0.1.8/tmticket/query.py`

 * *Files identical despite different names*

