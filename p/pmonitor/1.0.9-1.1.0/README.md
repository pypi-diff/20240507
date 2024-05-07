# Comparing `tmp/pmonitor-1.0.9.tar.gz` & `tmp/pmonitor-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmonitor-1.0.9.tar", last modified: Tue May  7 06:41:13 2024, max compression
+gzip compressed data, was "pmonitor-1.1.0.tar", last modified: Tue May  7 07:21:27 2024, max compression
```

## Comparing `pmonitor-1.0.9.tar` & `pmonitor-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 cfr        (501) staff       (20)        0 2024-05-07 06:41:13.701782 pmonitor-1.0.9/
--rw-r--r--   0 cfr        (501) staff       (20)      225 2024-05-07 06:41:13.701508 pmonitor-1.0.9/PKG-INFO
--rw-r--r--   0 cfr        (501) staff       (20)       26 2024-05-06 02:50:55.000000 pmonitor-1.0.9/README.md
-drwxr-xr-x   0 cfr        (501) staff       (20)        0 2024-05-07 06:41:13.699001 pmonitor-1.0.9/monitor/
--rw-r--r--   0 cfr        (501) staff       (20)     8523 2024-05-06 09:32:42.000000 pmonitor-1.0.9/monitor/WinPidUtil.py
--rw-r--r--   0 cfr        (501) staff       (20)        0 2024-05-06 02:50:55.000000 pmonitor-1.0.9/monitor/__init__.py
--rw-r--r--   0 cfr        (501) staff       (20)     3620 2024-05-06 08:11:43.000000 pmonitor-1.0.9/monitor/get_process_name.py
--rw-r--r--   0 cfr        (501) staff       (20)     4651 2024-05-06 02:50:55.000000 pmonitor-1.0.9/monitor/monitor_mac.py
--rw-r--r--   0 cfr        (501) staff       (20)    10377 2024-05-07 06:07:26.000000 pmonitor-1.0.9/monitor/monitor_pids.py
--rw-r--r--   0 cfr        (501) staff       (20)     6161 2024-05-06 02:50:55.000000 pmonitor-1.0.9/monitor/monitor_win.py
--rw-r--r--   0 cfr        (501) staff       (20)     2091 2024-05-07 06:08:01.000000 pmonitor-1.0.9/monitor/run_monitor.py
--rw-r--r--   0 cfr        (501) staff       (20)     3208 2024-05-06 02:50:55.000000 pmonitor-1.0.9/monitor/sys_info.py
-drwxr-xr-x   0 cfr        (501) staff       (20)        0 2024-05-07 06:41:13.701045 pmonitor-1.0.9/pmonitor.egg-info/
--rw-r--r--   0 cfr        (501) staff       (20)      225 2024-05-07 06:41:13.000000 pmonitor-1.0.9/pmonitor.egg-info/PKG-INFO
--rw-r--r--   0 cfr        (501) staff       (20)      364 2024-05-07 06:41:13.000000 pmonitor-1.0.9/pmonitor.egg-info/SOURCES.txt
--rw-r--r--   0 cfr        (501) staff       (20)        1 2024-05-07 06:41:13.000000 pmonitor-1.0.9/pmonitor.egg-info/dependency_links.txt
--rw-r--r--   0 cfr        (501) staff       (20)       55 2024-05-07 06:41:13.000000 pmonitor-1.0.9/pmonitor.egg-info/entry_points.txt
--rw-r--r--   0 cfr        (501) staff       (20)        8 2024-05-07 06:41:13.000000 pmonitor-1.0.9/pmonitor.egg-info/top_level.txt
--rw-r--r--   0 cfr        (501) staff       (20)       38 2024-05-07 06:41:13.701897 pmonitor-1.0.9/setup.cfg
--rw-r--r--   0 cfr        (501) staff       (20)      622 2024-05-07 06:36:42.000000 pmonitor-1.0.9/setup.py
+drwxr-xr-x   0 cfr        (501) staff       (20)        0 2024-05-07 07:21:27.257403 pmonitor-1.1.0/
+-rw-r--r--   0 cfr        (501) staff       (20)      225 2024-05-07 07:21:27.256830 pmonitor-1.1.0/PKG-INFO
+-rw-r--r--   0 cfr        (501) staff       (20)       26 2024-05-06 02:50:55.000000 pmonitor-1.1.0/README.md
+drwxr-xr-x   0 cfr        (501) staff       (20)        0 2024-05-07 07:21:27.252827 pmonitor-1.1.0/monitor/
+-rw-r--r--   0 cfr        (501) staff       (20)     8523 2024-05-06 09:32:42.000000 pmonitor-1.1.0/monitor/WinPidUtil.py
+-rw-r--r--   0 cfr        (501) staff       (20)        0 2024-05-06 02:50:55.000000 pmonitor-1.1.0/monitor/__init__.py
+-rw-r--r--   0 cfr        (501) staff       (20)     3620 2024-05-06 08:11:43.000000 pmonitor-1.1.0/monitor/get_process_name.py
+-rw-r--r--   0 cfr        (501) staff       (20)     4651 2024-05-06 02:50:55.000000 pmonitor-1.1.0/monitor/monitor_mac.py
+-rw-r--r--   0 cfr        (501) staff       (20)    10208 2024-05-07 07:21:02.000000 pmonitor-1.1.0/monitor/monitor_pids.py
+-rw-r--r--   0 cfr        (501) staff       (20)     6161 2024-05-06 02:50:55.000000 pmonitor-1.1.0/monitor/monitor_win.py
+-rw-r--r--   0 cfr        (501) staff       (20)     2106 2024-05-07 07:21:02.000000 pmonitor-1.1.0/monitor/run_monitor.py
+-rw-r--r--   0 cfr        (501) staff       (20)     3208 2024-05-06 02:50:55.000000 pmonitor-1.1.0/monitor/sys_info.py
+drwxr-xr-x   0 cfr        (501) staff       (20)        0 2024-05-07 07:21:27.255980 pmonitor-1.1.0/pmonitor.egg-info/
+-rw-r--r--   0 cfr        (501) staff       (20)      225 2024-05-07 07:21:27.000000 pmonitor-1.1.0/pmonitor.egg-info/PKG-INFO
+-rw-r--r--   0 cfr        (501) staff       (20)      364 2024-05-07 07:21:27.000000 pmonitor-1.1.0/pmonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 cfr        (501) staff       (20)        1 2024-05-07 07:21:27.000000 pmonitor-1.1.0/pmonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 cfr        (501) staff       (20)       55 2024-05-07 07:21:27.000000 pmonitor-1.1.0/pmonitor.egg-info/entry_points.txt
+-rw-r--r--   0 cfr        (501) staff       (20)        8 2024-05-07 07:21:27.000000 pmonitor-1.1.0/pmonitor.egg-info/top_level.txt
+-rw-r--r--   0 cfr        (501) staff       (20)       38 2024-05-07 07:21:27.257622 pmonitor-1.1.0/setup.cfg
+-rw-r--r--   0 cfr        (501) staff       (20)      622 2024-05-07 07:21:25.000000 pmonitor-1.1.0/setup.py
```

### Comparing `pmonitor-1.0.9/monitor/WinPidUtil.py` & `pmonitor-1.1.0/monitor/WinPidUtil.py`

 * *Files identical despite different names*

### Comparing `pmonitor-1.0.9/monitor/get_process_name.py` & `pmonitor-1.1.0/monitor/get_process_name.py`

 * *Files identical despite different names*

### Comparing `pmonitor-1.0.9/monitor/monitor_mac.py` & `pmonitor-1.1.0/monitor/monitor_mac.py`

 * *Files identical despite different names*

### Comparing `pmonitor-1.0.9/monitor/monitor_pids.py` & `pmonitor-1.1.0/monitor/monitor_pids.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import psutil
 import time
 import json
-import get_process_name
+from monitor.get_process_name import *
 import sys
 import platform
 if platform.system == 'Windows':
-    import WinPidUtil
+    from monitor.WinPidUtil import *
 import asyncio
 import platform
 import ctypes
 
 
 class PidsPerf:
 
     def __init__(self, process_name, interval=1):
         self.process_name = process_name
         self.interval = interval
-        self.processUtil = get_process_name.ProcessName()
+        self.processUtil = ProcessName()
 
     def get_mac_perf(self):
         current_pid = self.processUtil.find_main_process_pid(self.process_name)
         while True:
             minor_cpu_sum = 0
             minor_real_mem_sum = 0
             minor_mem_percent_sum = 0
@@ -85,16 +85,16 @@
             return io_read_bytes, io_write_bytes
         except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
             pass
         return 0, 0
 
     def get_win_perf(self):
         from ctypes import byref
-        pidWinPerf = WinPidUtil.PidWinPerformance()
-        system_time_pre = pidWinPerf.filetime_to_100nano_seconds(WinPidUtil.FILETIME())
+        pidWinPerf = PidWinPerformance()
+        system_time_pre = pidWinPerf.filetime_to_100nano_seconds(FILETIME())
         p_pid = self.processUtil.find_main_process_pid(self.process_name)
         child_pids = self.processUtil.get_children_pids(p_pid)
         child_pids.add(p_pid)  # app内所有pid
         process_cpu_times_pre = {pid: pidWinPerf.get_process_cpu_time(pid) for pid in child_pids}
         process_io_counters_pre = {pid: pidWinPerf.get_io_counters(pid) for pid in child_pids}
         monitor_interval_seconds = 1  # 监控间隔（秒）
         while True:
@@ -106,17 +106,17 @@
             minor_io_read_sum = 0
             minor_io_write_sum = 0
 
             current_pids = self.processUtil.get_children_pids(p_pid)  # 获取所有子进程
             current_pids.add(p_pid)  # 将主进程及子进程添加到list中
 
             start_time = time.time()  # 记录循环开始的时间
-            system_idle_time = WinPidUtil.FILETIME()
-            system_kernel_time = WinPidUtil.FILETIME()
-            system_user_time = WinPidUtil.FILETIME()
+            system_idle_time = FILETIME()
+            system_kernel_time = FILETIME()
+            system_user_time = FILETIME()
             ctypes.windll.kernel32.GetSystemTimes(byref(system_idle_time),
                                                   byref(system_kernel_time),
                                                   byref(system_user_time))
             system_time_post = pidWinPerf.filetime_to_100nano_seconds(
                 system_kernel_time) + pidWinPerf.filetime_to_100nano_seconds(system_user_time)
 
             child_pids = self.processUtil.get_children_pids(p_pid)
@@ -189,12 +189,7 @@
 
     async def start_perf(self):
         if platform.system() == 'Windows':
             await asyncio.gather(self.get_win_perf())
         else:
             await asyncio.gather(self.get_mac_perf())
 
-
-if __name__ == '__main__':
-    processName = 'WXWork.exe'
-    perf = PidsPerf(processName)
-    asyncio.run(perf.start_perf())
```

### Comparing `pmonitor-1.0.9/monitor/monitor_win.py` & `pmonitor-1.1.0/monitor/monitor_win.py`

 * *Files identical despite different names*

### Comparing `pmonitor-1.0.9/monitor/run_monitor.py` & `pmonitor-1.1.0/monitor/run_monitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import argparse
 import sys
 
-import sys_info
-import monitor_pids
+from monitor.sys_info import SysInfo
+from monitor. monitor_pids import *
 import get_process_name
 import asyncio
 
 
 def main():
     parser = argparse.ArgumentParser(description='指定进程名或进程Pid即可获取性能数据~')
     parser.add_argument('-n', '--name', required=True, help='进程名称')
     parser.add_argument('-t', '--time', help='采集间隔时间/s', type=int, default=1)
     parser.add_argument('-i', '--info', help='输出当前系统使用情况', action='store_true')
     args = parser.parse_args()
     print(args)
 
     if args.info:
-        print(sys_info.SysInfo().get_device_info())
+        print(SysInfo().get_device_info())
         exit()
 
     process = None
     if args.name:
         process = args.name
     else:
         parser.print_help()
@@ -41,15 +41,15 @@
         process = process_name.get_pid_find_pid(int(pid))
 
     if pid is None or process is None:
         print('进程列表中未找到<{}>，请检查应用是否启动！停止监测任务'.format(process))
         sys.exit(0)
 
     print('开始监测进程<{}>，主进程pid<{}>'.format(process, pid))
-    pidsPerf = monitor_pids.PidsPerf(process, interval)
+    pidsPerf = PidsPerf(process, interval)
     asyncio.run(pidsPerf.start_perf())
     # if platform.system() == 'Windows':
     #     monitor = WinPerformance(pid=int(pid))
     # else:
     #     monitor = MacPerformance(pid=int(pid))
     # print(f'{"   ".join(monitor.header)}')
     # while True:
```

### Comparing `pmonitor-1.0.9/monitor/sys_info.py` & `pmonitor-1.1.0/monitor/sys_info.py`

 * *Files identical despite different names*

### Comparing `pmonitor-1.0.9/setup.py` & `pmonitor-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(name='pmonitor',
-      version='1.0.9',
+      version='1.1.0',
       description='pc monitor',
       long_description=long_description,
       author='cfr',
       author_email='1354592998@qq.com',
       install_requires=[],
       license='MIT',
       packages=find_packages(),
```

