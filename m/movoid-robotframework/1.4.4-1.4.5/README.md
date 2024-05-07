# Comparing `tmp/movoid_robotframework-1.4.4.tar.gz` & `tmp/movoid_robotframework-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_robotframework-1.4.4.tar", last modified: Mon May  6 14:31:37 2024, max compression
+gzip compressed data, was "movoid_robotframework-1.4.5.tar", last modified: Mon May  6 14:37:52 2024, max compression
```

## Comparing `movoid_robotframework-1.4.4.tar` & `movoid_robotframework-1.4.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 14:31:37.816159 movoid_robotframework-1.4.4/
--rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.4/MANIFEST.in
--rw-rw-rw-   0        0        0      290 2024-05-06 14:31:37.814176 movoid_robotframework-1.4.4/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework-1.4.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 14:31:37.797222 movoid_robotframework-1.4.4/RobotFrameworkBasic/
--rw-rw-rw-   0        0        0      451 2024-02-20 17:41:03.000000 movoid_robotframework-1.4.4/RobotFrameworkBasic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 14:31:37.803203 movoid_robotframework-1.4.4/RobotFrameworkBasic/action/
--rw-rw-rw-   0        0        0      253 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.4/RobotFrameworkBasic/action/__init__.py
--rw-rw-rw-   0        0        0     7070 2024-02-20 17:45:15.000000 movoid_robotframework-1.4.4/RobotFrameworkBasic/action/calculate.py
--rw-rw-rw-   0        0        0     8305 2024-04-25 13:54:33.000000 movoid_robotframework-1.4.4/RobotFrameworkBasic/action/config.py
--rw-rw-rw-   0        0        0     6654 2024-05-06 14:28:24.000000 movoid_robotframework-1.4.4/RobotFrameworkBasic/common.py
--rw-rw-rw-   0        0        0    14138 2024-04-20 15:07:13.000000 movoid_robotframework-1.4.4/RobotFrameworkBasic/decorator.py
--rw-rw-rw-   0        0        0      497 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.4/RobotFrameworkBasic/error.py
--rw-rw-rw-   0        0        0      286 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.4/RobotFrameworkBasic/main.py
--rw-rw-rw-   0        0        0      911 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.4/RobotFrameworkBasic/version.py
-drwxrwxrwx   0        0        0        0 2024-05-06 14:31:37.813169 movoid_robotframework-1.4.4/movoid_robotframework.egg-info/
--rw-rw-rw-   0        0        0      290 2024-05-06 14:31:37.000000 movoid_robotframework-1.4.4/movoid_robotframework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2024-05-06 14:31:37.000000 movoid_robotframework-1.4.4/movoid_robotframework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 14:31:37.000000 movoid_robotframework-1.4.4/movoid_robotframework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-05-06 14:31:37.000000 movoid_robotframework-1.4.4/movoid_robotframework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-05-06 14:31:37.000000 movoid_robotframework-1.4.4/movoid_robotframework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 14:31:37.816159 movoid_robotframework-1.4.4/setup.cfg
--rw-rw-rw-   0        0        0      558 2024-05-06 14:29:51.000000 movoid_robotframework-1.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:37:52.966026 movoid_robotframework-1.4.5/
+-rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      290 2024-05-06 14:37:52.965018 movoid_robotframework-1.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework-1.4.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 14:37:52.952641 movoid_robotframework-1.4.5/RobotFrameworkBasic/
+-rw-rw-rw-   0        0        0      451 2024-02-20 17:41:03.000000 movoid_robotframework-1.4.5/RobotFrameworkBasic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:37:52.956633 movoid_robotframework-1.4.5/RobotFrameworkBasic/action/
+-rw-rw-rw-   0        0        0      253 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.5/RobotFrameworkBasic/action/__init__.py
+-rw-rw-rw-   0        0        0     7070 2024-02-20 17:45:15.000000 movoid_robotframework-1.4.5/RobotFrameworkBasic/action/calculate.py
+-rw-rw-rw-   0        0        0     8305 2024-04-25 13:54:33.000000 movoid_robotframework-1.4.5/RobotFrameworkBasic/action/config.py
+-rw-rw-rw-   0        0        0     6810 2024-05-06 14:37:08.000000 movoid_robotframework-1.4.5/RobotFrameworkBasic/common.py
+-rw-rw-rw-   0        0        0    14138 2024-04-20 15:07:13.000000 movoid_robotframework-1.4.5/RobotFrameworkBasic/decorator.py
+-rw-rw-rw-   0        0        0      497 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.5/RobotFrameworkBasic/error.py
+-rw-rw-rw-   0        0        0      286 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.5/RobotFrameworkBasic/main.py
+-rw-rw-rw-   0        0        0      911 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.5/RobotFrameworkBasic/version.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:37:52.963610 movoid_robotframework-1.4.5/movoid_robotframework.egg-info/
+-rw-rw-rw-   0        0        0      290 2024-05-06 14:37:52.000000 movoid_robotframework-1.4.5/movoid_robotframework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2024-05-06 14:37:52.000000 movoid_robotframework-1.4.5/movoid_robotframework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 14:37:52.000000 movoid_robotframework-1.4.5/movoid_robotframework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-06 14:37:52.000000 movoid_robotframework-1.4.5/movoid_robotframework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-05-06 14:37:52.000000 movoid_robotframework-1.4.5/movoid_robotframework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 14:37:52.967013 movoid_robotframework-1.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      558 2024-05-06 14:37:08.000000 movoid_robotframework-1.4.5/setup.py
```

### Comparing `movoid_robotframework-1.4.4/RobotFrameworkBasic/action/calculate.py` & `movoid_robotframework-1.4.5/RobotFrameworkBasic/action/calculate.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.4/RobotFrameworkBasic/action/config.py` & `movoid_robotframework-1.4.5/RobotFrameworkBasic/action/config.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.4/RobotFrameworkBasic/common.py` & `movoid_robotframework-1.4.5/RobotFrameworkBasic/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,25 +133,28 @@
     @robot_log_keyword
     def log_show_image(self, image_path: str):
         with open(image_path, mode='rb') as f:
             img_str = base64.b64encode(f.read()).decode()
             self.print(f'<img src="data:image/png;base64,{img_str}">', html=True)
 
     @robot_log_keyword
-    def robot_check_param(self, param_str: str, param_style: Union[str, type], default=None, error=False):
+    def robot_check_param(self, param_str: object, param_style: Union[str, type], default=None, error=False):
         if type(param_style) is str:
             param_style_str = param_style.lower()
         elif type(param_style) is type:
             param_style_str = param_style.__name__
         else:
             error_text = f'what is <{param_style}>({type(param_style).__name__}) which is not str or type?'
             if error:
                 raise TypeError(error_text)
             else:
                 return default
+        if type(param_str).__name__ == param_style_str:
+            self.print('style is correct, we do not change it.')
+            return param_str
         self.print(f'try to change <{param_str}> to {param_style}')
         try:
             if param_style_str in ('str',):
                 re_value = str(param_str)
             elif param_style_str in ('int',):
                 re_value = int(param_str)
             elif param_style_str in ('float',):
```

### Comparing `movoid_robotframework-1.4.4/RobotFrameworkBasic/decorator.py` & `movoid_robotframework-1.4.5/RobotFrameworkBasic/decorator.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.4/RobotFrameworkBasic/version.py` & `movoid_robotframework-1.4.5/RobotFrameworkBasic/version.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.4/movoid_robotframework.egg-info/SOURCES.txt` & `movoid_robotframework-1.4.5/movoid_robotframework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.4/setup.py` & `movoid_robotframework-1.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='movoid_robotframework',
-    version='1.4.4',
+    version='1.4.5',
     packages=find_packages(),
     url='',
     license='',
     author='movoid',
     author_email='bobrobotsun@163.com',
     description='',
     long_description=long_description,
```

