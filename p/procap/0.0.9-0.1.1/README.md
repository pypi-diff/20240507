# Comparing `tmp/procap-0.0.9.tar.gz` & `tmp/procap-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\procap-0.0.9.tar", last modified: Tue May  7 16:13:48 2024, max compression
+gzip compressed data, was "dist\procap-0.1.1.tar", last modified: Tue May  7 16:20:46 2024, max compression
```

## Comparing `procap-0.0.9.tar` & `procap-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 16:13:48.868793 procap-0.0.9/
--rw-rw-rw-   0        0        0     2940 2024-05-07 16:13:48.866795 procap-0.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-07 16:13:48.839681 procap-0.0.9/ProCap/
--rw-rw-rw-   0        0        0     2656 2024-05-07 16:05:54.000000 procap-0.0.9/ProCap/__init__.py
--rw-rw-rw-   0        0        0     2338 2024-05-07 16:08:57.000000 procap-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 16:13:48.863796 procap-0.0.9/procap.egg-info/
--rw-rw-rw-   0        0        0     2940 2024-05-07 16:13:48.000000 procap-0.0.9/procap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2024-05-07 16:13:48.000000 procap-0.0.9/procap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 16:13:48.000000 procap-0.0.9/procap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-07 16:13:48.000000 procap-0.0.9/procap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-07 16:13:48.000000 procap-0.0.9/procap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 16:13:48.868793 procap-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      802 2024-05-07 16:13:42.000000 procap-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 16:20:46.034277 procap-0.1.1/
+-rw-rw-rw-   0        0        0     2940 2024-05-07 16:20:46.032278 procap-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-07 16:20:45.999298 procap-0.1.1/ProCap/
+-rw-rw-rw-   0        0        0     2676 2024-05-07 16:19:31.000000 procap-0.1.1/ProCap/__init__.py
+-rw-rw-rw-   0        0        0     2338 2024-05-07 16:08:57.000000 procap-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 16:20:46.030280 procap-0.1.1/procap.egg-info/
+-rw-rw-rw-   0        0        0     2940 2024-05-07 16:20:45.000000 procap-0.1.1/procap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2024-05-07 16:20:45.000000 procap-0.1.1/procap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 16:20:45.000000 procap-0.1.1/procap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-07 16:20:45.000000 procap-0.1.1/procap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-07 16:20:45.000000 procap-0.1.1/procap.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 16:20:46.034277 procap-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      802 2024-05-07 16:20:39.000000 procap-0.1.1/setup.py
```

### Comparing `procap-0.0.9/PKG-INFO` & `procap-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: procap
-Version: 0.0.9
+Version: 0.1.1
 Summary: ProCap is a captcha solving service.
 Author: ProCap
 Keywords: python,captcha,solver,hcaptcha,procap,captcha solver,hcaptcha solver,captcha bypass,cheap solver,cheap captcha solver,cheap hcaptcha solver
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `procap-0.0.9/ProCap/__init__.py` & `procap-0.1.1/ProCap/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self.response = response
 class ProCap:
     def __init__(self, apikey) -> None:
         self.apikey = apikey
     def get_balance(self):
         request = requests.get("https://api.procap.wtf/user")
         return User(request.json())
-    def createTask(self, url, sitekey, proxy=None, userAgent=None, rqdata=None, isEnterprise=False, type="hCaptchaTask"):
+    def createTask(self, url=None, sitekey=None, proxy=None, userAgent=None, rqdata=None, isEnterprise=False, type="hCaptchaTask"):
         payload = {
             "clientKey": self.apikey,
             "task": {
                 "type": type,
                 "href":url,
                 "sitekey": sitekey,
                 "proxy": proxy,
@@ -45,15 +45,15 @@
         return Task(request)
     def checkTask(self, id):
         request = requests.get("https://api.procap.wtf/checkTask", json={
             "clientKey": self.apikey,
             "taskId": id
         })
         return Task(request.json())
-    def solve(self, url, sitekey, proxy=None, userAgent=None, rqdata=None, isEnterprise=False, type="hCaptchaTask"):
+    def solve(self, url=None, sitekey=None, proxy=None, userAgent=None, rqdata=None, isEnterprise=False, type="hCaptchaTask"):
         task = self.createTask(url, sitekey, proxy, userAgent, rqdata, isEnterprise, type)
         if task.error:
             return task.error
         while True:
             captcha_challenge = self.checkTask(task.id)
             if not captcha_challenge.status == "processing" and not captcha_challenge.status == "ready":
                 return None
```

### Comparing `procap-0.0.9/README.md` & `procap-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `procap-0.0.9/procap.egg-info/PKG-INFO` & `procap-0.1.1/procap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: procap
-Version: 0.0.9
+Version: 0.1.1
 Summary: ProCap is a captcha solving service.
 Author: ProCap
 Keywords: python,captcha,solver,hcaptcha,procap,captcha solver,hcaptcha solver,captcha bypass,cheap solver,cheap captcha solver,cheap hcaptcha solver
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `procap-0.0.9/setup.py` & `procap-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-VERSION = "0.0.9"
+VERSION = "0.1.1"
 DESCRIPTION = "ProCap is a captcha solving service."
 LONG_DESCRIPTION = open("README.md", encoding="utf-8").read()
 
 setup(
     name="procap",
     version=VERSION,
     author="ProCap",
```

