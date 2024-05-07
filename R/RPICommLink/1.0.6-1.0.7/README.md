# Comparing `tmp/RPICommLink-1.0.6.tar.gz` & `tmp/RPICommLink-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RPICommLink-1.0.6.tar", last modified: Sat May  4 10:44:11 2024, max compression
+gzip compressed data, was "dist\RPICommLink-1.0.7.tar", last modified: Tue May  7 10:00:27 2024, max compression
```

## Comparing `RPICommLink-1.0.6.tar` & `RPICommLink-1.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 10:44:11.971793 RPICommLink-1.0.6/
--rw-rw-rw-   0        0        0     1317 2024-05-04 10:44:11.970796 RPICommLink-1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-04 10:44:11.948536 RPICommLink-1.0.6/RPICommLink/
--rw-rw-rw-   0        0        0    15711 2024-05-04 10:41:48.000000 RPICommLink-1.0.6/RPICommLink/rpicommlink.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:44:11.968801 RPICommLink-1.0.6/RPICommLink.egg-info/
--rw-rw-rw-   0        0        0     1317 2024-05-04 10:44:11.000000 RPICommLink-1.0.6/RPICommLink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      175 2024-05-04 10:44:11.000000 RPICommLink-1.0.6/RPICommLink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 10:44:11.000000 RPICommLink-1.0.6/RPICommLink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-04 10:44:11.000000 RPICommLink-1.0.6/RPICommLink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 10:44:11.974810 RPICommLink-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1700 2024-05-04 10:44:01.000000 RPICommLink-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 10:00:27.000000 RPICommLink-1.0.7/
+-rw-rw-rw-   0        0        0     1749 2024-05-07 10:00:27.000000 RPICommLink-1.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-07 10:00:27.000000 RPICommLink-1.0.7/RPICommLink/
+-rw-rw-rw-   0        0        0    15711 2024-05-07 09:48:52.000000 RPICommLink-1.0.7/RPICommLink/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 10:00:27.000000 RPICommLink-1.0.7/RPICommLink.egg-info/
+-rw-rw-rw-   0        0        0     1749 2024-05-07 10:00:27.000000 RPICommLink-1.0.7/RPICommLink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-05-07 10:00:27.000000 RPICommLink-1.0.7/RPICommLink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 10:00:27.000000 RPICommLink-1.0.7/RPICommLink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-07 10:00:27.000000 RPICommLink-1.0.7/RPICommLink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 10:00:27.000000 RPICommLink-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1753 2024-05-07 09:52:36.000000 RPICommLink-1.0.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `RPICommLink-1.0.6/RPICommLink/rpicommlink.py` & `RPICommLink-1.0.7/RPICommLink/__init__.py`

 * *Files identical despite different names*

### Comparing `RPICommLink-1.0.6/setup.py` & `RPICommLink-1.0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup
 
 setup(
     name='RPICommLink',
-    version='1.0.6',
+    version='1.0.7',
     author='adixu',
     author_email='adixu7@gmail.com',
     description='A library for communication on Raspberry Pi',
     long_description="RPICommLink 是一个用于在不同设备之间建立通信连接的 Python 类。提供了一系列方法使设备能够通过 TCP/IP 协议进行数据交换。"
                      "灵活的通信设置可以轻松地在设备之间建立通信连接，无论是在局域网内部还是通过互联网。"
                      "具备完善的错误处理机制及时发现并处理连接中断、超时等异常情况，保证通信的稳定性和可靠性。"
                      "使用简单易用的接口可以方便地发送和接收数据，无需过多关注底层网络细节，让设备之间的通信变得更加简单和高效。"
                      "通过 RPICommLink 类，可以实现设备之间的数据交换，为项目提供强大的通信支持。"
                      "\n\n\n\n\n\n历代版本更新："
                      "\n\n\n\n\n\n1.0.2 -优化了函数的命名，发送模块不再进行死循环。"
                      "\n\n\n\n\n\n1.0.3 -修复了潜在bug，优化了获取IP的方式，现在可以不命名而使用默认设备名称了。添加了中文介绍。"
                      "\n\n\n\n\n\n1.0.4 -重新了上传中文介绍。"
                      "\n\n\n\n\n\n1.0.5 -修复了无法在无互联网下获取IP的报错，修复了无法同时连接两个服务器的bug。"
-                     "\n\n\n\n\n\n1.0.6 -修复了潜在bug",
+                     "\n\n\n\n\n\n1.0.6 -修复了潜在bug"
+                     "\n\n\n\n\n\n1.0.7 -轻量化",
     packages=['RPICommLink'],
     install_requires=[],
 )
```

