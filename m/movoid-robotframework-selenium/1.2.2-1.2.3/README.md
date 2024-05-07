# Comparing `tmp/movoid_robotframework_selenium-1.2.2.tar.gz` & `tmp/movoid_robotframework_selenium-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_robotframework_selenium-1.2.2.tar", last modified: Sat Apr 20 15:53:47 2024, max compression
+gzip compressed data, was "movoid_robotframework_selenium-1.2.3.tar", last modified: Tue May  7 13:35:21 2024, max compression
```

## Comparing `movoid_robotframework_selenium-1.2.2.tar` & `movoid_robotframework_selenium-1.2.3.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 15:53:47.396735 movoid_robotframework_selenium-1.2.2/
--rw-rw-rw-   0        0        0      439 2024-04-20 15:53:47.395733 movoid_robotframework_selenium-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework_selenium-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 15:53:47.380066 movoid_robotframework_selenium-1.2.2/RobotFrameworkSelenium/
--rw-rw-rw-   0        0        0      311 2024-02-20 17:47:42.000000 movoid_robotframework_selenium-1.2.2/RobotFrameworkSelenium/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:53:47.382058 movoid_robotframework_selenium-1.2.2/RobotFrameworkSelenium/action/
--rw-rw-rw-   0        0        0      218 2024-02-20 05:59:20.000000 movoid_robotframework_selenium-1.2.2/RobotFrameworkSelenium/action/__init__.py
--rw-rw-rw-   0        0        0    12876 2024-04-20 10:51:34.000000 movoid_robotframework_selenium-1.2.2/RobotFrameworkSelenium/action/action.py
--rw-rw-rw-   0        0        0     6393 2024-04-20 15:50:56.000000 movoid_robotframework_selenium-1.2.2/RobotFrameworkSelenium/action/action.pyi
--rw-rw-rw-   0        0        0     7367 2024-03-24 16:01:08.000000 movoid_robotframework_selenium-1.2.2/RobotFrameworkSelenium/common.py
--rw-rw-rw-   0        0        0     2530 2024-04-20 15:20:19.000000 movoid_robotframework_selenium-1.2.2/RobotFrameworkSelenium/common.pyi
--rw-rw-rw-   0        0        0      268 2024-02-20 05:59:20.000000 movoid_robotframework_selenium-1.2.2/RobotFrameworkSelenium/main.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:53:47.390259 movoid_robotframework_selenium-1.2.2/movoid_robotframework_selenium.egg-info/
--rw-rw-rw-   0        0        0      439 2024-04-20 15:53:47.000000 movoid_robotframework_selenium-1.2.2/movoid_robotframework_selenium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      560 2024-04-20 15:53:47.000000 movoid_robotframework_selenium-1.2.2/movoid_robotframework_selenium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 15:53:47.000000 movoid_robotframework_selenium-1.2.2/movoid_robotframework_selenium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2024-04-20 15:53:47.000000 movoid_robotframework_selenium-1.2.2/movoid_robotframework_selenium.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-04-20 15:53:47.000000 movoid_robotframework_selenium-1.2.2/movoid_robotframework_selenium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 15:53:47.396735 movoid_robotframework_selenium-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      748 2024-04-20 15:52:51.000000 movoid_robotframework_selenium-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:53:47.388265 movoid_robotframework_selenium-1.2.2/test/
--rw-rw-rw-   0        0        0      400 2024-04-20 15:13:11.000000 movoid_robotframework_selenium-1.2.2/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:35:21.819282 movoid_robotframework_selenium-1.2.3/
+-rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_robotframework_selenium-1.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      439 2024-05-07 13:35:21.818273 movoid_robotframework_selenium-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework_selenium-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 13:35:21.796605 movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/
+-rw-rw-rw-   0        0        0      311 2024-02-20 17:47:42.000000 movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:35:21.799664 movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/action/
+-rw-rw-rw-   0        0        0      218 2024-02-20 05:59:20.000000 movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/action/__init__.py
+-rw-rw-rw-   0        0        0    12876 2024-04-20 10:51:34.000000 movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/action/action.py
+-rw-rw-rw-   0        0        0     6393 2024-04-20 15:50:56.000000 movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/action/action.pyi
+-rw-rw-rw-   0        0        0     9778 2024-05-07 13:18:52.000000 movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/common.py
+-rw-rw-rw-   0        0        0     2596 2024-05-06 09:57:55.000000 movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/common.pyi
+-rw-rw-rw-   0        0        0      268 2024-02-20 05:59:20.000000 movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/main.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:35:21.817267 movoid_robotframework_selenium-1.2.3/movoid_robotframework_selenium.egg-info/
+-rw-rw-rw-   0        0        0      439 2024-05-07 13:35:21.000000 movoid_robotframework_selenium-1.2.3/movoid_robotframework_selenium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      555 2024-05-07 13:35:21.000000 movoid_robotframework_selenium-1.2.3/movoid_robotframework_selenium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 13:35:21.000000 movoid_robotframework_selenium-1.2.3/movoid_robotframework_selenium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2024-05-07 13:35:21.000000 movoid_robotframework_selenium-1.2.3/movoid_robotframework_selenium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-05-07 13:35:21.000000 movoid_robotframework_selenium-1.2.3/movoid_robotframework_selenium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 13:35:21.819282 movoid_robotframework_selenium-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      748 2024-05-07 13:33:07.000000 movoid_robotframework_selenium-1.2.3/setup.py
```

### Comparing `movoid_robotframework_selenium-1.2.2/RobotFrameworkSelenium/action/action.py` & `movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/action/action.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework_selenium-1.2.2/RobotFrameworkSelenium/action/action.pyi` & `movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/action/action.pyi`

 * *Files identical despite different names*

### Comparing `movoid_robotframework_selenium-1.2.2/RobotFrameworkSelenium/common.py` & `movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/common.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 # -*- coding: utf-8 -*-
 """
 # File          : common
 # Author        : Sun YiFan-Movoid
 # Time          : 2024/2/16 18:47
 # Description   : 
 """
+import base64
 import math
 import os
 from typing import List, Tuple, Union
 
 import cv2
+import numpy as np
 import robot.libraries.BuiltIn
 import selenium.webdriver.chrome.webdriver
-from Selenium2Library import Selenium2Library
 from RobotFrameworkBasic import RobotBasic, robot_log_keyword, RfError
+from Selenium2Library import Selenium2Library
 from selenium.webdriver import ActionChains
 from selenium.webdriver.remote.webelement import WebElement
 
 
 class BasicCommon(RobotBasic):
     def __init__(self):
         super().__init__()
@@ -29,29 +31,38 @@
         self.screenshot_root: str = getattr(self, 'screenshot_root', None)
         self.outer_coordinate: Tuple[float] = getattr(self, 'outer_coordinate', None)
         self.inner_coordinate: Tuple[float] = getattr(self, 'inner_coordinate', None)
         self.window_x: float = getattr(self, 'window_x', None)
         self.window_y: float = getattr(self, 'window_y', None)
 
     @robot_log_keyword
-    def selenium_init(self):
+    def selenium_init(self, screenshot_log: bool = False):
+        screenshot_log = self.robot_check_param(screenshot_log, bool, False)
         self.selenium_lib = self.built.get_library_instance('Selenium2Library')
         self.driver = self.selenium_lib.driver
         self.action_chains = ActionChains(self.driver)
-        self.screenshot_root = self.selenium_lib.screenshot_root_directory
+        self.screenshot_root = None if screenshot_log else ('.' if self.selenium_lib.screenshot_root_directory is None else self.selenium_lib.screenshot_root_directory)
 
     @robot_log_keyword
     def selenium_analyse_locator(self, locator: str) -> Tuple[str, str]:
         if locator.startswith('/'):
             return 'xpath', locator
         elif '=' in locator:
             by, path = locator.split('=', 1)
             by = by.lower().replace('_', ' ').strip(' ')
             if by in ["id", "xpath", "link text", "partial link text", "name", "tag name", "class name", "css selector"]:
                 return by, path
+            elif by in ('css',):
+                return "css selector", locator
+            elif by in ('link',):
+                return "partial link text", locator
+            elif by in ('tag',):
+                return "tag name", locator
+            elif by in ('class',):
+                return "class name", locator
             else:
                 return "css selector", locator
         else:
             return "css selector", locator
 
     @robot_log_keyword
     def selenium_find_elements_by_locator(self, locator) -> List[WebElement]:
@@ -83,57 +94,90 @@
 
     @robot_log_keyword
     def exchange_list3_to_color_function(self, formula_list):
         return lambda r, g, b: eval('r' + formula_list[0]) and eval('g' + formula_list[1]) and eval('b' + formula_list[2])
 
     @robot_log_keyword
     def selenium_get_full_screenshot_path(self, screenshot_name):
-        suite = self.get_robot_variable('SUITE NAME').replace(' ', '_')
-        case_ori = self.get_robot_variable('TEST NAME')
-        folder_name = suite if case_ori is None else f"{suite}-{case_ori.replace(' ', '_')}"
+        folder_name = self.get_suite_case_str().replace(' ', '_')
         full_folder_path = os.path.join(self.screenshot_root, folder_name)
         if not os.path.exists(full_folder_path):
             os.mkdir(full_folder_path)
             self.print(f'create image folder:{folder_name}')
         return os.path.join(full_folder_path, screenshot_name)
 
     @robot_log_keyword
     def selenium_cut_screenshot(self, screenshot_locator, image_name='element-cut-image.png'):
-        tar_name, tar_path = self.selenium_take_screenshot(None, image_name)
-        full_image = self.selenium_analyse_image(tar_name)
+        if self.screenshot_root is None:
+            cut_image = self.selenium_log_screenshot(screenshot_locator)
+        else:
+            tar_name, tar_path = self.selenium_take_screenshot(None, image_name)
+            full_image = self.selenium_analyse_image(tar_name)
+            if screenshot_locator is None:
+                cut_image = full_image
+            else:
+                tar_element = self.selenium_analyse_element(screenshot_locator)
+                element_position = self.selenium_execute_js_script('return arguments[0].getBoundingClientRect();', tar_element)
+                self.print(element_position)
+                cut_rect = [math.floor(element_position['left']), math.floor(element_position['top']), math.floor(element_position['right']), math.floor(element_position['bottom'])]
+                cut_image = full_image[cut_rect[1]:cut_rect[3], cut_rect[0]:cut_rect[2]]
+                self.print(cut_image.shape)
+                tar_path_split = os.path.splitext(tar_path)
+                cv2.imwrite(tar_path_split[0] + '(cut)' + tar_path_split[1], cut_image)
+        self.print(f'the shape of cut screenshot is {cut_image.shape}')
+        return cut_image
+
+    @robot_log_keyword
+    def selenium_take_screenshot(self, screenshot_locator=None, image_name='python-screenshot.png', rename=True):
+        if self.screenshot_root is None:
+            self.selenium_log_screenshot(screenshot_locator)
+            return None, None
+        else:
+            tar_name = image_name
+            ind = 1
+            tar_path = self.selenium_get_full_screenshot_path(tar_name)
+            while rename and os.path.isfile(tar_path):
+                ind += 1
+                name, post = os.path.splitext(image_name)
+                tar_name = f'{name}-{ind}{post}'
+                tar_path = self.selenium_get_full_screenshot_path(tar_name)
+            if screenshot_locator is None:
+                self.selenium_lib.capture_page_screenshot(tar_path)
+                self.print(f'take a full window screenshot:{tar_name}')
+            else:
+                self.selenium_lib.capture_element_screenshot(screenshot_locator, tar_path)
+                self.print(f'take a DOM({screenshot_locator}) screenshot:{tar_name}')
+            return tar_name, tar_path
+
+    @robot_log_keyword
+    def selenium_log_screenshot(self, screenshot_locator=None):
         if screenshot_locator is None:
-            return full_image
+            img = self.driver.get_screenshot_as_base64()
+            cv_value = np.frombuffer(base64.b64decode(img), np.uint8)
         else:
+            img_data = self.driver.get_screenshot_as_png()
+            img_array = np.fromstring(img_data, np.uint8)
+            full_image = cv2.imdecode(img_array, cv2.COLOR_RGB2BGR)
             tar_element = self.selenium_analyse_element(screenshot_locator)
             element_position = self.selenium_execute_js_script('return arguments[0].getBoundingClientRect();', tar_element)
-            self.print(element_position)
+            self.print("element_position:", element_position)
             cut_rect = [math.floor(element_position['left']), math.floor(element_position['top']), math.floor(element_position['right']), math.floor(element_position['bottom'])]
             cut_image = full_image[cut_rect[1]:cut_rect[3], cut_rect[0]:cut_rect[2]]
-            self.print(cut_image.shape)
-            tar_path_split = os.path.splitext(tar_path)
-            cv2.imwrite(tar_path_split[0] + '(cut)' + tar_path_split[1], cut_image)
-            return cut_image
+            cv_value = cut_image
+            self.print("cut image shape:", cut_image.shape)
+            image = cv2.imencode('.png', cut_image)[1]
+            img = str(base64.b64encode(image))[2:-1]
+        self.print(f'<img src="data:image/png;base64,{img}">', html=True)
+        return cv_value
 
     @robot_log_keyword
-    def selenium_take_screenshot(self, screenshot_locator=None, image_name='python-screenshot.png', rename=True):
-        tar_name = image_name
-        ind = 1
-        tar_path = self.selenium_get_full_screenshot_path(tar_name)
-        while rename and os.path.isfile(tar_path):
-            ind += 1
-            name, post = os.path.splitext(image_name)
-            tar_name = f'{name}-{ind}{post}'
-            tar_path = self.selenium_get_full_screenshot_path(tar_name)
-        if screenshot_locator is None:
-            self.selenium_lib.capture_page_screenshot(tar_path)
-            self.print(f'take a full window screenshot:{tar_name}')
-        else:
-            self.selenium_lib.capture_element_screenshot(screenshot_locator, tar_path)
-            self.print(f'take a DOM({screenshot_locator}) screenshot:{tar_name}')
-        return tar_name, tar_path
+    def selenium_log_screenshot_path(self, screenshot_name):
+        full_path = self.selenium_get_full_screenshot_path(screenshot_name)
+        self.print(full_path)
+        self.log_show_image(full_path)
 
     @robot_log_keyword
     def selenium_analyse_image(self, image):
         if isinstance(image, str):
             image_full_path = image if os.path.isfile(image) else self.selenium_get_full_screenshot_path(image)
             self.print(f'try to read image:{image_full_path}')
             return cv2.imread(image_full_path)
```

### Comparing `movoid_robotframework_selenium-1.2.2/RobotFrameworkSelenium/common.pyi` & `movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/common.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -33,12 +33,13 @@
 	def selenium_find_element_by_locator(self, locator) -> selenium.webdriver.remote.webelement.WebElement:	...
 	def selenium_execute_js_script(self, js_code: str, args):	...
 	def analyse_color_function(self, color_function):	...
 	def exchange_list3_to_color_function(self, formula_list):	...
 	def selenium_get_full_screenshot_path(self, screenshot_name):	...
 	def selenium_cut_screenshot(self, screenshot_locator, image_name = 'element-cut-image.png'):	...
 	def selenium_take_screenshot(self, screenshot_locator = None, image_name = 'python-screenshot.png', rename = True):	...
+	def selenium_log_screenshot(self, screenshot_locator=None):	...
 	def selenium_analyse_image(self, image):	...
 	def selenium_analyse_element(self, locator: typing.Union[selenium.webdriver.remote.webelement.WebElement, str]) -> selenium.webdriver.remote.webelement.WebElement:	...
 	def selenium_analyse_elements(self, locator: typing.Union[typing.List[selenium.webdriver.remote.webelement.WebElement], str]) -> typing.List[selenium.webdriver.remote.webelement.WebElement]:	...
 	...
```

### Comparing `movoid_robotframework_selenium-1.2.2/movoid_robotframework_selenium.egg-info/SOURCES.txt` & `movoid_robotframework_selenium-1.2.3/movoid_robotframework_selenium.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+MANIFEST.in
 README.md
 setup.py
 RobotFrameworkSelenium/__init__.py
 RobotFrameworkSelenium/common.py
 RobotFrameworkSelenium/common.pyi
 RobotFrameworkSelenium/main.py
 RobotFrameworkSelenium/action/__init__.py
 RobotFrameworkSelenium/action/action.py
 RobotFrameworkSelenium/action/action.pyi
 movoid_robotframework_selenium.egg-info/PKG-INFO
 movoid_robotframework_selenium.egg-info/SOURCES.txt
 movoid_robotframework_selenium.egg-info/dependency_links.txt
 movoid_robotframework_selenium.egg-info/requires.txt
-movoid_robotframework_selenium.egg-info/top_level.txt
-test/__init__.py
+movoid_robotframework_selenium.egg-info/top_level.txt
```

### Comparing `movoid_robotframework_selenium-1.2.2/setup.py` & `movoid_robotframework_selenium-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='movoid_robotframework_selenium',
-    version='1.2.2',
+    version='1.2.3',
     packages=find_packages(),
     url='',
     license='',
     author='movoid',
     author_email='bobrobotsun@163.com',
     description='',
     long_description=long_description,
```

