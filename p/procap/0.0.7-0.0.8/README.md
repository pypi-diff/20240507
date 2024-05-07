# Comparing `tmp/procap-0.0.7.tar.gz` & `tmp/procap-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\procap-0.0.7.tar", last modified: Mon Mar 25 22:17:03 2024, max compression
+gzip compressed data, was "dist\procap-0.0.8.tar", last modified: Tue May  7 16:06:57 2024, max compression
```

## Comparing `procap-0.0.7.tar` & `procap-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 22:17:03.787202 procap-0.0.7/
--rw-rw-rw-   0        0        0      549 2024-03-25 22:17:03.786203 procap-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-25 22:17:03.731235 procap-0.0.7/ProCap/
--rw-rw-rw-   0        0        0     2466 2024-03-25 22:11:09.000000 procap-0.0.7/ProCap/__init__.py
--rw-rw-rw-   0        0        0     1692 2024-02-29 12:49:40.000000 procap-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-03-25 22:17:03.784202 procap-0.0.7/procap.egg-info/
--rw-rw-rw-   0        0        0      549 2024-03-25 22:17:03.000000 procap-0.0.7/procap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2024-03-25 22:17:03.000000 procap-0.0.7/procap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 22:17:03.000000 procap-0.0.7/procap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-25 22:17:03.000000 procap-0.0.7/procap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-25 22:17:03.000000 procap-0.0.7/procap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-25 22:17:03.788200 procap-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      787 2024-03-25 22:13:55.000000 procap-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 16:06:57.403962 procap-0.0.8/
+-rw-rw-rw-   0        0        0      549 2024-05-07 16:06:57.401962 procap-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-07 16:06:57.316805 procap-0.0.8/ProCap/
+-rw-rw-rw-   0        0        0     2656 2024-05-07 16:05:54.000000 procap-0.0.8/ProCap/__init__.py
+-rw-rw-rw-   0        0        0     1692 2024-02-29 12:49:40.000000 procap-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 16:06:57.399961 procap-0.0.8/procap.egg-info/
+-rw-rw-rw-   0        0        0      549 2024-05-07 16:06:54.000000 procap-0.0.8/procap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2024-05-07 16:06:55.000000 procap-0.0.8/procap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 16:06:54.000000 procap-0.0.8/procap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-07 16:06:54.000000 procap-0.0.8/procap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-07 16:06:54.000000 procap-0.0.8/procap.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 16:06:57.403962 procap-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      787 2024-05-07 16:06:41.000000 procap-0.0.8/setup.py
```

### Comparing `procap-0.0.7/PKG-INFO` & `procap-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: procap
-Version: 0.0.7
+Version: 0.0.8
 Summary: ProCap is a captcha solving service.
 Author: ProCap
 Keywords: python,captcha,solver,hcaptcha,procap,captcha solver,hcaptcha solver,captcha bypass,cheap solver,cheap captcha solver,cheap hcaptcha solver
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `procap-0.0.7/ProCap/__init__.py` & `procap-0.0.8/ProCap/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,62 @@
 import requests
 import time
 class Task:
     def __init__(self, response: dict) -> None:
-        self.id = response.get("ID")
-        self.time = response.get("Time")
-        self.message = response.get("Message")
-        self.success = response.get("Success")
-        self.token = response["Results"].get("Pass")
-        self.challengeKey = response["Results"].get("ChallengeKey")
+        self.id = response.get("taskId")
+        self.time = response.get("time")
+        self.success = response.get("success")
+        self.error = response.get("error")
+        self.status = response.get("status")
+        self.token = response.get("solution").get("generated_pass_uuid")
+        self.challengeKey = response.get("solution").get("challenge_key")
         self.response = response
+
 class User:
     def __init__(self, response: dict) -> None:
         self.balance = response.get("balance")
         self.daily_limit = response.get("daily_limit")
         self.next_reset = response.get("next_reset")
         self.daily_used = response.get("daily_used")
         self.daily_remaining = response.get("daily_remaining")
         self.plan_expire = response.get("plan_expire")
         self.response = response
 class ProCap:
     def __init__(self, apikey) -> None:
         self.apikey = apikey
-        self.headers = {"apikey": apikey}
     def get_balance(self):
-        request = requests.get("https://api.procap.wtf/user", headers=self.headers)
+        request = requests.get("https://api.procap.wtf/user")
         return User(request.json())
-    def createTask(self, url, sitekey, proxy=None, userAgent=None, rqdata=None, isEnterprise=False):
+    def createTask(self, url, sitekey, proxy=None, userAgent=None, rqdata=None, isEnterprise=False, type="hCaptchaTask"):
         payload = {
-            "url": url,
-            "sitekey": sitekey,
-            "proxy": proxy,
-            "userAgent": userAgent,
-            "isEnterprise": isEnterprise,
-            "rqdata": rqdata
+            "clientKey": self.apikey,
+            "task": {
+                "type": type,
+                "href":url,
+                "sitekey": sitekey,
+                "proxy": proxy,
+                "useragent": userAgent,
+                "rqdata": rqdata,
+            }
         }
-        request = requests.post("https://api.procap.wtf/createTask", json=payload, headers=self.headers)
-        return Task(request.json())
+        if "hcaptcha" in type and isEnterprise:
+            payload.update({"isEnterprise": isEnterprise})
+        request = requests.post("https://api.procap.wtf/createTask", json=payload).json()
+        request["solution"] = {}
+        return Task(request)
     def checkTask(self, id):
-        request = requests.get("https://api.procap.wtf/checkTask/"+id)
+        request = requests.get("https://api.procap.wtf/checkTask", json={
+            "clientKey": self.apikey,
+            "taskId": id
+        })
         return Task(request.json())
-    def solve(self, url, sitekey, proxy=None, userAgent=None, rqdata=None, isEnterprise=False):
-        while True:
-            task = self.createTask(url, sitekey, proxy, userAgent, rqdata, isEnterprise)
-            if "busy" not in task.message:
-                break
-            else:
-                time.sleep(5)
-        if not task.success:
-            return task.message
+    def solve(self, url, sitekey, proxy=None, userAgent=None, rqdata=None, isEnterprise=False, type="hCaptchaTask"):
+        task = self.createTask(url, sitekey, proxy, userAgent, rqdata, isEnterprise, type)
+        if task.error:
+            return task.error
         while True:
             captcha_challenge = self.checkTask(task.id)
-            if captcha_challenge.message != "solving" and captcha_challenge.message != "solved":
+            if not captcha_challenge.status == "processing" and not captcha_challenge.status == "ready":
                 return None
-            if captcha_challenge.message == "solved":
+            if captcha_challenge.token:
                 return captcha_challenge.token
-            time.sleep(1)
+            time.sleep(0.5)
```

### Comparing `procap-0.0.7/README.md` & `procap-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `procap-0.0.7/procap.egg-info/PKG-INFO` & `procap-0.0.8/procap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: procap
-Version: 0.0.7
+Version: 0.0.8
 Summary: ProCap is a captcha solving service.
 Author: ProCap
 Keywords: python,captcha,solver,hcaptcha,procap,captcha solver,hcaptcha solver,captcha bypass,cheap solver,cheap captcha solver,cheap hcaptcha solver
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `procap-0.0.7/setup.py` & `procap-0.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-VERSION = "0.0.7"
+VERSION = "0.0.8"
 DESCRIPTION = "ProCap is a captcha solving service."
 LONG_DESCRIPTION = "A api wrapper for ProCap."
 
 setup(
     name="procap",
     version=VERSION,
     author="ProCap",
```

