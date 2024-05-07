# Comparing `tmp/physiocurve-2022.7.8.tar.gz` & `tmp/physiocurve-2024.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "physiocurve-2022.7.8.tar", max compression
+gzip compressed data, was "physiocurve-2024.5.7.tar", max compression
```

## Comparing `physiocurve-2022.7.8.tar` & `physiocurve-2024.5.7.tar`

### file list

```diff
@@ -1,54 +1,56 @@
--rw-r--r--   0        0        0      750 2020-07-11 07:20:18.276521 physiocurve-2022.7.8/LICENSE
--rw-r--r--   0        0        0      139 2022-04-03 20:14:04.579437 physiocurve-2022.7.8/README.md
--rw-r--r--   0        0        0      235 2022-06-26 19:31:07.040027 physiocurve-2022.7.8/physiocurve/__init__.py
--rw-r--r--   0        0        0     1081 2022-05-12 07:33:19.100101 physiocurve-2022.7.8/physiocurve/common/__init__.py
--rw-r--r--   0        0        0     1142 2022-06-30 07:57:54.561564 physiocurve-2022.7.8/physiocurve/common/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0       59 2022-05-12 07:41:33.231170 physiocurve-2022.7.8/physiocurve/ecg/__init__.py
--rw-r--r--   0        0        0      219 2022-06-30 07:57:38.117472 physiocurve-2022.7.8/physiocurve/ecg/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      219 2022-05-18 10:23:14.442956 physiocurve-2022.7.8/physiocurve/ecg/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1126 2022-06-30 07:57:38.117472 physiocurve-2022.7.8/physiocurve/ecg/__pycache__/wrapper.cpython-38.pyc
--rw-r--r--   0        0        0     1122 2022-06-26 19:15:32.623028 physiocurve-2022.7.8/physiocurve/ecg/__pycache__/wrapper.cpython-39.pyc
--rw-r--r--   0        0        0      843 2022-06-26 19:15:11.979038 physiocurve-2022.7.8/physiocurve/ecg/wrapper.py
--rw-r--r--   0        0        0      133 2022-05-12 07:22:55.155125 physiocurve-2022.7.8/physiocurve/flow/__init__.py
--rw-r--r--   0        0        0      291 2022-06-30 07:57:54.561564 physiocurve-2022.7.8/physiocurve/flow/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      291 2022-05-18 10:23:15.118945 physiocurve-2022.7.8/physiocurve/flow/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      547 2022-06-30 07:57:54.561564 physiocurve-2022.7.8/physiocurve/flow/__pycache__/flow.cpython-38.pyc
--rw-r--r--   0        0        0      547 2022-05-18 10:23:15.122944 physiocurve-2022.7.8/physiocurve/flow/__pycache__/flow.cpython-39.pyc
--rw-r--r--   0        0        0     1150 2022-06-30 07:57:55.165567 physiocurve-2022.7.8/physiocurve/flow/__pycache__/wrapper.cpython-38.pyc
--rw-r--r--   0        0        0     1150 2022-05-18 10:23:15.122944 physiocurve-2022.7.8/physiocurve/flow/__pycache__/wrapper.cpython-39.pyc
--rw-r--r--   0        0        0      467 2022-07-06 11:25:58.984545 physiocurve-2022.7.8/physiocurve/flow/flow.py
--rw-r--r--   0        0        0      580 2022-05-12 07:22:55.067124 physiocurve-2022.7.8/physiocurve/flow/wrapper.py
--rw-r--r--   0        0        0      142 2022-05-12 07:29:30.808869 physiocurve-2022.7.8/physiocurve/pandas/__init__.py
--rw-r--r--   0        0        0      328 2022-06-30 07:58:41.865822 physiocurve-2022.7.8/physiocurve/pandas/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      951 2022-06-30 07:58:41.865822 physiocurve-2022.7.8/physiocurve/pandas/__pycache__/ecg.cpython-38.pyc
--rw-r--r--   0        0        0     1246 2022-06-30 07:58:41.865822 physiocurve-2022.7.8/physiocurve/pandas/__pycache__/flow.cpython-38.pyc
--rw-r--r--   0        0        0      462 2022-06-30 07:58:41.869822 physiocurve-2022.7.8/physiocurve/pandas/__pycache__/ppg.cpython-38.pyc
--rw-r--r--   0        0        0     1866 2022-06-30 07:58:41.869822 physiocurve-2022.7.8/physiocurve/pandas/__pycache__/pressure.cpython-38.pyc
--rw-r--r--   0        0        0      505 2022-06-26 18:34:23.666269 physiocurve-2022.7.8/physiocurve/pandas/ecg.py
--rw-r--r--   0        0        0      685 2022-06-26 18:34:55.594203 physiocurve-2022.7.8/physiocurve/pandas/flow.py
--rw-r--r--   0        0        0      107 2022-05-12 07:13:50.898565 physiocurve-2022.7.8/physiocurve/pandas/ppg.py
--rw-r--r--   0        0        0     1036 2022-06-26 18:35:06.178182 physiocurve-2022.7.8/physiocurve/pandas/pressure.py
--rw-r--r--   0        0        0       59 2022-05-12 07:40:59.182522 physiocurve-2022.7.8/physiocurve/ppg/__init__.py
--rw-r--r--   0        0        0      219 2022-06-30 07:57:55.169567 physiocurve-2022.7.8/physiocurve/ppg/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      219 2022-05-18 10:23:15.122944 physiocurve-2022.7.8/physiocurve/ppg/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      679 2022-06-30 07:57:55.169567 physiocurve-2022.7.8/physiocurve/ppg/__pycache__/wrapper.cpython-38.pyc
--rw-r--r--   0        0        0      679 2022-05-18 10:23:15.122944 physiocurve-2022.7.8/physiocurve/ppg/__pycache__/wrapper.cpython-39.pyc
--rw-r--r--   0        0        0      208 2022-07-08 18:27:22.805351 physiocurve-2022.7.8/physiocurve/ppg/wrapper.py
--rw-r--r--   0        0        0      153 2022-05-12 07:38:37.788557 physiocurve-2022.7.8/physiocurve/pressure/__init__.py
--rw-r--r--   0        0        0      309 2022-06-30 07:57:55.169567 physiocurve-2022.7.8/physiocurve/pressure/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      309 2022-05-18 10:23:15.122944 physiocurve-2022.7.8/physiocurve/pressure/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2015 2022-06-30 07:57:55.169567 physiocurve-2022.7.8/physiocurve/pressure/__pycache__/foot.cpython-38.pyc
--rw-r--r--   0        0        0     2011 2022-05-18 10:23:15.122944 physiocurve-2022.7.8/physiocurve/pressure/__pycache__/foot.cpython-39.pyc
--rw-r--r--   0        0        0     3563 2022-06-30 07:57:55.173567 physiocurve-2022.7.8/physiocurve/pressure/__pycache__/incycle.cpython-38.pyc
--rw-r--r--   0        0        0     3563 2022-06-26 19:32:24.792050 physiocurve-2022.7.8/physiocurve/pressure/__pycache__/incycle.cpython-39.pyc
--rw-r--r--   0        0        0     2514 2022-06-30 07:57:55.173567 physiocurve-2022.7.8/physiocurve/pressure/__pycache__/wrapper.cpython-38.pyc
--rw-r--r--   0        0        0     2516 2022-05-18 10:23:15.126944 physiocurve-2022.7.8/physiocurve/pressure/__pycache__/wrapper.cpython-39.pyc
--rw-r--r--   0        0        0     1786 2022-05-12 07:39:42.309455 physiocurve-2022.7.8/physiocurve/pressure/foot.py
--rw-r--r--   0        0        0     4645 2022-07-08 18:46:48.812792 physiocurve-2022.7.8/physiocurve/pressure/incycle.py
--rw-r--r--   0        0        0        0 2020-05-30 15:02:39.370743 physiocurve-2022.7.8/physiocurve/pressure/reference/__init__.py
--rw-r--r--   0        0        0     3035 2020-05-29 11:14:02.138293 physiocurve-2022.7.8/physiocurve/pressure/reference/dic_sndderiv.py
--rw-r--r--   0        0        0     1817 2022-06-26 19:29:40.703994 physiocurve-2022.7.8/physiocurve/pressure/reference/foot.py
--rw-r--r--   0        0        0     1913 2022-05-12 07:38:38.600569 physiocurve-2022.7.8/physiocurve/pressure/wrapper.py
--rw-r--r--   0        0        0      758 2022-07-08 18:50:00.348079 physiocurve-2022.7.8/pyproject.toml
--rw-r--r--   0        0        0     1012 2022-07-08 19:13:27.813374 physiocurve-2022.7.8/setup.py
--rw-r--r--   0        0        0      837 2022-07-08 19:13:27.813610 physiocurve-2022.7.8/PKG-INFO
+-rw-r--r--   0        0        0      750 2020-07-11 07:20:18.276521 physiocurve-2024.5.7/LICENSE
+-rw-r--r--   0        0        0      139 2022-04-03 20:14:04.579437 physiocurve-2024.5.7/README.md
+-rw-r--r--   0        0        0      234 2022-07-12 21:38:20.943048 physiocurve-2024.5.7/physiocurve/__init__.py
+-rw-r--r--   0        0        0     1151 2022-07-12 21:38:13.843018 physiocurve-2024.5.7/physiocurve/common/__init__.py
+-rw-r--r--   0        0        0     1224 2024-05-07 15:00:22.927732 physiocurve-2024.5.7/physiocurve/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1218 2022-07-18 12:09:26.552695 physiocurve-2024.5.7/physiocurve/common/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0       59 2022-07-12 21:29:20.120775 physiocurve-2024.5.7/physiocurve/ecg/__init__.py
+-rw-r--r--   0        0        0      221 2024-05-07 15:00:22.067724 physiocurve-2024.5.7/physiocurve/ecg/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      219 2022-07-18 12:08:02.768907 physiocurve-2024.5.7/physiocurve/ecg/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1877 2024-05-07 15:00:22.067724 physiocurve-2024.5.7/physiocurve/ecg/__pycache__/wrapper.cpython-310.pyc
+-rw-r--r--   0        0        0     1645 2022-07-18 12:08:02.768907 physiocurve-2024.5.7/physiocurve/ecg/__pycache__/wrapper.cpython-38.pyc
+-rw-r--r--   0        0        0     1493 2024-05-06 11:30:04.951822 physiocurve-2024.5.7/physiocurve/ecg/wrapper.py
+-rw-r--r--   0        0        0      133 2022-05-12 07:22:55.155125 physiocurve-2024.5.7/physiocurve/flow/__init__.py
+-rw-r--r--   0        0        0      293 2024-05-07 15:00:22.927732 physiocurve-2024.5.7/physiocurve/flow/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      291 2022-07-18 12:09:26.552695 physiocurve-2024.5.7/physiocurve/flow/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      619 2024-05-07 15:00:22.927732 physiocurve-2024.5.7/physiocurve/flow/__pycache__/flow.cpython-310.pyc
+-rw-r--r--   0        0        0      615 2022-07-18 12:09:26.552695 physiocurve-2024.5.7/physiocurve/flow/__pycache__/flow.cpython-38.pyc
+-rw-r--r--   0        0        0     1150 2024-05-07 15:00:23.007732 physiocurve-2024.5.7/physiocurve/flow/__pycache__/wrapper.cpython-310.pyc
+-rw-r--r--   0        0        0     1150 2022-07-18 12:09:26.776694 physiocurve-2024.5.7/physiocurve/flow/__pycache__/wrapper.cpython-38.pyc
+-rw-r--r--   0        0        0      557 2022-07-11 10:07:44.655049 physiocurve-2024.5.7/physiocurve/flow/flow.py
+-rw-r--r--   0        0        0      580 2022-05-12 07:22:55.067124 physiocurve-2024.5.7/physiocurve/flow/wrapper.py
+-rw-r--r--   0        0        0      142 2022-07-12 21:29:05.772715 physiocurve-2024.5.7/physiocurve/pandas/__init__.py
+-rw-r--r--   0        0        0      328 2024-05-07 15:00:23.071733 physiocurve-2024.5.7/physiocurve/pandas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      328 2022-07-18 12:09:26.784695 physiocurve-2024.5.7/physiocurve/pandas/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1953 2024-05-07 15:00:23.071733 physiocurve-2024.5.7/physiocurve/pandas/__pycache__/ecg.cpython-310.pyc
+-rw-r--r--   0        0        0     1521 2022-07-18 12:09:26.784695 physiocurve-2024.5.7/physiocurve/pandas/__pycache__/ecg.cpython-38.pyc
+-rw-r--r--   0        0        0     1204 2024-05-07 15:00:23.075733 physiocurve-2024.5.7/physiocurve/pandas/__pycache__/flow.cpython-310.pyc
+-rw-r--r--   0        0        0     1246 2022-07-18 12:09:26.788694 physiocurve-2024.5.7/physiocurve/pandas/__pycache__/flow.cpython-38.pyc
+-rw-r--r--   0        0        0      462 2024-05-07 15:00:23.075733 physiocurve-2024.5.7/physiocurve/pandas/__pycache__/ppg.cpython-310.pyc
+-rw-r--r--   0        0        0      462 2022-07-18 12:09:26.788694 physiocurve-2024.5.7/physiocurve/pandas/__pycache__/ppg.cpython-38.pyc
+-rw-r--r--   0        0        0     2177 2024-05-07 15:00:23.075733 physiocurve-2024.5.7/physiocurve/pandas/__pycache__/pressure.cpython-310.pyc
+-rw-r--r--   0        0        0     2363 2022-07-18 12:09:26.788694 physiocurve-2024.5.7/physiocurve/pandas/__pycache__/pressure.cpython-38.pyc
+-rw-r--r--   0        0        0     1197 2024-05-06 11:29:27.287544 physiocurve-2024.5.7/physiocurve/pandas/ecg.py
+-rw-r--r--   0        0        0      685 2022-06-26 18:34:55.594203 physiocurve-2024.5.7/physiocurve/pandas/flow.py
+-rw-r--r--   0        0        0      107 2022-05-12 07:13:50.898565 physiocurve-2024.5.7/physiocurve/pandas/ppg.py
+-rw-r--r--   0        0        0     1445 2022-07-14 12:42:50.551734 physiocurve-2024.5.7/physiocurve/pandas/pressure.py
+-rw-r--r--   0        0        0       59 2022-05-12 07:40:59.182522 physiocurve-2024.5.7/physiocurve/ppg/__init__.py
+-rw-r--r--   0        0        0      221 2024-05-07 15:00:23.007732 physiocurve-2024.5.7/physiocurve/ppg/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      219 2022-07-18 12:09:26.780694 physiocurve-2024.5.7/physiocurve/ppg/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      664 2024-05-07 15:00:23.007732 physiocurve-2024.5.7/physiocurve/ppg/__pycache__/wrapper.cpython-310.pyc
+-rw-r--r--   0        0        0      664 2022-07-18 12:09:26.780694 physiocurve-2024.5.7/physiocurve/ppg/__pycache__/wrapper.cpython-38.pyc
+-rw-r--r--   0        0        0      208 2022-07-08 18:27:22.805351 physiocurve-2024.5.7/physiocurve/ppg/wrapper.py
+-rw-r--r--   0        0        0       74 2022-07-12 21:25:43.279882 physiocurve-2024.5.7/physiocurve/pressure/__init__.py
+-rw-r--r--   0        0        0      236 2024-05-07 15:00:23.007732 physiocurve-2024.5.7/physiocurve/pressure/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      234 2022-07-18 12:09:26.780694 physiocurve-2024.5.7/physiocurve/pressure/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3044 2024-05-07 15:00:23.011732 physiocurve-2024.5.7/physiocurve/pressure/__pycache__/foot.cpython-310.pyc
+-rw-r--r--   0        0        0     3068 2022-07-18 12:09:26.780694 physiocurve-2024.5.7/physiocurve/pressure/__pycache__/foot.cpython-38.pyc
+-rw-r--r--   0        0        0     2982 2024-05-07 15:00:23.011732 physiocurve-2024.5.7/physiocurve/pressure/__pycache__/incycle.cpython-310.pyc
+-rw-r--r--   0        0        0     2964 2022-07-18 12:09:26.784695 physiocurve-2024.5.7/physiocurve/pressure/__pycache__/incycle.cpython-38.pyc
+-rw-r--r--   0        0        0     3089 2024-05-07 15:14:37.346804 physiocurve-2024.5.7/physiocurve/pressure/__pycache__/wrapper.cpython-310.pyc
+-rw-r--r--   0        0        0     3035 2022-07-18 12:09:26.780694 physiocurve-2024.5.7/physiocurve/pressure/__pycache__/wrapper.cpython-38.pyc
+-rw-r--r--   0        0        0     3315 2022-07-14 11:22:26.534074 physiocurve-2024.5.7/physiocurve/pressure/foot.py
+-rw-r--r--   0        0        0     3843 2024-03-29 21:16:23.481865 physiocurve-2024.5.7/physiocurve/pressure/incycle.py
+-rw-r--r--   0        0        0     2392 2024-05-07 15:15:51.835421 physiocurve-2024.5.7/physiocurve/pressure/wrapper.py
+-rw-r--r--   0        0        0      819 2024-05-07 15:16:44.847860 physiocurve-2024.5.7/pyproject.toml
+-rw-r--r--   0        0        0      827 1970-01-01 00:00:00.000000 physiocurve-2024.5.7/PKG-INFO
```

### Comparing `physiocurve-2022.7.8/LICENSE` & `physiocurve-2024.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `physiocurve-2022.7.8/physiocurve/common/__init__.py` & `physiocurve-2024.5.7/physiocurve/common/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+from collections import defaultdict
+
 import numpy as np
 from numba import njit
 
+diagnostics = defaultdict(list)
+
 
 def estimate_samplerate(series):
     # This assumes datetime index
     idx = series.index.view(np.int64)
     intervals = np.diff(idx)
     # 1e9 to account for ns -> Hz
     fs = 1e9 // np.median(intervals)
```

### Comparing `physiocurve-2022.7.8/physiocurve/common/__pycache__/__init__.cpython-38.pyc` & `physiocurve-2024.5.7/physiocurve/common/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu May 12 07:33:19 2022 UTC, .py size: 1081 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,77 @@
-00000000: 550d 0d0a 0000 0000 3fb8 7c62 3904 0000  U.......?.|b9...
+00000000: 550d 0d0a 0000 0000 c5e9 cd62 7f04 0000  U..........b....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
-00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6403 6404 8400 5a04 6405 6406 8400  ..d.d...Z.d.d...
-00000050: 5a05 6503 6407 6408 8400 8301 5a06 6401  Z.e.d.d.....Z.d.
-00000060: 5300 2909 e900 0000 004e 2901 da04 6e6a  S.)......N)...nj
-00000070: 6974 6301 0000 0000 0000 0000 0000 0004  itc.............
-00000080: 0000 0004 0000 0043 0000 0073 3800 0000  .......C...s8...
-00000090: 7c00 6a00 a001 7402 6a03 a101 7d01 7402  |.j...t.j...}.t.
-000000a0: a004 7c01 a101 7d02 6401 7402 a005 7c02  ..|...}.d.t...|.
-000000b0: a101 1a00 7d03 7c03 7402 6a06 6b03 7234  ....}.|.t.j.k.r4
-000000c0: 7c03 5300 6402 5300 2903 4e67 0000 0000  |.S.d.S.).Ng....
-000000d0: 65cd cd41 7201 0000 0029 07da 0569 6e64  e..Ar....)...ind
-000000e0: 6578 da04 7669 6577 da02 6e70 da05 696e  ex..view..np..in
-000000f0: 7436 34da 0464 6966 66da 066d 6564 6961  t64..diff..media
-00000100: 6eda 0369 6e66 2904 da06 7365 7269 6573  n..inf)...series
-00000110: da03 6964 78da 0969 6e74 6572 7661 6c73  ..idx..intervals
-00000120: da02 6673 a900 720e 0000 00fa 3a2f 686f  ..fs..r.....:/ho
-00000130: 6d65 2f6a 616a 2f64 6576 656c 2f70 6879  me/jaj/devel/phy
-00000140: 7369 6f63 7572 7665 2f70 6879 7369 6f63  siocurve/physioc
-00000150: 7572 7665 2f63 6f6d 6d6f 6e2f 5f5f 696e  urve/common/__in
-00000160: 6974 5f5f 2e70 79da 1365 7374 696d 6174  it__.py..estimat
-00000170: 655f 7361 6d70 6c65 7261 7465 0500 0000  e_samplerate....
-00000180: 7308 0000 0000 020e 010a 020e 0172 1000  s............r..
-00000190: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-000001a0: 0000 0004 0000 0003 0000 0073 2000 0000  ...........s ...
-000001b0: 7400 7401 7402 7c00 8302 8301 8900 8700  t.t.t.|.........
-000001c0: 6601 6401 6402 8408 7c00 4400 8301 5300  f.d.d...|.D...S.
-000001d0: 2903 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
-000001e0: 0200 0000 0500 0000 1300 0000 7318 0000  ............s...
-000001f0: 0067 007c 005d 107d 017c 0164 0088 0085  .g.|.].}.|.d....
-00000200: 0219 0091 0271 0453 0029 0172 0100 0000  .....q.S.).r....
-00000210: 720e 0000 0029 02da 022e 30da 0376 6563  r....)....0..vec
-00000220: a901 5a06 6d61 7869 6478 720e 0000 0072  ..Z.maxidxr....r
-00000230: 0f00 0000 da0a 3c6c 6973 7463 6f6d 703e  ......<listcomp>
-00000240: 1100 0000 7304 0000 0006 0002 007a 2074  ....s........z t
-00000250: 7275 6e63 6174 6576 6563 732e 3c6c 6f63  runcatevecs.<loc
-00000260: 616c 733e 2e3c 6c69 7374 636f 6d70 3e29  als>.<listcomp>)
-00000270: 03da 036d 696e da03 6d61 70da 036c 656e  ...min..map..len
-00000280: 2901 da04 7665 6373 720e 0000 0072 1300  )...vecsr....r..
-00000290: 0000 720f 0000 00da 0c74 7275 6e63 6174  ..r......truncat
-000002a0: 6576 6563 730e 0000 0073 0400 0000 0002  evecs....s......
-000002b0: 0e01 7219 0000 0063 0200 0000 0000 0000  ..r....c........
-000002c0: 0000 0000 0900 0000 0500 0000 4300 0000  ............C...
-000002d0: 736e 0000 007c 0164 0118 007c 017c 0164  sn...|.d...|.|.d
-000002e0: 0117 0067 037d 0274 00a0 017c 007c 02a1  ...g.}.t...|.|..
-000002f0: 027d 0374 00a0 027c 03a1 0164 0118 007d  .}.t...|...d...}
-00000300: 047c 0464 026b 0272 387c 0153 007c 017d  .|.d.k.r8|.S.|.}
-00000310: 057c 057c 0417 007d 0674 00a0 017c 007c  .|.|...}.t...|.|
-00000320: 057c 0667 02a1 027d 0774 00a0 027c 07a1  .|.g...}.t...|..
-00000330: 017d 087c 0873 6471 6a7c 067d 0571 3c7c  .}.|.sdqj|.}.q<|
-00000340: 0553 0029 034e e901 0000 0072 0100 0000  .S.).N.....r....
-00000350: 2903 7205 0000 00da 0474 616b 65da 0661  ).r......take..a
-00000360: 7267 6d61 7829 09da 0361 7272 da09 7265  rgmax)...arr..re
-00000370: 6665 7265 6e63 655a 0e73 616d 706c 655f  ferenceZ.sample_
-00000380: 696e 6465 7865 735a 1064 6972 6563 7469  indexesZ.directi
-00000390: 6f6e 5f77 696e 646f 77da 0964 6972 6563  on_window..direc
-000003a0: 7469 6f6e 5a0d 6375 7272 656e 745f 696e  tionZ.current_in
-000003b0: 6465 78da 076e 6578 746c 6f63 5a09 7361  dex..nextlocZ.sa
-000003c0: 6d70 6c65 736f 695a 0c6e 6578 7469 7362  mplesoiZ.nextisb
-000003d0: 6574 7465 7272 0e00 0000 720e 0000 0072  etterr....r....r
-000003e0: 0f00 0000 da0e 6669 6e64 5f6c 6f63 616c  ......find_local
-000003f0: 5f6d 6178 1400 0000 731a 0000 0000 0212  _max....s.......
-00000400: 010c 010e 0108 0204 0104 0208 0110 010a  ................
-00000410: 0104 0202 0106 0172 2100 0000 2907 da05  .......r!...)...
-00000420: 6e75 6d70 7972 0500 0000 da05 6e75 6d62  numpyr......numb
-00000430: 6172 0200 0000 7210 0000 0072 1900 0000  ar....r....r....
-00000440: 7221 0000 0072 0e00 0000 720e 0000 0072  r!...r....r....r
-00000450: 0e00 0000 720f 0000 00da 083c 6d6f 6475  ....r......<modu
-00000460: 6c65 3e01 0000 0073 0a00 0000 0801 0c03  le>....s........
-00000470: 0809 0806 0201                           ......
+00000020: 0003 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
+00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
+00000040: 5a03 6400 6403 6c04 6d05 5a05 0100 6501  Z.d.d.l.m.Z...e.
+00000050: 6506 8301 5a07 6404 6405 8400 5a08 6406  e...Z.d.d...Z.d.
+00000060: 6407 8400 5a09 6505 6408 6409 8400 8301  d...Z.e.d.d.....
+00000070: 5a0a 6402 5300 290a e900 0000 0029 01da  Z.d.S.)......)..
+00000080: 0b64 6566 6175 6c74 6469 6374 4e29 01da  .defaultdictN)..
+00000090: 046e 6a69 7463 0100 0000 0000 0000 0000  .njitc..........
+000000a0: 0000 0400 0000 0400 0000 4300 0000 7338  ..........C...s8
+000000b0: 0000 007c 006a 00a0 0174 026a 03a1 017d  ...|.j...t.j...}
+000000c0: 0174 02a0 047c 01a1 017d 0264 0174 02a0  .t...|...}.d.t..
+000000d0: 057c 02a1 011a 007d 037c 0374 026a 066b  .|.....}.|.t.j.k
+000000e0: 0372 347c 0353 0064 0253 0029 034e 6700  .r4|.S.d.S.).Ng.
+000000f0: 0000 0065 cdcd 4172 0100 0000 2907 da05  ...e..Ar....)...
+00000100: 696e 6465 78da 0476 6965 77da 026e 70da  index..view..np.
+00000110: 0569 6e74 3634 da04 6469 6666 da06 6d65  .int64..diff..me
+00000120: 6469 616e da03 696e 6629 04da 0673 6572  dian..inf)...ser
+00000130: 6965 73da 0369 6478 da09 696e 7465 7276  ies..idx..interv
+00000140: 616c 73da 0266 73a9 0072 0f00 0000 fa3a  als..fs..r.....:
+00000150: 2f68 6f6d 652f 6a61 6a2f 6465 7665 6c2f  /home/jaj/devel/
+00000160: 7068 7973 696f 6375 7276 652f 7068 7973  physiocurve/phys
+00000170: 696f 6375 7276 652f 636f 6d6d 6f6e 2f5f  iocurve/common/_
+00000180: 5f69 6e69 745f 5f2e 7079 da13 6573 7469  _init__.py..esti
+00000190: 6d61 7465 5f73 616d 706c 6572 6174 6509  mate_samplerate.
+000001a0: 0000 0073 0800 0000 0002 0e01 0a02 0e01  ...s............
+000001b0: 7211 0000 0063 0100 0000 0000 0000 0000  r....c..........
+000001c0: 0000 0100 0000 0400 0000 0300 0000 7320  ..............s 
+000001d0: 0000 0074 0074 0174 027c 0083 0283 0189  ...t.t.t.|......
+000001e0: 0087 0066 0164 0164 0284 087c 0044 0083  ...f.d.d...|.D..
+000001f0: 0153 0029 034e 6301 0000 0000 0000 0000  .S.).Nc.........
+00000200: 0000 0002 0000 0005 0000 0013 0000 0073  ...............s
+00000210: 1800 0000 6700 7c00 5d10 7d01 7c01 6400  ....g.|.].}.|.d.
+00000220: 8800 8502 1900 9102 7104 5300 2901 7201  ........q.S.).r.
+00000230: 0000 0072 0f00 0000 2902 da02 2e30 da03  ...r....)....0..
+00000240: 7665 63a9 015a 066d 6178 6964 7872 0f00  vec..Z.maxidxr..
+00000250: 0000 7210 0000 00da 0a3c 6c69 7374 636f  ..r......<listco
+00000260: 6d70 3e15 0000 0073 0400 0000 0600 0200  mp>....s........
+00000270: 7a20 7472 756e 6361 7465 7665 6373 2e3c  z truncatevecs.<
+00000280: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00000290: 703e 2903 da03 6d69 6eda 036d 6170 da03  p>)...min..map..
+000002a0: 6c65 6e29 01da 0476 6563 7372 0f00 0000  len)...vecsr....
+000002b0: 7214 0000 0072 1000 0000 da0c 7472 756e  r....r......trun
+000002c0: 6361 7465 7665 6373 1200 0000 7304 0000  catevecs....s...
+000002d0: 0000 020e 0172 1a00 0000 6302 0000 0000  .....r....c.....
+000002e0: 0000 0000 0000 0009 0000 0005 0000 0043  ...............C
+000002f0: 0000 0073 6e00 0000 7c01 6401 1800 7c01  ...sn...|.d...|.
+00000300: 7c01 6401 1700 6703 7d02 7400 a001 7c00  |.d...g.}.t...|.
+00000310: 7c02 a102 7d03 7400 a002 7c03 a101 6401  |...}.t...|...d.
+00000320: 1800 7d04 7c04 6402 6b02 7238 7c01 5300  ..}.|.d.k.r8|.S.
+00000330: 7c01 7d05 7c05 7c04 1700 7d06 7400 a001  |.}.|.|...}.t...
+00000340: 7c00 7c05 7c06 6702 a102 7d07 7400 a002  |.|.|.g...}.t...
+00000350: 7c07 a101 7d08 7c08 7364 716a 7c06 7d05  |...}.|.sdqj|.}.
+00000360: 713c 7c05 5300 2903 4ee9 0100 0000 7201  q<|.S.).N.....r.
+00000370: 0000 0029 0372 0600 0000 da04 7461 6b65  ...).r......take
+00000380: da06 6172 676d 6178 2909 da03 6172 72da  ..argmax)...arr.
+00000390: 0972 6566 6572 656e 6365 5a0e 7361 6d70  .referenceZ.samp
+000003a0: 6c65 5f69 6e64 6578 6573 5a10 6469 7265  le_indexesZ.dire
+000003b0: 6374 696f 6e5f 7769 6e64 6f77 da09 6469  ction_window..di
+000003c0: 7265 6374 696f 6e5a 0d63 7572 7265 6e74  rectionZ.current
+000003d0: 5f69 6e64 6578 da07 6e65 7874 6c6f 635a  _index..nextlocZ
+000003e0: 0973 616d 706c 6573 6f69 5a0c 6e65 7874  .samplesoiZ.next
+000003f0: 6973 6265 7474 6572 720f 0000 0072 0f00  isbetterr....r..
+00000400: 0000 7210 0000 00da 0e66 696e 645f 6c6f  ..r......find_lo
+00000410: 6361 6c5f 6d61 7818 0000 0073 1a00 0000  cal_max....s....
+00000420: 0002 1201 0c01 0e01 0802 0401 0402 0801  ................
+00000430: 1001 0a01 0402 0201 0601 7222 0000 0029  ..........r"...)
+00000440: 0bda 0b63 6f6c 6c65 6374 696f 6e73 7202  ...collectionsr.
+00000450: 0000 00da 056e 756d 7079 7206 0000 00da  .....numpyr.....
+00000460: 056e 756d 6261 7203 0000 00da 046c 6973  .numbar......lis
+00000470: 745a 0b64 6961 676e 6f73 7469 6373 7211  tZ.diagnosticsr.
+00000480: 0000 0072 1a00 0000 7222 0000 0072 0f00  ...r....r"...r..
+00000490: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+000004a0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+000004b0: 0e00 0000 0c02 0801 0c02 0803 0809 0806  ................
+000004c0: 0201                                     ..
```

### Comparing `physiocurve-2022.7.8/physiocurve/ecg/__pycache__/wrapper.cpython-38.pyc` & `physiocurve-2024.5.7/physiocurve/ecg/__pycache__/wrapper.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sun Jun 26 19:15:11 2022 UTC, .py size: 843 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,71 +1,103 @@
-00000000: 550d 0d0a 0000 0000 3fb0 b862 4b03 0000  U.......?..bK...
+00000000: 550d 0d0a 0000 0000 afe7 cd62 fb04 0000  U..........b....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
+00000020: 0003 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 5a03 4700 6403 6404 8400 6404 8302 5a04  Z.G.d.d...d...Z.
-00000050: 6402 5300 2905 e900 0000 0029 01da 0f63  d.S.)......)...c
-00000060: 6163 6865 645f 7072 6f70 6572 7479 4e63  ached_propertyNc
-00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000080: 0300 0000 4000 0000 7338 0000 0065 005a  ....@...s8...e.Z
-00000090: 0164 005a 0264 0164 0284 005a 0365 0464  .d.Z.d.d...Z.e.d
-000000a0: 0364 0484 0083 015a 0565 0664 0564 0684  .d.....Z.e.d.d..
-000000b0: 0083 015a 0765 0664 0764 0884 0083 015a  ...Z.e.d.d.....Z
-000000c0: 0864 0953 0029 0ada 0345 6367 6303 0000  .d.S.)...Ecgc...
-000000d0: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-000000e0: 0043 0000 0073 1a00 0000 7c02 7c00 5f00  .C...s....|.|._.
-000000f0: 7401 6a02 7c01 7c02 6401 8d02 7c00 5f03  t.j.|.|.d...|._.
-00000100: 6400 5300 2902 4ea9 01da 0d73 616d 706c  d.S.).N....sampl
-00000110: 696e 675f 7261 7465 2904 da0b 5f73 616d  ing_rate)..._sam
-00000120: 706c 6572 6174 65da 026e 6b5a 0965 6367  plerate..nkZ.ecg
-00000130: 5f63 6c65 616e da07 5f76 616c 7565 7329  _clean.._values)
-00000140: 03da 0473 656c 66da 0676 616c 7565 73da  ...self..values.
-00000150: 0a73 616d 706c 6572 6174 65a9 0072 0c00  .samplerate..r..
-00000160: 0000 fa36 2f68 6f6d 652f 6a61 6a2f 6465  ...6/home/jaj/de
-00000170: 7665 6c2f 7068 7973 696f 6375 7276 652f  vel/physiocurve/
-00000180: 7068 7973 696f 6375 7276 652f 6563 672f  physiocurve/ecg/
-00000190: 7772 6170 7065 722e 7079 da08 5f5f 696e  wrapper.py..__in
-000001a0: 6974 5f5f 0700 0000 7304 0000 0000 0106  it__....s.......
-000001b0: 017a 0c45 6367 2e5f 5f69 6e69 745f 5f63  .z.Ecg.__init__c
-000001c0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000001d0: 0100 0000 4300 0000 7306 0000 007c 006a  ....C...s....|.j
-000001e0: 0053 0029 014e 2901 7206 0000 0029 0172  .S.).N).r....).r
-000001f0: 0900 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
-00000200: 0000 0072 0b00 0000 0b00 0000 7302 0000  ...r........s...
-00000210: 0000 027a 0e45 6367 2e73 616d 706c 6572  ...z.Ecg.sampler
-00000220: 6174 6563 0100 0000 0000 0000 0000 0000  atec............
-00000230: 0200 0000 0400 0000 4300 0000 731a 0000  ........C...s...
-00000240: 0074 006a 017c 006a 027c 006a 0364 018d  .t.j.|.j.|.j.d..
-00000250: 027d 017c 0164 0219 0053 0029 034e 7204  .}.|.d...S.).Nr.
-00000260: 0000 005a 0b45 4347 5f52 5f50 6561 6b73  ...Z.ECG_R_Peaks
-00000270: 2904 7207 0000 005a 0d65 6367 5f66 696e  ).r....Z.ecg_fin
-00000280: 6470 6561 6b73 7208 0000 0072 0600 0000  dpeaksr....r....
-00000290: 2902 7209 0000 00da 0469 6e66 6f72 0c00  ).r......infor..
-000002a0: 0000 720c 0000 0072 0d00 0000 da08 6172  ..r....r......ar
-000002b0: 6772 7761 7665 0f00 0000 7304 0000 0000  grwave....s.....
-000002c0: 0212 017a 0c45 6367 2e61 7267 7277 6176  ...z.Ecg.argrwav
-000002d0: 6563 0100 0000 0000 0000 0000 0000 0300  ec..............
-000002e0: 0000 0500 0000 4300 0000 731e 0000 0074  ......C...s....t
-000002f0: 006a 017c 006a 027c 006a 037c 006a 0464  .j.|.j.|.j.|.j.d
-00000300: 018d 035c 027d 017d 027c 0153 0029 024e  ...\.}.}.|.S.).N
-00000310: 2902 5a06 7270 6561 6b73 7205 0000 0029  ).Z.rpeaksr....)
-00000320: 0572 0700 0000 5a0d 6563 675f 6465 6c69  .r....Z.ecg_deli
-00000330: 6e65 6174 6572 0800 0000 7210 0000 0072  neater....r....r
-00000340: 0600 0000 2903 7209 0000 0072 0f00 0000  ....).r....r....
-00000350: da01 5f72 0c00 0000 720c 0000 0072 0d00  .._r....r....r..
-00000360: 0000 da0b 5f6f 7468 6572 7065 616b 7314  ...._otherpeaks.
-00000370: 0000 0073 0c00 0000 0002 0401 0400 0400  ...s............
-00000380: 04ff 0a06 7a0f 4563 672e 5f6f 7468 6572  ....z.Ecg._other
-00000390: 7065 616b 734e 2909 da08 5f5f 6e61 6d65  peaksN)...__name
-000003a0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-000003b0: 5f5f 7175 616c 6e61 6d65 5f5f 720e 0000  __qualname__r...
-000003c0: 00da 0870 726f 7065 7274 7972 0b00 0000  ...propertyr....
-000003d0: 7202 0000 0072 1000 0000 7212 0000 0072  r....r....r....r
-000003e0: 0c00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
-000003f0: 0000 0072 0300 0000 0600 0000 730e 0000  ...r........s...
-00000400: 0008 0108 0402 010a 0302 010a 0402 0172  ...............r
-00000410: 0300 0000 2905 da09 6675 6e63 746f 6f6c  ....)...functool
-00000420: 7372 0200 0000 5a09 6e65 7572 6f6b 6974  sr....Z.neurokit
-00000430: 3272 0700 0000 7203 0000 0072 0c00 0000  2r....r....r....
-00000440: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
-00000450: 083c 6d6f 6475 6c65 3e01 0000 0073 0400  .<module>....s..
-00000460: 0000 0c02 0803                           ......
+00000040: 5a03 6400 6402 6c04 5a05 4700 6403 6404  Z.d.d.l.Z.G.d.d.
+00000050: 8400 6404 8302 5a06 6402 5300 2905 e900  ..d...Z.d.S.)...
+00000060: 0000 0029 01da 0f63 6163 6865 645f 7072  ...)...cached_pr
+00000070: 6f70 6572 7479 4e63 0000 0000 0000 0000  opertyNc........
+00000080: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+00000090: 735c 0000 0065 005a 0164 005a 0264 0164  s\...e.Z.d.Z.d.d
+000000a0: 0284 005a 0365 0464 0364 0484 0083 015a  ...Z.e.d.d.....Z
+000000b0: 0565 0664 0564 0684 0083 015a 0765 0664  .e.d.d.....Z.e.d
+000000c0: 0764 0884 0083 015a 0865 0664 0964 0a84  .d.....Z.e.d.d..
+000000d0: 0083 015a 0965 0664 0b64 0c84 0083 015a  ...Z.e.d.d.....Z
+000000e0: 0a65 0664 0d64 0e84 0083 015a 0b64 0f53  .e.d.d.....Z.d.S
+000000f0: 0029 10da 0345 4347 6303 0000 0000 0000  .)...ECGc.......
+00000100: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
+00000110: 0073 1a00 0000 7c02 7c00 5f00 7401 6a02  .s....|.|._.t.j.
+00000120: 7c01 7c02 6401 8d02 7c00 5f03 6400 5300  |.|.d...|._.d.S.
+00000130: 2902 4ea9 01da 0d73 616d 706c 696e 675f  ).N....sampling_
+00000140: 7261 7465 2904 da0b 5f73 616d 706c 6572  rate)..._sampler
+00000150: 6174 65da 026e 6b5a 0965 6367 5f63 6c65  ate..nkZ.ecg_cle
+00000160: 616e da07 5f76 616c 7565 7329 03da 0473  an.._values)...s
+00000170: 656c 66da 0676 616c 7565 73da 0a73 616d  elf..values..sam
+00000180: 706c 6572 6174 65a9 0072 0c00 0000 fa36  plerate..r.....6
+00000190: 2f68 6f6d 652f 6a61 6a2f 6465 7665 6c2f  /home/jaj/devel/
+000001a0: 7068 7973 696f 6375 7276 652f 7068 7973  physiocurve/phys
+000001b0: 696f 6375 7276 652f 6563 672f 7772 6170  iocurve/ecg/wrap
+000001c0: 7065 722e 7079 da08 5f5f 696e 6974 5f5f  per.py..__init__
+000001d0: 0800 0000 7304 0000 0000 0106 017a 0c45  ....s........z.E
+000001e0: 4347 2e5f 5f69 6e69 745f 5f63 0100 0000  CG.__init__c....
+000001f0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
+00000200: 4300 0000 7306 0000 007c 006a 0053 0029  C...s....|.j.S.)
+00000210: 014e 2901 7206 0000 00a9 0172 0900 0000  .N).r......r....
+00000220: 720c 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
+00000230: 0b00 0000 0c00 0000 7302 0000 0000 027a  ........s......z
+00000240: 0e45 4347 2e73 616d 706c 6572 6174 6563  .ECG.sampleratec
+00000250: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000260: 0400 0000 4300 0000 7310 0000 0074 00a0  ....C...s....t..
+00000270: 017c 006a 0264 0119 00a1 0153 0029 024e  .|.j.d.....S.).N
+00000280: 5a0c 4543 475f 505f 4f6e 7365 7473 a903  Z.ECG_P_Onsets..
+00000290: da02 6e70 5a0b 666c 6174 6e6f 6e7a 6572  ..npZ.flatnonzer
+000002a0: 6fda 0b5f 6f74 6865 7270 6561 6b73 720f  o.._otherpeaksr.
+000002b0: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
+000002c0: 0000 da08 6172 6770 7761 7665 1000 0000  ....argpwave....
+000002d0: 7302 0000 0000 027a 0c45 4347 2e61 7267  s......z.ECG.arg
+000002e0: 7077 6176 6563 0100 0000 0000 0000 0000  pwavec..........
+000002f0: 0000 0200 0000 0400 0000 4300 0000 731a  ..........C...s.
+00000300: 0000 0074 006a 017c 006a 027c 006a 0364  ...t.j.|.j.|.j.d
+00000310: 018d 027d 017c 0164 0219 0053 0029 034e  ...}.|.d...S.).N
+00000320: 7204 0000 005a 0b45 4347 5f52 5f50 6561  r....Z.ECG_R_Pea
+00000330: 6b73 2904 7207 0000 005a 0d65 6367 5f66  ks).r....Z.ecg_f
+00000340: 696e 6470 6561 6b73 7208 0000 0072 0600  indpeaksr....r..
+00000350: 0000 2902 7209 0000 00da 0469 6e66 6f72  ..).r......infor
+00000360: 0c00 0000 720c 0000 0072 0d00 0000 da08  ....r....r......
+00000370: 6172 6772 7761 7665 1400 0000 7304 0000  argrwave....s...
+00000380: 0000 0212 017a 0c45 4347 2e61 7267 7277  .....z.ECG.argrw
+00000390: 6176 6563 0100 0000 0000 0000 0000 0000  avec............
+000003a0: 0100 0000 0400 0000 4300 0000 7310 0000  ........C...s...
+000003b0: 0074 00a0 017c 006a 0264 0119 00a1 0153  .t...|.j.d.....S
+000003c0: 0029 024e 5a0b 4543 475f 545f 5065 616b  .).NZ.ECG_T_Peak
+000003d0: 7372 1000 0000 720f 0000 0072 0c00 0000  sr....r....r....
+000003e0: 720c 0000 0072 0d00 0000 da08 6172 6774  r....r......argt
+000003f0: 7761 7665 1900 0000 7302 0000 0000 027a  wave....s......z
+00000400: 0c45 4347 2e61 7267 7477 6176 6563 0100  .ECG.argtwavec..
+00000410: 0000 0000 0000 0000 0000 0300 0000 0500  ................
+00000420: 0000 4300 0000 731e 0000 0074 006a 017c  ..C...s....t.j.|
+00000430: 006a 027c 006a 037c 006a 0464 018d 035c  .j.|.j.|.j.d...\
+00000440: 027d 017d 027c 0153 0029 024e 2902 5a06  .}.}.|.S.).N).Z.
+00000450: 7270 6561 6b73 7205 0000 0029 0572 0700  rpeaksr....).r..
+00000460: 0000 5a0d 6563 675f 6465 6c69 6e65 6174  ..Z.ecg_delineat
+00000470: 6572 0800 0000 7215 0000 0072 0600 0000  er....r....r....
+00000480: 2903 7209 0000 0072 1400 0000 da01 5f72  ).r....r......_r
+00000490: 0c00 0000 720c 0000 0072 0d00 0000 7212  ....r....r....r.
+000004a0: 0000 001d 0000 0073 0c00 0000 0002 0401  .......s........
+000004b0: 0400 0400 04ff 0a06 7a0f 4543 472e 5f6f  ........z.ECG._o
+000004c0: 7468 6572 7065 616b 7363 0100 0000 0000  therpeaksc......
+000004d0: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
+000004e0: 0000 731e 0000 0074 00a0 017c 006a 02a1  ..s....t...|.j..
+000004f0: 017d 017c 017c 006a 031b 007d 0264 017c  .}.|.|.j...}.d.|
+00000500: 021b 0053 0029 024e e93c 0000 0029 0472  ...S.).N.<...).r
+00000510: 1100 0000 da04 6469 6666 7215 0000 0072  ......diffr....r
+00000520: 0600 0000 2903 7209 0000 005a 0564 6665  ....).r....Z.dfe
+00000530: 6574 5a07 6466 6565 745f 7372 0c00 0000  etZ.dfeet_sr....
+00000540: 720c 0000 0072 0d00 0000 da09 6865 6172  r....r......hear
+00000550: 7472 6174 6527 0000 0073 0600 0000 0002  trate'...s......
+00000560: 0c01 0a02 7a0d 4543 472e 6865 6172 7472  ....z.ECG.heartr
+00000570: 6174 654e 290c da08 5f5f 6e61 6d65 5f5f  ateN)...__name__
+00000580: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000590: 7175 616c 6e61 6d65 5f5f 720e 0000 00da  qualname__r.....
+000005a0: 0870 726f 7065 7274 7972 0b00 0000 7202  .propertyr....r.
+000005b0: 0000 0072 1300 0000 7215 0000 0072 1600  ...r....r....r..
+000005c0: 0000 7212 0000 0072 1a00 0000 720c 0000  ..r....r....r...
+000005d0: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+000005e0: 7203 0000 0007 0000 0073 1a00 0000 0801  r........s......
+000005f0: 0804 0201 0a03 0201 0a03 0201 0a04 0201  ................
+00000600: 0a03 0201 0a09 0201 7203 0000 0029 07da  ........r....)..
+00000610: 0966 756e 6374 6f6f 6c73 7202 0000 005a  .functoolsr....Z
+00000620: 096e 6575 726f 6b69 7432 7207 0000 00da  .neurokit2r.....
+00000630: 056e 756d 7079 7211 0000 0072 0300 0000  .numpyr....r....
+00000640: 720c 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
+00000650: 0d00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000660: 0000 7306 0000 000c 0208 0108 03         ..s..........
```

### Comparing `physiocurve-2022.7.8/physiocurve/ecg/__pycache__/wrapper.cpython-39.pyc` & `physiocurve-2024.5.7/physiocurve/ecg/__pycache__/wrapper.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Jun 26 19:15:11 2022 UTC, .py size: 843 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,71 +1,118 @@
-00000000: 610d 0d0a 0000 0000 3fb0 b862 4b03 0000  a.......?..bK...
+00000000: 6f0d 0d0a 0000 0000 3cbf 3866 d505 0000  o.......<.8f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
+00000020: 0003 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 5a03 4700 6403 6404 8400 6404 8302 5a04  Z.G.d.d...d...Z.
-00000050: 6402 5300 2905 e900 0000 0029 01da 0f63  d.S.)......)...c
-00000060: 6163 6865 645f 7072 6f70 6572 7479 4e63  ached_propertyNc
-00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000080: 0300 0000 4000 0000 7338 0000 0065 005a  ....@...s8...e.Z
-00000090: 0164 005a 0264 0164 0284 005a 0365 0464  .d.Z.d.d...Z.e.d
-000000a0: 0364 0484 0083 015a 0565 0664 0564 0684  .d.....Z.e.d.d..
-000000b0: 0083 015a 0765 0664 0764 0884 0083 015a  ...Z.e.d.d.....Z
-000000c0: 0864 0953 0029 0ada 0345 6367 6303 0000  .d.S.)...Ecgc...
-000000d0: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-000000e0: 0043 0000 0073 1a00 0000 7c02 7c00 5f00  .C...s....|.|._.
-000000f0: 7401 6a02 7c01 7c02 6401 8d02 7c00 5f03  t.j.|.|.d...|._.
-00000100: 6400 5300 2902 4ea9 01da 0d73 616d 706c  d.S.).N....sampl
-00000110: 696e 675f 7261 7465 2904 da0b 5f73 616d  ing_rate)..._sam
-00000120: 706c 6572 6174 65da 026e 6b5a 0965 6367  plerate..nkZ.ecg
-00000130: 5f63 6c65 616e da07 5f76 616c 7565 7329  _clean.._values)
-00000140: 03da 0473 656c 66da 0676 616c 7565 73da  ...self..values.
-00000150: 0a73 616d 706c 6572 6174 65a9 0072 0c00  .samplerate..r..
-00000160: 0000 fa36 2f68 6f6d 652f 6a61 6a2f 6465  ...6/home/jaj/de
-00000170: 7665 6c2f 7068 7973 696f 6375 7276 652f  vel/physiocurve/
-00000180: 7068 7973 696f 6375 7276 652f 6563 672f  physiocurve/ecg/
-00000190: 7772 6170 7065 722e 7079 da08 5f5f 696e  wrapper.py..__in
-000001a0: 6974 5f5f 0700 0000 7304 0000 0000 0106  it__....s.......
-000001b0: 017a 0c45 6367 2e5f 5f69 6e69 745f 5f63  .z.Ecg.__init__c
-000001c0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000001d0: 0100 0000 4300 0000 7306 0000 007c 006a  ....C...s....|.j
-000001e0: 0053 0029 014e 2901 7206 0000 0029 0172  .S.).N).r....).r
-000001f0: 0900 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
-00000200: 0000 0072 0b00 0000 0b00 0000 7302 0000  ...r........s...
-00000210: 0000 027a 0e45 6367 2e73 616d 706c 6572  ...z.Ecg.sampler
-00000220: 6174 6563 0100 0000 0000 0000 0000 0000  atec............
-00000230: 0200 0000 0400 0000 4300 0000 731a 0000  ........C...s...
-00000240: 0074 006a 017c 006a 027c 006a 0364 018d  .t.j.|.j.|.j.d..
-00000250: 027d 017c 0164 0219 0053 0029 034e 7204  .}.|.d...S.).Nr.
-00000260: 0000 005a 0b45 4347 5f52 5f50 6561 6b73  ...Z.ECG_R_Peaks
-00000270: 2904 7207 0000 005a 0d65 6367 5f66 696e  ).r....Z.ecg_fin
-00000280: 6470 6561 6b73 7208 0000 0072 0600 0000  dpeaksr....r....
-00000290: 2902 7209 0000 00da 0469 6e66 6f72 0c00  ).r......infor..
-000002a0: 0000 720c 0000 0072 0d00 0000 da08 6172  ..r....r......ar
-000002b0: 6772 7761 7665 0f00 0000 7304 0000 0000  grwave....s.....
-000002c0: 0212 017a 0c45 6367 2e61 7267 7277 6176  ...z.Ecg.argrwav
-000002d0: 6563 0100 0000 0000 0000 0000 0000 0300  ec..............
-000002e0: 0000 0500 0000 4300 0000 731e 0000 0074  ......C...s....t
-000002f0: 006a 017c 006a 027c 006a 037c 006a 0464  .j.|.j.|.j.|.j.d
-00000300: 018d 035c 027d 017d 027c 0153 0029 024e  ...\.}.}.|.S.).N
-00000310: 2902 5a06 7270 6561 6b73 7205 0000 0029  ).Z.rpeaksr....)
-00000320: 0572 0700 0000 5a0d 6563 675f 6465 6c69  .r....Z.ecg_deli
-00000330: 6e65 6174 6572 0800 0000 7210 0000 0072  neater....r....r
-00000340: 0600 0000 2903 7209 0000 0072 0f00 0000  ....).r....r....
-00000350: da01 5f72 0c00 0000 720c 0000 0072 0d00  .._r....r....r..
-00000360: 0000 da0b 5f6f 7468 6572 7065 616b 7314  ...._otherpeaks.
-00000370: 0000 0073 0800 0000 0002 0401 0cff 0a06  ...s............
-00000380: 7a0f 4563 672e 5f6f 7468 6572 7065 616b  z.Ecg._otherpeak
-00000390: 734e 2909 da08 5f5f 6e61 6d65 5f5f da0a  sN)...__name__..
-000003a0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-000003b0: 616c 6e61 6d65 5f5f 720e 0000 00da 0870  alname__r......p
-000003c0: 726f 7065 7274 7972 0b00 0000 7202 0000  ropertyr....r...
-000003d0: 0072 1000 0000 7212 0000 0072 0c00 0000  .r....r....r....
-000003e0: 720c 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
-000003f0: 0300 0000 0600 0000 730e 0000 0008 0108  ........s.......
-00000400: 0402 010a 0302 010a 0402 0172 0300 0000  ...........r....
-00000410: 2905 da09 6675 6e63 746f 6f6c 7372 0200  )...functoolsr..
-00000420: 0000 5a09 6e65 7572 6f6b 6974 3272 0700  ..Z.neurokit2r..
-00000430: 0000 7203 0000 0072 0c00 0000 720c 0000  ..r....r....r...
-00000440: 0072 0c00 0000 720d 0000 00da 083c 6d6f  .r....r......<mo
-00000450: 6475 6c65 3e01 0000 0073 0400 0000 0c02  dule>....s......
-00000460: 0803                                     ..
+00000040: 5a03 6400 6402 6c04 5a05 4700 6403 6404  Z.d.d.l.Z.G.d.d.
+00000050: 8400 6404 8302 5a06 6402 5300 2905 e900  ..d...Z.d.S.)...
+00000060: 0000 0029 01da 0f63 6163 6865 645f 7072  ...)...cached_pr
+00000070: 6f70 6572 7479 4e63 0000 0000 0000 0000  opertyNc........
+00000080: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+00000090: 7374 0000 0065 005a 0164 005a 0264 0164  st...e.Z.d.Z.d.d
+000000a0: 0284 005a 0365 0464 0364 0484 0083 015a  ...Z.e.d.d.....Z
+000000b0: 0565 0664 0564 0684 0083 015a 0765 0664  .e.d.d.....Z.e.d
+000000c0: 0764 0884 0083 015a 0865 0664 0964 0a84  .d.....Z.e.d.d..
+000000d0: 0083 015a 0965 0664 0b64 0c84 0083 015a  ...Z.e.d.d.....Z
+000000e0: 0a65 0664 0d64 0e84 0083 015a 0b65 0664  .e.d.d.....Z.e.d
+000000f0: 0f64 1084 0083 015a 0c65 0664 1164 1284  .d.....Z.e.d.d..
+00000100: 0083 015a 0d64 1353 0029 14da 0345 4347  ...Z.d.S.)...ECG
+00000110: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
+00000120: 0004 0000 0043 0000 0073 1a00 0000 7c02  .....C...s....|.
+00000130: 7c00 5f00 7401 6a02 7c01 7c02 6401 8d02  |._.t.j.|.|.d...
+00000140: 7c00 5f03 6400 5300 2902 4ea9 01da 0d73  |._.d.S.).N....s
+00000150: 616d 706c 696e 675f 7261 7465 2904 da0b  ampling_rate)...
+00000160: 5f73 616d 706c 6572 6174 65da 026e 6b5a  _samplerate..nkZ
+00000170: 0965 6367 5f63 6c65 616e da07 5f76 616c  .ecg_clean.._val
+00000180: 7565 7329 03da 0473 656c 66da 0676 616c  ues)...self..val
+00000190: 7565 73da 0a73 616d 706c 6572 6174 65a9  ues..samplerate.
+000001a0: 0072 0c00 0000 fa36 2f68 6f6d 652f 6a61  .r.....6/home/ja
+000001b0: 6a2f 6465 7665 6c2f 7068 7973 696f 6375  j/devel/physiocu
+000001c0: 7276 652f 7068 7973 696f 6375 7276 652f  rve/physiocurve/
+000001d0: 6563 672f 7772 6170 7065 722e 7079 da08  ecg/wrapper.py..
+000001e0: 5f5f 696e 6974 5f5f 0800 0000 7304 0000  __init__....s...
+000001f0: 0006 0114 017a 0c45 4347 2e5f 5f69 6e69  .....z.ECG.__ini
+00000200: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
+00000210: 0100 0000 0100 0000 4300 0000 7306 0000  ........C...s...
+00000220: 007c 006a 0053 0029 014e 2901 7206 0000  .|.j.S.).N).r...
+00000230: 00a9 0172 0900 0000 720c 0000 0072 0c00  ...r....r....r..
+00000240: 0000 720d 0000 0072 0b00 0000 0c00 0000  ..r....r........
+00000250: 7302 0000 0006 027a 0e45 4347 2e73 616d  s......z.ECG.sam
+00000260: 706c 6572 6174 6563 0100 0000 0000 0000  pleratec........
+00000270: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+00000280: 731a 0000 0074 006a 017c 006a 027c 006a  s....t.j.|.j.|.j
+00000290: 0364 018d 027d 017c 0164 0219 0053 0029  .d...}.|.d...S.)
+000002a0: 034e 7204 0000 005a 0b45 4347 5f52 5f50  .Nr....Z.ECG_R_P
+000002b0: 6561 6b73 2904 7207 0000 005a 0d65 6367  eaks).r....Z.ecg
+000002c0: 5f66 696e 6470 6561 6b73 7208 0000 0072  _findpeaksr....r
+000002d0: 0600 0000 2902 7209 0000 00da 0469 6e66  ....).r......inf
+000002e0: 6f72 0c00 0000 720c 0000 0072 0d00 0000  or....r....r....
+000002f0: da08 6172 6772 7761 7665 1000 0000 7304  ..argrwave....s.
+00000300: 0000 0012 0208 017a 0c45 4347 2e61 7267  .......z.ECG.arg
+00000310: 7277 6176 6563 0100 0000 0000 0000 0000  rwavec..........
+00000320: 0000 0100 0000 0400 0000 4300 0000 f310  ..........C.....
+00000330: 0000 0074 00a0 017c 006a 0264 0119 00a1  ...t...|.j.d....
+00000340: 0153 0029 024e 5a0c 4543 475f 505f 4f6e  .S.).NZ.ECG_P_On
+00000350: 7365 7473 a903 da02 6e70 5a0b 666c 6174  sets....npZ.flat
+00000360: 6e6f 6e7a 6572 6fda 0b5f 6f74 6865 7270  nonzero.._otherp
+00000370: 6561 6b73 720f 0000 0072 0c00 0000 720c  eaksr....r....r.
+00000380: 0000 0072 0d00 0000 da08 6172 6770 7761  ...r......argpwa
+00000390: 7665 1500 0000 f302 0000 0010 027a 0c45  ve...........z.E
+000003a0: 4347 2e61 7267 7077 6176 6563 0100 0000  CG.argpwavec....
+000003b0: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+000003c0: 4300 0000 7212 0000 0029 024e 5a0b 4543  C...r....).NZ.EC
+000003d0: 475f 515f 5065 616b 7372 1300 0000 720f  G_Q_Peaksr....r.
+000003e0: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
+000003f0: 0000 da08 6172 6771 7761 7665 1900 0000  ....argqwave....
+00000400: 7217 0000 007a 0c45 4347 2e61 7267 7177  r....z.ECG.argqw
+00000410: 6176 6563 0100 0000 0000 0000 0000 0000  avec............
+00000420: 0100 0000 0400 0000 4300 0000 7212 0000  ........C...r...
+00000430: 0029 024e 5a0b 4543 475f 535f 5065 616b  .).NZ.ECG_S_Peak
+00000440: 7372 1300 0000 720f 0000 0072 0c00 0000  sr....r....r....
+00000450: 720c 0000 0072 0d00 0000 da08 6172 6773  r....r......args
+00000460: 7761 7665 1d00 0000 7217 0000 007a 0c45  wave....r....z.E
+00000470: 4347 2e61 7267 7377 6176 6563 0100 0000  CG.argswavec....
+00000480: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+00000490: 4300 0000 7212 0000 0029 024e 5a0b 4543  C...r....).NZ.EC
+000004a0: 475f 545f 5065 616b 7372 1300 0000 720f  G_T_Peaksr....r.
+000004b0: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
+000004c0: 0000 da08 6172 6774 7761 7665 2100 0000  ....argtwave!...
+000004d0: 7217 0000 007a 0c45 4347 2e61 7267 7477  r....z.ECG.argtw
+000004e0: 6176 6563 0100 0000 0000 0000 0000 0000  avec............
+000004f0: 0300 0000 0500 0000 4300 0000 731e 0000  ........C...s...
+00000500: 0074 006a 017c 006a 027c 006a 037c 006a  .t.j.|.j.|.j.|.j
+00000510: 0464 018d 035c 027d 017d 027c 0153 0029  .d...\.}.}.|.S.)
+00000520: 024e 2902 5a06 7270 6561 6b73 7205 0000  .N).Z.rpeaksr...
+00000530: 0029 0572 0700 0000 5a0d 6563 675f 6465  .).r....Z.ecg_de
+00000540: 6c69 6e65 6174 6572 0800 0000 7211 0000  lineater....r...
+00000550: 0072 0600 0000 2903 7209 0000 0072 1000  .r....).r....r..
+00000560: 0000 da01 5f72 0c00 0000 720c 0000 0072  ...._r....r....r
+00000570: 0d00 0000 7215 0000 0025 0000 0073 0800  ....r....%...s..
+00000580: 0000 0402 0c01 0aff 0406 7a0f 4543 472e  ..........z.ECG.
+00000590: 5f6f 7468 6572 7065 616b 7363 0100 0000  _otherpeaksc....
+000005a0: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+000005b0: 4300 0000 731e 0000 0074 00a0 017c 006a  C...s....t...|.j
+000005c0: 02a1 017d 017c 017c 006a 031b 007d 0264  ...}.|.|.j...}.d
+000005d0: 017c 021b 0053 0029 024e e93c 0000 0029  .|...S.).N.<...)
+000005e0: 0472 1400 0000 da04 6469 6666 7211 0000  .r......diffr...
+000005f0: 0072 0600 0000 2903 7209 0000 005a 0564  .r....).r....Z.d
+00000600: 6665 6574 5a07 6466 6565 745f 7372 0c00  feetZ.dfeet_sr..
+00000610: 0000 720c 0000 0072 0d00 0000 da09 6865  ..r....r......he
+00000620: 6172 7472 6174 652f 0000 0073 0600 0000  artrate/...s....
+00000630: 0c02 0a01 0802 7a0d 4543 472e 6865 6172  ......z.ECG.hear
+00000640: 7472 6174 654e 290e da08 5f5f 6e61 6d65  trateN)...__name
+00000650: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000660: 5f5f 7175 616c 6e61 6d65 5f5f 720e 0000  __qualname__r...
+00000670: 00da 0870 726f 7065 7274 7972 0b00 0000  ...propertyr....
+00000680: 7202 0000 0072 1100 0000 7216 0000 0072  r....r....r....r
+00000690: 1800 0000 7219 0000 0072 1a00 0000 7215  ....r....r....r.
+000006a0: 0000 0072 1e00 0000 720c 0000 0072 0c00  ...r....r....r..
+000006b0: 0000 720c 0000 0072 0d00 0000 7203 0000  ..r....r....r...
+000006c0: 0007 0000 0073 2400 0000 0800 0801 0204  .....s$.........
+000006d0: 0a01 0203 0a01 0204 0a01 0203 0a01 0203  ................
+000006e0: 0a01 0203 0a01 0203 0a01 0209 0e01 7203  ..............r.
+000006f0: 0000 0029 07da 0966 756e 6374 6f6f 6c73  ...)...functools
+00000700: 7202 0000 005a 096e 6575 726f 6b69 7432  r....Z.neurokit2
+00000710: 7207 0000 00da 056e 756d 7079 7214 0000  r......numpyr...
+00000720: 0072 0300 0000 720c 0000 0072 0c00 0000  .r....r....r....
+00000730: 720c 0000 0072 0d00 0000 da08 3c6d 6f64  r....r......<mod
+00000740: 756c 653e 0100 0000 7308 0000 000c 0008  ule>....s.......
+00000750: 0208 0112 03                             .....
```

### Comparing `physiocurve-2022.7.8/physiocurve/ecg/wrapper.py` & `physiocurve-2024.5.7/physiocurve/ecg/wrapper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,52 @@
 from functools import cached_property
 
 import neurokit2 as nk
+import numpy as np
 
 
-class Ecg:
+class ECG:
     def __init__(self, values, samplerate):
         self._samplerate = samplerate
         self._values = nk.ecg_clean(values, sampling_rate=samplerate)
 
     @property
     def samplerate(self):
         return self._samplerate
 
     @cached_property
     def argrwave(self):
         info = nk.ecg_findpeaks(self._values, sampling_rate=self._samplerate)
-        return info['ECG_R_Peaks']
+        return info["ECG_R_Peaks"]
+
+    @cached_property
+    def argpwave(self):
+        return np.flatnonzero(self._otherpeaks["ECG_P_Onsets"])
+
+    @cached_property
+    def argqwave(self):
+        return np.flatnonzero(self._otherpeaks["ECG_Q_Peaks"])
+
+    @cached_property
+    def argswave(self):
+        return np.flatnonzero(self._otherpeaks["ECG_S_Peaks"])
+
+    @cached_property
+    def argtwave(self):
+        return np.flatnonzero(self._otherpeaks["ECG_T_Peaks"])
 
     @cached_property
     def _otherpeaks(self):
         info, _ = nk.ecg_delineate(
             self._values, rpeaks=self.argrwave, sampling_rate=self._samplerate
         )
         # ['ECG_P_Peaks', 'ECG_P_Onsets', 'ECG_P_Offsets', 'ECG_Q_Peaks',
         # 'ECG_R_Onsets', 'ECG_R_Offsets', 'ECG_S_Peaks', 'ECG_T_Peaks',
         # 'ECG_T_Onsets', 'ECG_T_Offsets']
         return info
+
+    @cached_property
+    def heartrate(self):
+        dfeet = np.diff(self.argrwave)
+        dfeet_s = dfeet / self._samplerate
+        # Result in beats per minute
+        return 60 / dfeet_s
```

### Comparing `physiocurve-2022.7.8/physiocurve/flow/__pycache__/wrapper.cpython-38.pyc` & `physiocurve-2024.5.7/physiocurve/flow/__pycache__/wrapper.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `physiocurve-2022.7.8/physiocurve/flow/__pycache__/wrapper.cpython-39.pyc` & `physiocurve-2024.5.7/physiocurve/flow/__pycache__/wrapper.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May 12 07:22:55 2022 UTC, .py size: 580 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 cfb5 7c62 4402 0000  a.........|bD...
+00000000: 6f0d 0d0a 0000 0000 cfb5 7c62 4402 0000  o.........|bD...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 8302 5a04 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
 00000060: 01da 0f63 6163 6865 645f 7072 6f70 6572  ...cached_proper
 00000070: 7479 2901 da10 6669 6e64 5f66 6c6f 775f  ty)...find_flow_
@@ -20,53 +20,53 @@
 00000130: 616d 706c 6572 6174 6529 03da 0473 656c  amplerate)...sel
 00000140: 66da 0676 616c 7565 73da 0a73 616d 706c  f..values..sampl
 00000150: 6572 6174 65a9 0072 0b00 0000 fa37 2f68  erate..r.....7/h
 00000160: 6f6d 652f 6a61 6a2f 6465 7665 6c2f 7068  ome/jaj/devel/ph
 00000170: 7973 696f 6375 7276 652f 7068 7973 696f  ysiocurve/physio
 00000180: 6375 7276 652f 666c 6f77 2f77 7261 7070  curve/flow/wrapp
 00000190: 6572 2e70 79da 085f 5f69 6e69 745f 5f07  er.py..__init__.
-000001a0: 0000 0073 0400 0000 0001 0601 7a0d 466c  ...s........z.Fl
+000001a0: 0000 0073 0400 0000 0601 0a01 7a0d 466c  ...s........z.Fl
 000001b0: 6f77 2e5f 5f69 6e69 745f 5f63 0100 0000  ow.__init__c....
 000001c0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
 000001d0: 4300 0000 7306 0000 007c 006a 0053 0072  C...s....|.j.S.r
 000001e0: 0500 0000 2901 7207 0000 00a9 0172 0800  ....).r......r..
 000001f0: 0000 720b 0000 0072 0b00 0000 720c 0000  ..r....r....r...
-00000200: 0072 0a00 0000 0b00 0000 7302 0000 0000  .r........s.....
+00000200: 0072 0a00 0000 0b00 0000 7302 0000 0006  .r........s.....
 00000210: 027a 0f46 6c6f 772e 7361 6d70 6c65 7261  .z.Flow.samplera
 00000220: 7465 6301 0000 0000 0000 0000 0000 0001  tec.............
 00000230: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
 00000240: 7400 7c00 6a01 8301 5300 7205 0000 0029  t.|.j...S.r....)
 00000250: 0272 0300 0000 7206 0000 0072 0e00 0000  .r....r....r....
 00000260: 720b 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
 00000270: 0d5f 6172 6773 7461 7274 7374 6f70 0f00  ._argstartstop..
-00000280: 0000 7302 0000 0000 027a 1246 6c6f 772e  ..s......z.Flow.
+00000280: 0000 7302 0000 000a 027a 1246 6c6f 772e  ..s......z.Flow.
 00000290: 5f61 7267 7374 6172 7473 746f 7063 0100  _argstartstopc..
 000002a0: 0000 0000 0000 0000 0000 0300 0000 0200  ................
 000002b0: 0000 4300 0000 730e 0000 007c 006a 005c  ..C...s....|.j.\
 000002c0: 027d 017d 027c 0153 0072 0500 0000 a901  .}.}.|.S.r......
 000002d0: 720f 0000 0029 0372 0800 0000 da06 7374  r....).r......st
 000002e0: 6172 7473 da01 5f72 0b00 0000 720b 0000  arts.._r....r...
 000002f0: 0072 0c00 0000 da09 6172 6773 7461 7274  .r......argstart
-00000300: 7313 0000 0073 0400 0000 0002 0a01 7a0e  s....s........z.
+00000300: 7313 0000 00f3 0400 0000 0a02 0401 7a0e  s.............z.
 00000310: 466c 6f77 2e61 7267 7374 6172 7473 6301  Flow.argstartsc.
 00000320: 0000 0000 0000 0000 0000 0003 0000 0002  ................
 00000330: 0000 0043 0000 0073 0e00 0000 7c00 6a00  ...C...s....|.j.
 00000340: 5c02 7d01 7d02 7c02 5300 7205 0000 0072  \.}.}.|.S.r....r
 00000350: 1000 0000 2903 7208 0000 0072 1200 0000  ....).r....r....
-00000360: da05 7374 6f70 7372 0b00 0000 720b 0000  ..stopsr....r...
+00000360: 5a05 7374 6f70 7372 0b00 0000 720b 0000  Z.stopsr....r...
 00000370: 0072 0c00 0000 da08 6172 6773 746f 7073  .r......argstops
-00000380: 1800 0000 7304 0000 0000 020a 017a 0d46  ....s........z.F
-00000390: 6c6f 772e 6172 6773 746f 7073 4e29 0ada  low.argstopsN)..
-000003a0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-000003b0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-000003c0: 655f 5f72 0d00 0000 da08 7072 6f70 6572  e__r......proper
-000003d0: 7479 720a 0000 0072 0200 0000 720f 0000  tyr....r....r...
-000003e0: 0072 1300 0000 7215 0000 0072 0b00 0000  .r....r....r....
-000003f0: 720b 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
-00000400: 0400 0000 0600 0000 7312 0000 0008 0108  ........s.......
-00000410: 0402 010a 0302 010a 0302 010a 0402 0172  ...............r
-00000420: 0400 0000 4e29 05da 0966 756e 6374 6f6f  ....N)...functoo
-00000430: 6c73 7202 0000 00da 1070 6879 7369 6f63  lsr......physioc
-00000440: 7572 7665 2e66 6c6f 7772 0300 0000 7204  urve.flowr....r.
-00000450: 0000 0072 0b00 0000 720b 0000 0072 0b00  ...r....r....r..
-00000460: 0000 720c 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000470: 3e01 0000 0073 0400 0000 0c02 0c03       >....s........
+00000380: 1800 0000 7214 0000 007a 0d46 6c6f 772e  ....r....z.Flow.
+00000390: 6172 6773 746f 7073 4e29 0ada 085f 5f6e  argstopsN)...__n
+000003a0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+000003b0: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
+000003c0: 0d00 0000 da08 7072 6f70 6572 7479 720a  ......propertyr.
+000003d0: 0000 0072 0200 0000 720f 0000 0072 1300  ...r....r....r..
+000003e0: 0000 7215 0000 0072 0b00 0000 720b 0000  ..r....r....r...
+000003f0: 0072 0b00 0000 720c 0000 0072 0400 0000  .r....r....r....
+00000400: 0600 0000 7314 0000 0008 0008 0102 040a  ....s...........
+00000410: 0102 030a 0102 030a 0102 040e 0172 0400  .............r..
+00000420: 0000 4e29 05da 0966 756e 6374 6f6f 6c73  ..N)...functools
+00000430: 7202 0000 00da 1070 6879 7369 6f63 7572  r......physiocur
+00000440: 7665 2e66 6c6f 7772 0300 0000 7204 0000  ve.flowr....r...
+00000450: 0072 0b00 0000 720b 0000 0072 0b00 0000  .r....r....r....
+00000460: 720c 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000470: 0000 0073 0600 0000 0c00 0c02 1203       ...s..........
```

### Comparing `physiocurve-2022.7.8/physiocurve/flow/wrapper.py` & `physiocurve-2024.5.7/physiocurve/flow/wrapper.py`

 * *Files identical despite different names*

### Comparing `physiocurve-2022.7.8/physiocurve/pandas/__pycache__/flow.cpython-38.pyc` & `physiocurve-2024.5.7/physiocurve/pandas/__pycache__/flow.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `physiocurve-2022.7.8/physiocurve/pandas/__pycache__/pressure.cpython-38.pyc` & `physiocurve-2024.5.7/physiocurve/pandas/__pycache__/ecg.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sun Jun 26 18:35:06 2022 UTC, .py size: 1036 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,117 +1,96 @@
-00000000: 550d 0d0a 0000 0000 daa6 b862 0c04 0000  U..........b....
+00000000: 550d 0d0a 0000 0000 a50e d062 5303 0000  U..........bS...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a04 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 6504 8303 5a03 6405 5300 2906 e900 0000  e...Z.d.S.).....
 00000060: 0029 01da 1365 7374 696d 6174 655f 7361  .)...estimate_sa
-00000070: 6d70 6c65 7261 7465 2901 da08 5072 6573  mplerate)...Pres
-00000080: 7375 7265 6300 0000 0000 0000 0000 0000  surec...........
-00000090: 0000 0000 0004 0000 0000 0000 0073 7e00  .............s~.
-000000a0: 0000 6500 5a01 6400 5a02 6414 8700 6601  ..e.Z.d.Z.d...f.
-000000b0: 6402 6403 8409 5a03 6504 6404 6405 8400  d.d...Z.e.d.d...
-000000c0: 8301 5a05 6504 6406 6407 8400 8301 5a06  ..Z.e.d.d.....Z.
-000000d0: 6504 6408 6409 8400 8301 5a07 6504 640a  e.d.d.....Z.e.d.
-000000e0: 640b 8400 8301 5a08 6504 640c 640d 8400  d.....Z.e.d.d...
-000000f0: 8301 5a09 6504 640e 640f 8400 8301 5a0a  ..Z.e.d.d.....Z.
-00000100: 6504 6410 6411 8400 8301 5a0b 6504 6412  e.d.d.....Z.e.d.
-00000110: 6413 8400 8301 5a0c 8700 0400 5a0d 5300  d.....Z.....Z.S.
-00000120: 2915 7203 0000 004e 6303 0000 0000 0000  ).r....Nc.......
-00000130: 0000 0000 0003 0000 0004 0000 0003 0000  ................
-00000140: 0073 2c00 0000 7c01 7c00 5f00 7c02 6400  .s,...|.|._.|.d.
-00000150: 6b08 7216 7401 7c01 8301 7d02 7402 8300  k.r.t.|...}.t...
-00000160: a003 7c01 a004 a100 7c02 a102 0100 6400  ..|.....|.....d.
-00000170: 5300 a901 4e29 05da 075f 7365 7269 6573  S...N)..._series
-00000180: 7202 0000 00da 0573 7570 6572 da08 5f5f  r......super..__
-00000190: 696e 6974 5f5f da08 746f 5f6e 756d 7079  init__..to_numpy
-000001a0: 2903 da04 7365 6c66 da06 7365 7269 6573  )...self..series
-000001b0: da0a 7361 6d70 6c65 7261 7465 a901 da09  ..samplerate....
-000001c0: 5f5f 636c 6173 735f 5fa9 00fa 3a2f 686f  __class__...:/ho
-000001d0: 6d65 2f6a 616a 2f64 6576 656c 2f70 6879  me/jaj/devel/phy
-000001e0: 7369 6f63 7572 7665 2f70 6879 7369 6f63  siocurve/physioc
-000001f0: 7572 7665 2f70 616e 6461 732f 7072 6573  urve/pandas/pres
-00000200: 7375 7265 2e70 7972 0700 0000 0600 0000  sure.pyr........
-00000210: 7308 0000 0000 0106 0108 0108 027a 1150  s............z.P
-00000220: 7265 7373 7572 652e 5f5f 696e 6974 5f5f  ressure.__init__
-00000230: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000240: 0002 0000 0043 0000 0073 0e00 0000 7c00  .....C...s....|.
-00000250: 6a00 6a01 7c00 6a02 1900 5300 7204 0000  j.j.|.j...S.r...
-00000260: 0029 0372 0500 0000 da05 696e 6465 78da  .).r......index.
-00000270: 0761 7267 6665 6574 a901 7209 0000 0072  .argfeet..r....r
-00000280: 0e00 0000 720e 0000 0072 0f00 0000 da07  ....r....r......
-00000290: 6964 7866 6565 740d 0000 0073 0200 0000  idxfeet....s....
-000002a0: 0002 7a10 5072 6573 7375 7265 2e69 6478  ..z.Pressure.idx
-000002b0: 6665 6574 6301 0000 0000 0000 0000 0000  feetc...........
-000002c0: 0001 0000 0002 0000 0043 0000 0073 0e00  .........C...s..
-000002d0: 0000 7c00 6a00 6a01 7c00 6a02 1900 5300  ..|.j.j.|.j...S.
-000002e0: 7204 0000 0029 0372 0500 0000 da04 696c  r....).r......il
-000002f0: 6f63 7211 0000 0072 1200 0000 720e 0000  ocr....r....r...
-00000300: 0072 0e00 0000 720f 0000 00da 0466 6565  .r....r......fee
-00000310: 7411 0000 0073 0200 0000 0002 7a0d 5072  t....s......z.Pr
-00000320: 6573 7375 7265 2e66 6565 7463 0100 0000  essure.feetc....
-00000330: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00000340: 4300 0000 730e 0000 007c 006a 006a 017c  C...s....|.j.j.|
-00000350: 006a 0219 0053 0072 0400 0000 2903 7205  .j...S.r....).r.
-00000360: 0000 0072 1000 0000 da06 6172 6764 6961  ...r......argdia
-00000370: 7212 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
-00000380: 0f00 0000 da06 6964 7864 6961 1500 0000  ......idxdia....
-00000390: 7302 0000 0000 027a 0f50 7265 7373 7572  s......z.Pressur
-000003a0: 652e 6964 7864 6961 6301 0000 0000 0000  e.idxdiac.......
-000003b0: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-000003c0: 0073 0e00 0000 7c00 6a00 6a01 7c00 6a02  .s....|.j.j.|.j.
-000003d0: 1900 5300 7204 0000 0029 0372 0500 0000  ..S.r....).r....
-000003e0: 7214 0000 0072 1600 0000 7212 0000 0072  r....r....r....r
-000003f0: 0e00 0000 720e 0000 0072 0f00 0000 da0a  ....r....r......
-00000400: 6469 6173 746f 6c69 6373 1900 0000 7302  diastolics....s.
-00000410: 0000 0000 027a 1350 7265 7373 7572 652e  .....z.Pressure.
-00000420: 6469 6173 746f 6c69 6373 6301 0000 0000  diastolicsc.....
-00000430: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00000440: 0000 0073 0e00 0000 7c00 6a00 6a01 7c00  ...s....|.j.j.|.
-00000450: 6a02 1900 5300 7204 0000 0029 0372 0500  j...S.r....).r..
-00000460: 0000 7210 0000 00da 0661 7267 7379 7372  ..r......argsysr
-00000470: 1200 0000 720e 0000 0072 0e00 0000 720f  ....r....r....r.
-00000480: 0000 00da 0669 6478 7379 731d 0000 0073  .....idxsys....s
-00000490: 0200 0000 0002 7a0f 5072 6573 7375 7265  ......z.Pressure
-000004a0: 2e69 6478 7379 7363 0100 0000 0000 0000  .idxsysc........
-000004b0: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-000004c0: 730e 0000 007c 006a 006a 017c 006a 0219  s....|.j.j.|.j..
-000004d0: 0053 0072 0400 0000 2903 7205 0000 0072  .S.r....).r....r
-000004e0: 1400 0000 7219 0000 0072 1200 0000 720e  ....r....r....r.
-000004f0: 0000 0072 0e00 0000 720f 0000 00da 0973  ...r....r......s
-00000500: 7973 746f 6c69 6373 2100 0000 7302 0000  ystolics!...s...
-00000510: 0000 027a 1250 7265 7373 7572 652e 7379  ...z.Pressure.sy
-00000520: 7374 6f6c 6963 7363 0100 0000 0000 0000  stolicsc........
-00000530: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-00000540: 730e 0000 007c 006a 006a 017c 006a 0219  s....|.j.j.|.j..
-00000550: 0053 0072 0400 0000 2903 7205 0000 0072  .S.r....).r....r
-00000560: 1000 0000 da06 6172 6764 6963 7212 0000  ......argdicr...
-00000570: 0072 0e00 0000 720e 0000 0072 0f00 0000  .r....r....r....
-00000580: da06 6964 7864 6963 2500 0000 7302 0000  ..idxdic%...s...
-00000590: 0000 027a 0f50 7265 7373 7572 652e 6964  ...z.Pressure.id
-000005a0: 7864 6963 6301 0000 0000 0000 0000 0000  xdicc...........
-000005b0: 0001 0000 0002 0000 0043 0000 0073 0e00  .........C...s..
-000005c0: 0000 7c00 6a00 6a01 7c00 6a02 1900 5300  ..|.j.j.|.j...S.
-000005d0: 7204 0000 0029 0372 0500 0000 7214 0000  r....).r....r...
-000005e0: 0072 1c00 0000 7212 0000 0072 0e00 0000  .r....r....r....
-000005f0: 720e 0000 0072 0f00 0000 da09 6469 6372  r....r......dicr
-00000600: 6f74 6963 7329 0000 0073 0200 0000 0002  otics)...s......
-00000610: 7a12 5072 6573 7375 7265 2e64 6963 726f  z.Pressure.dicro
-00000620: 7469 6373 2901 4e29 0eda 085f 5f6e 616d  tics).N)...__nam
-00000630: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000640: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0700  .__qualname__r..
-00000650: 0000 da08 7072 6f70 6572 7479 7213 0000  ....propertyr...
-00000660: 0072 1500 0000 7217 0000 0072 1800 0000  .r....r....r....
-00000670: 721a 0000 0072 1b00 0000 721d 0000 0072  r....r....r....r
-00000680: 1e00 0000 da0d 5f5f 636c 6173 7363 656c  ......__classcel
-00000690: 6c5f 5f72 0e00 0000 720e 0000 0072 0c00  l__r....r....r..
-000006a0: 0000 720f 0000 0072 0300 0000 0500 0000  ..r....r........
-000006b0: 7322 0000 0008 010e 0702 010a 0302 010a  s"..............
-000006c0: 0302 010a 0302 010a 0302 010a 0302 010a  ................
-000006d0: 0302 010a 0302 0172 0300 0000 4e29 05da  .......r....N)..
-000006e0: 1270 6879 7369 6f63 7572 7665 2e63 6f6d  .physiocurve.com
-000006f0: 6d6f 6e72 0200 0000 da14 7068 7973 696f  monr......physio
-00000700: 6375 7276 652e 7072 6573 7375 7265 7203  curve.pressurer.
-00000710: 0000 005a 0a50 7265 7373 7572 654e 7072  ...Z.PressureNpr
-00000720: 0e00 0000 720e 0000 0072 0e00 0000 720f  ....r....r....r.
-00000730: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000740: 0073 0400 0000 0c01 0c03                 .s........
+00000070: 6d70 6c65 7261 7465 2901 da03 4543 4763  mplerate)...ECGc
+00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000090: 0400 0000 0000 0000 7366 0000 0065 005a  ........sf...e.Z
+000000a0: 0164 005a 0264 1087 0066 0164 0264 0384  .d.Z.d...f.d.d..
+000000b0: 095a 0365 0464 0464 0584 0083 015a 0565  .Z.e.d.d.....Z.e
+000000c0: 0464 0664 0784 0083 015a 0665 0464 0864  .d.d.....Z.e.d.d
+000000d0: 0984 0083 015a 0765 0464 0a64 0b84 0083  .....Z.e.d.d....
+000000e0: 015a 0865 0464 0c64 0d84 0083 015a 0965  .Z.e.d.d.....Z.e
+000000f0: 0464 0e64 0f84 0083 015a 0a87 0004 005a  .d.d.....Z.....Z
+00000100: 0b53 0029 1172 0300 0000 4e63 0300 0000  .S.).r....Nc....
+00000110: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00000120: 0300 0000 732c 0000 007c 017c 005f 007c  ....s,...|.|._.|
+00000130: 0264 006b 0872 1674 017c 0183 017d 0274  .d.k.r.t.|...}.t
+00000140: 0283 00a0 037c 01a0 04a1 007c 02a1 0201  .....|.....|....
+00000150: 0064 0053 00a9 014e 2905 da07 5f73 6572  .d.S...N)..._ser
+00000160: 6965 7372 0200 0000 da05 7375 7065 72da  iesr......super.
+00000170: 085f 5f69 6e69 745f 5fda 0874 6f5f 6e75  .__init__..to_nu
+00000180: 6d70 7929 03da 0473 656c 66da 0673 6572  mpy)...self..ser
+00000190: 6965 73da 0a73 616d 706c 6572 6174 65a9  ies..samplerate.
+000001a0: 01da 095f 5f63 6c61 7373 5f5f a900 fa35  ...__class__...5
+000001b0: 2f68 6f6d 652f 6a61 6a2f 6465 7665 6c2f  /home/jaj/devel/
+000001c0: 7068 7973 696f 6375 7276 652f 7068 7973  physiocurve/phys
+000001d0: 696f 6375 7276 652f 7061 6e64 6173 2f65  iocurve/pandas/e
+000001e0: 6367 2e70 7972 0700 0000 0600 0000 7308  cg.pyr........s.
+000001f0: 0000 0000 0106 0108 0108 027a 0c45 4347  ...........z.ECG
+00000200: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
+00000210: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
+00000220: 0000 730e 0000 007c 006a 006a 017c 006a  ..s....|.j.j.|.j
+00000230: 0219 0053 0072 0400 0000 2903 7205 0000  ...S.r....).r...
+00000240: 00da 0569 6e64 6578 da08 6172 6770 7761  ...index..argpwa
+00000250: 7665 a901 7209 0000 0072 0e00 0000 720e  ve..r....r....r.
+00000260: 0000 0072 0f00 0000 da08 6964 7870 7761  ...r......idxpwa
+00000270: 7665 0d00 0000 7302 0000 0000 027a 0c45  ve....s......z.E
+00000280: 4347 2e69 6478 7077 6176 6563 0100 0000  CG.idxpwavec....
+00000290: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+000002a0: 4300 0000 730e 0000 007c 006a 006a 017c  C...s....|.j.j.|
+000002b0: 006a 0219 0053 0072 0400 0000 2903 7205  .j...S.r....).r.
+000002c0: 0000 0072 1000 0000 da08 6172 6772 7761  ...r......argrwa
+000002d0: 7665 7212 0000 0072 0e00 0000 720e 0000  ver....r....r...
+000002e0: 0072 0f00 0000 da08 6964 7872 7761 7665  .r......idxrwave
+000002f0: 1100 0000 7302 0000 0000 027a 0c45 4347  ....s......z.ECG
+00000300: 2e69 6478 7277 6176 6563 0100 0000 0000  .idxrwavec......
+00000310: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
+00000320: 0000 730e 0000 007c 006a 006a 017c 006a  ..s....|.j.j.|.j
+00000330: 0219 0053 0072 0400 0000 2903 7205 0000  ...S.r....).r...
+00000340: 0072 1000 0000 da08 6172 6774 7761 7665  .r......argtwave
+00000350: 7212 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
+00000360: 0f00 0000 da08 6964 7874 7761 7665 1500  ......idxtwave..
+00000370: 0000 7302 0000 0000 027a 0c45 4347 2e69  ..s......z.ECG.i
+00000380: 6478 7477 6176 6563 0100 0000 0000 0000  dxtwavec........
+00000390: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+000003a0: 730e 0000 007c 006a 006a 017c 006a 0219  s....|.j.j.|.j..
+000003b0: 0053 0072 0400 0000 2903 7205 0000 00da  .S.r....).r.....
+000003c0: 0469 6c6f 6372 1100 0000 7212 0000 0072  .ilocr....r....r
+000003d0: 0e00 0000 720e 0000 0072 0f00 0000 da06  ....r....r......
+000003e0: 7077 6176 6573 1900 0000 7302 0000 0000  pwaves....s.....
+000003f0: 027a 0a45 4347 2e70 7761 7665 7363 0100  .z.ECG.pwavesc..
+00000400: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00000410: 0000 4300 0000 730e 0000 007c 006a 006a  ..C...s....|.j.j
+00000420: 017c 006a 0219 0053 0072 0400 0000 2903  .|.j...S.r....).
+00000430: 7205 0000 0072 1800 0000 7214 0000 0072  r....r....r....r
+00000440: 1200 0000 720e 0000 0072 0e00 0000 720f  ....r....r....r.
+00000450: 0000 00da 0672 7761 7665 731d 0000 0073  .....rwaves....s
+00000460: 0200 0000 0002 7a0a 4543 472e 7277 6176  ......z.ECG.rwav
+00000470: 6573 6301 0000 0000 0000 0000 0000 0001  esc.............
+00000480: 0000 0002 0000 0043 0000 0073 0e00 0000  .......C...s....
+00000490: 7c00 6a00 6a01 7c00 6a02 1900 5300 7204  |.j.j.|.j...S.r.
+000004a0: 0000 0029 0372 0500 0000 7218 0000 0072  ...).r....r....r
+000004b0: 1600 0000 7212 0000 0072 0e00 0000 720e  ....r....r....r.
+000004c0: 0000 0072 0f00 0000 da06 7477 6176 6573  ...r......twaves
+000004d0: 2100 0000 7302 0000 0000 027a 0a45 4347  !...s......z.ECG
+000004e0: 2e74 7761 7665 7329 014e 290c da08 5f5f  .twaves).N)...__
+000004f0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00000500: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00000510: 7207 0000 00da 0870 726f 7065 7274 7972  r......propertyr
+00000520: 1300 0000 7215 0000 0072 1700 0000 7219  ....r....r....r.
+00000530: 0000 0072 1a00 0000 721b 0000 00da 0d5f  ...r....r......_
+00000540: 5f63 6c61 7373 6365 6c6c 5f5f 720e 0000  _classcell__r...
+00000550: 0072 0e00 0000 720c 0000 0072 0f00 0000  .r....r....r....
+00000560: 7203 0000 0005 0000 0073 1a00 0000 0801  r........s......
+00000570: 0e07 0201 0a03 0201 0a03 0201 0a03 0201  ................
+00000580: 0a03 0201 0a03 0201 7203 0000 004e 2905  ........r....N).
+00000590: da12 7068 7973 696f 6375 7276 652e 636f  ..physiocurve.co
+000005a0: 6d6d 6f6e 7202 0000 00da 0f70 6879 7369  mmonr......physi
+000005b0: 6f63 7572 7665 2e65 6367 7203 0000 005a  ocurve.ecgr....Z
+000005c0: 0545 4347 4e70 720e 0000 0072 0e00 0000  .ECGNpr....r....
+000005d0: 720e 0000 0072 0f00 0000 da08 3c6d 6f64  r....r......<mod
+000005e0: 756c 653e 0100 0000 7304 0000 000c 010c  ule>....s.......
+000005f0: 03                                       .
```

### Comparing `physiocurve-2022.7.8/physiocurve/pandas/flow.py` & `physiocurve-2024.5.7/physiocurve/pandas/flow.py`

 * *Files identical despite different names*

### Comparing `physiocurve-2022.7.8/physiocurve/pandas/pressure.py` & `physiocurve-2024.5.7/physiocurve/pandas/pressure.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,57 @@
+import numpy as np
 from physiocurve.common import estimate_samplerate
 from physiocurve.pressure import Pressure as PressureNp
 
 
 class Pressure(PressureNp):
     def __init__(self, series, samplerate=None):
         self._series = series
         if samplerate is None:
             samplerate = estimate_samplerate(series)
 
         super().__init__(series.to_numpy(), samplerate)
 
     @property
     def idxfeet(self):
-        return self._series.index[self.argfeet]
+        locs = np.ma.masked_equal(self.argfeet, 0)
+        return self._series.index[locs]
 
     @property
     def feet(self):
-        return self._series.iloc[self.argfeet]
+        return self._series.loc[self.idxfeet]
+
+    @property
+    def idxtanfeet(self):
+        locs = np.ma.masked_equal(self.argtanfeet, 0)
+        return self._series.index[locs]
+
+    @property
+    def tanfeet(self):
+        return self._series.loc[self.idxtanfeet]
 
     @property
     def idxdia(self):
-        return self._series.index[self.argdia]
+        locs = np.ma.masked_equal(self.argdia, 0)
+        return self._series.index[locs]
 
     @property
     def diastolics(self):
-        return self._series.iloc[self.argdia]
+        return self._series.loc[self.idxdia]
 
     @property
     def idxsys(self):
-        return self._series.index[self.argsys]
+        locs = np.ma.masked_equal(self.argsys, 0)
+        return self._series.index[locs]
 
     @property
     def systolics(self):
-        return self._series.iloc[self.argsys]
+        return self._series.loc[self.idxsys]
 
     @property
     def idxdic(self):
-        return self._series.index[self.argdic]
+        locs = np.ma.masked_equal(self.argdic, 0)
+        return self._series.index[locs]
 
     @property
     def dicrotics(self):
-        return self._series.iloc[self.argdic]
+        return self._series.loc[self.idxdic]
```

### Comparing `physiocurve-2022.7.8/physiocurve/ppg/__pycache__/wrapper.cpython-38.pyc` & `physiocurve-2024.5.7/physiocurve/ppg/__pycache__/wrapper.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sun Apr  3 19:50:10 2022 UTC, .py size: 227 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,42 @@
-00000000: 550d 0d0a 0000 0000 72fa 4962 e300 0000  U.......r.Ib....
+00000000: 6f0d 0d0a 0000 0000 0a77 c862 d000 0000  o........w.b....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 8303 5a02 6404 5300 2905  ..d.e...Z.d.S.).
 00000050: e900 0000 0029 01da 0850 7265 7373 7572  .....)...Pressur
 00000060: 6563 0000 0000 0000 0000 0000 0000 0000  ec..............
-00000070: 0000 0400 0000 0000 0000 7326 0000 0065  ..........s&...e
-00000080: 005a 0164 005a 0264 0687 0066 0164 0264  .Z.d.Z.d...f.d.d
-00000090: 0384 095a 0364 0464 0584 005a 0487 0004  ...Z.d.d...Z....
-000000a0: 005a 0553 0029 07da 0350 5047 4e63 0400  .Z.S.)...PPGNc..
-000000b0: 0000 0000 0000 0000 0000 0400 0000 0500  ................
-000000c0: 0000 0300 0000 7314 0000 0074 0083 00a0  ......s....t....
-000000d0: 017c 017c 027c 03a1 0301 0064 0053 00a9  .|.|.|.....d.S..
-000000e0: 014e 2902 da05 7375 7065 72da 085f 5f69  .N)...super..__i
-000000f0: 6e69 745f 5f29 04da 0473 656c 66da 0676  nit__)...self..v
-00000100: 616c 7565 73da 0a73 616d 706c 6572 6174  alues..samplerat
-00000110: 65da 0569 6e64 6578 a901 da09 5f5f 636c  e..index....__cl
-00000120: 6173 735f 5fa9 00fa 362f 686f 6d65 2f6a  ass__...6/home/j
-00000130: 616a 2f64 6576 656c 2f70 6879 7369 6f63  aj/devel/physioc
-00000140: 7572 7665 2f70 6879 7369 6f63 7572 7665  urve/physiocurve
-00000150: 2f70 7067 2f77 7261 7070 6572 2e70 7972  /ppg/wrapper.pyr
-00000160: 0600 0000 0500 0000 7302 0000 0000 017a  ........s......z
-00000170: 0c50 5047 2e5f 5f69 6e69 745f 5f63 0100  .PPG.__init__c..
-00000180: 0000 0000 0000 0000 0000 0100 0000 0100  ................
-00000190: 0000 4300 0000 7308 0000 0074 0082 0164  ..C...s....t...d
-000001a0: 0053 0072 0400 0000 2901 da13 4e6f 7449  .S.r....)...NotI
-000001b0: 6d70 6c65 6d65 6e74 6564 4572 726f 7229  mplementedError)
-000001c0: 0172 0700 0000 720d 0000 0072 0d00 0000  .r....r....r....
-000001d0: 720e 0000 00da 0373 7169 0800 0000 7302  r......sqi....s.
-000001e0: 0000 0000 017a 0750 5047 2e73 7169 2901  .....z.PPG.sqi).
-000001f0: 4e29 06da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
-00000200: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00000210: 6c6e 616d 655f 5f72 0600 0000 7210 0000  lname__r....r...
-00000220: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
-00000230: 720d 0000 0072 0d00 0000 720b 0000 0072  r....r....r....r
-00000240: 0e00 0000 7203 0000 0004 0000 0073 0400  ....r........s..
-00000250: 0000 0801 0e03 7203 0000 004e 2903 da14  ......r....N)...
-00000260: 7068 7973 696f 6375 7276 652e 7072 6573  physiocurve.pres
-00000270: 7375 7265 7202 0000 0072 0300 0000 720d  surer....r....r.
-00000280: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-00000290: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-000002a0: 7302 0000 000c 03                        s......
+00000070: 0000 0300 0000 0000 0000 7324 0000 0065  ..........s$...e
+00000080: 005a 0164 005a 0287 0066 0164 0164 0284  .Z.d.Z...f.d.d..
+00000090: 085a 0364 0364 0484 005a 0487 0004 005a  .Z.d.d...Z.....Z
+000000a0: 0553 0029 05da 0350 5047 6303 0000 0000  .S.)...PPGc.....
+000000b0: 0000 0000 0000 0003 0000 0004 0000 0003  ................
+000000c0: 0000 0073 1200 0000 7400 8300 a001 7c01  ...s....t.....|.
+000000d0: 7c02 a102 0100 6400 5300 a901 4e29 02da  |.....d.S...N)..
+000000e0: 0573 7570 6572 da08 5f5f 696e 6974 5f5f  .super..__init__
+000000f0: 2903 da04 7365 6c66 da06 7661 6c75 6573  )...self..values
+00000100: da0a 7361 6d70 6c65 7261 7465 a901 da09  ..samplerate....
+00000110: 5f5f 636c 6173 735f 5fa9 00fa 362f 686f  __class__...6/ho
+00000120: 6d65 2f6a 616a 2f64 6576 656c 2f70 6879  me/jaj/devel/phy
+00000130: 7369 6f63 7572 7665 2f70 6879 7369 6f63  siocurve/physioc
+00000140: 7572 7665 2f70 7067 2f77 7261 7070 6572  urve/ppg/wrapper
+00000150: 2e70 7972 0600 0000 0500 0000 7302 0000  .pyr........s...
+00000160: 0012 017a 0c50 5047 2e5f 5f69 6e69 745f  ...z.PPG.__init_
+00000170: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
+00000180: 0000 0100 0000 4300 0000 7304 0000 0074  ......C...s....t
+00000190: 0082 0172 0400 0000 2901 da13 4e6f 7449  ...r....)...NotI
+000001a0: 6d70 6c65 6d65 6e74 6564 4572 726f 7229  mplementedError)
+000001b0: 0172 0700 0000 720c 0000 0072 0c00 0000  .r....r....r....
+000001c0: 720d 0000 00da 0373 7169 0800 0000 7302  r......sqi....s.
+000001d0: 0000 0004 017a 0750 5047 2e73 7169 2906  .....z.PPG.sqi).
+000001e0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+000001f0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000200: 6d65 5f5f 7206 0000 0072 0f00 0000 da0d  me__r....r......
+00000210: 5f5f 636c 6173 7363 656c 6c5f 5f72 0c00  __classcell__r..
+00000220: 0000 720c 0000 0072 0a00 0000 720d 0000  ..r....r....r...
+00000230: 0072 0300 0000 0400 0000 7306 0000 0008  .r........s.....
+00000240: 000c 0110 0372 0300 0000 4e29 03da 1470  .....r....N)...p
+00000250: 6879 7369 6f63 7572 7665 2e70 7265 7373  hysiocurve.press
+00000260: 7572 6572 0200 0000 7203 0000 0072 0c00  urer....r....r..
+00000270: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+00000280: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000290: 0400 0000 0c00 1403                      ........
```

### Comparing `physiocurve-2022.7.8/physiocurve/pressure/__pycache__/foot.cpython-38.pyc` & `physiocurve-2024.5.7/physiocurve/pressure/__pycache__/foot.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu May 12 07:39:42 2022 UTC, .py size: 1786 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,126 +1,191 @@
-00000000: 550d 0d0a 0000 0000 beb9 7c62 fa06 0000  U.........|b....
+00000000: 6f0d 0d0a 0000 0000 72fc cf62 f30c 0000  o.......r..b....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
+00000020: 0004 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6503 6403 6404 8d01 6405 6406 8400  ..e.d.d...d.d...
-00000050: 8301 5a04 6503 6411 6407 6408 8401 8301  ..Z.e.d.d.d.....
-00000060: 5a05 6503 6412 6409 640a 8401 8301 5a06  Z.e.d.d.d.....Z.
-00000070: 6503 6403 6404 8d01 6413 640d 640e 8401  e.d.d...d.d.d...
-00000080: 8301 5a07 6503 6403 6404 8d01 640f 6410  ..Z.e.d.d...d.d.
-00000090: 8400 8301 5a08 6401 5300 2914 e900 0000  ....Z.d.S.).....
-000000a0: 004e 2901 da04 6e6a 6974 5429 01da 0870  .N)...njitT)...p
-000000b0: 6172 616c 6c65 6c63 0200 0000 0000 0000  arallelc........
-000000c0: 0000 0000 0b00 0000 0700 0000 4300 0000  ............C...
-000000d0: 73b0 0000 0074 00a0 017c 0064 01a1 027d  s....t...|.d...}
-000000e0: 0274 00a0 027c 0274 006a 03a1 027d 0274  .t...|.t.j...}.t
-000000f0: 00a0 017c 0264 01a1 027d 0374 00a0 027c  ...|.d...}.t...|
-00000100: 0374 006a 03a1 027d 037c 037c 0264 026b  .t.j...}.|.|.d.k
-00000110: 0414 007d 0374 047c 037c 0183 025c 027d  ...}.t.|.|...\.}
-00000120: 047d 0574 0564 0364 0484 007c 047c 0566  .}.t.d.d...|.|.f
-00000130: 0244 0083 0183 017d 0674 006a 067c 0674  .D.....}.t.j.|.t
-00000140: 006a 0764 058d 027d 0774 087c 0683 0144  .j.d...}.t.|...D
-00000150: 005d 2e7d 087c 047c 0819 007d 097c 057c  .].}.|.|...}.|.|
-00000160: 0819 007d 0a7c 0974 00a0 097c 037c 097c  ...}.|.t...|.|.|
-00000170: 0a85 0219 00a1 0117 007c 077c 083c 0071  .........|.|.<.q
-00000180: 7c7c 0753 0029 064e e901 0000 0072 0100  ||.S.).N.....r..
-00000190: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-000001a0: 0000 0004 0000 0053 0000 0073 1400 0000  .......S...s....
-000001b0: 6700 7c00 5d0c 7d01 7400 7c01 8301 9102  g.|.].}.t.|.....
-000001c0: 7104 5300 a900 2901 da03 6c65 6e29 02da  q.S...)...len)..
-000001d0: 022e 30da 0178 7205 0000 0072 0500 0000  ..0..xr....r....
-000001e0: fa38 2f68 6f6d 652f 6a61 6a2f 6465 7665  .8/home/jaj/deve
-000001f0: 6c2f 7068 7973 696f 6375 7276 652f 7068  l/physiocurve/ph
-00000200: 7973 696f 6375 7276 652f 7072 6573 7375  ysiocurve/pressu
-00000210: 7265 2f66 6f6f 742e 7079 da0a 3c6c 6973  re/foot.py..<lis
-00000220: 7463 6f6d 703e 0d00 0000 7304 0000 0006  tcomp>....s.....
-00000230: 0002 007a 2666 696e 645f 7072 6573 7375  ...z&find_pressu
-00000240: 7265 5f66 6565 742e 3c6c 6f63 616c 733e  re_feet.<locals>
-00000250: 2e3c 6c69 7374 636f 6d70 3e29 01da 0564  .<listcomp>)...d
-00000260: 7479 7065 290a da02 6e70 da04 6469 6666  type)...np..diff
-00000270: da06 6170 7065 6e64 da03 6e61 6eda 1373  ..append..nan..s
-00000280: 6c69 6469 6e67 5f73 6561 7263 685f 7a6f  liding_search_zo
-00000290: 6973 da03 6d69 6eda 0565 6d70 7479 da05  is..min..empty..
-000002a0: 696e 7436 34da 0572 616e 6765 da06 6172  int64..range..ar
-000002b0: 676d 6178 290b da06 7661 6c75 6573 da0a  gmax)...values..
-000002c0: 7361 6d70 6c65 7261 7465 5a08 6673 7464  samplerateZ.fstd
-000002d0: 6572 6976 5a08 736e 6464 6572 6976 da0c  erivZ.sndderiv..
-000002e0: 7269 7369 6e67 5374 6172 7473 da0b 7269  risingStarts..ri
-000002f0: 7369 6e67 5374 6f70 735a 066f 7574 6c65  singStopsZ.outle
-00000300: 6eda 066f 7574 6172 72da 0169 da05 7374  n..outarr..i..st
-00000310: 6172 74da 0473 746f 7072 0500 0000 7205  art..stopr....r.
-00000320: 0000 0072 0900 0000 da12 6669 6e64 5f70  ...r......find_p
-00000330: 7265 7373 7572 655f 6665 6574 0500 0000  ressure_feet....
-00000340: 731a 0000 0000 020c 010e 010c 010e 010c  s...............
-00000350: 010e 0116 0110 010c 0108 0108 011c 0172  ...............r
-00000360: 1e00 0000 6304 0000 0000 0000 0000 0000  ....c...........
-00000370: 0007 0000 0006 0000 0043 0000 0073 4800  .........C...sH.
-00000380: 0000 7400 7c00 8301 7c01 1800 6401 1700  ..t.|...|...d...
-00000390: 7d04 7401 a002 7400 7c00 8301 a101 7d05  }.t...t.|.....}.
-000003a0: 7403 7c04 8301 4400 5d1c 7d06 7c02 7c00  t.|...D.].}.|.|.
-000003b0: 7c06 7c06 7c01 1700 8502 1900 8301 7c05  |.|.|.........|.
-000003c0: 7c06 3c00 7126 7c05 5300 2902 4e72 0400  |.<.q&|.S.).Nr..
-000003d0: 0000 2904 7206 0000 0072 0c00 0000 7212  ..).r....r....r.
-000003e0: 0000 0072 1400 0000 2907 da01 61da 0177  ...r....)...a..w
-000003f0: da01 66da 0663 656e 7465 72da 016e da03  ..f..center..n..
-00000400: 6275 6672 1b00 0000 7205 0000 0072 0500  bufr....r....r..
-00000410: 0000 7209 0000 00da 0972 6f6c 6c5f 7769  ..r......roll_wi
-00000420: 7468 1600 0000 730a 0000 0000 0210 020e  th....s.........
-00000430: 010c 011a 0172 2500 0000 6303 0000 0000  .....r%...c.....
-00000440: 0000 0000 0000 0006 0000 0007 0000 0043  ...............C
-00000450: 0000 0073 4c00 0000 7400 7c00 8301 7c01  ...sL...t.|...|.
-00000460: 1800 6401 1700 7d03 7401 a002 7400 7c00  ..d...}.t...t.|.
-00000470: 8301 a101 7d04 7403 7c03 8301 4400 5d20  ....}.t.|...D.] 
-00000480: 7d05 7401 a004 7c00 7c05 7c05 7c01 1700  }.t...|.|.|.|...
-00000490: 8502 1900 6402 a102 7c04 7c05 3c00 7126  ....d...|.|.<.q&
-000004a0: 7c04 5300 2903 4e72 0400 0000 6766 6666  |.S.).Nr....gfff
-000004b0: 6666 66e6 3f29 0572 0600 0000 720c 0000  fff.?).r....r...
-000004c0: 0072 1200 0000 7214 0000 00da 0b6e 616e  .r....r......nan
-000004d0: 7175 616e 7469 6c65 2906 721f 0000 0072  quantile).r....r
-000004e0: 2000 0000 7222 0000 0072 2300 0000 7224   ...r"...r#...r$
-000004f0: 0000 0072 1b00 0000 7205 0000 0072 0500  ...r....r....r..
-00000500: 0000 7209 0000 00da 0b72 6f6c 6c5f 7175  ..r......roll_qu
-00000510: 616e 7437 2000 0000 730a 0000 0000 0210  ant7 ...s.......
-00000520: 020e 010c 011e 0172 2700 0000 e904 0000  .......r'.......
-00000530: 00e9 0300 0000 6304 0000 0000 0000 0000  ......c.........
-00000540: 0000 000d 0000 0005 0000 0043 0000 0073  ...........C...s
-00000550: 8200 0000 7c01 7c02 1a00 7d04 7400 7c01  ....|.|...}.t.|.
-00000560: 7c03 1400 8301 7d05 7c00 6401 1300 7d06  |.....}.|.d...}.
-00000570: 7401 7c06 7c04 7402 6a03 8303 7d07 7404  t.|.|.t.j...}.t.
-00000580: 7c07 7c05 8302 7d08 7c07 7c08 6b04 7d09  |.|...}.|.|.k.}.
-00000590: 7402 a005 7c09 a006 7402 6a07 a101 a101  t...|...t.j.....
-000005a0: 7d0a 7402 a008 7c0a 6402 6b04 a101 7d0b  }.t...|.d.k...}.
-000005b0: 7402 a008 7c0a 6402 6b00 a101 7d0c 7c0c  t...|.d.k...}.|.
-000005c0: 7c0c 7c0b 6402 1900 6b04 1900 7d0c 7c0b  |.|.d...k...}.|.
-000005d0: 7c0c 6602 5300 2903 4ee9 0200 0000 7201  |.f.S.).N.....r.
-000005e0: 0000 0029 09da 0369 6e74 7225 0000 0072  ...)...intr%...r
-000005f0: 0c00 0000 da06 6e61 6e73 756d 7227 0000  ......nansumr'..
-00000600: 0072 0d00 0000 da06 6173 7479 7065 da04  .r......astype..
-00000610: 696e 7438 da0b 666c 6174 6e6f 6e7a 6572  int8..flatnonzer
-00000620: 6f29 0d72 1f00 0000 7217 0000 005a 0773  o).r....r....Z.s
-00000630: 756d 636f 6566 5a09 7175 616e 7463 6f65  umcoefZ.quantcoe
-00000640: 665a 0677 696e 7375 6d5a 0877 696e 7175  fZ.winsumZ.winqu
-00000650: 616e 74da 0273 71da 0869 6e74 6567 7261  ant..sq..integra
-00000660: 6c5a 0574 6872 6573 5a07 7269 7369 6e67  lZ.thresZ.rising
-00000670: 735a 0972 6973 696e 6776 6172 7218 0000  sZ.risingvarr...
-00000680: 0072 1900 0000 7205 0000 0072 0500 0000  .r....r....r....
-00000690: 7209 0000 0072 1000 0000 2a00 0000 7316  r....r....*...s.
-000006a0: 0000 0000 0208 010c 0108 010e 010a 0108  ................
-000006b0: 0112 010e 010e 0110 0172 1000 0000 6302  .........r....c.
-000006c0: 0000 0000 0000 0000 0000 0004 0000 0003  ................
-000006d0: 0000 0043 0000 0073 1a00 0000 7400 a001  ...C...s....t...
-000006e0: 7c00 a101 7d02 7c02 7c01 1b00 7d03 6401  |...}.|.|...}.d.
-000006f0: 7c03 1b00 5300 2902 4ee9 3c00 0000 2902  |...S.).N.<...).
-00000700: 720c 0000 0072 0d00 0000 2904 5a07 6665  r....r....).Z.fe
-00000710: 6574 6964 7872 1700 0000 5a05 6466 6565  etidxr....Z.dfee
-00000720: 745a 0764 6665 6574 5f73 7205 0000 0072  tZ.dfeet_sr....r
-00000730: 0500 0000 7209 0000 00da 0e63 616c 635f  ....r......calc_
-00000740: 6865 6172 7472 6174 6539 0000 0073 0600  heartrate9...s..
-00000750: 0000 0002 0a01 0802 7233 0000 0029 0154  ........r3...).T
-00000760: 2901 5429 0272 2800 0000 7229 0000 0029  ).T).r(...r)...)
-00000770: 09da 056e 756d 7079 720c 0000 00da 056e  ...numpyr......n
-00000780: 756d 6261 7202 0000 0072 1e00 0000 7225  umbar....r....r%
-00000790: 0000 0072 2700 0000 7210 0000 0072 3300  ...r'...r....r3.
-000007a0: 0000 7205 0000 0072 0500 0000 7205 0000  ..r....r....r...
-000007b0: 0072 0900 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-000007c0: 0100 0000 7316 0000 0008 010c 0308 010a  ....s...........
-000007d0: 1002 010c 0902 010c 0908 010c 0e08 01    ...............
+00000040: 0100 6503 6403 6404 8400 8301 5a04 6503  ..e.d.d.....Z.e.
+00000050: 6405 6406 8400 8301 5a05 6503 6407 6408  d.d.....Z.e.d.d.
+00000060: 8400 8301 5a06 6503 6413 640b 640c 8401  ....Z.e.d.d.d...
+00000070: 8301 5a07 640d 640e 8400 5a08 640f 6410  ..Z.d.d...Z.d.d.
+00000080: 8400 5a09 6411 6412 8400 5a0a 6401 5300  ..Z.d.d...Z.d.S.
+00000090: 2914 e900 0000 004e 2901 da04 6e6a 6974  )......N)...njit
+000000a0: 6302 0000 0000 0000 0000 0000 000b 0000  c...............
+000000b0: 0007 0000 0043 0000 0073 b000 0000 7400  .....C...s....t.
+000000c0: a001 7c00 6401 a102 7d02 7400 a002 7c02  ..|.d...}.t...|.
+000000d0: 7400 6a03 a102 7d02 7400 a001 7c02 6401  t.j...}.t...|.d.
+000000e0: a102 7d03 7400 a002 7c03 7400 6a03 a102  ..}.t...|.t.j...
+000000f0: 7d03 7c03 7c02 6402 6b04 1400 7d03 7404  }.|.|.d.k...}.t.
+00000100: 7c03 7c01 8302 5c02 7d04 7d05 7405 6403  |.|...\.}.}.t.d.
+00000110: 6404 8400 7c04 7c05 6602 4400 8301 8301  d...|.|.f.D.....
+00000120: 7d06 7400 6a06 7c06 7400 6a07 6405 8d02  }.t.j.|.t.j.d...
+00000130: 7d07 7408 7c06 8301 4400 5d17 7d08 7c04  }.t.|...D.].}.|.
+00000140: 7c08 1900 7d09 7c05 7c08 1900 7d0a 7c09  |...}.|.|...}.|.
+00000150: 7400 a009 7c03 7c09 7c0a 8502 1900 a101  t...|.|.|.......
+00000160: 1700 7c07 7c08 3c00 713e 7c07 5300 2906  ..|.|.<.q>|.S.).
+00000170: 4ee9 0100 0000 7201 0000 0063 0100 0000  N.....r....c....
+00000180: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00000190: 5300 0000 f314 0000 0067 007c 005d 067d  S........g.|.].}
+000001a0: 0174 007c 0183 0191 0271 0253 00a9 00a9  .t.|.....q.S....
+000001b0: 01da 036c 656e a902 da02 2e30 da01 7872  ...len.....0..xr
+000001c0: 0500 0000 7205 0000 00fa 382f 686f 6d65  ....r.....8/home
+000001d0: 2f6a 616a 2f64 6576 656c 2f70 6879 7369  /jaj/devel/physi
+000001e0: 6f63 7572 7665 2f70 6879 7369 6f63 7572  ocurve/physiocur
+000001f0: 7665 2f70 7265 7373 7572 652f 666f 6f74  ve/pressure/foot
+00000200: 2e70 79da 0a3c 6c69 7374 636f 6d70 3e10  .py..<listcomp>.
+00000210: 0000 00f3 0200 0000 1400 7a28 6669 6e64  ..........z(find
+00000220: 5f64 6572 6976 6174 6976 655f 6665 6574  _derivative_feet
+00000230: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00000240: 6f6d 703e a901 da05 6474 7970 6529 0ada  omp>....dtype)..
+00000250: 026e 70da 0464 6966 66da 0661 7070 656e  .np..diff..appen
+00000260: 64da 036e 616e da13 736c 6964 696e 675f  d..nan..sliding_
+00000270: 7365 6172 6368 5f7a 6f69 73da 036d 696e  search_zois..min
+00000280: da05 7a65 726f 73da 0569 6e74 3634 da05  ..zeros..int64..
+00000290: 7261 6e67 65da 0661 7267 6d61 7829 0bda  range..argmax)..
+000002a0: 0676 616c 7565 73da 0a73 616d 706c 6572  .values..sampler
+000002b0: 6174 655a 0866 7374 6465 7269 765a 0873  ateZ.fstderivZ.s
+000002c0: 6e64 6465 7269 76da 0c72 6973 696e 6753  ndderiv..risingS
+000002d0: 7461 7274 73da 0b72 6973 696e 6753 746f  tarts..risingSto
+000002e0: 7073 da06 6f75 746c 656e da06 6f75 7461  ps..outlen..outa
+000002f0: 7272 da01 69da 0573 7461 7274 da04 7374  rr..i..start..st
+00000300: 6f70 7205 0000 0072 0500 0000 720b 0000  opr....r....r...
+00000310: 00da 1466 696e 645f 6465 7269 7661 7469  ...find_derivati
+00000320: 7665 5f66 6565 7408 0000 0073 1a00 0000  ve_feet....s....
+00000330: 0c02 0e01 0c01 0e01 0c01 0e01 1601 1001  ................
+00000340: 0c01 0801 0801 1c01 0401 7223 0000 0063  ..........r#...c
+00000350: 0200 0000 0000 0000 0000 0000 0500 0000  ................
+00000360: 0700 0000 4300 0000 734a 0000 0074 007c  ....C...sJ...t.|
+00000370: 0083 017c 0118 0064 0117 007d 0274 01a0  ...|...d...}.t..
+00000380: 0274 007c 0083 01a1 017d 0374 037c 0283  .t.|.....}.t.|..
+00000390: 0144 005d 0f7d 0474 01a0 047c 007c 047c  .D.].}.t...|.|.|
+000003a0: 047c 0117 0085 0219 00a1 017c 037c 043c  .|.........|.|.<
+000003b0: 0071 137c 0353 0029 024e 7203 0000 0029  .q.|.S.).Nr....)
+000003c0: 0572 0700 0000 7210 0000 0072 1600 0000  .r....r....r....
+000003d0: 7218 0000 00da 066e 616e 7375 6da9 05da  r......nansum...
+000003e0: 0161 da01 77da 016e da03 6275 6672 2000  .a..w..n..bufr .
+000003f0: 0000 7205 0000 0072 0500 0000 720b 0000  ..r....r....r...
+00000400: 00da 0872 6f6c 6c5f 7375 6d19 0000 0073  ...roll_sum....s
+00000410: 0a00 0000 1002 0e01 0c01 1c01 0401 722a  ..............r*
+00000420: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00000430: 0500 0000 0700 0000 4300 0000 734c 0000  ........C...sL..
+00000440: 0074 007c 0083 017c 0118 0064 0117 007d  .t.|...|...d...}
+00000450: 0274 01a0 0274 007c 0083 01a1 017d 0374  .t...t.|.....}.t
+00000460: 037c 0283 0144 005d 107d 0474 01a0 047c  .|...D.].}.t...|
+00000470: 007c 047c 047c 0117 0085 0219 0064 02a1  .|.|.|.......d..
+00000480: 027c 037c 043c 0071 137c 0353 0029 034e  .|.|.<.q.|.S.).N
+00000490: 7203 0000 0067 6666 6666 6666 e63f 2905  r....gffffff.?).
+000004a0: 7207 0000 0072 1000 0000 7216 0000 0072  r....r....r....r
+000004b0: 1800 0000 da0b 6e61 6e71 7561 6e74 696c  ......nanquantil
+000004c0: 6572 2500 0000 7205 0000 0072 0500 0000  er%...r....r....
+000004d0: 720b 0000 00da 0b72 6f6c 6c5f 7175 616e  r......roll_quan
+000004e0: 7437 2200 0000 730a 0000 0010 020e 010c  t7"...s.........
+000004f0: 011e 0104 0172 2c00 0000 e904 0000 00e9  .....r,.........
+00000500: 0300 0000 6304 0000 0000 0000 0000 0000  ....c...........
+00000510: 000d 0000 0005 0000 0043 0000 0073 7e00  .........C...s~.
+00000520: 0000 7c01 7c02 1a00 7d04 7400 7c01 7c03  ..|.|...}.t.|.|.
+00000530: 1400 8301 7d05 7c00 6401 1300 7d06 7401  ....}.|.d...}.t.
+00000540: 7c06 7c04 8302 7d07 7402 7c07 7c05 8302  |.|...}.t.|.|...
+00000550: 7d08 7c07 7c08 6b04 7d09 7403 a004 7c09  }.|.|.k.}.t...|.
+00000560: a005 7403 6a06 a101 a101 7d0a 7403 a007  ..t.j.....}.t...
+00000570: 7c0a 6402 6b04 a101 7d0b 7403 a007 7c0a  |.d.k...}.t...|.
+00000580: 6402 6b00 a101 7d0c 7c0c 7c0c 7c0b 6402  d.k...}.|.|.|.d.
+00000590: 1900 6b04 1900 7d0c 7c0b 7c0c 6602 5300  ..k...}.|.|.f.S.
+000005a0: 2903 4ee9 0200 0000 7201 0000 0029 08da  ).N.....r....)..
+000005b0: 0369 6e74 722a 0000 0072 2c00 0000 7210  .intr*...r,...r.
+000005c0: 0000 0072 1100 0000 da06 6173 7479 7065  ...r......astype
+000005d0: da04 696e 7438 da0b 666c 6174 6e6f 6e7a  ..int8..flatnonz
+000005e0: 6572 6f29 0d72 2600 0000 721b 0000 005a  ero).r&...r....Z
+000005f0: 0773 756d 636f 6566 5a09 7175 616e 7463  .sumcoefZ.quantc
+00000600: 6f65 665a 0677 696e 7375 6d5a 0877 696e  oefZ.winsumZ.win
+00000610: 7175 616e 74da 0273 71da 0869 6e74 6567  quant..sq..integ
+00000620: 7261 6c5a 0574 6872 6573 5a07 7269 7369  ralZ.thresZ.risi
+00000630: 6e67 735a 0972 6973 696e 6776 6172 721c  ngsZ.risingvarr.
+00000640: 0000 0072 1d00 0000 7205 0000 0072 0500  ...r....r....r..
+00000650: 0000 720b 0000 0072 1400 0000 2b00 0000  ..r....r....+...
+00000660: 7316 0000 0008 020c 0108 010a 010a 0108  s...............
+00000670: 0112 010e 010e 0110 0108 0172 1400 0000  ...........r....
+00000680: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
+00000690: 0006 0000 0043 0000 0073 1a00 0000 7400  .....C...s....t.
+000006a0: a001 7402 7c00 7c01 7c02 8303 a101 a003  ..t.|.|.|.......
+000006b0: 7400 6a04 a101 5300 2901 4e29 0572 1000  t.j...S.).N).r..
+000006c0: 0000 da04 7269 6e74 da1a 6669 6e64 5f74  ....rint..find_t
+000006d0: 616e 6765 6e74 5f69 6e74 6572 7365 6374  angent_intersect
+000006e0: 696f 6e73 7231 0000 0072 1700 0000 2903  ionsr1...r....).
+000006f0: 721a 0000 00da 0661 7267 6469 61da 0661  r......argdia..a
+00000700: 7267 7379 7372 0500 0000 7205 0000 0072  rgsysr....r....r
+00000710: 0b00 0000 da11 6669 6e64 5f74 616e 6765  ......find_tange
+00000720: 6e74 5f66 6565 743c 0000 0073 0200 0000  nt_feet<...s....
+00000730: 1a01 723a 0000 0063 0300 0000 0000 0000  ..r:...c........
+00000740: 0000 0000 0e00 0000 0600 0000 4300 0000  ............C...
+00000750: 73a0 0000 0074 0064 0164 0284 007c 017c  s....t.d.d...|.|
+00000760: 0266 0244 0083 0183 017d 0374 016a 027c  .f.D.....}.t.j.|
+00000770: 0374 016a 0364 038d 027d 0474 01a0 047c  .t.j.d...}.t...|
+00000780: 0064 04a1 027d 0574 01a0 057c 0574 016a  .d...}.t...|.t.j
+00000790: 06a1 027d 0574 01a0 077c 017c 0266 02a1  ...}.t...|.|.f..
+000007a0: 017d 0674 087c 0683 0144 005d 225c 027d  .}.t.|...D.]"\.}
+000007b0: 075c 027d 087d 0974 097c 007c 057c 087c  .\.}.}.t.|.|.|.|
+000007c0: 0983 045c 027d 0a7d 0b7c 0a64 056b 0272  ...\.}.}.|.d.k.r
+000007d0: 3f71 2b7c 007c 0819 007d 0c7c 0c7c 0b18  ?q+|.|...}.|.|..
+000007e0: 007c 0a1b 007d 0d7c 0d7c 047c 073c 0071  .|...}.|.|.|.<.q
+000007f0: 2b7c 0453 0029 064e 6301 0000 0000 0000  +|.S.).Nc.......
+00000800: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
+00000810: 0072 0400 0000 7205 0000 0072 0600 0000  .r....r....r....
+00000820: 7208 0000 0072 0500 0000 7205 0000 0072  r....r....r....r
+00000830: 0b00 0000 720c 0000 0042 0000 0072 0d00  ....r....B...r..
+00000840: 0000 7a2e 6669 6e64 5f74 616e 6765 6e74  ..z.find_tangent
+00000850: 5f69 6e74 6572 7365 6374 696f 6e73 2e3c  _intersections.<
+00000860: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00000870: 703e 720e 0000 0072 0300 0000 7201 0000  p>r....r....r...
+00000880: 0029 0a72 1500 0000 7210 0000 0072 1600  .).r....r....r..
+00000890: 0000 da07 666c 6f61 7436 3472 1100 0000  ....float64r....
+000008a0: 7212 0000 0072 1300 0000 da0c 636f 6c75  r....r......colu
+000008b0: 6d6e 5f73 7461 636b da09 656e 756d 6572  mn_stack..enumer
+000008c0: 6174 65da 0c63 616c 635f 7461 6e67 656e  ate..calc_tangen
+000008d0: 7429 0e72 1a00 0000 7238 0000 0072 3900  t).r....r8...r9.
+000008e0: 0000 721e 0000 0072 1f00 0000 da05 6465  ..r....r......de
+000008f0: 7269 765a 0f73 6c6f 7065 5f69 6e74 6572  rivZ.slope_inter
+00000900: 7661 6c73 7220 0000 00da 0664 6961 6964  valsr .....diaid
+00000910: 78da 0673 7973 6964 78da 0573 6c6f 7065  x..sysidx..slope
+00000920: da09 7461 6e67 656e 745f 625a 0464 6961  ..tangent_bZ.dia
+00000930: 795a 0666 6f6f 745f 7872 0500 0000 7205  yZ.foot_xr....r.
+00000940: 0000 0072 0b00 0000 7237 0000 0041 0000  ...r....r7...A..
+00000950: 0073 1a00 0000 1601 1001 0c02 0e01 0e02  .s..............
+00000960: 1402 1201 0801 0201 0801 0c01 0a01 0405  ................
+00000970: 7237 0000 0063 0400 0000 0000 0000 0000  r7...c..........
+00000980: 0000 0c00 0000 0500 0000 4300 0000 73a2  ..........C...s.
+00000990: 0000 007c 0264 016b 0273 087c 0364 016b  ...|.d.k.s.|.d.k
+000009a0: 0272 0a64 0253 007c 017c 027c 0385 0219  .r.d.S.|.|.|....
+000009b0: 007d 0474 007c 0483 0164 016b 0272 1864  .}.t.|...d.k.r.d
+000009c0: 0253 0074 01a0 027c 04a1 017d 0574 016a  .S.t...|...}.t.j
+000009d0: 037c 0564 0318 007c 0564 0417 0064 0564  .|.d...|.d...d.d
+000009e0: 068d 037d 0674 016a 047c 047c 0664 0764  ...}.t.j.|.|.d.d
+000009f0: 088d 037d 077c 027c 06a0 05a1 0017 007d  ...}.|.|.......}
+00000a00: 0874 016a 047c 007c 027c 0617 0064 0764  .t.j.|.|.|...d.d
+00000a10: 088d 03a0 05a1 007d 097c 07a0 05a1 007d  .......}.|.....}
+00000a20: 0a7c 097c 0a7c 0814 0018 007d 0b7c 0a7c  .|.|.|.....}.|.|
+00000a30: 0b66 0253 0029 094e 7201 0000 0029 0272  .f.S.).Nr....).r
+00000a40: 0100 0000 7201 0000 0072 2f00 0000 722e  ....r....r/...r.
+00000a50: 0000 0072 0300 0000 2901 da04 7374 6570  ...r....)...step
+00000a60: da04 636c 6970 2901 da04 6d6f 6465 2906  ..clip)...mode).
+00000a70: 7207 0000 0072 1000 0000 7219 0000 00da  r....r....r.....
+00000a80: 0661 7261 6e67 65da 0474 616b 65da 046d  .arange..take..m
+00000a90: 6561 6e29 0c72 1a00 0000 723f 0000 005a  ean).r....r?...Z
+00000aa0: 0c62 6567 5f69 6e74 6572 7661 6cda 0c65  .beg_interval..e
+00000ab0: 6e64 5f69 6e74 6572 7661 6c5a 0c64 6572  nd_intervalZ.der
+00000ac0: 6976 5f73 616d 706c 655a 0d6d 6178 5f73  iv_sampleZ.max_s
+00000ad0: 6c6f 7065 5f69 6478 5a11 6465 7269 765f  lope_idxZ.deriv_
+00000ae0: 7375 6273 616d 706c 655f 785a 1164 6572  subsample_xZ.der
+00000af0: 6976 5f73 7562 7361 6d70 6c65 5f79 5a09  iv_subsample_yZ.
+00000b00: 7461 6e67 656e 745f 785a 0974 616e 6765  tangent_xZ.tange
+00000b10: 6e74 5f79 7242 0000 0072 4300 0000 7205  nt_yrB...rC...r.
+00000b20: 0000 0072 0500 0000 720b 0000 0072 3e00  ...r....r....r>.
+00000b30: 0000 5900 0000 731a 0000 0010 0104 010c  ..Y...s.........
+00000b40: 010c 0104 010a 0218 0310 010c 0218 0108  ................
+00000b50: 020c 0108 0272 3e00 0000 2902 722d 0000  .....r>...).r-..
+00000b60: 0072 2e00 0000 290b da05 6e75 6d70 7972  .r....)...numpyr
+00000b70: 1000 0000 da05 6e75 6d62 6172 0200 0000  ......numbar....
+00000b80: 7223 0000 0072 2a00 0000 722c 0000 0072  r#...r*...r,...r
+00000b90: 1400 0000 723a 0000 0072 3700 0000 723e  ....r:...r7...r>
+00000ba0: 0000 0072 0500 0000 7205 0000 0072 0500  ...r....r....r..
+00000bb0: 0000 720b 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000bc0: 3e01 0000 0073 1a00 0000 0800 0c01 0206  >....s..........
+00000bd0: 0a01 0210 0a01 0208 0a01 0208 0c01 0810  ................
+00000be0: 0805 0c18                                ....
```

### Comparing `physiocurve-2022.7.8/physiocurve/pressure/__pycache__/incycle.cpython-38.pyc` & `physiocurve-2024.5.7/physiocurve/pressure/__pycache__/incycle.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sun Jun 26 19:27:22 2022 UTC, .py size: 4554 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,223 +1,187 @@
-00000000: 550d 0d0a 0000 0000 1ab3 b862 ca11 0000  U..........b....
+00000000: 6f0d 0d0a 0000 0000 a72f 0766 030f 0000  o......../.f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
-00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6403 6404 8400 5a04 6405 6406 8400  ..d.d...Z.d.d...
-00000050: 5a05 6407 6408 8400 5a06 6409 640a 8400  Z.d.d...Z.d.d...
-00000060: 5a07 640b 640c 8400 5a08 6412 640e 640f  Z.d.d...Z.d.d.d.
-00000070: 8401 5a09 6410 6411 8400 5a0a 6401 5300  ..Z.d.d...Z.d.S.
-00000080: 2913 e900 0000 004e 2901 da04 666f 6f74  )......N)...foot
-00000090: 6302 0000 0000 0000 0000 0000 0006 0000  c...............
-000000a0: 0004 0000 0043 0000 0073 3400 0000 7400  .....C...s4...t.
-000000b0: a001 7c00 7c01 a102 7d02 7402 7c00 7c01  ..|.|...}.t.|.|.
-000000c0: 7c02 8303 5c02 7d03 7d04 7403 7c00 7c03  |...\.}.}.t.|.|.
-000000d0: 7c04 8303 7d05 7c02 7c03 7c04 7c05 6704  |...}.|.|.|.|.g.
-000000e0: 5300 a901 4e29 0472 0200 0000 da12 6669  S...N).r......fi
-000000f0: 6e64 5f70 7265 7373 7572 655f 6665 6574  nd_pressure_feet
-00000100: da0c 6669 6e64 5f64 6961 5f73 7973 da0e  ..find_dia_sys..
-00000110: 6669 6e64 5f64 6963 726f 7469 6373 2906  find_dicrotics).
-00000120: da06 7661 6c75 6573 da0a 7361 6d70 6c65  ..values..sample
-00000130: 7261 7465 da07 6665 6574 6964 78da 0664  rate..feetidx..d
-00000140: 6961 6964 78da 0673 7973 6964 785a 0664  iaidx..sysidxZ.d
-00000150: 6963 6964 78a9 0072 0c00 0000 fa3b 2f68  icidx..r.....;/h
-00000160: 6f6d 652f 6a61 6a2f 6465 7665 6c2f 7068  ome/jaj/devel/ph
-00000170: 7973 696f 6375 7276 652f 7068 7973 696f  ysiocurve/physio
-00000180: 6375 7276 652f 7072 6573 7375 7265 2f69  curve/pressure/i
-00000190: 6e63 7963 6c65 2e70 79da 1266 696e 645f  ncycle.py..find_
-000001a0: 7072 6573 7375 7265 5f66 756c 6c05 0000  pressure_full...
-000001b0: 0073 0800 0000 0001 0c01 1001 0c01 720e  .s............r.
-000001c0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-000001d0: 0900 0000 0600 0000 4300 0000 736a 0000  ........C...sj..
-000001e0: 007c 0164 0064 0185 0219 007d 027c 0164  .|.d.d.....}.|.d
-000001f0: 0264 0085 0219 007d 0374 007c 0183 0164  .d.....}.t.|...d
-00000200: 0218 007d 0474 016a 027c 0474 016a 0364  ...}.t.j.|.t.j.d
-00000210: 038d 027d 0574 0474 057c 027c 0383 0283  ...}.t.t.|.|....
-00000220: 0144 005d 225c 027d 065c 027d 077d 0874  .D.]"\.}.\.}.}.t
-00000230: 01a0 067c 007c 077c 0885 0219 00a1 017c  ...|.|.|.......|
-00000240: 057c 063c 0071 427c 0553 0029 044e e9ff  .|.<.qB|.S.).N..
-00000250: ffff ffe9 0100 0000 a901 da05 6474 7970  ............dtyp
-00000260: 6529 07da 036c 656e da02 6e70 da05 7a65  e)...len..np..ze
-00000270: 726f 73da 0566 6c6f 6174 da09 656e 756d  ros..float..enum
-00000280: 6572 6174 65da 037a 6970 da07 6e61 6e6d  erate..zip..nanm
-00000290: 6561 6e29 0972 0700 0000 720a 0000 00da  ean).r....r.....
-000002a0: 0873 7461 7274 6964 78da 0665 6e64 6964  .startidx..endid
-000002b0: 78da 076e 7661 6c75 6573 da05 6d65 616e  x..nvalues..mean
-000002c0: 73da 0169 da05 7374 6172 74da 0473 746f  s..i..start..sto
-000002d0: 7072 0c00 0000 720c 0000 0072 0d00 0000  pr....r....r....
-000002e0: da0a 6361 6c63 5f6d 6561 6e73 0c00 0000  ..calc_means....
-000002f0: 730e 0000 0000 010c 010c 010c 0110 011a  s...............
-00000300: 0118 0172 2100 0000 6303 0000 0000 0000  ...r!...c.......
-00000310: 0000 0000 000e 0000 0008 0000 0043 0000  .............C..
-00000320: 0073 a800 0000 7c02 6401 6402 8502 1900  .s....|.d.d.....
-00000330: 7d03 7c02 6403 6400 8502 1900 7d04 7400  }.|.d.d.....}.t.
-00000340: 6404 7c01 1400 8301 7d05 7401 7c03 8301  d.|.....}.t.|...
-00000350: 7d06 7402 6a03 7c06 7402 6a04 6405 8d02  }.t.j.|.t.j.d...
-00000360: 7d07 7402 6a03 7c06 7402 6a04 6405 8d02  }.t.j.|.t.j.d...
-00000370: 7d08 7405 7406 7c03 7c04 8302 8301 4400  }.t.t.|.|.....D.
-00000380: 5d44 5c02 7d09 5c02 7d0a 7d0b 7c0b 7c0a  ]D\.}.\.}.}.|.|.
-00000390: 1800 7d0c 7c0a 7c0c 1800 7d0d 7407 7c00  ..}.|.|...}.t.|.
-000003a0: 7c0a 7c0d 7c05 8304 7c07 7c09 3c00 7407  |.|.|...|.|.<.t.
-000003b0: 7c00 7c0a 7c0b 7c05 6406 6407 8d05 7c08  |.|.|.|.d.d...|.
-000003c0: 7c09 3c00 715a 7c07 7c08 6602 5300 2908  |.<.qZ|.|.f.S.).
-000003d0: 4e72 0100 0000 720f 0000 0072 1000 0000  Nr....r....r....
-000003e0: 679a 9999 9999 99a9 3f72 1100 0000 5429  g.......?r....T)
-000003f0: 01da 0973 6561 7263 686d 6178 2908 da03  ...searchmax)...
-00000400: 696e 7472 1300 0000 7214 0000 0072 1500  intr....r....r..
-00000410: 0000 da05 696e 7436 3472 1700 0000 7218  ....int64r....r.
-00000420: 0000 00da 1266 696e 645f 6c6f 6361 6c5f  .....find_local_
-00000430: 6578 7472 656d 6529 0e72 0700 0000 7208  extreme).r....r.
-00000440: 0000 0072 0900 0000 da06 7374 6172 7473  ...r......starts
-00000450: da05 7374 6f70 73da 0a77 696e 646f 7773  ..stops..windows
-00000460: 697a 6572 1c00 0000 da03 6469 61da 0373  izer......dia..s
-00000470: 7973 721e 0000 0072 1f00 0000 7220 0000  ysr....r....r ..
-00000480: 00da 0864 7572 6174 696f 6e5a 0764 6961  ...durationZ.dia
-00000490: 7374 6f70 720c 0000 0072 0c00 0000 720d  stopr....r....r.
-000004a0: 0000 0072 0500 0000 1700 0000 7318 0000  ...r........s...
-000004b0: 0000 010c 010c 010c 0108 0110 0110 011a  ................
-000004c0: 0108 0108 0112 0118 0172 0500 0000 6303  .........r....c.
-000004d0: 0000 0000 0000 0000 0000 0003 0000 0005  ................
-000004e0: 0000 0043 0000 0073 1400 0000 7400 a001  ...C...s....t...
-000004f0: 7c01 7c00 1800 7c02 7c00 1800 a102 5300  |.|...|.|.....S.
-00000500: 7203 0000 0029 0272 1400 0000 da05 6372  r....).r......cr
-00000510: 6f73 7329 03da 026c 31da 026c 32da 0170  oss)...l1..l2..p
-00000520: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
-00000530: 0864 6973 7461 6e63 6527 0000 0073 0200  .distance'...s..
-00000540: 0000 0001 7230 0000 0063 0300 0000 0000  ....r0...c......
-00000550: 0000 0000 0000 0f00 0000 0600 0000 4300  ..............C.
-00000560: 0000 73f8 0000 0074 007c 0183 0144 005d  ..s....t.|...D.]
-00000570: 185c 027d 037d 047c 047c 0264 0119 006b  .\.}.}.|.|.d...k
-00000580: 0472 0801 0071 3071 0874 016a 0264 0174  .r...q0q.t.j.d.t
-00000590: 0364 028d 0253 007c 017c 0364 0085 0219  .d...S.|.|.d....
-000005a0: 007d 0174 047c 0183 017d 0574 016a 057c  .}.t.|...}.t.j.|
-000005b0: 0574 016a 0664 028d 027d 0674 0074 077c  .t.j.d...}.t.t.|
-000005c0: 017c 0283 0283 0144 005d 905c 027d 075c  .|.....D.].\.}.\
-000005d0: 027d 087d 097c 007c 097c 0885 0219 007d  .}.}.|.|.|.....}
-000005e0: 0a74 047c 0a83 0173 8471 6274 01a0 0864  .t.|...s.qbt...d
-000005f0: 017c 0a64 0119 0067 02a1 017d 0b74 01a0  .|.d...g...}.t..
-00000600: 087c 087c 0918 007c 0a64 0319 0067 02a1  .|.|...|.d...g..
-00000610: 017d 0c74 01a0 0974 047c 0a83 01a1 017d  .}.t...t.|.....}
-00000620: 0d74 01a0 0a7c 0d7c 0a66 02a1 016a 0b7d  .t...|.|.f...j.}
-00000630: 0e74 0c7c 0b7c 0c7c 0e83 037d 0474 047c  .t.|.|.|...}.t.|
-00000640: 0483 0173 e071 627c 0974 01a0 0d7c 04a1  ...s.qb|.t...|..
-00000650: 0117 007c 067c 073c 0071 627c 0653 0029  ...|.|.<.qb|.S.)
-00000660: 044e 7201 0000 0072 1100 0000 720f 0000  .Nr....r....r...
-00000670: 0029 0e72 1700 0000 7214 0000 00da 0565  .).r....r......e
-00000680: 6d70 7479 7223 0000 0072 1300 0000 7215  mptyr#...r....r.
-00000690: 0000 0072 2400 0000 7218 0000 00da 0561  ...r$...r......a
-000006a0: 7272 6179 da06 6172 616e 6765 da06 7673  rray..arange..vs
-000006b0: 7461 636b da01 5472 3000 0000 da06 6172  tack..Tr0.....ar
-000006c0: 676d 696e 290f 7207 0000 0072 0a00 0000  gmin).r....r....
-000006d0: 720b 0000 00da 016e da01 6472 1c00 0000  r......n..dr....
-000006e0: da04 6469 6373 721e 0000 00da 0264 69da  ..dicsr......di.
-000006f0: 0273 695a 037a 6f69 da02 7031 da02 7032  .siZ.zoi..p1..p2
-00000700: 5a06 7a6f 6969 6478 da02 7033 720c 0000  Z.zoiidx..p3r...
-00000710: 0072 0c00 0000 720d 0000 0072 0600 0000  .r....r....r....
-00000720: 2c00 0000 7328 0000 0000 0210 010c 0106  ,...s(..........
-00000730: 030e 010c 0208 0110 011a 010c 0108 0102  ................
-00000740: 0112 0116 050e 0110 020c 0108 0102 0114  ................
-00000750: 0372 0600 0000 4663 0500 0000 0000 0000  .r....Fc........
-00000760: 0000 0000 1400 0000 0400 0000 4300 0000  ............C...
-00000770: 7328 0100 007c 0472 2074 006a 017d 0574  s(...|.r t.j.}.t
-00000780: 006a 027d 0674 006a 037d 0774 006a 040b  .j.}.t.j.}.t.j..
-00000790: 007d 086e 1874 006a 057d 0574 006a 067d  .}.n.t.j.}.t.j.}
-000007a0: 0674 006a 077d 0774 006a 047d 0874 00a0  .t.j.}.t.j.}.t..
-000007b0: 087c 027c 0118 00a1 017d 097c 0964 016b  .|.|.....}.|.d.k
-000007c0: 0272 527c 0053 007c 037c 0914 007d 0a74  .rR|.S.|.|...}.t
-000007d0: 097c 027c 0118 007c 0a1b 0083 017d 0b7c  .|.|...|.....}.|
-000007e0: 0174 00a0 0a7c 0ba1 017c 0a14 0017 007d  .t...|...|.....}
-000007f0: 0c74 0b7c 0c83 0173 8864 0153 007c 0c7c  .t.|...s.d.S.|.|
-00000800: 0a17 007d 0d74 006a 0c64 027c 006a 0d64  ...}.t.j.d.|.j.d
-00000810: 038d 027d 0e74 0e7c 0c7c 0d83 0244 005d  ...}.t.|.|...D.]
-00000820: 525c 027d 0f7d 107c 0964 016b 0472 c87c  R\.}.}.|.d.k.r.|
-00000830: 007c 0f7c 1085 0219 007d 116e 0c7c 007c  .|.|.....}.n.|.|
-00000840: 107c 0f85 0219 007d 1174 0b7c 1183 0173  .|.....}.t.|...s
-00000850: de71 aa7c 057c 1183 017d 127c 077c 127c  .q.|.|...}.|.|.|
-00000860: 0883 0272 f401 0071 fe7c 127d 087c 117d  ...r...q.|.}.|.}
-00000870: 0e71 aa7c 0f7c 0a18 007c 067c 0e83 0117  .q.|.|...|.|....
-00000880: 007d 137c 0964 016b 0090 0172 247c 1374  .}.|.d.k...r$|.t
-00000890: 0b7c 0e83 0118 007d 137c 1353 0029 044e  .|.....}.|.S.).N
-000008a0: 7201 0000 0072 1000 0000 7211 0000 0029  r....r....r....)
-000008b0: 0f72 1400 0000 da03 6d61 78da 0661 7267  .r......max..arg
-000008c0: 6d61 78da 0a6c 6573 735f 6571 7561 6cda  max..less_equal.
-000008d0: 0369 6e66 da03 6d69 6e72 3600 0000 da0d  .inf..minr6.....
-000008e0: 6772 6561 7465 725f 6571 7561 6cda 0473  greater_equal..s
-000008f0: 6967 6e72 2300 0000 7233 0000 0072 1300  ignr#...r3...r..
-00000900: 0000 7215 0000 0072 1200 0000 7218 0000  ..r....r....r...
-00000910: 0029 14da 0161 da05 6265 6769 6eda 0365  .)...a..begin..e
-00000920: 6e64 7228 0000 0072 2200 0000 5a05 6665  ndr(...r"...Z.fe
-00000930: 7874 725a 0866 6172 6765 7874 72da 0566  xtrZ.fargextr..f
-00000940: 636f 6d70 5a06 6375 7265 7874 da09 6469  compZ.curext..di
-00000950: 7265 6374 696f 6eda 0473 7465 705a 086e  rection..stepZ.n
-00000960: 7769 6e64 6f77 7372 2600 0000 7227 0000  windowsr&...r'..
-00000970: 005a 0767 6f6f 647a 6f69 721f 0000 0072  .Z.goodzoir....r
-00000980: 2000 0000 5a06 6e65 777a 6f69 5a06 6e65   ...Z.newzoiZ.ne
-00000990: 7765 7874 da03 7265 7472 0c00 0000 720c  wext..retr....r.
-000009a0: 0000 0072 0d00 0000 7225 0000 004f 0000  ...r....r%...O..
-000009b0: 0073 4400 0000 0001 0401 0601 0601 0601  .sD.............
-000009c0: 0a02 0601 0601 0601 0601 0e01 0801 0402  ................
-000009d0: 0801 1001 1201 0801 0401 0802 1001 1201  ................
-000009e0: 0801 0e02 0c01 0801 0201 0801 0a01 0401  ................
-000009f0: 0401 0601 1001 0a01 0c01 7225 0000 0063  ..........r%...c
-00000a00: 0600 0000 0000 0000 0000 0000 2000 0000  ............ ...
-00000a10: 0b00 0000 4300 0000 737a 0100 007c 0164  ....C...sz...|.d
-00000a20: 0064 0185 0219 007d 067c 0164 0264 0085  .d.....}.|.d.d..
-00000a30: 0219 007d 0774 006a 0174 027c 0183 0174  ...}.t.j.t.|...t
-00000a40: 0364 038d 027d 087c 007c 0219 007d 097c  .d...}.|.|...}.|
-00000a50: 007c 0119 007d 0a7c 097c 0a18 007d 0b74  .|...}.|.|...}.t
-00000a60: 00a0 047c 09a1 017d 0c74 00a0 047c 0aa1  ...|...}.t...|..
-00000a70: 017d 0d74 00a0 0474 00a0 047c 0aa1 017c  .}.t...t...|...|
-00000a80: 051b 00a1 017d 0e74 00a0 047c 00a1 017d  .....}.t...|...}
-00000a90: 0f74 057c 067c 077c 097c 0a7c 037c 0b7c  .t.|.|.|.|.|.|.|
-00000aa0: 0c7c 0d7c 0e7c 0483 0a7d 1074 067c 1083  .|.|.|...}.t.|..
-00000ab0: 0144 005d de5c 027d 115c 0a7d 127d 137d  .D.].\.}.\.}.}.}
-00000ac0: 147d 157d 167d 177d 187d 197d 1a7d 1b74  .}.}.}.}.}.}.}.t
-00000ad0: 00a0 0164 04a1 017d 1c7c 1464 056b 047c  ...d...}.|.d.k.|
-00000ae0: 1c64 063c 007c 1564 076b 007c 1c64 023c  .d.<.|.d.k.|.d.<
-00000af0: 007c 1664 086b 0070 e27c 1664 096b 047c  .|.d.k.p.|.d.k.|
-00000b00: 1c64 0a3c 007c 1b64 076b 0070 f67c 1b64  .d.<.|.d.k.p.|.d
-00000b10: 096b 047c 1c64 0b3c 007c 1764 076b 007c  .k.|.d.<.|.d.k.|
-00000b20: 1c64 0c3c 007c 0f7c 127c 1385 0219 007d  .d.<.|.|.|.....}
-00000b30: 1d7c 1d7c 1d64 066b 0019 007d 1e74 00a0  .|.|.d.k...}.t..
-00000b40: 077c 1ea1 017d 1f7c 1f64 0d6b 007c 1c64  .|...}.|.d.k.|.d
-00000b50: 0e3c 0074 087c 1883 0164 076b 047c 1c64  .<.t.|...d.k.|.d
-00000b60: 0f3c 0074 087c 1983 0164 076b 047c 1c64  .<.t.|...d.k.|.d
-00000b70: 103c 0074 087c 1a83 0164 116b 047c 1c64  .<.t.|...d.k.|.d
-00000b80: 123c 0074 00a0 097c 1ca1 017c 087c 113c  .<.t...|...|.|.<
-00000b90: 0071 967c 0853 0029 134e 720f 0000 0072  .q.|.S.).Nr....r
-00000ba0: 1000 0000 7211 0000 00e9 0900 0000 692c  ....r.........i,
-00000bb0: 0100 0072 0100 0000 e914 0000 00e9 1e00  ...r............
-00000bc0: 0000 e9c8 0000 00e9 0200 0000 e903 0000  ................
-00000bd0: 00e9 0400 0000 69d8 ffff ffe9 0500 0000  ......i.........
-00000be0: e906 0000 00e9 0700 0000 671f 85eb 51b8  ..........g...Q.
-00000bf0: 1ee5 3fe9 0800 0000 290a 7214 0000 0072  ..?.....).r....r
-00000c00: 1500 0000 7213 0000 00da 0462 6f6f 6cda  ....r......bool.
-00000c10: 0464 6966 6672 1800 0000 7217 0000 0072  .diffr....r....r
-00000c20: 1900 0000 da03 6162 73da 0361 6e79 2920  ......abs..any) 
-00000c30: 7207 0000 0072 0a00 0000 720b 0000 00da  r....r....r.....
-00000c40: 036d 6170 da02 6872 7208 0000 0072 1a00  .map..hrr....r..
-00000c50: 0000 721b 0000 00da 0373 7169 722a 0000  ..r......sqir*..
-00000c60: 0072 2900 0000 da02 7070 5a04 6473 7973  .r).....ppZ.dsys
-00000c70: 5a04 6464 6961 5a03 6464 745a 0764 7661  Z.ddiaZ.ddtZ.dva
-00000c80: 6c75 6573 da06 7061 7261 6d73 721e 0000  lues..paramsr...
-00000c90: 00da 0669 7374 6172 74da 0569 7374 6f70  ...istart..istop
-00000ca0: 5a04 6973 7973 5a04 6964 6961 5a05 696d  Z.isysZ.idiaZ.im
-00000cb0: 6561 6e5a 0369 7070 5a05 6964 7379 735a  eanZ.ippZ.idsysZ
-00000cc0: 0569 6464 6961 5a04 6964 6474 5a03 6968  .iddiaZ.iddtZ.ih
-00000cd0: 72da 0863 7269 7465 7269 61da 0673 6c6f  r..criteria..slo
-00000ce0: 7065 735a 096e 6567 736c 6f70 6573 5a08  pesZ.negslopesZ.
-00000cf0: 6e65 6773 6c6f 7065 720c 0000 0072 0c00  negsloper....r..
-00000d00: 0000 720d 0000 00da 1263 616c 635f 7175  ..r......calc_qu
-00000d10: 616c 6974 795f 696e 6465 7878 0000 0073  ality_indexx...s
-00000d20: 3c00 0000 0002 0c01 0c01 1202 0801 0801  <...............
-00000d30: 0801 0a01 0a01 1401 0a02 1a04 06fd 0601  ................
-00000d40: 0201 1602 0a01 0c01 0c01 1401 1401 0c01  ................
-00000d50: 0c01 0c01 0a01 0c01 1001 1001 1001 1001  ................
-00000d60: 7265 0000 0029 0146 290b da05 6e75 6d70  re...).F)...nump
-00000d70: 7972 1400 0000 da14 7068 7973 696f 6375  yr......physiocu
-00000d80: 7276 652e 7072 6573 7375 7265 7202 0000  rve.pressurer...
-00000d90: 0072 0e00 0000 7221 0000 0072 0500 0000  .r....r!...r....
-00000da0: 7230 0000 0072 0600 0000 7225 0000 0072  r0...r....r%...r
-00000db0: 6500 0000 720c 0000 0072 0c00 0000 720c  e...r....r....r.
-00000dc0: 0000 0072 0d00 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000dd0: 653e 0100 0000 7310 0000 0008 010c 0308  e>....s.........
-00000de0: 0708 0b08 1008 0508 230a 29              ........#.)
+00000020: 0003 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
+00000030: 6401 6c00 5a01 6402 6403 8400 5a02 6404  d.l.Z.d.d...Z.d.
+00000040: 6405 8400 5a03 6406 6407 8400 5a04 640d  d...Z.d.d...Z.d.
+00000050: 6409 640a 8401 5a05 640b 640c 8400 5a06  d.d...Z.d.d...Z.
+00000060: 6401 5300 290e e900 0000 004e 6303 0000  d.S.)......Nc...
+00000070: 0000 0000 0000 0000 000e 0000 0008 0000  ................
+00000080: 0043 0000 0073 a800 0000 7c02 6401 6402  .C...s....|.d.d.
+00000090: 8502 1900 7d03 7c02 6403 6400 8502 1900  ....}.|.d.d.....
+000000a0: 7d04 7400 6404 7c01 1400 8301 7d05 7401  }.t.d.|.....}.t.
+000000b0: 7c03 8301 7d06 7402 6a03 7c06 7402 6a04  |...}.t.j.|.t.j.
+000000c0: 6405 8d02 7d07 7402 6a03 7c06 7402 6a04  d...}.t.j.|.t.j.
+000000d0: 6405 8d02 7d08 7405 7406 7c03 7c04 8302  d...}.t.t.|.|...
+000000e0: 8301 4400 5d22 5c02 7d09 5c02 7d0a 7d0b  ..D.]"\.}.\.}.}.
+000000f0: 7c0b 7c0a 1800 7d0c 7c0a 7c0c 1800 7d0d  |.|...}.|.|...}.
+00000100: 7407 7c00 7c0a 7c0d 7c05 8304 7c07 7c09  t.|.|.|.|...|.|.
+00000110: 3c00 7407 7c00 7c0a 7c0b 7c05 6406 6407  <.t.|.|.|.|.d.d.
+00000120: 8d05 7c08 7c09 3c00 712d 7c07 7c08 6602  ..|.|.<.q-|.|.f.
+00000130: 5300 2908 4e72 0100 0000 e9ff ffff ffe9  S.).Nr..........
+00000140: 0100 0000 679a 9999 9999 99a9 3fa9 01da  ....g.......?...
+00000150: 0564 7479 7065 5429 01da 0973 6561 7263  .dtypeT)...searc
+00000160: 686d 6178 2908 da03 696e 74da 036c 656e  hmax)...int..len
+00000170: da02 6e70 da05 7a65 726f 73da 0569 6e74  ..np..zeros..int
+00000180: 3634 da09 656e 756d 6572 6174 65da 037a  64..enumerate..z
+00000190: 6970 da12 6669 6e64 5f6c 6f63 616c 5f65  ip..find_local_e
+000001a0: 7874 7265 6d65 290e da06 7661 6c75 6573  xtreme)...values
+000001b0: da0a 7361 6d70 6c65 7261 7465 5a07 6665  ..samplerateZ.fe
+000001c0: 6574 6964 78da 0673 7461 7274 73da 0573  etidx..starts..s
+000001d0: 746f 7073 da0a 7769 6e64 6f77 7369 7a65  tops..windowsize
+000001e0: da07 6e76 616c 7565 73da 0364 6961 da03  ..nvalues..dia..
+000001f0: 7379 73da 0169 da05 7374 6172 74da 0473  sys..i..start..s
+00000200: 746f 70da 0864 7572 6174 696f 6e5a 0764  top..durationZ.d
+00000210: 6961 7374 6f70 a900 721b 0000 00fa 3b2f  iastop..r.....;/
+00000220: 686f 6d65 2f6a 616a 2f64 6576 656c 2f70  home/jaj/devel/p
+00000230: 6879 7369 6f63 7572 7665 2f70 6879 7369  hysiocurve/physi
+00000240: 6f63 7572 7665 2f70 7265 7373 7572 652f  ocurve/pressure/
+00000250: 696e 6379 636c 652e 7079 da0c 6669 6e64  incycle.py..find
+00000260: 5f64 6961 5f73 7973 0700 0000 7318 0000  _dia_sys....s...
+00000270: 000c 010c 010c 0108 0110 0110 011a 0108  ................
+00000280: 0108 0112 0118 0108 0172 1d00 0000 6303  .........r....c.
+00000290: 0000 0000 0000 0000 0000 0003 0000 0005  ................
+000002a0: 0000 0043 0000 0073 1400 0000 7400 a001  ...C...s....t...
+000002b0: 7c01 7c00 1800 7c02 7c00 1800 a102 5300  |.|...|.|.....S.
+000002c0: 2901 4e29 0272 0900 0000 da05 6372 6f73  ).N).r......cros
+000002d0: 7329 03da 026c 31da 026c 32da 0170 721b  s)...l1..l2..pr.
+000002e0: 0000 0072 1b00 0000 721c 0000 00da 0864  ...r....r......d
+000002f0: 6973 7461 6e63 6517 0000 0073 0200 0000  istance....s....
+00000300: 1401 7222 0000 0063 0300 0000 0000 0000  ..r"...c........
+00000310: 0000 0000 0f00 0000 0600 0000 4300 0000  ............C...
+00000320: 73f8 0000 0074 007c 0183 0144 005d 0c5c  s....t.|...D.].\
+00000330: 027d 037d 047c 047c 0264 0119 006b 0472  .}.}.|.|.d...k.r
+00000340: 1001 006e 0871 0474 016a 0264 0174 0364  ...n.q.t.j.d.t.d
+00000350: 028d 0253 007c 017c 0364 0085 0219 007d  ...S.|.|.d.....}
+00000360: 0174 047c 0183 017d 0574 016a 027c 0574  .t.|...}.t.j.|.t
+00000370: 016a 0564 028d 027d 0674 0074 067c 017c  .j.d...}.t.t.|.|
+00000380: 0283 0283 0144 005d 485c 027d 075c 027d  .....D.]H\.}.\.}
+00000390: 087d 097c 007c 097c 0885 0219 007d 0a74  .}.|.|.|.....}.t
+000003a0: 047c 0a83 0173 4271 3174 01a0 0764 017c  .|...sBq1t...d.|
+000003b0: 0a64 0119 0067 02a1 017d 0b74 01a0 077c  .d...g...}.t...|
+000003c0: 087c 0918 007c 0a64 0319 0067 02a1 017d  .|...|.d...g...}
+000003d0: 0c74 01a0 0874 047c 0a83 01a1 017d 0d74  .t...t.|.....}.t
+000003e0: 01a0 097c 0d7c 0a66 02a1 016a 0a7d 0e74  ...|.|.f...j.}.t
+000003f0: 0b7c 0b7c 0c7c 0e83 037d 0474 047c 0483  .|.|.|...}.t.|..
+00000400: 0173 7071 317c 0974 01a0 0c7c 04a1 0117  .spq1|.t...|....
+00000410: 007c 067c 073c 0071 317c 0653 0029 044e  .|.|.<.q1|.S.).N
+00000420: 7201 0000 0072 0400 0000 7202 0000 0029  r....r....r....)
+00000430: 0d72 0c00 0000 7209 0000 0072 0a00 0000  .r....r....r....
+00000440: 7207 0000 0072 0800 0000 720b 0000 0072  r....r....r....r
+00000450: 0d00 0000 da05 6172 7261 79da 0661 7261  ......array..ara
+00000460: 6e67 65da 0676 7374 6163 6bda 0154 7222  nge..vstack..Tr"
+00000470: 0000 00da 0661 7267 6d69 6e29 0f72 0f00  .....argmin).r..
+00000480: 0000 da06 6469 6169 6478 da06 7379 7369  ....diaidx..sysi
+00000490: 6478 da01 6eda 0164 7214 0000 00da 0464  dx..n..dr......d
+000004a0: 6963 7372 1700 0000 da02 6469 da02 7369  icsr......di..si
+000004b0: 5a03 7a6f 69da 0270 31da 0270 325a 067a  Z.zoi..p1..p2Z.z
+000004c0: 6f69 6964 785a 0270 3372 1b00 0000 721b  oiidxZ.p3r....r.
+000004d0: 0000 0072 1c00 0000 da0e 6669 6e64 5f64  ...r......find_d
+000004e0: 6963 726f 7469 6373 1c00 0000 732a 0000  icrotics....s*..
+000004f0: 0010 020c 0104 0102 ff0e 040c 0108 0210  ................
+00000500: 011a 010c 0108 0102 0112 0116 010e 0210  ................
+00000510: 010c 0208 0102 0114 0104 0172 3100 0000  ...........r1...
+00000520: 4663 0500 0000 0000 0000 0000 0000 1400  Fc..............
+00000530: 0000 0400 0000 4300 0000 7326 0100 007c  ......C...s&...|
+00000540: 0472 1074 006a 017d 0574 006a 027d 0674  .r.t.j.}.t.j.}.t
+00000550: 006a 037d 0774 006a 040b 007d 086e 0c74  .j.}.t.j...}.n.t
+00000560: 006a 057d 0574 006a 067d 0674 006a 077d  .j.}.t.j.}.t.j.}
+00000570: 0774 006a 047d 0874 00a0 087c 027c 0118  .t.j.}.t...|.|..
+00000580: 00a1 017d 097c 0964 016b 0272 297c 0053  ...}.|.d.k.r)|.S
+00000590: 007c 037c 0914 007d 0a74 097c 027c 0118  .|.|...}.t.|.|..
+000005a0: 007c 0a1b 0083 017d 0b7c 0174 00a0 0a7c  .|.....}.|.t...|
+000005b0: 0ba1 017c 0a14 0017 007d 0c74 0b7c 0c83  ...|.....}.t.|..
+000005c0: 0173 4464 0153 007c 0c7c 0a17 007d 0d74  .sDd.S.|.|...}.t
+000005d0: 006a 0c64 027c 006a 0d64 038d 027d 0e74  .j.d.|.j.d...}.t
+000005e0: 0e7c 0c7c 0d83 0244 005d 295c 027d 0f7d  .|.|...D.])\.}.}
+000005f0: 107c 0964 016b 0472 647c 007c 0f7c 1085  .|.d.k.rd|.|.|..
+00000600: 0219 007d 116e 067c 007c 107c 0f85 0219  ...}.n.|.|.|....
+00000610: 007d 1174 0b7c 1183 0173 6f71 557c 057c  .}.t.|...soqU|.|
+00000620: 1183 017d 127c 077c 127c 0883 0272 7a01  ...}.|.|.|...rz.
+00000630: 006e 057c 127d 087c 117d 0e71 557c 0f7c  .n.|.}.|.}.qU|.|
+00000640: 0a18 007c 067c 0e83 0117 007d 137c 0964  ...|.|.....}.|.d
+00000650: 016b 0072 917c 1374 0b7c 0e83 0118 007d  .k.r.|.t.|.....}
+00000660: 137c 1353 0029 044e 7201 0000 0072 0300  .|.S.).Nr....r..
+00000670: 0000 7204 0000 0029 0f72 0900 0000 da03  ..r....).r......
+00000680: 6d61 78da 0661 7267 6d61 78da 0a6c 6573  max..argmax..les
+00000690: 735f 6571 7561 6cda 0369 6e66 da03 6d69  s_equal..inf..mi
+000006a0: 6e72 2700 0000 da0d 6772 6561 7465 725f  nr'.....greater_
+000006b0: 6571 7561 6cda 0473 6967 6e72 0700 0000  equal..signr....
+000006c0: 7224 0000 0072 0800 0000 720a 0000 0072  r$...r....r....r
+000006d0: 0500 0000 720d 0000 0029 14da 0161 da05  ....r....)...a..
+000006e0: 6265 6769 6eda 0365 6e64 7213 0000 0072  begin..endr....r
+000006f0: 0600 0000 5a05 6665 7874 725a 0866 6172  ....Z.fextrZ.far
+00000700: 6765 7874 72da 0566 636f 6d70 5a06 6375  gextr..fcompZ.cu
+00000710: 7265 7874 da09 6469 7265 6374 696f 6eda  rext..direction.
+00000720: 0473 7465 705a 086e 7769 6e64 6f77 7372  .stepZ.nwindowsr
+00000730: 1100 0000 7212 0000 005a 0767 6f6f 647a  ....r....Z.goodz
+00000740: 6f69 7218 0000 0072 1900 0000 5a06 6e65  oir....r....Z.ne
+00000750: 777a 6f69 5a06 6e65 7765 7874 da03 7265  wzoiZ.newext..re
+00000760: 7472 1b00 0000 721b 0000 0072 1c00 0000  tr....r....r....
+00000770: 720e 0000 003a 0000 0073 4400 0000 0401  r....:...sD.....
+00000780: 0601 0601 0601 0a01 0602 0601 0601 0601  ................
+00000790: 0e01 0801 0401 0802 1001 1201 0801 0401  ................
+000007a0: 0801 1002 1201 0801 0e01 0c02 0801 0201  ................
+000007b0: 0801 0a01 0401 0401 0601 1001 0801 0c01  ................
+000007c0: 0401 720e 0000 0063 0600 0000 0000 0000  ..r....c........
+000007d0: 0000 0000 2000 0000 0b00 0000 4300 0000  .... .......C...
+000007e0: 738a 0100 007c 0164 0064 0185 0219 007d  s....|.d.d.....}
+000007f0: 067c 0164 0264 0085 0219 007d 0774 006a  .|.d.d.....}.t.j
+00000800: 0174 027c 0183 0174 0364 038d 027d 087c  .t.|...t.d...}.|
+00000810: 007c 0219 007d 097c 007c 0119 007d 0a7c  .|...}.|.|...}.|
+00000820: 097c 0a18 007d 0b74 00a0 047c 09a1 017d  .|...}.t...|...}
+00000830: 0c74 00a0 047c 0aa1 017d 0d74 00a0 0474  .t...|...}.t...t
+00000840: 00a0 047c 0aa1 017c 051b 00a1 017d 0e74  ...|...|.....}.t
+00000850: 00a0 047c 00a1 017d 0f74 057c 067c 077c  ...|...}.t.|.|.|
+00000860: 097c 0a7c 037c 0b7c 0c7c 0d7c 0e7c 0483  .|.|.|.|.|.|.|..
+00000870: 0a7d 1074 067c 1083 0144 005d 775c 027d  .}.t.|...D.]w\.}
+00000880: 115c 0a7d 127d 137d 147d 157d 167d 177d  .\.}.}.}.}.}.}.}
+00000890: 187d 197d 1a7d 1b74 00a0 0164 04a1 017d  .}.}.}.t...d...}
+000008a0: 1c7c 1464 056b 047c 1c64 063c 007c 1564  .|.d.k.|.d.<.|.d
+000008b0: 076b 007c 1c64 023c 007c 1664 086b 0070  .k.|.d.<.|.d.k.p
+000008c0: 717c 1664 096b 047c 1c64 0a3c 007c 1b64  q|.d.k.|.d.<.|.d
+000008d0: 076b 0070 7b7c 1b64 096b 047c 1c64 0b3c  .k.p{|.d.k.|.d.<
+000008e0: 007c 1764 076b 007c 1c64 0c3c 007c 0f7c  .|.d.k.|.d.<.|.|
+000008f0: 127c 1385 0219 007d 1d7c 1d7c 1d64 066b  .|.....}.|.|.d.k
+00000900: 0019 007d 1e74 027c 1e64 066b 0483 0172  ...}.t.|.d.k...r
+00000910: 9b74 00a0 077c 1ea1 016e 0164 067d 1f7c  .t...|...n.d.}.|
+00000920: 1f64 0d6b 007c 1c64 0e3c 0074 087c 1883  .d.k.|.d.<.t.|..
+00000930: 0164 076b 047c 1c64 0f3c 0074 087c 1983  .d.k.|.d.<.t.|..
+00000940: 0164 076b 047c 1c64 103c 0074 087c 1a83  .d.k.|.d.<.t.|..
+00000950: 0164 116b 047c 1c64 123c 0074 00a0 097c  .d.k.|.d.<.t...|
+00000960: 1ca1 017c 087c 113c 0071 4b7c 0853 0029  ...|.|.<.qK|.S.)
+00000970: 134e 7202 0000 0072 0300 0000 7204 0000  .Nr....r....r...
+00000980: 00e9 0900 0000 692c 0100 0072 0100 0000  ......i,...r....
+00000990: e914 0000 00e9 1e00 0000 e9c8 0000 00e9  ................
+000009a0: 0200 0000 e903 0000 00e9 0400 0000 69d8  ..............i.
+000009b0: ffff ffe9 0500 0000 e906 0000 00e9 0700  ................
+000009c0: 0000 671f 85eb 51b8 1ee5 3fe9 0800 0000  ..g...Q...?.....
+000009d0: 290a 7209 0000 0072 0a00 0000 7208 0000  ).r....r....r...
+000009e0: 00da 0462 6f6f 6cda 0464 6966 6672 0d00  ...bool..diffr..
+000009f0: 0000 720c 0000 00da 076e 616e 6d65 616e  ..r......nanmean
+00000a00: da03 6162 73da 0361 6e79 2920 720f 0000  ..abs..any) r...
+00000a10: 0072 2800 0000 7229 0000 00da 036d 6170  .r(...r).....map
+00000a20: da02 6872 7210 0000 005a 0873 7461 7274  ..hrr....Z.start
+00000a30: 6964 78da 0665 6e64 6964 78da 0373 7169  idx..endidx..sqi
+00000a40: 7216 0000 0072 1500 0000 da02 7070 5a04  r....r......ppZ.
+00000a50: 6473 7973 5a04 6464 6961 5a03 6464 745a  dsysZ.ddiaZ.ddtZ
+00000a60: 0764 7661 6c75 6573 da06 7061 7261 6d73  .dvalues..params
+00000a70: 7217 0000 00da 0669 7374 6172 74da 0569  r......istart..i
+00000a80: 7374 6f70 5a04 6973 7973 5a04 6964 6961  stopZ.isysZ.idia
+00000a90: 5a05 696d 6561 6e5a 0369 7070 5a05 6964  Z.imeanZ.ippZ.id
+00000aa0: 7379 735a 0569 6464 6961 5a04 6964 6474  sysZ.iddiaZ.iddt
+00000ab0: 5a03 6968 72da 0863 7269 7465 7269 61da  Z.ihr..criteria.
+00000ac0: 0673 6c6f 7065 735a 096e 6567 736c 6f70  .slopesZ.negslop
+00000ad0: 6573 5a08 6e65 6773 6c6f 7065 721b 0000  esZ.negsloper...
+00000ae0: 0072 1b00 0000 721c 0000 00da 1263 616c  .r....r......cal
+00000af0: 635f 7175 616c 6974 795f 696e 6465 7863  c_quality_indexc
+00000b00: 0000 0073 3c00 0000 0c03 0c01 1201 0802  ...s<...........
+00000b10: 0801 0801 0a01 0a01 1401 0a01 1a02 0604  ................
+00000b20: 06fd 0201 1601 0a02 0c01 0c01 1401 1401  ................
+00000b30: 0c01 0c01 0c01 1a01 0c01 1001 1001 1001  ................
+00000b40: 1001 0401 725a 0000 0029 0146 2907 da05  ....rZ...).F)...
+00000b50: 6e75 6d70 7972 0900 0000 721d 0000 0072  numpyr....r....r
+00000b60: 2200 0000 7231 0000 0072 0e00 0000 725a  "...r1...r....rZ
+00000b70: 0000 0072 1b00 0000 721b 0000 0072 1b00  ...r....r....r..
+00000b80: 0000 721c 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000b90: 3e01 0000 0073 0c00 0000 0800 0806 0810  >....s..........
+00000ba0: 0805 0a1e 0c29                           .....)
```

### Comparing `physiocurve-2022.7.8/physiocurve/pressure/__pycache__/incycle.cpython-39.pyc` & `physiocurve-2024.5.7/physiocurve/pressure/__pycache__/incycle.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Jun 26 19:27:22 2022 UTC, .py size: 4554 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,223 +1,186 @@
-00000000: 610d 0d0a 0000 0000 1ab3 b862 ca11 0000  a..........b....
+00000000: 550d 0d0a 0000 0000 bcca cd62 e60e 0000  U..........b....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
-00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6403 6404 8400 5a04 6405 6406 8400  ..d.d...Z.d.d...
-00000050: 5a05 6407 6408 8400 5a06 6409 640a 8400  Z.d.d...Z.d.d...
-00000060: 5a07 640b 640c 8400 5a08 6412 640e 640f  Z.d.d...Z.d.d.d.
-00000070: 8401 5a09 6410 6411 8400 5a0a 6401 5300  ..Z.d.d...Z.d.S.
-00000080: 2913 e900 0000 004e 2901 da04 666f 6f74  )......N)...foot
-00000090: 6302 0000 0000 0000 0000 0000 0006 0000  c...............
-000000a0: 0004 0000 0043 0000 0073 3400 0000 7400  .....C...s4...t.
-000000b0: a001 7c00 7c01 a102 7d02 7402 7c00 7c01  ..|.|...}.t.|.|.
-000000c0: 7c02 8303 5c02 7d03 7d04 7403 7c00 7c03  |...\.}.}.t.|.|.
-000000d0: 7c04 8303 7d05 7c02 7c03 7c04 7c05 6704  |...}.|.|.|.|.g.
-000000e0: 5300 a901 4e29 0472 0200 0000 da12 6669  S...N).r......fi
-000000f0: 6e64 5f70 7265 7373 7572 655f 6665 6574  nd_pressure_feet
-00000100: da0c 6669 6e64 5f64 6961 5f73 7973 da0e  ..find_dia_sys..
-00000110: 6669 6e64 5f64 6963 726f 7469 6373 2906  find_dicrotics).
-00000120: da06 7661 6c75 6573 da0a 7361 6d70 6c65  ..values..sample
-00000130: 7261 7465 da07 6665 6574 6964 78da 0664  rate..feetidx..d
-00000140: 6961 6964 78da 0673 7973 6964 785a 0664  iaidx..sysidxZ.d
-00000150: 6963 6964 78a9 0072 0c00 0000 fa3b 2f68  icidx..r.....;/h
-00000160: 6f6d 652f 6a61 6a2f 6465 7665 6c2f 7068  ome/jaj/devel/ph
-00000170: 7973 696f 6375 7276 652f 7068 7973 696f  ysiocurve/physio
-00000180: 6375 7276 652f 7072 6573 7375 7265 2f69  curve/pressure/i
-00000190: 6e63 7963 6c65 2e70 79da 1266 696e 645f  ncycle.py..find_
-000001a0: 7072 6573 7375 7265 5f66 756c 6c05 0000  pressure_full...
-000001b0: 0073 0800 0000 0001 0c01 1001 0c01 720e  .s............r.
-000001c0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-000001d0: 0900 0000 0600 0000 4300 0000 736a 0000  ........C...sj..
-000001e0: 007c 0164 0064 0185 0219 007d 027c 0164  .|.d.d.....}.|.d
-000001f0: 0264 0085 0219 007d 0374 007c 0183 0164  .d.....}.t.|...d
-00000200: 0218 007d 0474 016a 027c 0474 016a 0364  ...}.t.j.|.t.j.d
-00000210: 038d 027d 0574 0474 057c 027c 0383 0283  ...}.t.t.|.|....
-00000220: 0144 005d 225c 027d 065c 027d 077d 0874  .D.]"\.}.\.}.}.t
-00000230: 01a0 067c 007c 077c 0885 0219 00a1 017c  ...|.|.|.......|
-00000240: 057c 063c 0071 427c 0553 0029 044e e9ff  .|.<.qB|.S.).N..
-00000250: ffff ffe9 0100 0000 a901 da05 6474 7970  ............dtyp
-00000260: 6529 07da 036c 656e da02 6e70 da05 7a65  e)...len..np..ze
-00000270: 726f 73da 0566 6c6f 6174 da09 656e 756d  ros..float..enum
-00000280: 6572 6174 65da 037a 6970 da07 6e61 6e6d  erate..zip..nanm
-00000290: 6561 6e29 0972 0700 0000 720a 0000 00da  ean).r....r.....
-000002a0: 0873 7461 7274 6964 78da 0665 6e64 6964  .startidx..endid
-000002b0: 78da 076e 7661 6c75 6573 da05 6d65 616e  x..nvalues..mean
-000002c0: 73da 0169 da05 7374 6172 74da 0473 746f  s..i..start..sto
-000002d0: 7072 0c00 0000 720c 0000 0072 0d00 0000  pr....r....r....
-000002e0: da0a 6361 6c63 5f6d 6561 6e73 0c00 0000  ..calc_means....
-000002f0: 730e 0000 0000 010c 010c 010c 0110 011a  s...............
-00000300: 0118 0172 2100 0000 6303 0000 0000 0000  ...r!...c.......
-00000310: 0000 0000 000e 0000 0008 0000 0043 0000  .............C..
-00000320: 0073 a800 0000 7c02 6401 6402 8502 1900  .s....|.d.d.....
-00000330: 7d03 7c02 6403 6400 8502 1900 7d04 7400  }.|.d.d.....}.t.
-00000340: 6404 7c01 1400 8301 7d05 7401 7c03 8301  d.|.....}.t.|...
-00000350: 7d06 7402 6a03 7c06 7402 6a04 6405 8d02  }.t.j.|.t.j.d...
-00000360: 7d07 7402 6a03 7c06 7402 6a04 6405 8d02  }.t.j.|.t.j.d...
-00000370: 7d08 7405 7406 7c03 7c04 8302 8301 4400  }.t.t.|.|.....D.
-00000380: 5d44 5c02 7d09 5c02 7d0a 7d0b 7c0b 7c0a  ]D\.}.\.}.}.|.|.
-00000390: 1800 7d0c 7c0a 7c0c 1800 7d0d 7407 7c00  ..}.|.|...}.t.|.
-000003a0: 7c0a 7c0d 7c05 8304 7c07 7c09 3c00 7407  |.|.|...|.|.<.t.
-000003b0: 7c00 7c0a 7c0b 7c05 6406 6407 8d05 7c08  |.|.|.|.d.d...|.
-000003c0: 7c09 3c00 715a 7c07 7c08 6602 5300 2908  |.<.qZ|.|.f.S.).
-000003d0: 4e72 0100 0000 720f 0000 0072 1000 0000  Nr....r....r....
-000003e0: 679a 9999 9999 99a9 3f72 1100 0000 5429  g.......?r....T)
-000003f0: 01da 0973 6561 7263 686d 6178 2908 da03  ...searchmax)...
-00000400: 696e 7472 1300 0000 7214 0000 0072 1500  intr....r....r..
-00000410: 0000 da05 696e 7436 3472 1700 0000 7218  ....int64r....r.
-00000420: 0000 00da 1266 696e 645f 6c6f 6361 6c5f  .....find_local_
-00000430: 6578 7472 656d 6529 0e72 0700 0000 7208  extreme).r....r.
-00000440: 0000 0072 0900 0000 da06 7374 6172 7473  ...r......starts
-00000450: da05 7374 6f70 73da 0a77 696e 646f 7773  ..stops..windows
-00000460: 697a 6572 1c00 0000 da03 6469 61da 0373  izer......dia..s
-00000470: 7973 721e 0000 0072 1f00 0000 7220 0000  ysr....r....r ..
-00000480: 00da 0864 7572 6174 696f 6eda 0764 6961  ...duration..dia
-00000490: 7374 6f70 720c 0000 0072 0c00 0000 720d  stopr....r....r.
-000004a0: 0000 0072 0500 0000 1700 0000 7318 0000  ...r........s...
-000004b0: 0000 010c 010c 010c 0108 0110 0110 011a  ................
-000004c0: 0108 0108 0112 0118 0172 0500 0000 6303  .........r....c.
-000004d0: 0000 0000 0000 0000 0000 0003 0000 0005  ................
-000004e0: 0000 0043 0000 0073 1400 0000 7400 a001  ...C...s....t...
-000004f0: 7c01 7c00 1800 7c02 7c00 1800 a102 5300  |.|...|.|.....S.
-00000500: 7203 0000 0029 0272 1400 0000 da05 6372  r....).r......cr
-00000510: 6f73 7329 03da 026c 31da 026c 32da 0170  oss)...l1..l2..p
-00000520: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
-00000530: 0864 6973 7461 6e63 6527 0000 0073 0200  .distance'...s..
-00000540: 0000 0001 7231 0000 0063 0300 0000 0000  ....r1...c......
-00000550: 0000 0000 0000 0f00 0000 0600 0000 4300  ..............C.
-00000560: 0000 73f8 0000 0074 007c 0183 0144 005d  ..s....t.|...D.]
-00000570: 185c 027d 037d 047c 047c 0264 0119 006b  .\.}.}.|.|.d...k
-00000580: 0472 0801 0071 3071 0874 016a 0264 0174  .r...q0q.t.j.d.t
-00000590: 0364 028d 0253 007c 017c 0364 0085 0219  .d...S.|.|.d....
-000005a0: 007d 0174 047c 0183 017d 0574 016a 057c  .}.t.|...}.t.j.|
-000005b0: 0574 016a 0664 028d 027d 0674 0074 077c  .t.j.d...}.t.t.|
-000005c0: 017c 0283 0283 0144 005d 905c 027d 075c  .|.....D.].\.}.\
-000005d0: 027d 087d 097c 007c 097c 0885 0219 007d  .}.}.|.|.|.....}
-000005e0: 0a74 047c 0a83 0173 8471 6274 01a0 0864  .t.|...s.qbt...d
-000005f0: 017c 0a64 0119 0067 02a1 017d 0b74 01a0  .|.d...g...}.t..
-00000600: 087c 087c 0918 007c 0a64 0319 0067 02a1  .|.|...|.d...g..
-00000610: 017d 0c74 01a0 0974 047c 0a83 01a1 017d  .}.t...t.|.....}
-00000620: 0d74 01a0 0a7c 0d7c 0a66 02a1 016a 0b7d  .t...|.|.f...j.}
-00000630: 0e74 0c7c 0b7c 0c7c 0e83 037d 0474 047c  .t.|.|.|...}.t.|
-00000640: 0483 0173 e071 627c 0974 01a0 0d7c 04a1  ...s.qb|.t...|..
-00000650: 0117 007c 067c 073c 0071 627c 0653 0029  ...|.|.<.qb|.S.)
-00000660: 044e 7201 0000 0072 1100 0000 720f 0000  .Nr....r....r...
-00000670: 0029 0e72 1700 0000 7214 0000 00da 0565  .).r....r......e
-00000680: 6d70 7479 7223 0000 0072 1300 0000 7215  mptyr#...r....r.
-00000690: 0000 0072 2400 0000 7218 0000 00da 0561  ...r$...r......a
-000006a0: 7272 6179 da06 6172 616e 6765 da06 7673  rray..arange..vs
-000006b0: 7461 636b da01 5472 3100 0000 da06 6172  tack..Tr1.....ar
-000006c0: 676d 696e 290f 7207 0000 0072 0a00 0000  gmin).r....r....
-000006d0: 720b 0000 00da 016e da01 6472 1c00 0000  r......n..dr....
-000006e0: da04 6469 6373 721e 0000 00da 0264 69da  ..dicsr......di.
-000006f0: 0273 69da 037a 6f69 da02 7031 da02 7032  .si..zoi..p1..p2
-00000700: 5a06 7a6f 6969 6478 da02 7033 720c 0000  Z.zoiidx..p3r...
-00000710: 0072 0c00 0000 720d 0000 0072 0600 0000  .r....r....r....
-00000720: 2c00 0000 7328 0000 0000 0210 010c 0106  ,...s(..........
-00000730: 030e 010c 0208 0110 011a 010c 0108 0102  ................
-00000740: 0112 0116 050e 0110 020c 0108 0102 0114  ................
-00000750: 0372 0600 0000 4663 0500 0000 0000 0000  .r....Fc........
-00000760: 0000 0000 1400 0000 0400 0000 4300 0000  ............C...
-00000770: 7328 0100 007c 0472 2074 006a 017d 0574  s(...|.r t.j.}.t
-00000780: 006a 027d 0674 006a 037d 0774 006a 040b  .j.}.t.j.}.t.j..
-00000790: 007d 086e 1874 006a 057d 0574 006a 067d  .}.n.t.j.}.t.j.}
-000007a0: 0674 006a 077d 0774 006a 047d 0874 00a0  .t.j.}.t.j.}.t..
-000007b0: 087c 027c 0118 00a1 017d 097c 0964 016b  .|.|.....}.|.d.k
-000007c0: 0272 527c 0053 007c 037c 0914 007d 0a74  .rR|.S.|.|...}.t
-000007d0: 097c 027c 0118 007c 0a1b 0083 017d 0b7c  .|.|...|.....}.|
-000007e0: 0174 00a0 0a7c 0ba1 017c 0a14 0017 007d  .t...|...|.....}
-000007f0: 0c74 0b7c 0c83 0173 8864 0153 007c 0c7c  .t.|...s.d.S.|.|
-00000800: 0a17 007d 0d74 006a 0c64 027c 006a 0d64  ...}.t.j.d.|.j.d
-00000810: 038d 027d 0e74 0e7c 0c7c 0d83 0244 005d  ...}.t.|.|...D.]
-00000820: 525c 027d 0f7d 107c 0964 016b 0472 c87c  R\.}.}.|.d.k.r.|
-00000830: 007c 0f7c 1085 0219 007d 116e 0c7c 007c  .|.|.....}.n.|.|
-00000840: 107c 0f85 0219 007d 1174 0b7c 1183 0173  .|.....}.t.|...s
-00000850: de71 aa7c 057c 1183 017d 127c 077c 127c  .q.|.|...}.|.|.|
-00000860: 0883 0272 f401 0071 fe7c 127d 087c 117d  ...r...q.|.}.|.}
-00000870: 0e71 aa7c 0f7c 0a18 007c 067c 0e83 0117  .q.|.|...|.|....
-00000880: 007d 137c 0964 016b 0090 0172 247c 1374  .}.|.d.k...r$|.t
-00000890: 0b7c 0e83 0118 007d 137c 1353 0029 044e  .|.....}.|.S.).N
-000008a0: 7201 0000 0072 1000 0000 7211 0000 0029  r....r....r....)
-000008b0: 0f72 1400 0000 da03 6d61 78da 0661 7267  .r......max..arg
-000008c0: 6d61 78da 0a6c 6573 735f 6571 7561 6cda  max..less_equal.
-000008d0: 0369 6e66 da03 6d69 6e72 3700 0000 da0d  .inf..minr7.....
-000008e0: 6772 6561 7465 725f 6571 7561 6cda 0473  greater_equal..s
-000008f0: 6967 6e72 2300 0000 7234 0000 0072 1300  ignr#...r4...r..
-00000900: 0000 7215 0000 0072 1200 0000 7218 0000  ..r....r....r...
-00000910: 0029 14da 0161 da05 6265 6769 6eda 0365  .)...a..begin..e
-00000920: 6e64 7228 0000 0072 2200 0000 5a05 6665  ndr(...r"...Z.fe
-00000930: 7874 725a 0866 6172 6765 7874 72da 0566  xtrZ.fargextr..f
-00000940: 636f 6d70 5a06 6375 7265 7874 da09 6469  compZ.curext..di
-00000950: 7265 6374 696f 6eda 0473 7465 70da 086e  rection..step..n
-00000960: 7769 6e64 6f77 7372 2600 0000 7227 0000  windowsr&...r'..
-00000970: 005a 0767 6f6f 647a 6f69 721f 0000 0072  .Z.goodzoir....r
-00000980: 2000 0000 5a06 6e65 777a 6f69 5a06 6e65   ...Z.newzoiZ.ne
-00000990: 7765 7874 da03 7265 7472 0c00 0000 720c  wext..retr....r.
-000009a0: 0000 0072 0d00 0000 7225 0000 004f 0000  ...r....r%...O..
-000009b0: 0073 4400 0000 0001 0401 0601 0601 0601  .sD.............
-000009c0: 0a02 0601 0601 0601 0601 0e01 0801 0402  ................
-000009d0: 0801 1001 1201 0801 0401 0802 1001 1201  ................
-000009e0: 0801 0e02 0c01 0801 0201 0801 0a01 0401  ................
-000009f0: 0401 0601 1001 0a01 0c01 7225 0000 0063  ..........r%...c
-00000a00: 0600 0000 0000 0000 0000 0000 2000 0000  ............ ...
-00000a10: 0b00 0000 4300 0000 737a 0100 007c 0164  ....C...sz...|.d
-00000a20: 0064 0185 0219 007d 067c 0164 0264 0085  .d.....}.|.d.d..
-00000a30: 0219 007d 0774 006a 0174 027c 0183 0174  ...}.t.j.t.|...t
-00000a40: 0364 038d 027d 087c 007c 0219 007d 097c  .d...}.|.|...}.|
-00000a50: 007c 0119 007d 0a7c 097c 0a18 007d 0b74  .|...}.|.|...}.t
-00000a60: 00a0 047c 09a1 017d 0c74 00a0 047c 0aa1  ...|...}.t...|..
-00000a70: 017d 0d74 00a0 0474 00a0 047c 0aa1 017c  .}.t...t...|...|
-00000a80: 051b 00a1 017d 0e74 00a0 047c 00a1 017d  .....}.t...|...}
-00000a90: 0f74 057c 067c 077c 097c 0a7c 037c 0b7c  .t.|.|.|.|.|.|.|
-00000aa0: 0c7c 0d7c 0e7c 0483 0a7d 1074 067c 1083  .|.|.|...}.t.|..
-00000ab0: 0144 005d de5c 027d 115c 0a7d 127d 137d  .D.].\.}.\.}.}.}
-00000ac0: 147d 157d 167d 177d 187d 197d 1a7d 1b74  .}.}.}.}.}.}.}.t
-00000ad0: 00a0 0164 04a1 017d 1c7c 1464 056b 047c  ...d...}.|.d.k.|
-00000ae0: 1c64 063c 007c 1564 076b 007c 1c64 023c  .d.<.|.d.k.|.d.<
-00000af0: 007c 1664 086b 0070 e27c 1664 096b 047c  .|.d.k.p.|.d.k.|
-00000b00: 1c64 0a3c 007c 1b64 076b 0070 f67c 1b64  .d.<.|.d.k.p.|.d
-00000b10: 096b 047c 1c64 0b3c 007c 1764 076b 007c  .k.|.d.<.|.d.k.|
-00000b20: 1c64 0c3c 007c 0f7c 127c 1385 0219 007d  .d.<.|.|.|.....}
-00000b30: 1d7c 1d7c 1d64 066b 0019 007d 1e74 00a0  .|.|.d.k...}.t..
-00000b40: 077c 1ea1 017d 1f7c 1f64 0d6b 007c 1c64  .|...}.|.d.k.|.d
-00000b50: 0e3c 0074 087c 1883 0164 076b 047c 1c64  .<.t.|...d.k.|.d
-00000b60: 0f3c 0074 087c 1983 0164 076b 047c 1c64  .<.t.|...d.k.|.d
-00000b70: 103c 0074 087c 1a83 0164 116b 047c 1c64  .<.t.|...d.k.|.d
-00000b80: 123c 0074 00a0 097c 1ca1 017c 087c 113c  .<.t...|...|.|.<
-00000b90: 0071 967c 0853 0029 134e 720f 0000 0072  .q.|.S.).Nr....r
-00000ba0: 1000 0000 7211 0000 00e9 0900 0000 692c  ....r.........i,
-00000bb0: 0100 0072 0100 0000 e914 0000 00e9 1e00  ...r............
-00000bc0: 0000 e9c8 0000 00e9 0200 0000 e903 0000  ................
-00000bd0: 00e9 0400 0000 69d8 ffff ffe9 0500 0000  ......i.........
-00000be0: e906 0000 00e9 0700 0000 671f 85eb 51b8  ..........g...Q.
-00000bf0: 1ee5 3fe9 0800 0000 290a 7214 0000 0072  ..?.....).r....r
-00000c00: 1500 0000 7213 0000 00da 0462 6f6f 6cda  ....r......bool.
-00000c10: 0464 6966 6672 1800 0000 7217 0000 0072  .diffr....r....r
-00000c20: 1900 0000 da03 6162 73da 0361 6e79 2920  ......abs..any) 
-00000c30: 7207 0000 0072 0a00 0000 720b 0000 00da  r....r....r.....
-00000c40: 036d 6170 da02 6872 7208 0000 0072 1a00  .map..hrr....r..
-00000c50: 0000 721b 0000 00da 0373 7169 722a 0000  ..r......sqir*..
-00000c60: 0072 2900 0000 da02 7070 5a04 6473 7973  .r).....ppZ.dsys
-00000c70: 5a04 6464 6961 5a03 6464 745a 0764 7661  Z.ddiaZ.ddtZ.dva
-00000c80: 6c75 6573 da06 7061 7261 6d73 721e 0000  lues..paramsr...
-00000c90: 00da 0669 7374 6172 74da 0569 7374 6f70  ...istart..istop
-00000ca0: 5a04 6973 7973 5a04 6964 6961 5a05 696d  Z.isysZ.idiaZ.im
-00000cb0: 6561 6e5a 0369 7070 5a05 6964 7379 735a  eanZ.ippZ.idsysZ
-00000cc0: 0569 6464 6961 5a04 6964 6474 5a03 6968  .iddiaZ.iddtZ.ih
-00000cd0: 72da 0863 7269 7465 7269 61da 0673 6c6f  r..criteria..slo
-00000ce0: 7065 735a 096e 6567 736c 6f70 6573 5a08  pesZ.negslopesZ.
-00000cf0: 6e65 6773 6c6f 7065 720c 0000 0072 0c00  negsloper....r..
-00000d00: 0000 720d 0000 00da 1263 616c 635f 7175  ..r......calc_qu
-00000d10: 616c 6974 795f 696e 6465 7878 0000 0073  ality_indexx...s
-00000d20: 3c00 0000 0002 0c01 0c01 1202 0801 0801  <...............
-00000d30: 0801 0a01 0a01 1401 0a02 1a04 06fd 0601  ................
-00000d40: 0201 1602 0a01 0c01 0c01 1401 1401 0c01  ................
-00000d50: 0c01 0c01 0a01 0c01 1001 1001 1001 1001  ................
-00000d60: 7268 0000 0029 0146 290b da05 6e75 6d70  rh...).F)...nump
-00000d70: 7972 1400 0000 da14 7068 7973 696f 6375  yr......physiocu
-00000d80: 7276 652e 7072 6573 7375 7265 7202 0000  rve.pressurer...
-00000d90: 0072 0e00 0000 7221 0000 0072 0500 0000  .r....r!...r....
-00000da0: 7231 0000 0072 0600 0000 7225 0000 0072  r1...r....r%...r
-00000db0: 6800 0000 720c 0000 0072 0c00 0000 720c  h...r....r....r.
-00000dc0: 0000 0072 0d00 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000dd0: 653e 0100 0000 7310 0000 0008 010c 0308  e>....s.........
-00000de0: 0708 0b08 1008 0508 230a 29              ........#.)
+00000020: 0003 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
+00000030: 6401 6c00 5a01 6402 6403 8400 5a02 6404  d.l.Z.d.d...Z.d.
+00000040: 6405 8400 5a03 6406 6407 8400 5a04 640d  d...Z.d.d...Z.d.
+00000050: 6409 640a 8401 5a05 640b 640c 8400 5a06  d.d...Z.d.d...Z.
+00000060: 6401 5300 290e e900 0000 004e 6303 0000  d.S.)......Nc...
+00000070: 0000 0000 0000 0000 000e 0000 0008 0000  ................
+00000080: 0043 0000 0073 a800 0000 7c02 6401 6402  .C...s....|.d.d.
+00000090: 8502 1900 7d03 7c02 6403 6400 8502 1900  ....}.|.d.d.....
+000000a0: 7d04 7400 6404 7c01 1400 8301 7d05 7401  }.t.d.|.....}.t.
+000000b0: 7c03 8301 7d06 7402 6a03 7c06 7402 6a04  |...}.t.j.|.t.j.
+000000c0: 6405 8d02 7d07 7402 6a03 7c06 7402 6a04  d...}.t.j.|.t.j.
+000000d0: 6405 8d02 7d08 7405 7406 7c03 7c04 8302  d...}.t.t.|.|...
+000000e0: 8301 4400 5d44 5c02 7d09 5c02 7d0a 7d0b  ..D.]D\.}.\.}.}.
+000000f0: 7c0b 7c0a 1800 7d0c 7c0a 7c0c 1800 7d0d  |.|...}.|.|...}.
+00000100: 7407 7c00 7c0a 7c0d 7c05 8304 7c07 7c09  t.|.|.|.|...|.|.
+00000110: 3c00 7407 7c00 7c0a 7c0b 7c05 6406 6407  <.t.|.|.|.|.d.d.
+00000120: 8d05 7c08 7c09 3c00 715a 7c07 7c08 6602  ..|.|.<.qZ|.|.f.
+00000130: 5300 2908 4e72 0100 0000 e9ff ffff ffe9  S.).Nr..........
+00000140: 0100 0000 679a 9999 9999 99a9 3fa9 01da  ....g.......?...
+00000150: 0564 7479 7065 5429 01da 0973 6561 7263  .dtypeT)...searc
+00000160: 686d 6178 2908 da03 696e 74da 036c 656e  hmax)...int..len
+00000170: da02 6e70 da05 7a65 726f 73da 0569 6e74  ..np..zeros..int
+00000180: 3634 da09 656e 756d 6572 6174 65da 037a  64..enumerate..z
+00000190: 6970 da12 6669 6e64 5f6c 6f63 616c 5f65  ip..find_local_e
+000001a0: 7874 7265 6d65 290e da06 7661 6c75 6573  xtreme)...values
+000001b0: da0a 7361 6d70 6c65 7261 7465 5a07 6665  ..samplerateZ.fe
+000001c0: 6574 6964 78da 0673 7461 7274 73da 0573  etidx..starts..s
+000001d0: 746f 7073 da0a 7769 6e64 6f77 7369 7a65  tops..windowsize
+000001e0: da07 6e76 616c 7565 73da 0364 6961 da03  ..nvalues..dia..
+000001f0: 7379 73da 0169 da05 7374 6172 74da 0473  sys..i..start..s
+00000200: 746f 70da 0864 7572 6174 696f 6e5a 0764  top..durationZ.d
+00000210: 6961 7374 6f70 a900 721b 0000 00fa 3b2f  iastop..r.....;/
+00000220: 686f 6d65 2f6a 616a 2f64 6576 656c 2f70  home/jaj/devel/p
+00000230: 6879 7369 6f63 7572 7665 2f70 6879 7369  hysiocurve/physi
+00000240: 6f63 7572 7665 2f70 7265 7373 7572 652f  ocurve/pressure/
+00000250: 696e 6379 636c 652e 7079 da0c 6669 6e64  incycle.py..find
+00000260: 5f64 6961 5f73 7973 0700 0000 7318 0000  _dia_sys....s...
+00000270: 0000 010c 010c 010c 0108 0110 0110 011a  ................
+00000280: 0108 0108 0112 0118 0172 1d00 0000 6303  .........r....c.
+00000290: 0000 0000 0000 0000 0000 0003 0000 0005  ................
+000002a0: 0000 0043 0000 0073 1400 0000 7400 a001  ...C...s....t...
+000002b0: 7c01 7c00 1800 7c02 7c00 1800 a102 5300  |.|...|.|.....S.
+000002c0: 2901 4e29 0272 0900 0000 da05 6372 6f73  ).N).r......cros
+000002d0: 7329 03da 026c 31da 026c 32da 0170 721b  s)...l1..l2..pr.
+000002e0: 0000 0072 1b00 0000 721c 0000 00da 0864  ...r....r......d
+000002f0: 6973 7461 6e63 6517 0000 0073 0200 0000  istance....s....
+00000300: 0001 7222 0000 0063 0300 0000 0000 0000  ..r"...c........
+00000310: 0000 0000 0f00 0000 0600 0000 4300 0000  ............C...
+00000320: 73f8 0000 0074 007c 0183 0144 005d 185c  s....t.|...D.].\
+00000330: 027d 037d 047c 047c 0264 0119 006b 0472  .}.}.|.|.d...k.r
+00000340: 0801 0071 3071 0874 016a 0264 0174 0364  ...q0q.t.j.d.t.d
+00000350: 028d 0253 007c 017c 0364 0085 0219 007d  ...S.|.|.d.....}
+00000360: 0174 047c 0183 017d 0574 016a 027c 0574  .t.|...}.t.j.|.t
+00000370: 016a 0564 028d 027d 0674 0074 067c 017c  .j.d...}.t.t.|.|
+00000380: 0283 0283 0144 005d 905c 027d 075c 027d  .....D.].\.}.\.}
+00000390: 087d 097c 007c 097c 0885 0219 007d 0a74  .}.|.|.|.....}.t
+000003a0: 047c 0a83 0173 8471 6274 01a0 0764 017c  .|...s.qbt...d.|
+000003b0: 0a64 0119 0067 02a1 017d 0b74 01a0 077c  .d...g...}.t...|
+000003c0: 087c 0918 007c 0a64 0319 0067 02a1 017d  .|...|.d...g...}
+000003d0: 0c74 01a0 0874 047c 0a83 01a1 017d 0d74  .t...t.|.....}.t
+000003e0: 01a0 097c 0d7c 0a66 02a1 016a 0a7d 0e74  ...|.|.f...j.}.t
+000003f0: 0b7c 0b7c 0c7c 0e83 037d 0474 047c 0483  .|.|.|...}.t.|..
+00000400: 0173 e071 627c 0974 01a0 0c7c 04a1 0117  .s.qb|.t...|....
+00000410: 007c 067c 073c 0071 627c 0653 0029 044e  .|.|.<.qb|.S.).N
+00000420: 7201 0000 0072 0400 0000 7202 0000 0029  r....r....r....)
+00000430: 0d72 0c00 0000 7209 0000 0072 0a00 0000  .r....r....r....
+00000440: 7207 0000 0072 0800 0000 720b 0000 0072  r....r....r....r
+00000450: 0d00 0000 da05 6172 7261 79da 0661 7261  ......array..ara
+00000460: 6e67 65da 0676 7374 6163 6bda 0154 7222  nge..vstack..Tr"
+00000470: 0000 00da 0661 7267 6d69 6e29 0f72 0f00  .....argmin).r..
+00000480: 0000 da06 6469 6169 6478 da06 7379 7369  ....diaidx..sysi
+00000490: 6478 da01 6eda 0164 7214 0000 00da 0464  dx..n..dr......d
+000004a0: 6963 7372 1700 0000 da02 6469 da02 7369  icsr......di..si
+000004b0: 5a03 7a6f 69da 0270 31da 0270 325a 067a  Z.zoi..p1..p2Z.z
+000004c0: 6f69 6964 785a 0270 3372 1b00 0000 721b  oiidxZ.p3r....r.
+000004d0: 0000 0072 1c00 0000 da0e 6669 6e64 5f64  ...r......find_d
+000004e0: 6963 726f 7469 6373 1c00 0000 7328 0000  icrotics....s(..
+000004f0: 0000 0210 010c 0106 030e 010c 0208 0110  ................
+00000500: 011a 010c 0108 0102 0112 0116 020e 0110  ................
+00000510: 020c 0108 0102 0114 0172 3100 0000 4663  .........r1...Fc
+00000520: 0500 0000 0000 0000 0000 0000 1400 0000  ................
+00000530: 0400 0000 4300 0000 7328 0100 007c 0472  ....C...s(...|.r
+00000540: 2074 006a 017d 0574 006a 027d 0674 006a   t.j.}.t.j.}.t.j
+00000550: 037d 0774 006a 040b 007d 086e 1874 006a  .}.t.j...}.n.t.j
+00000560: 057d 0574 006a 067d 0674 006a 077d 0774  .}.t.j.}.t.j.}.t
+00000570: 006a 047d 0874 00a0 087c 027c 0118 00a1  .j.}.t...|.|....
+00000580: 017d 097c 0964 016b 0272 527c 0053 007c  .}.|.d.k.rR|.S.|
+00000590: 037c 0914 007d 0a74 097c 027c 0118 007c  .|...}.t.|.|...|
+000005a0: 0a1b 0083 017d 0b7c 0174 00a0 0a7c 0ba1  .....}.|.t...|..
+000005b0: 017c 0a14 0017 007d 0c74 0b7c 0c83 0173  .|.....}.t.|...s
+000005c0: 8864 0153 007c 0c7c 0a17 007d 0d74 006a  .d.S.|.|...}.t.j
+000005d0: 0c64 027c 006a 0d64 038d 027d 0e74 0e7c  .d.|.j.d...}.t.|
+000005e0: 0c7c 0d83 0244 005d 525c 027d 0f7d 107c  .|...D.]R\.}.}.|
+000005f0: 0964 016b 0472 c87c 007c 0f7c 1085 0219  .d.k.r.|.|.|....
+00000600: 007d 116e 0c7c 007c 107c 0f85 0219 007d  .}.n.|.|.|.....}
+00000610: 1174 0b7c 1183 0173 de71 aa7c 057c 1183  .t.|...s.q.|.|..
+00000620: 017d 127c 077c 127c 0883 0272 f401 0071  .}.|.|.|...r...q
+00000630: fe7c 127d 087c 117d 0e71 aa7c 0f7c 0a18  .|.}.|.}.q.|.|..
+00000640: 007c 067c 0e83 0117 007d 137c 0964 016b  .|.|.....}.|.d.k
+00000650: 0090 0172 247c 1374 0b7c 0e83 0118 007d  ...r$|.t.|.....}
+00000660: 137c 1353 0029 044e 7201 0000 0072 0300  .|.S.).Nr....r..
+00000670: 0000 7204 0000 0029 0f72 0900 0000 da03  ..r....).r......
+00000680: 6d61 78da 0661 7267 6d61 78da 0a6c 6573  max..argmax..les
+00000690: 735f 6571 7561 6cda 0369 6e66 da03 6d69  s_equal..inf..mi
+000006a0: 6e72 2700 0000 da0d 6772 6561 7465 725f  nr'.....greater_
+000006b0: 6571 7561 6cda 0473 6967 6e72 0700 0000  equal..signr....
+000006c0: 7224 0000 0072 0800 0000 720a 0000 0072  r$...r....r....r
+000006d0: 0500 0000 720d 0000 0029 14da 0161 da05  ....r....)...a..
+000006e0: 6265 6769 6eda 0365 6e64 7213 0000 0072  begin..endr....r
+000006f0: 0600 0000 5a05 6665 7874 725a 0866 6172  ....Z.fextrZ.far
+00000700: 6765 7874 72da 0566 636f 6d70 5a06 6375  gextr..fcompZ.cu
+00000710: 7265 7874 da09 6469 7265 6374 696f 6eda  rext..direction.
+00000720: 0473 7465 705a 086e 7769 6e64 6f77 7372  .stepZ.nwindowsr
+00000730: 1100 0000 7212 0000 005a 0767 6f6f 647a  ....r....Z.goodz
+00000740: 6f69 7218 0000 0072 1900 0000 5a06 6e65  oir....r....Z.ne
+00000750: 777a 6f69 5a06 6e65 7765 7874 da03 7265  wzoiZ.newext..re
+00000760: 7472 1b00 0000 721b 0000 0072 1c00 0000  tr....r....r....
+00000770: 720e 0000 003a 0000 0073 4400 0000 0001  r....:...sD.....
+00000780: 0401 0601 0601 0601 0a02 0601 0601 0601  ................
+00000790: 0601 0e01 0801 0402 0801 1001 1201 0801  ................
+000007a0: 0401 0802 1001 1201 0801 0e02 0c01 0801  ................
+000007b0: 0201 0801 0a01 0401 0401 0601 1001 0a01  ................
+000007c0: 0c01 720e 0000 0063 0600 0000 0000 0000  ..r....c........
+000007d0: 0000 0000 2000 0000 0b00 0000 4300 0000  .... .......C...
+000007e0: 737a 0100 007c 0164 0064 0185 0219 007d  sz...|.d.d.....}
+000007f0: 067c 0164 0264 0085 0219 007d 0774 006a  .|.d.d.....}.t.j
+00000800: 0174 027c 0183 0174 0364 038d 027d 087c  .t.|...t.d...}.|
+00000810: 007c 0219 007d 097c 007c 0119 007d 0a7c  .|...}.|.|...}.|
+00000820: 097c 0a18 007d 0b74 00a0 047c 09a1 017d  .|...}.t...|...}
+00000830: 0c74 00a0 047c 0aa1 017d 0d74 00a0 0474  .t...|...}.t...t
+00000840: 00a0 047c 0aa1 017c 051b 00a1 017d 0e74  ...|...|.....}.t
+00000850: 00a0 047c 00a1 017d 0f74 057c 067c 077c  ...|...}.t.|.|.|
+00000860: 097c 0a7c 037c 0b7c 0c7c 0d7c 0e7c 0483  .|.|.|.|.|.|.|..
+00000870: 0a7d 1074 067c 1083 0144 005d de5c 027d  .}.t.|...D.].\.}
+00000880: 115c 0a7d 127d 137d 147d 157d 167d 177d  .\.}.}.}.}.}.}.}
+00000890: 187d 197d 1a7d 1b74 00a0 0164 04a1 017d  .}.}.}.t...d...}
+000008a0: 1c7c 1464 056b 047c 1c64 063c 007c 1564  .|.d.k.|.d.<.|.d
+000008b0: 076b 007c 1c64 023c 007c 1664 086b 0070  .k.|.d.<.|.d.k.p
+000008c0: e27c 1664 096b 047c 1c64 0a3c 007c 1b64  .|.d.k.|.d.<.|.d
+000008d0: 076b 0070 f67c 1b64 096b 047c 1c64 0b3c  .k.p.|.d.k.|.d.<
+000008e0: 007c 1764 076b 007c 1c64 0c3c 007c 0f7c  .|.d.k.|.d.<.|.|
+000008f0: 127c 1385 0219 007d 1d7c 1d7c 1d64 066b  .|.....}.|.|.d.k
+00000900: 0019 007d 1e74 00a0 077c 1ea1 017d 1f7c  ...}.t...|...}.|
+00000910: 1f64 0d6b 007c 1c64 0e3c 0074 087c 1883  .d.k.|.d.<.t.|..
+00000920: 0164 076b 047c 1c64 0f3c 0074 087c 1983  .d.k.|.d.<.t.|..
+00000930: 0164 076b 047c 1c64 103c 0074 087c 1a83  .d.k.|.d.<.t.|..
+00000940: 0164 116b 047c 1c64 123c 0074 00a0 097c  .d.k.|.d.<.t...|
+00000950: 1ca1 017c 087c 113c 0071 967c 0853 0029  ...|.|.<.q.|.S.)
+00000960: 134e 7202 0000 0072 0300 0000 7204 0000  .Nr....r....r...
+00000970: 00e9 0900 0000 692c 0100 0072 0100 0000  ......i,...r....
+00000980: e914 0000 00e9 1e00 0000 e9c8 0000 00e9  ................
+00000990: 0200 0000 e903 0000 00e9 0400 0000 69d8  ..............i.
+000009a0: ffff ffe9 0500 0000 e906 0000 00e9 0700  ................
+000009b0: 0000 671f 85eb 51b8 1ee5 3fe9 0800 0000  ..g...Q...?.....
+000009c0: 290a 7209 0000 0072 0a00 0000 7208 0000  ).r....r....r...
+000009d0: 00da 0462 6f6f 6cda 0464 6966 6672 0d00  ...bool..diffr..
+000009e0: 0000 720c 0000 00da 076e 616e 6d65 616e  ..r......nanmean
+000009f0: da03 6162 73da 0361 6e79 2920 720f 0000  ..abs..any) r...
+00000a00: 0072 2800 0000 7229 0000 00da 036d 6170  .r(...r).....map
+00000a10: da02 6872 7210 0000 005a 0873 7461 7274  ..hrr....Z.start
+00000a20: 6964 78da 0665 6e64 6964 78da 0373 7169  idx..endidx..sqi
+00000a30: 7216 0000 0072 1500 0000 da02 7070 5a04  r....r......ppZ.
+00000a40: 6473 7973 5a04 6464 6961 5a03 6464 745a  dsysZ.ddiaZ.ddtZ
+00000a50: 0764 7661 6c75 6573 da06 7061 7261 6d73  .dvalues..params
+00000a60: 7217 0000 00da 0669 7374 6172 74da 0569  r......istart..i
+00000a70: 7374 6f70 5a04 6973 7973 5a04 6964 6961  stopZ.isysZ.idia
+00000a80: 5a05 696d 6561 6e5a 0369 7070 5a05 6964  Z.imeanZ.ippZ.id
+00000a90: 7379 735a 0569 6464 6961 5a04 6964 6474  sysZ.iddiaZ.iddt
+00000aa0: 5a03 6968 72da 0863 7269 7465 7269 61da  Z.ihr..criteria.
+00000ab0: 0673 6c6f 7065 735a 096e 6567 736c 6f70  .slopesZ.negslop
+00000ac0: 6573 5a08 6e65 6773 6c6f 7065 721b 0000  esZ.negsloper...
+00000ad0: 0072 1b00 0000 721c 0000 00da 1263 616c  .r....r......cal
+00000ae0: 635f 7175 616c 6974 795f 696e 6465 7863  c_quality_indexc
+00000af0: 0000 0073 3c00 0000 0003 0c01 0c01 1202  ...s<...........
+00000b00: 0801 0801 0801 0a01 0a01 1401 0a02 1a04  ................
+00000b10: 06fd 0601 0201 1602 0a01 0c01 0c01 1401  ................
+00000b20: 1401 0c01 0c01 0c01 0a01 0c01 1001 1001  ................
+00000b30: 1001 1001 725a 0000 0029 0146 2907 da05  ....rZ...).F)...
+00000b40: 6e75 6d70 7972 0900 0000 721d 0000 0072  numpyr....r....r
+00000b50: 2200 0000 7231 0000 0072 0e00 0000 725a  "...r1...r....rZ
+00000b60: 0000 0072 1b00 0000 721b 0000 0072 1b00  ...r....r....r..
+00000b70: 0000 721c 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000b80: 3e01 0000 0073 0a00 0000 0806 0810 0805  >....s..........
+00000b90: 081e 0a29                                ...)
```

### Comparing `physiocurve-2022.7.8/physiocurve/pressure/incycle.py` & `physiocurve-2024.5.7/physiocurve/pressure/incycle.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,13 @@
 import numpy as np
-from physiocurve.pressure import foot
 
+# from numba import njit
 
-def find_pressure_full(values, samplerate):
-    feetidx = foot.find_pressure_feet(values, samplerate)
-    diaidx, sysidx = find_dia_sys(values, samplerate, feetidx)
-    dicidx = find_dicrotics(values, diaidx, sysidx)
-    return [feetidx, diaidx, sysidx, dicidx]
 
-
-def calc_means(values, diaidx):
-    startidx = diaidx[:-1]
-    endidx = diaidx[1:]
-    nvalues = len(diaidx) - 1
-    means = np.zeros(nvalues, dtype=np.float)
-    for i, (start, stop) in enumerate(zip(startidx, endidx)):
-        means[i] = np.nanmean(values[start:stop])
-    return means
-
-
-# @njit(parallel=True)
+# @njit
 def find_dia_sys(values, samplerate, feetidx):
     starts = feetidx[0:-1]
     stops = feetidx[1:]
     windowsize = int(0.05 * samplerate)
     nvalues = len(starts)
     dia = np.zeros(nvalues, dtype=np.int64)
     sys = np.zeros(nvalues, dtype=np.int64)
@@ -31,51 +15,46 @@
         duration = stop - start
         diastop = start - duration
         dia[i] = find_local_extreme(values, start, diastop, windowsize)
         sys[i] = find_local_extreme(values, start, stop, windowsize, searchmax=True)
     return (dia, sys)
 
 
-# @njit(parallel=True)
+# @njit
 def distance(l1, l2, p):
     return np.cross(l2 - l1, p - l1)  # / np.linalg.norm(l2 - l1)
 
 
-# @njit(parallel=True)
+# @njit
 def find_dicrotics(values, diaidx, sysidx):
     # Start from sys
     for n, d in enumerate(diaidx):  # noqa: B007
         if d > sysidx[0]:
             break
     else:
         # No break condition -> no cycle
-        return np.empty(0, dtype=int)
+        return np.zeros(0, dtype=int)
     diaidx = diaidx[n:]
 
     nvalues = len(diaidx)
     dics = np.zeros(nvalues, dtype=np.int64)
     for i, (di, si) in enumerate(zip(diaidx, sysidx)):
         zoi = values[si:di]
         if not len(zoi):
             continue
         p1 = np.array([0, zoi[0]])
         p2 = np.array([di - si, zoi[-1]])
 
-        # partidx = np.arange(int(len(zoi) / 3))
-        # partzoi = zoi[zoiidx]
-        # p3 = np.vstack((zoiidx, partzoi)).T
         zoiidx = np.arange(len(zoi))
         p3 = np.vstack((zoiidx, zoi)).T
 
         d = distance(p1, p2, p3)
         if not len(d):
             continue
         dics[i] = si + np.argmin(d)
-    # Remove zero values corresponding to not found dic
-    # return dics[dics.astype(bool)]
     return dics
 
 
 # @njit
 def find_local_extreme(a, begin, end, windowsize, searchmax=False):
     if searchmax:
         fextr = np.max
@@ -141,14 +120,14 @@
         criteria[0] = isys > 300
         criteria[1] = idia < 20
         criteria[2] = imean < 30 or imean > 200
         criteria[3] = ihr < 20 or ihr > 200
         criteria[4] = ipp < 20
         slopes = dvalues[istart:istop]
         negslopes = slopes[slopes < 0]
-        negslope = np.nanmean(negslopes)
+        negslope = np.nanmean(negslopes) if len(negslopes > 0) else 0
         criteria[5] = negslope < -40
         criteria[6] = abs(idsys) > 20
         criteria[7] = abs(iddia) > 20
         criteria[8] = abs(iddt) > 0.66
         sqi[i] = np.any(criteria)
     return sqi
```

### Comparing `physiocurve-2022.7.8/physiocurve/pressure/wrapper.py` & `physiocurve-2024.5.7/physiocurve/pressure/wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from functools import cached_property
 
 import numpy as np
+
 from physiocurve.pressure import foot, incycle
 
 
 class Pressure:
     def __init__(self, values, samplerate):
         self._values = values
         self._samplerate = samplerate
@@ -12,15 +13,20 @@
     @property
     def samplerate(self):
         return self._samplerate
 
     @cached_property
     def argfeet(self):
         """Return the numerical index of feet."""
-        return foot.find_pressure_feet(self._values, self._samplerate)
+        return foot.find_derivative_feet(self._values, self._samplerate)
+
+    @cached_property
+    def argtanfeet(self):
+        """Return the numerical index of feet with intersection tangent method."""
+        return foot.find_tangent_feet(self._values, self.argdia, self.argsys)
 
     @cached_property
     def _argdiasys(self):
         return incycle.find_dia_sys(self._values, self._samplerate, self.argfeet)
 
     @property
     def argdia(self):
@@ -34,19 +40,25 @@
 
     @cached_property
     def argdic(self):
         return incycle.find_dicrotics(self._values, *self._argdiasys)
 
     @cached_property
     def means(self):
-        return incycle.calc_means(self._values, self.argdia)
+        feet = self.argfeet
+        cycles = zip(feet, feet[1:])
+        means = [np.mean(self._values[beg:end]) for beg, end in cycles]
+        return np.array(means)
 
     @cached_property
     def heartrate(self):
-        return foot.calc_heartrate(self.argfeet, self._samplerate)
+        dfeet = np.diff(self.argfeet)
+        dfeet_s = dfeet / self._samplerate
+        # Result in beats per minute
+        return 60 / dfeet_s
 
     @cached_property
     def sqi(self):
         return incycle.calc_quality_index(
             self._values,
             self.argdia,
             self.argsys,
@@ -65,8 +77,12 @@
         sysidx = np.zeros(self.argsys.shape[0], dtype=bool)
         sysidx[: idxok.shape[0]] = idxok
         syss = values[self.argsys[sysidx]]
 
         diaidx = np.zeros(self.argdia.shape[0], dtype=bool)
         diaidx[: idxok.shape[0]] = idxok
         dias = values[self.argdia[diaidx]]
-        return (dics - dias) / (syss - dias)
+
+        den =  np.where((syss - dias) != 0, syss - dias, np.inf)
+        result = (dics - dias) / den
+
+        return result
```

### Comparing `physiocurve-2022.7.8/pyproject.toml` & `physiocurve-2024.5.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "physiocurve"
-version = "2022.7.8"
+version = "2024.5.7"
 description = "Analyse biometric time series"
 authors = ["Jona Joachim <jona@joachim.cc>"]
 license = "ISC"
 readme = "README.md"
 repository = "https://framagit.org/jaj/physiocurve"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
-pandas = "^1.4.3"
-numba = "^0.55.2"
-neurokit2 = "^0.2.0"
+python = ">=3.9,<3.13"
+pandas = ">=2"
+numba = "^0.59.1"
+neurokit2 = "^0.2.7"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^4.0.1"
 flake8-bandit = "^3.0.0"
 safety = "^1.10.3"
 flake8-bugbear = "^22.4.25"
 Sphinx = "^5.0.1"
 sphinx-autodoc-typehints = "^1.18.2"
 flake8-docstrings = "^1.6.0"
 darglint = "^1.8.1"
+vulture = "^2.5"
+vermin = "^1.4.0"
+pytest = "^7.1.2"
 
 [tool.black]
 line-length = 88
 target-version = ['py38', 'py39', 'py310']
 skip-string-normalization = true
```

### Comparing `physiocurve-2022.7.8/PKG-INFO` & `physiocurve-2024.5.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: physiocurve
-Version: 2022.7.8
+Version: 2024.5.7
 Summary: Analyse biometric time series
 Home-page: https://framagit.org/jaj/physiocurve
 License: ISC
 Author: Jona Joachim
 Author-email: jona@joachim.cc
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: neurokit2 (>=0.2.0,<0.3.0)
-Requires-Dist: numba (>=0.55.2,<0.56.0)
-Requires-Dist: pandas (>=1.4.3,<2.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: neurokit2 (>=0.2.7,<0.3.0)
+Requires-Dist: numba (>=0.59.1,<0.60.0)
+Requires-Dist: pandas (>=2)
 Project-URL: Repository, https://framagit.org/jaj/physiocurve
 Description-Content-Type: text/markdown
 
 # physiocurve
 physiocurve is a library to analyze biometric time series such as ECG and pulse waves, often obtained from patient monitors.
```

