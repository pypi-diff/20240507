# Comparing `tmp/pmonitor-1.1.0.tar.gz` & `tmp/pmonitor-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmonitor-1.1.0.tar", last modified: Tue May  7 07:21:27 2024, max compression
+gzip compressed data, was "pmonitor-1.1.1.tar", last modified: Tue May  7 07:41:52 2024, max compression
```

## Comparing `pmonitor-1.1.0.tar` & `pmonitor-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 cfr        (501) staff       (20)        0 2024-05-07 07:21:27.257403 pmonitor-1.1.0/
--rw-r--r--   0 cfr        (501) staff       (20)      225 2024-05-07 07:21:27.256830 pmonitor-1.1.0/PKG-INFO
--rw-r--r--   0 cfr        (501) staff       (20)       26 2024-05-06 02:50:55.000000 pmonitor-1.1.0/README.md
-drwxr-xr-x   0 cfr        (501) staff       (20)        0 2024-05-07 07:21:27.252827 pmonitor-1.1.0/monitor/
--rw-r--r--   0 cfr        (501) staff       (20)     8523 2024-05-06 09:32:42.000000 pmonitor-1.1.0/monitor/WinPidUtil.py
--rw-r--r--   0 cfr        (501) staff       (20)        0 2024-05-06 02:50:55.000000 pmonitor-1.1.0/monitor/__init__.py
--rw-r--r--   0 cfr        (501) staff       (20)     3620 2024-05-06 08:11:43.000000 pmonitor-1.1.0/monitor/get_process_name.py
--rw-r--r--   0 cfr        (501) staff       (20)     4651 2024-05-06 02:50:55.000000 pmonitor-1.1.0/monitor/monitor_mac.py
--rw-r--r--   0 cfr        (501) staff       (20)    10208 2024-05-07 07:21:02.000000 pmonitor-1.1.0/monitor/monitor_pids.py
--rw-r--r--   0 cfr        (501) staff       (20)     6161 2024-05-06 02:50:55.000000 pmonitor-1.1.0/monitor/monitor_win.py
--rw-r--r--   0 cfr        (501) staff       (20)     2106 2024-05-07 07:21:02.000000 pmonitor-1.1.0/monitor/run_monitor.py
--rw-r--r--   0 cfr        (501) staff       (20)     3208 2024-05-06 02:50:55.000000 pmonitor-1.1.0/monitor/sys_info.py
-drwxr-xr-x   0 cfr        (501) staff       (20)        0 2024-05-07 07:21:27.255980 pmonitor-1.1.0/pmonitor.egg-info/
--rw-r--r--   0 cfr        (501) staff       (20)      225 2024-05-07 07:21:27.000000 pmonitor-1.1.0/pmonitor.egg-info/PKG-INFO
--rw-r--r--   0 cfr        (501) staff       (20)      364 2024-05-07 07:21:27.000000 pmonitor-1.1.0/pmonitor.egg-info/SOURCES.txt
--rw-r--r--   0 cfr        (501) staff       (20)        1 2024-05-07 07:21:27.000000 pmonitor-1.1.0/pmonitor.egg-info/dependency_links.txt
--rw-r--r--   0 cfr        (501) staff       (20)       55 2024-05-07 07:21:27.000000 pmonitor-1.1.0/pmonitor.egg-info/entry_points.txt
--rw-r--r--   0 cfr        (501) staff       (20)        8 2024-05-07 07:21:27.000000 pmonitor-1.1.0/pmonitor.egg-info/top_level.txt
--rw-r--r--   0 cfr        (501) staff       (20)       38 2024-05-07 07:21:27.257622 pmonitor-1.1.0/setup.cfg
--rw-r--r--   0 cfr        (501) staff       (20)      622 2024-05-07 07:21:25.000000 pmonitor-1.1.0/setup.py
+drwxr-xr-x   0 cfr        (501) staff       (20)        0 2024-05-07 07:41:52.570284 pmonitor-1.1.1/
+-rw-r--r--   0 cfr        (501) staff       (20)      225 2024-05-07 07:41:52.569752 pmonitor-1.1.1/PKG-INFO
+-rw-r--r--   0 cfr        (501) staff       (20)       26 2024-05-06 02:50:55.000000 pmonitor-1.1.1/README.md
+drwxr-xr-x   0 cfr        (501) staff       (20)        0 2024-05-07 07:41:52.565272 pmonitor-1.1.1/monitor/
+-rw-r--r--   0 cfr        (501) staff       (20)     8523 2024-05-06 09:32:42.000000 pmonitor-1.1.1/monitor/WinPidUtil.py
+-rw-r--r--   0 cfr        (501) staff       (20)        0 2024-05-06 02:50:55.000000 pmonitor-1.1.1/monitor/__init__.py
+-rw-r--r--   0 cfr        (501) staff       (20)     3620 2024-05-06 08:11:43.000000 pmonitor-1.1.1/monitor/get_process_name.py
+-rw-r--r--   0 cfr        (501) staff       (20)     4651 2024-05-06 02:50:55.000000 pmonitor-1.1.1/monitor/monitor_mac.py
+-rw-r--r--   0 cfr        (501) staff       (20)    10208 2024-05-07 07:21:02.000000 pmonitor-1.1.1/monitor/monitor_pids.py
+-rw-r--r--   0 cfr        (501) staff       (20)     6161 2024-05-06 02:50:55.000000 pmonitor-1.1.1/monitor/monitor_win.py
+-rw-r--r--   0 cfr        (501) staff       (20)     2104 2024-05-07 07:41:37.000000 pmonitor-1.1.1/monitor/run_monitor.py
+-rw-r--r--   0 cfr        (501) staff       (20)     3208 2024-05-06 02:50:55.000000 pmonitor-1.1.1/monitor/sys_info.py
+drwxr-xr-x   0 cfr        (501) staff       (20)        0 2024-05-07 07:41:52.568883 pmonitor-1.1.1/pmonitor.egg-info/
+-rw-r--r--   0 cfr        (501) staff       (20)      225 2024-05-07 07:41:52.000000 pmonitor-1.1.1/pmonitor.egg-info/PKG-INFO
+-rw-r--r--   0 cfr        (501) staff       (20)      364 2024-05-07 07:41:52.000000 pmonitor-1.1.1/pmonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 cfr        (501) staff       (20)        1 2024-05-07 07:41:52.000000 pmonitor-1.1.1/pmonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 cfr        (501) staff       (20)       55 2024-05-07 07:41:52.000000 pmonitor-1.1.1/pmonitor.egg-info/entry_points.txt
+-rw-r--r--   0 cfr        (501) staff       (20)        8 2024-05-07 07:41:52.000000 pmonitor-1.1.1/pmonitor.egg-info/top_level.txt
+-rw-r--r--   0 cfr        (501) staff       (20)       38 2024-05-07 07:41:52.570545 pmonitor-1.1.1/setup.cfg
+-rw-r--r--   0 cfr        (501) staff       (20)      622 2024-05-07 07:41:51.000000 pmonitor-1.1.1/setup.py
```

### Comparing `pmonitor-1.1.0/monitor/WinPidUtil.py` & `pmonitor-1.1.1/monitor/WinPidUtil.py`

 * *Files identical despite different names*

### Comparing `pmonitor-1.1.0/monitor/get_process_name.py` & `pmonitor-1.1.1/monitor/get_process_name.py`

 * *Files identical despite different names*

### Comparing `pmonitor-1.1.0/monitor/monitor_mac.py` & `pmonitor-1.1.1/monitor/monitor_mac.py`

 * *Files identical despite different names*

### Comparing `pmonitor-1.1.0/monitor/monitor_pids.py` & `pmonitor-1.1.1/monitor/monitor_pids.py`

 * *Files identical despite different names*

### Comparing `pmonitor-1.1.0/monitor/monitor_win.py` & `pmonitor-1.1.1/monitor/monitor_win.py`

 * *Files identical despite different names*

### Comparing `pmonitor-1.1.0/monitor/run_monitor.py` & `pmonitor-1.1.1/monitor/run_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import sys
 
 from monitor.sys_info import SysInfo
 from monitor. monitor_pids import *
-import get_process_name
+from monitor.get_process_name import *
 import asyncio
 
 
 def main():
     parser = argparse.ArgumentParser(description='指定进程名或进程Pid即可获取性能数据~')
     parser.add_argument('-n', '--name', required=True, help='进程名称')
     parser.add_argument('-t', '--time', help='采集间隔时间/s', type=int, default=1)
@@ -25,15 +25,15 @@
     else:
         parser.print_help()
         exit()
 
     if args.time:
         interval = args.time
 
-    process_name = get_process_name.ProcessName()
+    process_name = ProcessName()
     if process is not None:
         print('监测进程<{}>，采集数据间隔<{}s>'.format(process, interval))
     else:
         parser.print_help()
         exit()
 
     pid = process_name.find_main_process_pid(process)
```

### Comparing `pmonitor-1.1.0/monitor/sys_info.py` & `pmonitor-1.1.1/monitor/sys_info.py`

 * *Files identical despite different names*

### Comparing `pmonitor-1.1.0/setup.py` & `pmonitor-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(name='pmonitor',
-      version='1.1.0',
+      version='1.1.1',
       description='pc monitor',
       long_description=long_description,
       author='cfr',
       author_email='1354592998@qq.com',
       install_requires=[],
       license='MIT',
       packages=find_packages(),
```

