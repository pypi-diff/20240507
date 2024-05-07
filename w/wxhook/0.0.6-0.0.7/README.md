# Comparing `tmp/wxhook-0.0.6.tar.gz` & `tmp/wxhook-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxhook-0.0.6.tar", last modified: Mon May  6 11:41:26 2024, max compression
+gzip compressed data, was "wxhook-0.0.7.tar", last modified: Mon May  6 12:03:52 2024, max compression
```

## Comparing `wxhook-0.0.6.tar` & `wxhook-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 11:41:26.092171 wxhook-0.0.6/
--rw-rw-rw-   0        0        0     1077 2024-05-06 06:49:40.000000 wxhook-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       51 2024-05-06 09:07:02.000000 wxhook-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     3397 2024-05-06 11:41:26.092171 wxhook-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2653 2024-05-06 10:56:59.000000 wxhook-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-06 11:41:26.093174 wxhook-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     3928 2024-05-06 11:41:17.000000 wxhook-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 11:41:26.067622 wxhook-0.0.6/wxhook/
--rw-rw-rw-   0        0        0       44 2024-05-06 11:41:17.000000 wxhook-0.0.6/wxhook/__init__.py
--rw-rw-rw-   0        0        0    16311 2024-05-06 11:32:10.000000 wxhook-0.0.6/wxhook/core.py
--rw-rw-rw-   0        0        0      630 2024-05-06 06:49:40.000000 wxhook-0.0.6/wxhook/events.py
--rw-rw-rw-   0        0        0      310 2024-05-06 08:37:49.000000 wxhook-0.0.6/wxhook/logger.py
--rw-rw-rw-   0        0        0     3930 2024-05-06 07:14:37.000000 wxhook-0.0.6/wxhook/model.py
-drwxrwxrwx   0        0        0        0 2024-05-06 11:41:26.090011 wxhook-0.0.6/wxhook/tools/
--rwxrwxrwx   0        0        0   270336 2024-05-06 06:49:40.000000 wxhook-0.0.6/wxhook/tools/faker.exe
--rwxrwxrwx   0        0        0   911872 2024-05-06 06:49:40.000000 wxhook-0.0.6/wxhook/tools/start-wechat.exe
--rw-rw-rw-   0        0        0   592384 2024-05-06 06:49:40.000000 wxhook-0.0.6/wxhook/tools/wxhook.dll
--rw-rw-rw-   0        0        0     3763 2024-05-06 11:32:10.000000 wxhook-0.0.6/wxhook/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-06 11:41:26.086893 wxhook-0.0.6/wxhook.egg-info/
--rw-rw-rw-   0        0        0     3397 2024-05-06 11:41:26.000000 wxhook-0.0.6/wxhook.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2024-05-06 11:41:26.000000 wxhook-0.0.6/wxhook.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 11:41:26.000000 wxhook-0.0.6/wxhook.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-06 11:41:26.000000 wxhook-0.0.6/wxhook.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-06 11:41:26.000000 wxhook-0.0.6/wxhook.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 12:03:52.675193 wxhook-0.0.7/
+-rw-rw-rw-   0        0        0     1077 2024-05-06 06:49:40.000000 wxhook-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0       51 2024-05-06 09:07:02.000000 wxhook-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     3397 2024-05-06 12:03:52.674183 wxhook-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2653 2024-05-06 10:56:59.000000 wxhook-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-06 12:03:52.675193 wxhook-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     3928 2024-05-06 12:03:30.000000 wxhook-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:03:52.648854 wxhook-0.0.7/wxhook/
+-rw-rw-rw-   0        0        0       44 2024-05-06 12:03:30.000000 wxhook-0.0.7/wxhook/__init__.py
+-rw-rw-rw-   0        0        0    16311 2024-05-06 12:02:21.000000 wxhook-0.0.7/wxhook/core.py
+-rw-rw-rw-   0        0        0      630 2024-05-06 06:49:40.000000 wxhook-0.0.7/wxhook/events.py
+-rw-rw-rw-   0        0        0      310 2024-05-06 08:37:49.000000 wxhook-0.0.7/wxhook/logger.py
+-rw-rw-rw-   0        0        0     3930 2024-05-06 07:14:37.000000 wxhook-0.0.7/wxhook/model.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:03:52.671823 wxhook-0.0.7/wxhook/tools/
+-rwxrwxrwx   0        0        0   270336 2024-05-06 06:49:40.000000 wxhook-0.0.7/wxhook/tools/faker.exe
+-rwxrwxrwx   0        0        0   911872 2024-05-06 06:49:40.000000 wxhook-0.0.7/wxhook/tools/start-wechat.exe
+-rw-rw-rw-   0        0        0   592384 2024-05-06 06:49:40.000000 wxhook-0.0.7/wxhook/tools/wxhook.dll
+-rw-rw-rw-   0        0        0     3785 2024-05-06 12:02:21.000000 wxhook-0.0.7/wxhook/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:03:52.666676 wxhook-0.0.7/wxhook.egg-info/
+-rw-rw-rw-   0        0        0     3397 2024-05-06 12:03:52.000000 wxhook-0.0.7/wxhook.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2024-05-06 12:03:52.000000 wxhook-0.0.7/wxhook.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 12:03:52.000000 wxhook-0.0.7/wxhook.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-06 12:03:52.000000 wxhook-0.0.7/wxhook.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-06 12:03:52.000000 wxhook-0.0.7/wxhook.egg-info/top_level.txt
```

### Comparing `wxhook-0.0.6/LICENSE` & `wxhook-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.6/PKG-INFO` & `wxhook-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxhook
-Version: 0.0.6
+Version: 0.0.7
 Summary: wechat robot framework.
 Home-page: https://github.com/miloira/wxhook
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `wxhook-0.0.6/README.md` & `wxhook-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.6/setup.py` & `wxhook-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'wxhook'
 DESCRIPTION = 'wechat robot framework.'
 URL = 'https://github.com/miloira/wxhook'
 EMAIL = '690126048@qq.com'
 AUTHOR = 'Msky'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'loguru',
     'psutil',
     'pyee',
     'requests',
```

### Comparing `wxhook-0.0.6/wxhook/core.py` & `wxhook-0.0.7/wxhook/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,18 +66,19 @@
         self.WXHELPER_PATH = None
         self.FILE_SAVE_PATH = None
         self.IMAGE_SAVE_PATH = None
         self.VIDEO_SAVE_PATH = None
 
         try:
             code, output = start_wechat_with_inject(self.remote_port)
-            if code == 1:
-                raise Exception(output)
         except Exception:
-            output = get_pid(self.remote_port)
+            code, output = get_pid(self.remote_port)
+
+        if code == 1:
+            raise Exception(output)
 
         self.process = psutil.Process(int(output))
 
         if self.faked_version is not None:
             if fake_wechat_version(self.process.pid, self.version, faked_version) == 0:
                 logger.success(f"wechat version faked: {self.version} -> {faked_version}")
             else:
```

### Comparing `wxhook-0.0.6/wxhook/events.py` & `wxhook-0.0.7/wxhook/events.py`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.6/wxhook/model.py` & `wxhook-0.0.7/wxhook/model.py`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.6/wxhook/tools/faker.exe` & `wxhook-0.0.7/wxhook/tools/faker.exe`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.6/wxhook/tools/start-wechat.exe` & `wxhook-0.0.7/wxhook/tools/start-wechat.exe`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.6/wxhook/tools/wxhook.dll` & `wxhook-0.0.7/wxhook/tools/wxhook.dll`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.6/wxhook/utils.py` & `wxhook-0.0.7/wxhook/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     processes = []
     for process in psutil.process_iter():
         if process.name().lower() == process_name.lower():
             processes.append(process)
     return processes
 
 
-def get_pid(port: int) -> int:
+def get_pid(port: int) -> typing.Tuple[int, int]:
     output = subprocess.run(f"netstat -ano | findStr \"{port}\"", capture_output=True, text=True, shell=True).stdout
-    return int(output.split("\n")[0].split("LISTENING")[-1])
+    return 0, int(output.split("\n")[0].split("LISTENING")[-1])
 
 
 def parse_xml(xml: str) -> dict:
     return xmltodict.parse(xml)
 
 
 def parse_event(event: dict, fields=None) -> dict:
```

### Comparing `wxhook-0.0.6/wxhook.egg-info/PKG-INFO` & `wxhook-0.0.7/wxhook.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxhook
-Version: 0.0.6
+Version: 0.0.7
 Summary: wechat robot framework.
 Home-page: https://github.com/miloira/wxhook
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

