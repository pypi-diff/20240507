# Comparing `tmp/dzwl-20240409.tar.gz` & `tmp/dzwl-20240507.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dzwl-20240409.tar", last modified: Tue Apr  9 09:48:07 2024, max compression
+gzip compressed data, was "dist\dzwl-20240507.tar", last modified: Tue May  7 09:08:49 2024, max compression
```

## Comparing `dzwl-20240409.tar` & `dzwl-20240507.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 09:48:07.050726 dzwl-20240409/
--rw-rw-rw-   0        0        0      153 2024-04-09 09:48:07.050726 dzwl-20240409/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-09 09:48:07.044725 dzwl-20240409/dzwl/
--rw-rw-rw-   0        0        0        0 2023-12-19 10:07:17.000000 dzwl-20240409/dzwl/__init__.py
--rw-rw-rw-   0        0        0     9475 2024-04-09 09:46:01.000000 dzwl-20240409/dzwl/airtest_util.py
--rw-rw-rw-   0        0        0     8915 2024-04-09 09:46:49.000000 dzwl-20240409/dzwl/fun_util.py
--rw-rw-rw-   0        0        0     5917 2024-04-09 09:46:49.000000 dzwl-20240409/dzwl/interface_util.py
-drwxrwxrwx   0        0        0        0 2024-04-09 09:48:07.048726 dzwl-20240409/dzwl.egg-info/
--rw-rw-rw-   0        0        0      153 2024-04-09 09:48:06.000000 dzwl-20240409/dzwl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2024-04-09 09:48:06.000000 dzwl-20240409/dzwl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 09:48:06.000000 dzwl-20240409/dzwl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-09 09:48:06.000000 dzwl-20240409/dzwl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 09:48:07.050726 dzwl-20240409/setup.cfg
--rw-rw-rw-   0        0        0      872 2024-04-09 09:48:02.000000 dzwl-20240409/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 09:08:49.297526 dzwl-20240507/
+-rw-rw-rw-   0        0        0      153 2024-05-07 09:08:49.296526 dzwl-20240507/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-07 09:08:49.291525 dzwl-20240507/dzwl/
+-rw-rw-rw-   0        0        0        0 2023-12-19 10:07:17.000000 dzwl-20240507/dzwl/__init__.py
+-rw-rw-rw-   0        0        0    10148 2024-04-29 08:41:13.000000 dzwl-20240507/dzwl/airtest_util.py
+-rw-rw-rw-   0        0        0     5316 2024-05-06 09:58:33.000000 dzwl-20240507/dzwl/fun_util.py
+-rw-rw-rw-   0        0        0    13849 2024-04-28 08:07:27.000000 dzwl-20240507/dzwl/interface_util.py
+drwxrwxrwx   0        0        0        0 2024-05-07 09:08:49.295525 dzwl-20240507/dzwl.egg-info/
+-rw-rw-rw-   0        0        0      153 2024-05-07 09:08:49.000000 dzwl-20240507/dzwl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2024-05-07 09:08:49.000000 dzwl-20240507/dzwl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 09:08:49.000000 dzwl-20240507/dzwl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-07 09:08:49.000000 dzwl-20240507/dzwl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 09:08:49.297526 dzwl-20240507/setup.cfg
+-rw-rw-rw-   0        0        0      872 2024-05-07 09:08:23.000000 dzwl-20240507/setup.py
```

### Comparing `dzwl-20240409/dzwl/airtest_util.py` & `dzwl-20240507/dzwl/airtest_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -157,87 +157,104 @@
             else:
                 cls.click(imgPath,type)
                 time.sleep(1)
         print('返回正确验证码' + res)
         return res
 class MobileBasePage:
     @classmethod
-    def locator(self, loc, type):
+    # def locator(self, loc, type):
+    #     if type == 'text':
+    #         self.poco(text=loc).wait_for_appearance(timeout=10)
+    #         fun_util.logView("元素定位-成功(text)：" + str(loc))
+    #         return True
+    #     if type == 'name':
+    #         self.poco(name=loc).wait_for_appearance(timeout=10)
+    #         fun_util.logView("元素定位-成功(name)：" + str(loc))
+    #         return True
+    #     if type == 'image':
+    #         if exists(loc):
+    #             fun_util.logView("元素定位-成功(image)：" + str(loc))
+    #             return True
+    #     else:
+    #         fun_util.logView("不存在元素类型：类型为：" +type+"，属性为："+str(loc))
+    #         pytest.assume(False)
+    #         return False
+    #poco方式定位
+    def locator(cls, loc, type):
         if type == 'text':
-            self.poco(text=loc).wait_for_appearance(timeout=10)
-            fun_util.logView("元素定位-成功(text)：" + str(loc))
-            return True
+            element = cls.poco(text=loc).wait()
+            return element
         if type == 'name':
-            self.poco(name=loc).wait_for_appearance(timeout=10)
-            fun_util.logView("元素定位-成功(name)：" + str(loc))
-            return True
+            element = cls.poco(name=loc).wait()
+            return element
         if type == 'image':
             if exists(loc):
-                fun_util.logView("元素定位-成功(image)：" + str(loc))
-                return True
+                return loc
         else:
-            fun_util.logView("不存在元素类型：类型为：" +type+"，属性为："+str(loc))
+            fun_util.logView('不存在元素类型：类型为：%s，属性为：%s' %(type,str(loc)))
             pytest.assume(False)
-            return False
+    #airtest判断图片是否存在
     @classmethod
-    def click(self, loc, type):
-        if self.locator(loc, type):
-            if type == 'text':
-                self.poco(text=loc).click()
-                fun_util.logView("点击元素(text)：" + str(loc))
-                return True
-
-            if type == 'name':
-                self.poco(name=loc).click()
-                fun_util.logView("点击元素(name)：" + str(loc))
-                return True
-
-            if type == 'image':
-                touch(loc)
-                fun_util.logView("点击元素(image)：" + str(loc))
-                return True
-
+    def assertExists(cls,loc,msg =''):
+        if assert_exists(loc,msg):
+            fun_util.logView('图片定位-成功：%s' % str(loc))
         else:
-            fun_util.logView("点击元素-失败：" + str(loc) + type)
-            pytest.assume(False)
-            return False
+            fun_util.logView('图片定位-失败：%s' % str(loc))
     @classmethod
-    def setValue(self,loc,value,type):
-        if self.locator(loc, type):
-            if type == 'name':
-                input_box = self.poco(name=loc)
-                input_box.setattr("text", value)
-                fun_util.logView("元素赋值-成功(name)：" + str(loc))
-            if type == 'text':
-                input_box = self.poco(text=loc)
-                input_box.setattr("text", value)
-                fun_util.logView("元素赋值-成功(text)：" + str(loc))
-        else:
-            fun_util.logView("元素赋值-失败：" + str(loc) + type)
-            pytest.assume(False)
+    # def click(self, loc, type):
+    #     if self.locator(loc, type):
+    #         if type == 'text':
+    #             self.poco(text=loc).click()
+    #             fun_util.logView("点击元素(text)：" + str(loc))
+    #             return True
+    # 
+    #         if type == 'name':
+    #             self.poco(name=loc).click()
+    #             fun_util.logView("点击元素(name)：" + str(loc))
+    #             return True
+    # 
+    #         if type == 'image':
+    #             touch(loc)
+    #             fun_util.logView("点击元素(image)：" + str(loc))
+    #             return True
+    # 
+    #     else:
+    #         fun_util.logView("点击元素-失败：" + str(loc) + type)
+    #         pytest.assume(False)
+    #         return False
+    def click(cls, loc, type):
+        element = cls.locator(loc, type)
+        if type == 'text' or type == 'name':
+            element.click()
+        if type == 'image':
+            touch(loc)
+        fun_util.logView("点击元素(%s)：%s" %(type,loc))
     @classmethod
-    def inputValueAirtest(self,loc,value,type):
-        if self.click(loc, type):
-            if type == 'name':
-                text(value)
-                fun_util.logView("元素赋值-成功(name)：" + str(loc))
-            if type == 'text':
-                text(value)
-                fun_util.logView("元素赋值-成功(text)：" + str(loc))
-            if type == 'image':
-                text(value)
-                fun_util.logView("元素赋值-成功(image)：" + str(loc))
+    def setAttrValuePoco(cls,loc,value,type):
+        element = cls.locator(loc, type)
+        if type == 'text' or type == 'name':
+            element.setattr('text', value)
+            fun_util.logView(f'元素赋值-成功({type})：{loc}')
         else:
-            fun_util.logView("元素赋值-失败：" + str(loc) + type)
+            fun_util.logView(f'元素赋值-失败({type})：{loc}')
             pytest.assume(False)
+    #使用airtest识别图片的方式，点击图片后直接赋值
     @classmethod
-    def inputValuePoco(self,loc,value,type):
-        if self.click(loc, type):
-            if type == 'name':
-                self.poco(name=loc).set_text(value)
-                fun_util.logView("元素赋值-成功(name)：" + str(loc))
-            if type == 'text':
-                self.poco(text=loc).set_text(value)
-                fun_util.logView("元素赋值-成功(text)：" + str(loc))
-        else:
-            fun_util.logView("元素赋值-失败：" + str(loc) + type)
-            pytest.assume(False)
+    # def inputValueAirtest(self,loc,value,type):
+    #     if self.click(loc, type):
+    #         if type == 'name':
+    #             text(value)
+    #             fun_util.logView("元素赋值-成功(name)：" + str(loc))
+    #         if type == 'text':
+    #             text(value)
+    #             fun_util.logView("元素赋值-成功(text)：" + str(loc))
+    #         if type == 'image':
+    #             text(value)
+    #             print(loc.get_attribute('value'))
+    #             fun_util.logView("元素赋值-成功(image)：" + str(loc))
+    #     else:
+    #         fun_util.logView("元素赋值-失败：" + str(loc) + type)
+    #         pytest.assume(False)
+    def inputValueAirtest(cls, loc, value, type):
+        cls.click(loc,type)
+        text(value)
+        fun_util.logView('元素赋值-成功(%s)：%s' %(type,loc))
```

### Comparing `dzwl-20240409/setup.py` & `dzwl-20240507/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 
 
 setuptools.setup(
     name="dzwl",                                     # 包的分发名称，使用字母、数字、_、-
-    version="20240409",                                        # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
+    version="20240507",                                        # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
     author="zj",                                       # 作者名字
     author_email="author@example.com",                      # 作者邮箱
     description="PyPI Tutorial",                            # 包的简介描述
     long_description='123',                      # 包的详细介绍(一般通过加载README.md)
     packages=setuptools.find_packages(),  
     install_requires=[],  # 依赖的包
     python_requires='>=3'
```

