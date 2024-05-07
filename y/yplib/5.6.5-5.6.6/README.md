# Comparing `tmp/yplib-5.6.5.tar.gz` & `tmp/yplib-5.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yplib-5.6.5.tar", last modified: Mon Apr 29 04:00:05 2024, max compression
+gzip compressed data, was "yplib-5.6.6.tar", last modified: Tue May  7 03:27:19 2024, max compression
```

## Comparing `yplib-5.6.5.tar` & `yplib-5.6.6.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 04:00:05.403570 yplib-5.6.5/
--rw-rw-rw-   0        0        0     1091 2023-06-13 07:19:46.000000 yplib-5.6.5/LICENSE
--rw-rw-rw-   0        0        0      355 2024-04-29 04:00:05.403570 yplib-5.6.5/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.6.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 04:00:05.403570 yplib-5.6.5/setup.cfg
--rw-rw-rw-   0        0        0      555 2024-04-29 03:59:45.000000 yplib-5.6.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 04:00:05.403570 yplib-5.6.5/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 02:25:38.000000 yplib-5.6.5/yplib/__init__.py
--rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.6.5/yplib/chart.py
--rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.6.5/yplib/chart_html.py
--rw-rw-rw-   0        0        0    11786 2024-04-29 03:59:19.000000 yplib-5.6.5/yplib/db.py
--rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.6.5/yplib/file.py
--rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.6.5/yplib/http_util.py
--rw-rw-rw-   0        0        0    40804 2024-04-10 06:44:07.000000 yplib-5.6.5/yplib/index.py
--rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.6.5/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.6.5/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.6.5/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.6.5/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2024-04-29 04:00:05.403570 yplib-5.6.5/yplib.egg-info/
--rw-rw-rw-   0        0        0      355 2024-04-29 04:00:05.000000 yplib-5.6.5/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-04-29 04:00:05.000000 yplib-5.6.5/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 04:00:05.000000 yplib-5.6.5/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-29 04:00:05.000000 yplib-5.6.5/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 03:27:19.051218 yplib-5.6.6/
+-rw-rw-rw-   0        0        0     1091 2023-06-13 07:19:46.000000 yplib-5.6.6/LICENSE
+-rw-rw-rw-   0        0        0      355 2024-05-07 03:27:19.051218 yplib-5.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.6.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-07 03:27:19.051218 yplib-5.6.6/setup.cfg
+-rw-rw-rw-   0        0        0      555 2024-05-07 03:26:54.000000 yplib-5.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:27:19.036223 yplib-5.6.6/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 02:25:38.000000 yplib-5.6.6/yplib/__init__.py
+-rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.6.6/yplib/chart.py
+-rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.6.6/yplib/chart_html.py
+-rw-rw-rw-   0        0        0    11786 2024-04-29 03:59:19.000000 yplib-5.6.6/yplib/db.py
+-rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.6.6/yplib/file.py
+-rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.6.6/yplib/http_util.py
+-rw-rw-rw-   0        0        0    41364 2024-05-07 03:26:32.000000 yplib-5.6.6/yplib/index.py
+-rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.6.6/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.6.6/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.6.6/yplib/markdown.py
+-rw-rw-rw-   0        0        0     1683 2024-05-07 03:26:17.000000 yplib-5.6.6/yplib/multi_thread.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.6.6/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:27:19.051218 yplib-5.6.6/yplib.egg-info/
+-rw-rw-rw-   0        0        0      355 2024-05-07 03:27:18.000000 yplib-5.6.6/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-05-07 03:27:18.000000 yplib-5.6.6/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 03:27:18.000000 yplib-5.6.6/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-07 03:27:18.000000 yplib-5.6.6/yplib.egg-info/top_level.txt
```

### Comparing `yplib-5.6.5/LICENSE` & `yplib-5.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-5.6.5/setup.py` & `yplib-5.6.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yplib",
-    version="5.6.5",
+    version="5.6.6",
     author="yangpu",
     author_email="wantwaterfish@gmail.com",
     description="util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `yplib-5.6.5/yplib/__init__.py` & `yplib-5.6.6/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.5/yplib/chart.py` & `yplib-5.6.6/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.5/yplib/chart_html.py` & `yplib-5.6.6/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.5/yplib/db.py` & `yplib-5.6.6/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.5/yplib/file.py` & `yplib-5.6.6/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.5/yplib/http_util.py` & `yplib-5.6.6/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.5/yplib/index.py` & `yplib-5.6.6/yplib/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -926,25 +926,45 @@
 
 # 将文件导出成csv格式的
 # data_list 格式
 # data_list = [['Name', 'Age', 'Gender'],
 #              ['Alice', 25, 'Female'],
 #              ['Bob', 30, 'Male'],
 #              ['Charlie', 35, 'Male']]
+# data_list = [{
+#       "a": 1,
+#       "b": 2,
+#   },{
+#       "a": 1,
+#       "b": 2,
+# }]
 # file_name = 'data'
 def to_csv(data_list, file_name=None, file_path='csv'):
     if file_name is None:
         file_name = 'csv'
     file_name = get_file_name(file_name, '.csv', True)
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
     check_file(file_path)
+    d_list = []
+    if len(data_list) and (isinstance(data_list[0], dict) or isinstance(data_list[0], tuple)):
+        title_list = []
+        for key in data_list[0]:
+            title_list.append(key)
+        d_list.append(title_list)
+        for one_data in data_list:
+            one_list = []
+            for k in title_list:
+                one_list.append(one_data[k])
+            d_list.append(one_list)
+    else:
+        d_list = data_list
     with open(file_path + '/' + file_name, 'w', newline='') as file:
         writer = csv.writer(file)
-        writer.writerows(data_list)
+        writer.writerows(d_list)
 
 
 # 将数据写入到 config 中
 def set_config_data(file_name='config', data=None):
     if data is None:
         data = {}
     set_data_in_user_home(file_name, data)
```

### Comparing `yplib-5.6.5/yplib/mail.py` & `yplib-5.6.6/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.5/yplib/mail_html.py` & `yplib-5.6.6/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.5/yplib/markdown.py` & `yplib-5.6.6/yplib/markdown.py`

 * *Files identical despite different names*

