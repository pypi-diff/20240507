# Comparing `tmp/erp5.util-0.4.8.tar.gz` & `tmp/erp5.util-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/erp5.util-0.4.8.tar", last modified: Thu Sep 27 14:24:55 2012, max compression
+gzip compressed data, was "dist/erp5.util-0.4.9.tar", last modified: Mon Oct  1 20:23:29 2012, max compression
```

## Comparing `erp5.util-0.4.8.tar` & `erp5.util-0.4.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-09-27 14:24:55.000000 erp5.util-0.4.8/
--rw-rw-r--   0 seb       (1000) seb       (1000)     8065 2012-09-27 14:24:55.000000 erp5.util-0.4.8/PKG-INFO
--rw-rw-r--   0 seb       (1000) seb       (1000)       59 2012-09-27 14:24:55.000000 erp5.util-0.4.8/setup.cfg
--rw-r--r--   0 seb       (1000) seb       (1000)      109 2011-07-22 04:22:42.000000 erp5.util-0.4.8/MANIFEST.in
--rw-rw-r--   0 seb       (1000) seb       (1000)     2999 2012-09-27 14:23:52.000000 erp5.util-0.4.8/CHANGES.erp5.util.txt
-drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-09-27 14:24:55.000000 erp5.util-0.4.8/erp5/
--rw-r--r--   0 seb       (1000) seb       (1000)      244 2011-07-22 04:22:42.000000 erp5.util-0.4.8/erp5/__init__.py
-drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-09-27 14:24:55.000000 erp5.util-0.4.8/erp5/util/
-drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-09-27 14:24:55.000000 erp5.util-0.4.8/erp5/util/timinglogparser/
--rwxrwxr-x   0 seb       (1000) seb       (1000)    10027 2012-09-05 14:30:24.000000 erp5.util-0.4.8/erp5/util/timinglogparser/__init__.py
-drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-09-27 14:24:55.000000 erp5.util-0.4.8/erp5/util/testbrowser/
--rw-rw-r--   0 seb       (1000) seb       (1000)    42708 2012-09-05 14:30:24.000000 erp5.util-0.4.8/erp5/util/testbrowser/browser.py
--rw-r--r--   0 seb       (1000) seb       (1000)        0 2011-09-06 08:51:46.000000 erp5.util-0.4.8/erp5/util/testbrowser/__init__.py
--rw-r--r--   0 seb       (1000) seb       (1000)      244 2011-07-22 04:22:42.000000 erp5.util-0.4.8/erp5/util/__init__.py
-drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-09-27 14:24:55.000000 erp5.util-0.4.8/erp5/util/testnode/
--rw-rw-r--   0 seb       (1000) seb       (1000)     5511 2012-04-30 12:05:35.000000 erp5.util-0.4.8/erp5/util/testnode/ProcessManager.py
--rw-rw-r--   0 seb       (1000) seb       (1000)     5384 2012-06-08 15:24:30.000000 erp5.util-0.4.8/erp5/util/testnode/__init__.py
--rw-rw-r--   0 seb       (1000) seb       (1000)     6478 2012-04-30 12:05:35.000000 erp5.util-0.4.8/erp5/util/testnode/Updater.py
-drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-09-27 14:24:55.000000 erp5.util-0.4.8/erp5/util/testnode/template/
--rw-r--r--   0 seb       (1000) seb       (1000)      226 2011-07-22 04:22:42.000000 erp5.util-0.4.8/erp5/util/testnode/template/slapos.cfg.in
--rw-rw-r--   0 seb       (1000) seb       (1000)     7139 2012-09-27 14:17:51.000000 erp5.util-0.4.8/erp5/util/testnode/SlapOSControler.py
--rw-rw-r--   0 seb       (1000) seb       (1000)    12304 2012-09-27 14:17:51.000000 erp5.util-0.4.8/erp5/util/testnode/testnode.py
-drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-09-27 14:24:55.000000 erp5.util-0.4.8/erp5/util/testsuite/
--rw-rw-r--   0 seb       (1000) seb       (1000)    10024 2012-09-05 14:30:24.000000 erp5.util-0.4.8/erp5/util/testsuite/__init__.py
-drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-09-27 14:24:55.000000 erp5.util-0.4.8/erp5/util/taskdistribution/
--rw-rw-r--   0 seb       (1000) seb       (1000)    16354 2012-09-05 14:30:24.000000 erp5.util-0.4.8/erp5/util/taskdistribution/__init__.py
-drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-09-27 14:24:55.000000 erp5.util-0.4.8/erp5/util/benchmark/
--rwxrwxr-x   0 seb       (1000) seb       (1000)    20224 2012-09-05 14:30:24.000000 erp5.util-0.4.8/erp5/util/benchmark/report.py
--rw-rw-r--   0 seb       (1000) seb       (1000)    12515 2012-01-24 14:58:29.000000 erp5.util-0.4.8/erp5/util/benchmark/result.py
--rw-r--r--   0 seb       (1000) seb       (1000)        0 2011-09-06 08:51:46.000000 erp5.util-0.4.8/erp5/util/benchmark/__init__.py
--rwxr-xr-x   0 seb       (1000) seb       (1000)    12312 2011-09-20 07:38:08.000000 erp5.util-0.4.8/erp5/util/benchmark/performance_tester.py
--rw-rw-r--   0 seb       (1000) seb       (1000)     6747 2011-12-05 20:47:31.000000 erp5.util-0.4.8/erp5/util/benchmark/process.py
--rw-r--r--   0 seb       (1000) seb       (1000)     3774 2011-10-06 09:36:53.000000 erp5.util-0.4.8/erp5/util/benchmark/argument.py
--rw-r--r--   0 seb       (1000) seb       (1000)     3482 2011-09-12 12:46:10.000000 erp5.util-0.4.8/erp5/util/benchmark/scalability_tester.py
-drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-09-27 14:24:55.000000 erp5.util-0.4.8/erp5/util/webchecker/
--rw-rw-r--   0 seb       (1000) seb       (1000)    27734 2012-01-31 10:30:45.000000 erp5.util-0.4.8/erp5/util/webchecker/__init__.py
-drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-09-27 14:24:55.000000 erp5.util-0.4.8/erp5/util/timinglogplotter/
--rwxrwxr-x   0 seb       (1000) seb       (1000)     9069 2012-09-05 14:30:24.000000 erp5.util-0.4.8/erp5/util/timinglogplotter/__init__.py
-lrwxrwxrwx   0 seb       (1000) seb       (1000)        0 2012-09-27 14:24:54.000000 erp5.util-0.4.8/README.txt -> README.erp5.util.txt
-drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-09-27 14:24:55.000000 erp5.util-0.4.8/erp5.util.egg-info/
--rw-rw-r--   0 seb       (1000) seb       (1000)     1079 2012-09-27 14:24:55.000000 erp5.util-0.4.8/erp5.util.egg-info/SOURCES.txt
--rw-rw-r--   0 seb       (1000) seb       (1000)        5 2012-09-27 14:24:54.000000 erp5.util-0.4.8/erp5.util.egg-info/top_level.txt
--rw-rw-r--   0 seb       (1000) seb       (1000)     8065 2012-09-27 14:24:54.000000 erp5.util-0.4.8/erp5.util.egg-info/PKG-INFO
--rw-rw-r--   0 seb       (1000) seb       (1000)      392 2012-09-27 14:24:54.000000 erp5.util-0.4.8/erp5.util.egg-info/entry_points.txt
--rw-rw-r--   0 seb       (1000) seb       (1000)      269 2012-09-27 14:24:54.000000 erp5.util-0.4.8/erp5.util.egg-info/requires.txt
--rw-rw-r--   0 seb       (1000) seb       (1000)        1 2012-04-11 17:22:28.000000 erp5.util-0.4.8/erp5.util.egg-info/zip-safe
--rw-rw-r--   0 seb       (1000) seb       (1000)       15 2012-09-27 14:24:54.000000 erp5.util-0.4.8/erp5.util.egg-info/namespace_packages.txt
--rw-rw-r--   0 seb       (1000) seb       (1000)        1 2012-09-27 14:24:54.000000 erp5.util-0.4.8/erp5.util.egg-info/dependency_links.txt
--rw-rw-r--   0 seb       (1000) seb       (1000)     2959 2012-09-27 14:24:26.000000 erp5.util-0.4.8/setup.py
--rw-r--r--   0 seb       (1000) seb       (1000)      117 2011-07-22 04:22:42.000000 erp5.util-0.4.8/README.erp5.util.txt
+drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-10-01 20:23:29.000000 erp5.util-0.4.9/
+-rw-rw-r--   0 seb       (1000) seb       (1000)     8302 2012-10-01 20:23:29.000000 erp5.util-0.4.9/PKG-INFO
+-rw-rw-r--   0 seb       (1000) seb       (1000)       59 2012-10-01 20:23:29.000000 erp5.util-0.4.9/setup.cfg
+-rw-r--r--   0 seb       (1000) seb       (1000)      109 2011-07-22 04:22:42.000000 erp5.util-0.4.9/MANIFEST.in
+-rw-rw-r--   0 seb       (1000) seb       (1000)     3172 2012-10-01 20:23:00.000000 erp5.util-0.4.9/CHANGES.erp5.util.txt
+drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-10-01 20:23:29.000000 erp5.util-0.4.9/erp5/
+-rw-r--r--   0 seb       (1000) seb       (1000)      244 2011-07-22 04:22:42.000000 erp5.util-0.4.9/erp5/__init__.py
+drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-10-01 20:23:29.000000 erp5.util-0.4.9/erp5/util/
+drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-10-01 20:23:29.000000 erp5.util-0.4.9/erp5/util/timinglogparser/
+-rwxrwxr-x   0 seb       (1000) seb       (1000)    10027 2012-09-05 14:30:24.000000 erp5.util-0.4.9/erp5/util/timinglogparser/__init__.py
+drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-10-01 20:23:29.000000 erp5.util-0.4.9/erp5/util/testbrowser/
+-rw-rw-r--   0 seb       (1000) seb       (1000)    42708 2012-09-05 14:30:24.000000 erp5.util-0.4.9/erp5/util/testbrowser/browser.py
+-rw-r--r--   0 seb       (1000) seb       (1000)        0 2011-09-06 08:51:46.000000 erp5.util-0.4.9/erp5/util/testbrowser/__init__.py
+-rw-r--r--   0 seb       (1000) seb       (1000)      244 2011-07-22 04:22:42.000000 erp5.util-0.4.9/erp5/util/__init__.py
+drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-10-01 20:23:29.000000 erp5.util-0.4.9/erp5/util/testnode/
+-rw-rw-r--   0 seb       (1000) seb       (1000)     5511 2012-04-30 12:05:35.000000 erp5.util-0.4.9/erp5/util/testnode/ProcessManager.py
+-rw-rw-r--   0 seb       (1000) seb       (1000)     5384 2012-06-08 15:24:30.000000 erp5.util-0.4.9/erp5/util/testnode/__init__.py
+-rw-rw-r--   0 seb       (1000) seb       (1000)     6478 2012-04-30 12:05:35.000000 erp5.util-0.4.9/erp5/util/testnode/Updater.py
+drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-10-01 20:23:29.000000 erp5.util-0.4.9/erp5/util/testnode/template/
+-rw-r--r--   0 seb       (1000) seb       (1000)      226 2011-07-22 04:22:42.000000 erp5.util-0.4.9/erp5/util/testnode/template/slapos.cfg.in
+-rw-rw-r--   0 seb       (1000) seb       (1000)     7131 2012-10-01 20:21:00.000000 erp5.util-0.4.9/erp5/util/testnode/SlapOSControler.py
+-rw-rw-r--   0 seb       (1000) seb       (1000)    12304 2012-09-28 08:02:52.000000 erp5.util-0.4.9/erp5/util/testnode/testnode.py
+drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-10-01 20:23:29.000000 erp5.util-0.4.9/erp5/util/testsuite/
+-rw-rw-r--   0 seb       (1000) seb       (1000)    10024 2012-09-05 14:30:24.000000 erp5.util-0.4.9/erp5/util/testsuite/__init__.py
+drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-10-01 20:23:29.000000 erp5.util-0.4.9/erp5/util/taskdistribution/
+-rw-rw-r--   0 seb       (1000) seb       (1000)    16354 2012-09-05 14:30:24.000000 erp5.util-0.4.9/erp5/util/taskdistribution/__init__.py
+drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-10-01 20:23:29.000000 erp5.util-0.4.9/erp5/util/benchmark/
+-rwxrwxr-x   0 seb       (1000) seb       (1000)    20224 2012-09-05 14:30:24.000000 erp5.util-0.4.9/erp5/util/benchmark/report.py
+-rw-rw-r--   0 seb       (1000) seb       (1000)    12515 2012-01-24 14:58:29.000000 erp5.util-0.4.9/erp5/util/benchmark/result.py
+-rw-r--r--   0 seb       (1000) seb       (1000)        0 2011-09-06 08:51:46.000000 erp5.util-0.4.9/erp5/util/benchmark/__init__.py
+-rwxr-xr-x   0 seb       (1000) seb       (1000)    12312 2011-09-20 07:38:08.000000 erp5.util-0.4.9/erp5/util/benchmark/performance_tester.py
+-rw-rw-r--   0 seb       (1000) seb       (1000)     6747 2011-12-05 20:47:31.000000 erp5.util-0.4.9/erp5/util/benchmark/process.py
+-rw-r--r--   0 seb       (1000) seb       (1000)     3774 2011-10-06 09:36:53.000000 erp5.util-0.4.9/erp5/util/benchmark/argument.py
+-rw-r--r--   0 seb       (1000) seb       (1000)     3482 2011-09-12 12:46:10.000000 erp5.util-0.4.9/erp5/util/benchmark/scalability_tester.py
+drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-10-01 20:23:29.000000 erp5.util-0.4.9/erp5/util/webchecker/
+-rw-rw-r--   0 seb       (1000) seb       (1000)    27734 2012-01-31 10:30:45.000000 erp5.util-0.4.9/erp5/util/webchecker/__init__.py
+drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-10-01 20:23:29.000000 erp5.util-0.4.9/erp5/util/timinglogplotter/
+-rwxrwxr-x   0 seb       (1000) seb       (1000)     9069 2012-09-05 14:30:24.000000 erp5.util-0.4.9/erp5/util/timinglogplotter/__init__.py
+lrwxrwxrwx   0 seb       (1000) seb       (1000)        0 2012-10-01 20:23:28.000000 erp5.util-0.4.9/README.txt -> README.erp5.util.txt
+drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2012-10-01 20:23:29.000000 erp5.util-0.4.9/erp5.util.egg-info/
+-rw-rw-r--   0 seb       (1000) seb       (1000)     1079 2012-10-01 20:23:29.000000 erp5.util-0.4.9/erp5.util.egg-info/SOURCES.txt
+-rw-rw-r--   0 seb       (1000) seb       (1000)        5 2012-10-01 20:23:28.000000 erp5.util-0.4.9/erp5.util.egg-info/top_level.txt
+-rw-rw-r--   0 seb       (1000) seb       (1000)     8302 2012-10-01 20:23:28.000000 erp5.util-0.4.9/erp5.util.egg-info/PKG-INFO
+-rw-rw-r--   0 seb       (1000) seb       (1000)      392 2012-10-01 20:23:28.000000 erp5.util-0.4.9/erp5.util.egg-info/entry_points.txt
+-rw-rw-r--   0 seb       (1000) seb       (1000)      269 2012-10-01 20:23:28.000000 erp5.util-0.4.9/erp5.util.egg-info/requires.txt
+-rw-rw-r--   0 seb       (1000) seb       (1000)        1 2012-04-11 17:22:28.000000 erp5.util-0.4.9/erp5.util.egg-info/zip-safe
+-rw-rw-r--   0 seb       (1000) seb       (1000)       15 2012-10-01 20:23:28.000000 erp5.util-0.4.9/erp5.util.egg-info/namespace_packages.txt
+-rw-rw-r--   0 seb       (1000) seb       (1000)        1 2012-10-01 20:23:28.000000 erp5.util-0.4.9/erp5.util.egg-info/dependency_links.txt
+-rw-rw-r--   0 seb       (1000) seb       (1000)     2959 2012-10-01 20:23:09.000000 erp5.util-0.4.9/setup.py
+-rw-r--r--   0 seb       (1000) seb       (1000)      117 2011-07-22 04:22:42.000000 erp5.util-0.4.9/README.erp5.util.txt
```

### Comparing `erp5.util-0.4.8/PKG-INFO` & `erp5.util-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: erp5.util
-Version: 0.4.8
+Version: 0.4.9
 Summary: ERP5 related utilities.
 Home-page: http://www.erp5.org
 Author: The ERP5 Development Team
 Author-email: erp5-dev@erp5.org
 License: GPLv3
 Description: erp5.util
         =========
@@ -103,14 +103,22 @@
         The utility must be run on same server where varnish is running.
         
         web_checker reads varnishlogs to detect if a Query goes to the backend.
         
         Changes
         =======
         
+        0.4.9 (2012-10-01)
+        ------------------
+        
+         * erp5.util.testnode:
+        
+          - remove --now parameter when calling slapgrid-sr since
+            it is not yet well supported [Sebastien Robin]
+        
         0.4.8 (2012-09-27)
         ------------------
         
          * erp5.util.testnode:
         
           - use taskdistribution module to reduce code
             [Vincent Pelletier], [Pere Cortes]
```

### Comparing `erp5.util-0.4.8/CHANGES.erp5.util.txt` & `erp5.util-0.4.9/CHANGES.erp5.util.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changes
 =======
 
+0.4.9 (2012-10-01)
+------------------
+
+ * erp5.util.testnode:
+
+  - remove --now parameter when calling slapgrid-sr since
+    it is not yet well supported [Sebastien Robin]
+
 0.4.8 (2012-09-27)
 ------------------
 
  * erp5.util.testnode:
 
   - use taskdistribution module to reduce code
     [Vincent Pelletier], [Pere Cortes]
```

### Comparing `erp5.util-0.4.8/erp5/util/timinglogparser/__init__.py` & `erp5.util-0.4.9/erp5/util/timinglogparser/__init__.py`

 * *Files identical despite different names*

### Comparing `erp5.util-0.4.8/erp5/util/testbrowser/browser.py` & `erp5.util-0.4.9/erp5/util/testbrowser/browser.py`

 * *Files identical despite different names*

### Comparing `erp5.util-0.4.8/erp5/util/testnode/ProcessManager.py` & `erp5.util-0.4.9/erp5/util/testnode/ProcessManager.py`

 * *Files identical despite different names*

### Comparing `erp5.util-0.4.8/erp5/util/testnode/__init__.py` & `erp5.util-0.4.9/erp5/util/testnode/__init__.py`

 * *Files identical despite different names*

### Comparing `erp5.util-0.4.8/erp5/util/testnode/Updater.py` & `erp5.util-0.4.9/erp5/util/testnode/Updater.py`

 * *Files identical despite different names*

### Comparing `erp5.util-0.4.8/erp5/util/testnode/SlapOSControler.py` & `erp5.util-0.4.9/erp5/util/testnode/SlapOSControler.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     self.log("SlapOSControler.runSoftwareRelease")
     cpu_count = os.sysconf("SC_NPROCESSORS_ONLN")
     os.putenv('MAKEFLAGS', '-j%s' % cpu_count)
     os.environ['PATH'] = environment['PATH']
     # a SR may fail for number of reasons (incl. network failures)
     # so be tolerant and run it a few times before giving up
     for runs in range(0, MAX_SR_RETRIES):
-      status_dict = self.spawn(config['slapgrid_software_binary'], '-v', '-c','--now',
+      status_dict = self.spawn(config['slapgrid_software_binary'], '-v', '-c',
                  config['slapos_config'], raise_error_if_fail=False,
                  log_prefix='slapgrid_sr', get_output=False)
     return status_dict
 
   def runComputerPartition(self, config, environment,
                            stdout=None, stderr=None):
     self.log("SlapOSControler.runComputerPartition")
```

### Comparing `erp5.util-0.4.8/erp5/util/testnode/testnode.py` & `erp5.util-0.4.9/erp5/util/testnode/testnode.py`

 * *Files identical despite different names*

### Comparing `erp5.util-0.4.8/erp5/util/testsuite/__init__.py` & `erp5.util-0.4.9/erp5/util/testsuite/__init__.py`

 * *Files identical despite different names*

### Comparing `erp5.util-0.4.8/erp5/util/taskdistribution/__init__.py` & `erp5.util-0.4.9/erp5/util/taskdistribution/__init__.py`

 * *Files identical despite different names*

### Comparing `erp5.util-0.4.8/erp5/util/benchmark/report.py` & `erp5.util-0.4.9/erp5/util/benchmark/report.py`

 * *Files identical despite different names*

### Comparing `erp5.util-0.4.8/erp5/util/benchmark/result.py` & `erp5.util-0.4.9/erp5/util/benchmark/result.py`

 * *Files identical despite different names*

### Comparing `erp5.util-0.4.8/erp5/util/benchmark/performance_tester.py` & `erp5.util-0.4.9/erp5/util/benchmark/performance_tester.py`

 * *Files identical despite different names*

### Comparing `erp5.util-0.4.8/erp5/util/benchmark/process.py` & `erp5.util-0.4.9/erp5/util/benchmark/process.py`

 * *Files identical despite different names*

### Comparing `erp5.util-0.4.8/erp5/util/benchmark/argument.py` & `erp5.util-0.4.9/erp5/util/benchmark/argument.py`

 * *Files identical despite different names*

### Comparing `erp5.util-0.4.8/erp5/util/benchmark/scalability_tester.py` & `erp5.util-0.4.9/erp5/util/benchmark/scalability_tester.py`

 * *Files identical despite different names*

### Comparing `erp5.util-0.4.8/erp5/util/webchecker/__init__.py` & `erp5.util-0.4.9/erp5/util/webchecker/__init__.py`

 * *Files identical despite different names*

### Comparing `erp5.util-0.4.8/erp5/util/timinglogplotter/__init__.py` & `erp5.util-0.4.9/erp5/util/timinglogplotter/__init__.py`

 * *Files identical despite different names*

### Comparing `erp5.util-0.4.8/erp5.util.egg-info/SOURCES.txt` & `erp5.util-0.4.9/erp5.util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `erp5.util-0.4.8/erp5.util.egg-info/PKG-INFO` & `erp5.util-0.4.9/erp5.util.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: erp5.util
-Version: 0.4.8
+Version: 0.4.9
 Summary: ERP5 related utilities.
 Home-page: http://www.erp5.org
 Author: The ERP5 Development Team
 Author-email: erp5-dev@erp5.org
 License: GPLv3
 Description: erp5.util
         =========
@@ -103,14 +103,22 @@
         The utility must be run on same server where varnish is running.
         
         web_checker reads varnishlogs to detect if a Query goes to the backend.
         
         Changes
         =======
         
+        0.4.9 (2012-10-01)
+        ------------------
+        
+         * erp5.util.testnode:
+        
+          - remove --now parameter when calling slapgrid-sr since
+            it is not yet well supported [Sebastien Robin]
+        
         0.4.8 (2012-09-27)
         ------------------
         
          * erp5.util.testnode:
         
           - use taskdistribution module to reduce code
             [Vincent Pelletier], [Pere Cortes]
```

### Comparing `erp5.util-0.4.8/setup.py` & `erp5.util-0.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import glob
 import os
 
-version = '0.4.8'
+version = '0.4.9'
 name = 'erp5.util'
 long_description = open("README.erp5.util.txt").read() + "\n"
 
 for f in sorted(glob.glob(os.path.join('erp5', 'util', 'README.*.txt'))):
   long_description += '\n' + open(f).read() + '\n'
 
 long_description += open("CHANGES.erp5.util.txt").read() + "\n"
```

