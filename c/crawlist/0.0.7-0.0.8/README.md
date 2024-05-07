# Comparing `tmp/crawlist-0.0.7.tar.gz` & `tmp/crawlist-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlist-0.0.7.tar", last modified: Tue Apr 30 06:32:40 2024, max compression
+gzip compressed data, was "crawlist-0.0.8.tar", last modified: Tue May  7 09:14:33 2024, max compression
```

## Comparing `crawlist-0.0.7.tar` & `crawlist-0.0.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:32:40.811454 crawlist-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-30 06:32:36.000000 crawlist-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 06:32:36.000000 crawlist-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-30 06:32:40.811454 crawlist-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-30 06:32:36.000000 crawlist-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:32:40.807454 crawlist-0.0.7/crawlist/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:32:40.811454 crawlist-0.0.7/crawlist/analyzers/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/analyzers/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/analyzers/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:32:40.811454 crawlist-0.0.7/crawlist/analyzers/pager/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/analyzers/pager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11536 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/analyzers/pager/dynamic_pager.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/analyzers/pager/pager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/analyzers/pager/static_pager.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/analyzers/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/analyzers/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/analyzers/trie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/analyzers/valid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:32:40.811454 crawlist-0.0.7/crawlist/processings/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/processings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/processings/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/processings/script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:32:40.811454 crawlist-0.0.7/crawlist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-30 06:32:40.000000 crawlist-0.0.7/crawlist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-30 06:32:40.000000 crawlist-0.0.7/crawlist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:32:40.000000 crawlist-0.0.7/crawlist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 06:32:40.000000 crawlist-0.0.7/crawlist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 06:32:40.000000 crawlist-0.0.7/crawlist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 06:32:40.811454 crawlist-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-30 06:32:36.000000 crawlist-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:14:33.604374 crawlist-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-07 09:14:29.000000 crawlist-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 09:14:29.000000 crawlist-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-07 09:14:33.604374 crawlist-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-07 09:14:29.000000 crawlist-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:14:33.600374 crawlist-0.0.8/crawlist/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:14:33.600374 crawlist-0.0.8/crawlist/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/analyzers/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/analyzers/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:14:33.604374 crawlist-0.0.8/crawlist/analyzers/pager/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/analyzers/pager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11674 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/analyzers/pager/dynamic_pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/analyzers/pager/pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/analyzers/pager/static_pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/analyzers/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/analyzers/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/analyzers/trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/analyzers/valid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:14:33.604374 crawlist-0.0.8/crawlist/processings/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/processings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/processings/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/processings/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:14:33.604374 crawlist-0.0.8/crawlist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-07 09:14:33.000000 crawlist-0.0.8/crawlist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-07 09:14:33.000000 crawlist-0.0.8/crawlist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:14:33.000000 crawlist-0.0.8/crawlist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-07 09:14:33.000000 crawlist-0.0.8/crawlist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 09:14:33.000000 crawlist-0.0.8/crawlist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 09:14:33.604374 crawlist-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-07 09:14:29.000000 crawlist-0.0.8/setup.py
```

### Comparing `crawlist-0.0.7/LICENSE` & `crawlist-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.7/PKG-INFO` & `crawlist-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlist
-Version: 0.0.7
+Version: 0.0.8
 Summary: A universal solution for web crawling lists
 Home-page: https://github.com/WwwwwyDev/crawlist
 Author: WwyDev
 Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `crawlist-0.0.7/README.md` & `crawlist-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.7/crawlist/analyzers/analyzer.py` & `crawlist-0.0.8/crawlist/analyzers/analyzer.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.7/crawlist/analyzers/driver.py` & `crawlist-0.0.8/crawlist/analyzers/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         self.is_eager = is_eager
 
     def get_driver(self) -> WebDriver:
         option = wd.ChromeOptions()
         add_default_chrome_options(option)
         if not self.is_debug:
             option.add_argument("--headless")
-        if not self.is_eager:
+        if self.is_eager:
             option.page_load_strategy = 'eager'
         option.add_experimental_option('excludeSwitches', ['enable-automation'])
         webdriver = wd.Chrome(service=Service(ChromeDriverManager().install()), options=option)
         webdriver.execute_cdp_cmd("Page.addScriptToEvaluateOnNewDocument", {
             "source": """
                 Object.defineProperty(navigator, 'webdriver', {
                   get: () => false
@@ -49,15 +49,15 @@
         self.webdriver_url = webdriver_url
         self.is_eager = is_eager
 
     def get_driver(self) -> WebDriver:
         option = wd.ChromeOptions()
         add_default_chrome_options(option)
         option.add_argument("--headless")
-        if not self.is_eager:
+        if self.is_eager:
             option.page_load_strategy = 'eager'
         option.set_capability('cloud:options', DesiredCapabilities.CHROME)
         option.add_experimental_option('excludeSwitches', ['enable-automation'])
         webdriver = wd.Remote(command_executor=self.webdriver_url, options=option)
         webdriver.execute_cdp_cmd("Page.addScriptToEvaluateOnNewDocument", {
             "source": """
                 Object.defineProperty(navigator, 'webdriver', {
```

### Comparing `crawlist-0.0.7/crawlist/analyzers/pager/dynamic_pager.py` & `crawlist-0.0.8/crawlist/analyzers/pager/dynamic_pager.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 class DynamicPager(Pager):
     @check
     def __init__(self, webdriver: Driver | WebDriver = None, interval: float = 0.1) -> None:
         """
         :param webdriver: WebDriver object for selenium
         :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
+        self.default_driver_flag = False
         if not webdriver:
+            self.default_driver_flag = True
             self.webdriver = DefaultDriver()()
         else:
             if isinstance(webdriver, WebDriver):
                 self.webdriver = webdriver
             else:
                 self.webdriver = webdriver()
         super().__init__(interval=interval)
@@ -40,18 +42,19 @@
             except Exception:
                 pass
 
     def pre_load(self, webdriver: WebDriver) -> None:
         pass
 
     def __del__(self):
-        try:
-            self.webdriver.quit()
-        except:
-            pass
+        if self.default_driver_flag:
+            try:
+                self.webdriver.quit()
+            except:
+                pass
 
 
 class DynamicRedirectPager(DynamicPager):
     @check
     def __init__(self, uri: str, uri_split: str, webdriver: Driver | WebDriver = None, start: int = 1, offset: int = 1,
                  interval: float = 0.1) -> None:
         """
```

### Comparing `crawlist-0.0.7/crawlist/analyzers/pager/pager.py` & `crawlist-0.0.8/crawlist/analyzers/pager/pager.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.7/crawlist/analyzers/pager/static_pager.py` & `crawlist-0.0.8/crawlist/analyzers/pager/static_pager.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.7/crawlist/analyzers/request.py` & `crawlist-0.0.8/crawlist/analyzers/request.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.7/crawlist/analyzers/selector.py` & `crawlist-0.0.8/crawlist/analyzers/selector.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.7/crawlist/analyzers/trie.py` & `crawlist-0.0.8/crawlist/analyzers/trie.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.7/crawlist/analyzers/valid.py` & `crawlist-0.0.8/crawlist/analyzers/valid.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.7/crawlist/annotation.py` & `crawlist-0.0.8/crawlist/annotation.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.7/crawlist/processings/action.py` & `crawlist-0.0.8/crawlist/processings/action.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.7/crawlist/processings/script.py` & `crawlist-0.0.8/crawlist/processings/script.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.7/crawlist.egg-info/PKG-INFO` & `crawlist-0.0.8/crawlist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlist
-Version: 0.0.7
+Version: 0.0.8
 Summary: A universal solution for web crawling lists
 Home-page: https://github.com/WwwwwyDev/crawlist
 Author: WwyDev
 Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `crawlist-0.0.7/crawlist.egg-info/SOURCES.txt` & `crawlist-0.0.8/crawlist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.7/setup.py` & `crawlist-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'crawlist'
 DESCRIPTION = 'A universal solution for web crawling lists'
 URL = 'https://github.com/WwwwwyDev/crawlist'
 EMAIL = 'wwy20001014@foxmail.com'
 AUTHOR = 'WwyDev'
 REQUIRES_PYTHON = '>=3.10.0'
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 # What packages are required for this module to be executed?
 REQUIRED = [
     'parsel', 'selenium>=4.0.0', 'cssselect', 'lxml', 'requests', 'webdriver-manager'
 ]
 
 # What packages are optional?
 EXTRAS = {
```

