# Comparing `tmp/neco_m3u8-0.0.2.tar.gz` & `tmp/neco_m3u8-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neco_m3u8-0.0.2.tar", last modified: Mon May  6 12:24:39 2024, max compression
+gzip compressed data, was "neco_m3u8-0.0.3.tar", last modified: Mon May  6 13:35:03 2024, max compression
```

## Comparing `neco_m3u8-0.0.2.tar` & `neco_m3u8-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 12:24:39.724205 neco_m3u8-0.0.2/
--rw-rw-rw-   0        0        0      593 2024-05-06 12:24:39.723209 neco_m3u8-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       62 2024-05-06 12:04:48.000000 neco_m3u8-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 12:24:39.723209 neco_m3u8-0.0.2/neco_m3u8.egg-info/
--rw-rw-rw-   0        0        0      593 2024-05-06 12:24:39.000000 neco_m3u8-0.0.2/neco_m3u8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2024-05-06 12:24:39.000000 neco_m3u8-0.0.2/neco_m3u8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 12:24:39.000000 neco_m3u8-0.0.2/neco_m3u8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-05-06 12:24:39.000000 neco_m3u8-0.0.2/neco_m3u8.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-06 12:24:39.000000 neco_m3u8-0.0.2/neco_m3u8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 12:24:39.724205 neco_m3u8-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      939 2024-05-06 12:24:39.000000 neco_m3u8-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 12:24:39.722211 neco_m3u8-0.0.2/src/
--rw-rw-rw-   0        0        0     1332 2024-05-06 10:12:25.000000 neco_m3u8-0.0.2/src/decrypto.py
--rw-rw-rw-   0        0        0     1456 2024-05-06 11:49:58.000000 neco_m3u8-0.0.2/src/ffmpeg.py
--rw-rw-rw-   0        0        0     7870 2024-05-06 12:24:29.000000 neco_m3u8-0.0.2/src/neco_m3u8.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:35:03.000620 neco_m3u8-0.0.3/
+-rw-rw-rw-   0        0        0      593 2024-05-06 13:35:02.999623 neco_m3u8-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       62 2024-05-06 12:04:48.000000 neco_m3u8-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 13:35:02.998625 neco_m3u8-0.0.3/neco_m3u8.egg-info/
+-rw-rw-rw-   0        0        0      593 2024-05-06 13:35:02.000000 neco_m3u8-0.0.3/neco_m3u8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2024-05-06 13:35:02.000000 neco_m3u8-0.0.3/neco_m3u8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 13:35:02.000000 neco_m3u8-0.0.3/neco_m3u8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-06 13:35:02.000000 neco_m3u8-0.0.3/neco_m3u8.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-06 13:35:02.000000 neco_m3u8-0.0.3/neco_m3u8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 13:35:03.000620 neco_m3u8-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      940 2024-05-06 13:35:02.000000 neco_m3u8-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:35:02.997628 neco_m3u8-0.0.3/src/
+-rw-rw-rw-   0        0        0     1332 2024-05-06 10:12:25.000000 neco_m3u8-0.0.3/src/decrypto.py
+-rw-rw-rw-   0        0        0     1903 2024-05-06 13:34:58.000000 neco_m3u8-0.0.3/src/ffmpeg.py
+-rw-rw-rw-   0        0        0     7870 2024-05-06 12:24:29.000000 neco_m3u8-0.0.3/src/neco_m3u8.py
```

### Comparing `neco_m3u8-0.0.2/PKG-INFO` & `neco_m3u8-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neco_m3u8
-Version: 0.0.2
+Version: 0.0.3
 Summary: m3u8解析与下载库,自动获取key解密,需要ffmpeg用于合并ts流
 Home-page: 
 Author: neco_arc
 Author-email: 3306601284@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neco_m3u8-0.0.2/neco_m3u8.egg-info/PKG-INFO` & `neco_m3u8-0.0.3/neco_m3u8.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neco_m3u8
-Version: 0.0.2
+Version: 0.0.3
 Summary: m3u8解析与下载库,自动获取key解密,需要ffmpeg用于合并ts流
 Home-page: 
 Author: neco_arc
 Author-email: 3306601284@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neco_m3u8-0.0.2/setup.py` & `neco_m3u8-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 name = 'neco_m3u8'
 author = 'neco_arc'
 description = 'm3u8解析与下载库,自动获取key解密,需要ffmpeg用于合并ts流'
 email = '3306601284@qq.com'
 
 with open('README.md', mode='r', encoding='utf-8') as f:
     long_description = f.read()
@@ -20,15 +20,15 @@
     package_dir={'neco_m3u8': 'src'},
     packages=['neco_m3u8'],
     python_requires='>=3.9',
     install_requires=[
         'requests',
         'pycryptodome',
         'DownloadKit',
-        'm3u8'
+        'm3u8',
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
 )
```

### Comparing `neco_m3u8-0.0.2/src/decrypto.py` & `neco_m3u8-0.0.3/src/decrypto.py`

 * *Files identical despite different names*

### Comparing `neco_m3u8-0.0.2/src/ffmpeg.py` & `neco_m3u8-0.0.3/src/ffmpeg.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import shutil
 import subprocess
 import os
 import random
 import glob
 
 
 def merge_ts_files(input_folder, output_file):
@@ -23,14 +24,29 @@
         # 调用ffmpeg命令
     subprocess.run(command, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL, check=True)
 
     # 清理创建的'list.txt'文件（可选）
     os.remove(list_txt_name)
 
     print(f"{output_file}合并完成!")
+    del_dir(input_folder, mode=2)
+
+
+def del_dir(dir_name: str, mode=1):
+    """
+    :param dir_name: 文件夹名字
+    :param mode: 1为删除文件夹里面内容 2为连着文件夹一起删除
+    :return:
+    """
+    if mode == 1:
+        for file in os.listdir(dir_name):
+            file_path = os.path.join(dir_name, file)
+            os.remove(file_path)
+    elif mode == 2:
+        shutil.rmtree(dir_name)
 
 
 if __name__ == '__main__':
     save_dir = 'E:/番\精灵宝可梦超世代'
     file_name = '第01集'
     ts_file_dir = os.path.join(save_dir, file_name)
     merge_ts_files(ts_file_dir, os.path.join(save_dir, f'{file_name}.mp4'))
```

### Comparing `neco_m3u8-0.0.2/src/neco_m3u8.py` & `neco_m3u8-0.0.3/src/neco_m3u8.py`

 * *Files identical despite different names*

