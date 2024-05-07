# Comparing `tmp/setup_selenium_testing-0.1.4.tar.gz` & `tmp/setup_selenium_testing-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setup_selenium_testing-0.1.4.tar", max compression
+gzip compressed data, was "setup_selenium_testing-0.1.6.tar", max compression
```

## Comparing `setup_selenium_testing-0.1.4.tar` & `setup_selenium_testing-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2024-02-26 22:37:41.634831 setup_selenium_testing-0.1.4/LICENSE
--rw-r--r--   0        0        0     4060 2024-02-26 22:37:41.634831 setup_selenium_testing-0.1.4/README.md
--rw-r--r--   0        0        0     6521 2024-02-26 22:37:41.634831 setup_selenium_testing-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       63 2024-02-26 22:37:41.634831 setup_selenium_testing-0.1.4/setup_selenium/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 22:37:41.634831 setup_selenium_testing-0.1.4/setup_selenium/py.typed
--rw-r--r--   0        0        0    21155 2024-02-26 22:37:41.634831 setup_selenium_testing-0.1.4/setup_selenium/setup_selenium.py
--rw-r--r--   0        0        0     5357 1970-01-01 00:00:00.000000 setup_selenium_testing-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-07 18:02:32.685570 setup_selenium_testing-0.1.6/LICENSE
+-rw-r--r--   0        0        0     4060 2024-05-07 18:02:32.689570 setup_selenium_testing-0.1.6/README.md
+-rw-r--r--   0        0        0     6521 2024-05-07 18:02:32.689570 setup_selenium_testing-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       63 2024-05-07 18:02:32.689570 setup_selenium_testing-0.1.6/setup_selenium/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 18:02:32.689570 setup_selenium_testing-0.1.6/setup_selenium/py.typed
+-rw-r--r--   0        0        0    21576 2024-05-07 18:02:32.689570 setup_selenium_testing-0.1.6/setup_selenium/setup_selenium.py
+-rw-r--r--   0        0        0     5357 1970-01-01 00:00:00.000000 setup_selenium_testing-0.1.6/PKG-INFO
```

### Comparing `setup_selenium_testing-0.1.4/LICENSE` & `setup_selenium_testing-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `setup_selenium_testing-0.1.4/README.md` & `setup_selenium_testing-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `setup_selenium_testing-0.1.4/pyproject.toml` & `setup_selenium_testing-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "setup-selenium-testing"
-version = "0.1.4"
+version = "0.1.6"
 description = "Setup Selenium for automation testing"
 authors = ["Marcel Wilson <trenchrats@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/bandophahita/setup_selenium"
 #documentation = ""
 readme = "README.md"
 classifiers = [
```

### Comparing `setup_selenium_testing-0.1.4/setup_selenium/setup_selenium.py` & `setup_selenium_testing-0.1.6/setup_selenium/setup_selenium.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 import logging
 import os as os
 from enum import Enum
 from typing import TYPE_CHECKING, Optional, Union
 
-from selenium import webdriver
+from selenium import __version__, webdriver
 from selenium.common.exceptions import NoSuchWindowException, WebDriverException
 from selenium.webdriver.chrome.service import Service as ChromeService
 from selenium.webdriver.common.selenium_manager import SeleniumManager
 from selenium.webdriver.edge.service import Service as EdgeService
 from selenium.webdriver.firefox.service import Service as FirefoxService
 from semantic_version import Version  # type: ignore[import-untyped]
 from typing_extensions import TypeAlias
@@ -24,14 +24,19 @@
     from selenium.webdriver.common.options import ArgOptions
 
     T_WebDriver: TypeAlias = Union[Firefox, Chrome, Edge]
     T_DrvOpts: TypeAlias = Union[
         webdriver.FirefoxOptions, webdriver.ChromeOptions, webdriver.EdgeOptions
     ]
 
+NEW_SELENIUM = False
+if Version(__version__) >= Version("4.20.0"):
+    NEW_SELENIUM = True
+
+
 __all__ = ["SetupSelenium"]
 
 
 def create_logger(name: str) -> logging.Logger:
     __logger: type[logging.Logger] = logging.getLoggerClass()
     logr: logging.Logger = logging.getLogger(name)
     logging.setLoggerClass(__logger)
@@ -167,15 +172,19 @@
         install_browser: bool = False,
     ) -> tuple[str, str]:
         """Install the webdriver and browser if needed."""
         browser = Browser[browser.upper()].lower()
         driver_version = driver_version or None
 
         sm = SeleniumManager()
-        args = [f"{sm.get_binary()}", "--browser", browser]
+
+        if NEW_SELENIUM:
+            args = [f"{sm._get_binary()}", "--browser", browser]
+        else:
+            args = [f"{sm.get_binary()}", "--browser", browser]  # type: ignore[attr-defined]
 
         if browser_version:
             args.append("--browser-version")
             args.append(browser_version)
         elif driver_version:
             args.append("--driver-version")
             args.append(driver_version)
@@ -183,15 +192,20 @@
         if install_browser or browser_version:
             args.append("--force-browser-download")
         if browser_path:
             browser_path = os.path.abspath(os.path.expanduser(browser_path))
             args.append("--browser-path")
             args.append(browser_path)
 
-        output = sm.run(args)
+        if NEW_SELENIUM:
+            args.append("--output")
+            args.append("json")
+            output = sm._run(args)
+        else:
+            output = sm.run(args)  # type: ignore[attr-defined]
         driver_path = output["driver_path"]
         browser_path = output["browser_path"]
 
         logger.debug(f"Driver path: {driver_path}")
         logger.debug(f"Browser path: {browser_path}")
 
         return driver_path, browser_path
```

### Comparing `setup_selenium_testing-0.1.4/PKG-INFO` & `setup_selenium_testing-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setup-selenium-testing
-Version: 0.1.4
+Version: 0.1.6
 Summary: Setup Selenium for automation testing
 Home-page: https://github.com/bandophahita/setup_selenium
 License: MIT
 Author: Marcel Wilson
 Author-email: trenchrats@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

