# Comparing `tmp/pmonitor-1.0.8.tar.gz` & `tmp/pmonitor-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmonitor-1.0.8.tar", last modified: Thu Sep  7 08:07:54 2023, max compression
+gzip compressed data, was "pmonitor-1.0.9.tar", last modified: Tue May  7 06:41:13 2024, max compression
```

## Comparing `pmonitor-1.0.8.tar` & `pmonitor-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 cfr        (501) staff       (20)        0 2023-09-07 08:07:54.553434 pmonitor-1.0.8/
--rw-r--r--   0 cfr        (501) staff       (20)      214 2023-09-07 08:07:54.552796 pmonitor-1.0.8/PKG-INFO
--rw-r--r--   0 cfr        (501) staff       (20)       26 2023-08-23 09:22:36.000000 pmonitor-1.0.8/README.md
-drwxr-xr-x   0 cfr        (501) staff       (20)        0 2023-09-07 08:07:54.549910 pmonitor-1.0.8/monitor/
--rw-r--r--   0 cfr        (501) staff       (20)        0 2023-08-23 06:56:09.000000 pmonitor-1.0.8/monitor/__init__.py
--rw-r--r--   0 cfr        (501) staff       (20)     2154 2023-08-23 09:55:27.000000 pmonitor-1.0.8/monitor/get_process_name.py
--rw-r--r--   0 cfr        (501) staff       (20)     4651 2023-09-06 06:10:52.000000 pmonitor-1.0.8/monitor/monitor_mac.py
--rw-r--r--   0 cfr        (501) staff       (20)     6161 2023-08-23 09:08:48.000000 pmonitor-1.0.8/monitor/monitor_win.py
--rw-r--r--   0 cfr        (501) staff       (20)     2267 2023-09-07 08:06:42.000000 pmonitor-1.0.8/monitor/run_monitor.py
--rw-r--r--   0 cfr        (501) staff       (20)     3208 2023-07-10 07:11:55.000000 pmonitor-1.0.8/monitor/sys_info.py
-drwxr-xr-x   0 cfr        (501) staff       (20)        0 2023-09-07 08:07:54.552162 pmonitor-1.0.8/pmonitor.egg-info/
--rw-r--r--   0 cfr        (501) staff       (20)      214 2023-09-07 08:07:54.000000 pmonitor-1.0.8/pmonitor.egg-info/PKG-INFO
--rw-r--r--   0 cfr        (501) staff       (20)      318 2023-09-07 08:07:54.000000 pmonitor-1.0.8/pmonitor.egg-info/SOURCES.txt
--rw-r--r--   0 cfr        (501) staff       (20)        1 2023-09-07 08:07:54.000000 pmonitor-1.0.8/pmonitor.egg-info/dependency_links.txt
--rw-r--r--   0 cfr        (501) staff       (20)       55 2023-09-07 08:07:54.000000 pmonitor-1.0.8/pmonitor.egg-info/entry_points.txt
--rw-r--r--   0 cfr        (501) staff       (20)        8 2023-09-07 08:07:54.000000 pmonitor-1.0.8/pmonitor.egg-info/top_level.txt
--rw-r--r--   0 cfr        (501) staff       (20)       38 2023-09-07 08:07:54.553624 pmonitor-1.0.8/setup.cfg
--rw-r--r--   0 cfr        (501) staff       (20)      622 2023-09-07 08:06:42.000000 pmonitor-1.0.8/setup.py
+drwxr-xr-x   0 cfr        (501) staff       (20)        0 2024-05-07 06:41:13.701782 pmonitor-1.0.9/
+-rw-r--r--   0 cfr        (501) staff       (20)      225 2024-05-07 06:41:13.701508 pmonitor-1.0.9/PKG-INFO
+-rw-r--r--   0 cfr        (501) staff       (20)       26 2024-05-06 02:50:55.000000 pmonitor-1.0.9/README.md
+drwxr-xr-x   0 cfr        (501) staff       (20)        0 2024-05-07 06:41:13.699001 pmonitor-1.0.9/monitor/
+-rw-r--r--   0 cfr        (501) staff       (20)     8523 2024-05-06 09:32:42.000000 pmonitor-1.0.9/monitor/WinPidUtil.py
+-rw-r--r--   0 cfr        (501) staff       (20)        0 2024-05-06 02:50:55.000000 pmonitor-1.0.9/monitor/__init__.py
+-rw-r--r--   0 cfr        (501) staff       (20)     3620 2024-05-06 08:11:43.000000 pmonitor-1.0.9/monitor/get_process_name.py
+-rw-r--r--   0 cfr        (501) staff       (20)     4651 2024-05-06 02:50:55.000000 pmonitor-1.0.9/monitor/monitor_mac.py
+-rw-r--r--   0 cfr        (501) staff       (20)    10377 2024-05-07 06:07:26.000000 pmonitor-1.0.9/monitor/monitor_pids.py
+-rw-r--r--   0 cfr        (501) staff       (20)     6161 2024-05-06 02:50:55.000000 pmonitor-1.0.9/monitor/monitor_win.py
+-rw-r--r--   0 cfr        (501) staff       (20)     2091 2024-05-07 06:08:01.000000 pmonitor-1.0.9/monitor/run_monitor.py
+-rw-r--r--   0 cfr        (501) staff       (20)     3208 2024-05-06 02:50:55.000000 pmonitor-1.0.9/monitor/sys_info.py
+drwxr-xr-x   0 cfr        (501) staff       (20)        0 2024-05-07 06:41:13.701045 pmonitor-1.0.9/pmonitor.egg-info/
+-rw-r--r--   0 cfr        (501) staff       (20)      225 2024-05-07 06:41:13.000000 pmonitor-1.0.9/pmonitor.egg-info/PKG-INFO
+-rw-r--r--   0 cfr        (501) staff       (20)      364 2024-05-07 06:41:13.000000 pmonitor-1.0.9/pmonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 cfr        (501) staff       (20)        1 2024-05-07 06:41:13.000000 pmonitor-1.0.9/pmonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 cfr        (501) staff       (20)       55 2024-05-07 06:41:13.000000 pmonitor-1.0.9/pmonitor.egg-info/entry_points.txt
+-rw-r--r--   0 cfr        (501) staff       (20)        8 2024-05-07 06:41:13.000000 pmonitor-1.0.9/pmonitor.egg-info/top_level.txt
+-rw-r--r--   0 cfr        (501) staff       (20)       38 2024-05-07 06:41:13.701897 pmonitor-1.0.9/setup.cfg
+-rw-r--r--   0 cfr        (501) staff       (20)      622 2024-05-07 06:36:42.000000 pmonitor-1.0.9/setup.py
```

### Comparing `pmonitor-1.0.8/monitor/monitor_mac.py` & `pmonitor-1.0.9/monitor/monitor_mac.py`

 * *Files identical despite different names*

### Comparing `pmonitor-1.0.8/monitor/monitor_win.py` & `pmonitor-1.0.9/monitor/monitor_win.py`

 * *Files identical despite different names*

### Comparing `pmonitor-1.0.8/monitor/run_monitor.py` & `pmonitor-1.0.9/monitor/run_monitor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,68 @@
 import argparse
 import sys
 
-import platform
-from monitor.sys_info import SysInfo
-from monitor.get_process_name import ProcessName
-
-if platform.system() == 'Windows':
-    from monitor.monitor_win import *
-else:
-    from monitor.monitor_mac import *
+import sys_info
+import monitor_pids
+import get_process_name
+import asyncio
 
 
 def main():
     parser = argparse.ArgumentParser(description='指定进程名或进程Pid即可获取性能数据~')
-    parser.add_argument('-n', '--name', help='进程名称')
-    parser.add_argument('-p', '--pid', help='进程Pid')
+    parser.add_argument('-n', '--name', required=True, help='进程名称')
     parser.add_argument('-t', '--time', help='采集间隔时间/s', type=int, default=1)
     parser.add_argument('-i', '--info', help='输出当前系统使用情况', action='store_true')
     args = parser.parse_args()
     print(args)
 
     if args.info:
-        print(SysInfo().get_device_info())
+        print(sys_info.SysInfo().get_device_info())
         exit()
 
-    pid = None
     process = None
-
-    if args.pid:
-        pid = args.pid
-    elif args.name:
+    if args.name:
         process = args.name
     else:
         parser.print_help()
         exit()
 
     if args.time:
         interval = args.time
 
-    process_name = ProcessName()
-    if pid is not None:
-        print('监测进程Pid<{}>，采集数据间隔<{}s>'.format(pid, interval))
-    elif process is not None:
+    process_name = get_process_name.ProcessName()
+    if process is not None:
         print('监测进程<{}>，采集数据间隔<{}s>'.format(process, interval))
-    if pid is None:
-        pid = process_name.find_main_process_pid(process)
+    else:
+        parser.print_help()
+        exit()
 
+    pid = process_name.find_main_process_pid(process)
     if process is None:
         process = process_name.get_pid_find_pid(int(pid))
 
     if pid is None or process is None:
         print('进程列表中未找到<{}>，请检查应用是否启动！停止监测任务'.format(process))
         sys.exit(0)
 
     print('开始监测进程<{}>，主进程pid<{}>'.format(process, pid))
-    if platform.system() == 'Windows':
-        monitor = WinPerformance(pid=int(pid))
-    else:
-        monitor = MacPerformance(pid=int(pid))
-    print(f'{"   ".join(monitor.header)}')
-    while True:
-        try:
-            result = asyncio.run(monitor.get_all_monitor())
-        except Exception as e:
-            result = monitor.get_all_usage()
-        result.insert(0, time.strftime('%H:%M:%S'))
-        line = [str(item) for item in result]
-        info = "        ".join(line)
-        print(info)
-        sys.stdout.flush()
+    pidsPerf = monitor_pids.PidsPerf(process, interval)
+    asyncio.run(pidsPerf.start_perf())
+    # if platform.system() == 'Windows':
+    #     monitor = WinPerformance(pid=int(pid))
+    # else:
+    #     monitor = MacPerformance(pid=int(pid))
+    # print(f'{"   ".join(monitor.header)}')
+    # while True:
+    #     try:
+    #         result = asyncio.run(monitor.get_all_monitor())
+    #     except Exception as e:
+    #         result = monitor.get_all_usage()
+    #     result.insert(0, time.strftime('%H:%M:%S'))
+    #     line = [str(item) for item in result]
+    #     info = "        ".join(line)
+    #     print(info)
+    #     sys.stdout.flush()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pmonitor-1.0.8/monitor/sys_info.py` & `pmonitor-1.0.9/monitor/sys_info.py`

 * *Files identical despite different names*

### Comparing `pmonitor-1.0.8/setup.py` & `pmonitor-1.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(name='pmonitor',
-      version='1.0.8',
+      version='1.0.9',
       description='pc monitor',
       long_description=long_description,
       author='cfr',
       author_email='1354592998@qq.com',
       install_requires=[],
       license='MIT',
       packages=find_packages(),
```

