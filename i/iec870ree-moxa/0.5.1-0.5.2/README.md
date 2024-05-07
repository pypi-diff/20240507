# Comparing `tmp/iec870ree_moxa-0.5.1.tar.gz` & `tmp/iec870ree_moxa-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/iec870ree_moxa-0.5.1.tar", last modified: Thu Dec 23 12:26:30 2021, max compression
+gzip compressed data, was "dist/iec870ree_moxa-0.5.2.tar", last modified: Tue May  7 09:03:43 2024, max compression
```

## Comparing `iec870ree_moxa-0.5.1.tar` & `iec870ree_moxa-0.5.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2021-12-23 12:26:30.000000 iec870ree_moxa-0.5.1/
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2021-12-23 12:26:30.000000 iec870ree_moxa-0.5.1/iec870ree_moxa.egg-info/
--rw-r--r--   0 afita     (1000) afita     (1000)       15 2021-12-23 12:26:30.000000 iec870ree_moxa-0.5.1/iec870ree_moxa.egg-info/top_level.txt
--rw-r--r--   0 afita     (1000) afita     (1000)      258 2021-12-23 12:26:30.000000 iec870ree_moxa-0.5.1/iec870ree_moxa.egg-info/SOURCES.txt
--rw-r--r--   0 afita     (1000) afita     (1000)     2021 2021-12-23 12:26:30.000000 iec870ree_moxa-0.5.1/iec870ree_moxa.egg-info/PKG-INFO
--rw-r--r--   0 afita     (1000) afita     (1000)        1 2021-12-23 12:26:30.000000 iec870ree_moxa-0.5.1/iec870ree_moxa.egg-info/dependency_links.txt
--rw-r--r--   0 afita     (1000) afita     (1000)       14 2021-12-23 12:26:30.000000 iec870ree_moxa-0.5.1/iec870ree_moxa.egg-info/requires.txt
--rw-rw-r--   0 afita     (1000) afita     (1000)     2021 2021-12-23 12:26:30.000000 iec870ree_moxa-0.5.1/PKG-INFO
--rw-rw-r--   0 afita     (1000) afita     (1000)       38 2021-12-23 12:26:30.000000 iec870ree_moxa-0.5.1/setup.cfg
--rw-r--r--   0 afita     (1000) afita     (1000)      724 2021-12-23 12:25:39.000000 iec870ree_moxa-0.5.1/setup.py
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2021-12-23 12:26:30.000000 iec870ree_moxa-0.5.1/iec870ree_moxa/
--rw-rw-r--   0 afita     (1000) afita     (1000)     5312 2021-12-23 12:25:18.000000 iec870ree_moxa-0.5.1/iec870ree_moxa/moxa.py
--rw-r--r--   0 afita     (1000) afita     (1000)       23 2020-03-30 08:48:14.000000 iec870ree_moxa-0.5.1/iec870ree_moxa/__init__.py
--rw-r--r--   0 afita     (1000) afita     (1000)     1247 2020-03-30 08:48:14.000000 iec870ree_moxa-0.5.1/README.rst
+drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2024-05-07 09:03:43.000000 iec870ree_moxa-0.5.2/
+drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2024-05-07 09:03:43.000000 iec870ree_moxa-0.5.2/iec870ree_moxa.egg-info/
+-rw-r--r--   0 afita     (1000) afita     (1000)       15 2024-05-07 09:03:43.000000 iec870ree_moxa-0.5.2/iec870ree_moxa.egg-info/top_level.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)      258 2024-05-07 09:03:43.000000 iec870ree_moxa-0.5.2/iec870ree_moxa.egg-info/SOURCES.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)     2021 2024-05-07 09:03:43.000000 iec870ree_moxa-0.5.2/iec870ree_moxa.egg-info/PKG-INFO
+-rw-r--r--   0 afita     (1000) afita     (1000)        1 2024-05-07 09:03:43.000000 iec870ree_moxa-0.5.2/iec870ree_moxa.egg-info/dependency_links.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)       14 2024-05-07 09:03:43.000000 iec870ree_moxa-0.5.2/iec870ree_moxa.egg-info/requires.txt
+-rw-rw-r--   0 afita     (1000) afita     (1000)     2021 2024-05-07 09:03:43.000000 iec870ree_moxa-0.5.2/PKG-INFO
+-rw-rw-r--   0 afita     (1000) afita     (1000)       38 2024-05-07 09:03:43.000000 iec870ree_moxa-0.5.2/setup.cfg
+-rw-r--r--   0 afita     (1000) afita     (1000)      724 2024-05-07 09:02:05.000000 iec870ree_moxa-0.5.2/setup.py
+drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2024-05-07 09:03:43.000000 iec870ree_moxa-0.5.2/iec870ree_moxa/
+-rw-rw-r--   0 afita     (1000) afita     (1000)     5531 2024-05-07 09:01:57.000000 iec870ree_moxa-0.5.2/iec870ree_moxa/moxa.py
+-rw-r--r--   0 afita     (1000) afita     (1000)       23 2020-03-30 08:48:14.000000 iec870ree_moxa-0.5.2/iec870ree_moxa/__init__.py
+-rw-r--r--   0 afita     (1000) afita     (1000)     1247 2020-03-30 08:48:14.000000 iec870ree_moxa-0.5.2/README.rst
```

### Comparing `iec870ree_moxa-0.5.1/iec870ree_moxa.egg-info/PKG-INFO` & `iec870ree_moxa-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: iec870ree-moxa
-Version: 0.5.1
+Name: iec870ree_moxa
+Version: 0.5.2
 Summary: Physical layer for using a Moxa devices with IEC870REE library
 Home-page: http://www.gisce.net
 Author: GISCE-TI, S.L.
 Author-email: devel@gisce.net
 License: AGPL3
 Description: Moxa Physical layer
         ===================
```

### Comparing `iec870ree_moxa-0.5.1/PKG-INFO` & `iec870ree_moxa-0.5.2/iec870ree_moxa.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: iec870ree_moxa
-Version: 0.5.1
+Name: iec870ree-moxa
+Version: 0.5.2
 Summary: Physical layer for using a Moxa devices with IEC870REE library
 Home-page: http://www.gisce.net
 Author: GISCE-TI, S.L.
 Author-email: devel@gisce.net
 License: AGPL3
 Description: Moxa Physical layer
         ===================
```

### Comparing `iec870ree_moxa-0.5.1/setup.py` & `iec870ree_moxa-0.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst') as f:
     readme = f.read()
 
 setup(
     name="iec870ree_moxa",
-    version="0.5.1",
+    version="0.5.2",
     author="GISCE-TI, S.L.",
     author_email="devel@gisce.net",
     description="Physical layer for using a Moxa devices with IEC870REE library",
     license='AGPL3',
     keywords="REE electric meters IEC 870-5-102",
     url="http://www.gisce.net",
     install_requires=[
```

### Comparing `iec870ree_moxa-0.5.1/iec870ree_moxa/moxa.py` & `iec870ree_moxa-0.5.2/iec870ree_moxa/moxa.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,46 +47,55 @@
         try:
             self.ip.connect()
             self.initialize_modem()
         except Exception as e:
             self.disconnect()
             raise ConnectionError(e)
 
+    def empty_queue(self):
+        for i in range(80):
+            try:
+                self.queue.get(False, 1)
+            except:
+                # Empty
+                break
+
     def initialize_modem(self):
         self.writeat("+++", no_r=True)
         time.sleep(3)
 
         split_write_sleep = self.init_string.split(';')
         for x in split_write_sleep:
             init_text, init_sleep = x.split(':')
             if not init_text.strip() or not init_sleep.strip():
                 raise "Init modem string has some empty values."
             self.writeat(init_text)
             time.sleep(int(init_sleep))
 
+        self.empty_queue()
         self.writeat("ATD" + str(self.phone_number))
         self.waitforconnect()
         time.sleep(self.ip.waiting)
 
     def waitforconnect(self):
         max_tries = 80
         for i in range(max_tries):
             try:
-                i = self.queue.get(False, 1)
-                logger.debug("got message> {}".format(i))
+                data = self.queue.get(False, 1)
+                logger.debug("got message> {}".format(data))
                 for word in self.CONNECTED_WORDS:
 
-                    if word in i:
+                    if word in data:
                         logger.debug("---- CONNECTION SUCCEEDED ----")
                         self.data_mode = True
                         self.queue.task_done()
                         time.sleep(5)  # everything smooth in read thread
                         return
                 for word in self.NO_CONNECT_WORDS:
-                    if word in i:
+                    if word in data:
                         logger.debug("--- NOT CONNECTED ---")
                         raise ConnectionError("Connection not stablished: {}".format(word))
                 self.queue.task_done()
             except queue.Empty:
                 logger.debug("nothing yet...")
                 time.sleep(1)
         raise ConnectionError("Error Waiting for connection")
```

### Comparing `iec870ree_moxa-0.5.1/README.rst` & `iec870ree_moxa-0.5.2/README.rst`

 * *Files identical despite different names*

