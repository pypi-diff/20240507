# Comparing `tmp/procap-0.0.8.tar.gz` & `tmp/procap-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\procap-0.0.8.tar", last modified: Tue May  7 16:06:57 2024, max compression
+gzip compressed data, was "dist\procap-0.0.9.tar", last modified: Tue May  7 16:13:48 2024, max compression
```

## Comparing `procap-0.0.8.tar` & `procap-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 16:06:57.403962 procap-0.0.8/
--rw-rw-rw-   0        0        0      549 2024-05-07 16:06:57.401962 procap-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-07 16:06:57.316805 procap-0.0.8/ProCap/
--rw-rw-rw-   0        0        0     2656 2024-05-07 16:05:54.000000 procap-0.0.8/ProCap/__init__.py
--rw-rw-rw-   0        0        0     1692 2024-02-29 12:49:40.000000 procap-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 16:06:57.399961 procap-0.0.8/procap.egg-info/
--rw-rw-rw-   0        0        0      549 2024-05-07 16:06:54.000000 procap-0.0.8/procap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2024-05-07 16:06:55.000000 procap-0.0.8/procap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 16:06:54.000000 procap-0.0.8/procap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-07 16:06:54.000000 procap-0.0.8/procap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-07 16:06:54.000000 procap-0.0.8/procap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 16:06:57.403962 procap-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      787 2024-05-07 16:06:41.000000 procap-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 16:13:48.868793 procap-0.0.9/
+-rw-rw-rw-   0        0        0     2940 2024-05-07 16:13:48.866795 procap-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-07 16:13:48.839681 procap-0.0.9/ProCap/
+-rw-rw-rw-   0        0        0     2656 2024-05-07 16:05:54.000000 procap-0.0.9/ProCap/__init__.py
+-rw-rw-rw-   0        0        0     2338 2024-05-07 16:08:57.000000 procap-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 16:13:48.863796 procap-0.0.9/procap.egg-info/
+-rw-rw-rw-   0        0        0     2940 2024-05-07 16:13:48.000000 procap-0.0.9/procap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2024-05-07 16:13:48.000000 procap-0.0.9/procap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 16:13:48.000000 procap-0.0.9/procap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-07 16:13:48.000000 procap-0.0.9/procap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-07 16:13:48.000000 procap-0.0.9/procap.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 16:13:48.868793 procap-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      802 2024-05-07 16:13:42.000000 procap-0.0.9/setup.py
```

### Comparing `procap-0.0.8/ProCap/__init__.py` & `procap-0.0.9/ProCap/__init__.py`

 * *Files identical despite different names*

### Comparing `procap-0.0.8/README.md` & `procap-0.0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -7,55 +7,73 @@
 ```
 
 ### ⚠️ Requirements
 * Apikey : **Join [ProCap](https://procap.wtf/), to get api key**
 
 ### 💡 Examples
 
-* 1 - Example (Solve)
+* 1 - Example (hCaptcha Solve)
 
 ```python
-from procap import ProCap
+from ProCap import ProCap
 apikey = "" # Api key (required)
 url = "" # Link to captcha (required)
 sitekey = "" # Sitekey (required)
 proxy = "" # Proxy (optional)
 userAgent = "" # User agent (optional)
 rqdata = "" # RQData (optional)
 solver = ProCap(apikey)
-captchaToken = solver.solve(url=url, sitekey=sitekey, proxy=proxy, userAgent=userAgent, rqdata=rqdata)
+captchaToken = solver.solve(url=url, sitekey=sitekey, proxy=proxy, userAgent=userAgent, rqdata=rqdata, type="hCaptchaTask")
+print(f"Captcha token : {captchaToken}")
 ```
 
-* 2 - Example 2 (Create task)
+* 2 - Example 2 (Create task for hCaptcha)
 
 ```python
-from procap import ProCap
+from ProCap import ProCap
 apikey = "" # Api key (required)
 url = "" # Link to captcha (required)
 sitekey = "" # Sitekey (required)
 proxy = "" # Proxy (optional)
 userAgent = "" # User agent (optional)
 rqdata = "" # RQData (optional)
 solver = ProCap(apikey)
-captchaTask = solver.createTask(url=url, sitekey=sitekey, proxy=proxy, userAgent=userAgent, rqdata=rqdata)
+captchaTask = solver.createTask(url=url, sitekey=sitekey, proxy=proxy, userAgent=userAgent, rqdata=rqdata, type="hCaptchaTask")
 captchaTask.id # Task id
 captchaTask.time # Time taken
 captchaTask.message # Message
 captchaTask.success # Success [True or False]
 captchaTask.token # Captcha Token (if solved)
 captchaTask.challengeKey # Captcha challenge key
+captchaTask.response # Get api json response
 ```
 
 * 3 - Example (Get Task Result)
 ```python
-from procap import ProCap
+from ProCap import ProCap
 apikey = "" # Your api key
 solver = ProCap(apikey)
 id = "Challenge ID" 
 captchaTask = solver.checkTask(id)
 captchaTask.id # Task id
 captchaTask.time # Time taken
 captchaTask.message # Message
 captchaTask.success # Success [True or False]
 captchaTask.token # Captcha Token (if solved)
 captchaTask.challengeKey # Captcha challenge key
+captchaTask.response # Get api json response
 ```
+
+* 4 - Example (Get account information)
+```python
+from ProCap import ProCap
+apikey = "" # Api key (required)
+solver = ProCap(apikey)
+user = solver.get_balance()
+user.balance # Get user balance
+user.daily_limit # Get user daily limit
+user.next_reset # Get user next credits reset
+user.daily_used # Get user daily used
+user.daily_remaining # Get user daily remaining
+user.plan_expire # Get user plan expiration
+user.response # Get api json response
+```
```

### Comparing `procap-0.0.8/setup.py` & `procap-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 DESCRIPTION = "ProCap is a captcha solving service."
-LONG_DESCRIPTION = "A api wrapper for ProCap."
+LONG_DESCRIPTION = open("README.md", encoding="utf-8").read()
 
 setup(
     name="procap",
     version=VERSION,
     author="ProCap",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
```

