# Comparing `tmp/pyDEM-0.2.0.tar.gz` & `tmp/pyDEM-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyDEM-0.2.0.tar", last modified: Wed Jul 26 15:37:19 2017, max compression
+gzip compressed data, was "pyDEM-1.0.0.tar", last modified: Tue May  7 12:05:40 2024, max compression
```

## Comparing `pyDEM-0.2.0.tar` & `pyDEM-1.0.0.tar`

### file list

```diff
@@ -1,82 +1,38 @@
-drwxrwxrwx   0        0        0        0 2017-07-26 15:37:19.000000 pyDEM-0.2.0/
--rw-rw-rw-   0        0        0     1180 2017-06-23 19:14:53.000000 pyDEM-0.2.0/INSTALL.md
--rw-rw-rw-   0        0        0    10347 2017-06-23 19:14:53.000000 pyDEM-0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0      136 2017-06-23 19:14:53.000000 pyDEM-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      553 2017-07-26 15:37:19.000000 pyDEM-0.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2017-07-26 15:37:17.000000 pyDEM-0.2.0/pydem/
--rw-rw-rw-   0        0        0     7113 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/commandline_utils.py
-drwxrwxrwx   0        0        0        0 2017-07-26 15:37:17.000000 pyDEM-0.2.0/pydem/cyfuncs/
--rw-rw-rw-   0        0        0   424900 2017-07-26 15:33:34.000000 pyDEM-0.2.0/pydem/cyfuncs/cyutils.cpp
--rw-rw-rw-   0        0        0     8660 2017-07-26 15:25:27.000000 pyDEM-0.2.0/pydem/cyfuncs/cyutils.pyx
--rw-rw-rw-   0        0        0      598 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/cyfuncs/__init__.py
--rw-rw-rw-   0        0        0   111148 2017-07-26 15:25:27.000000 pyDEM-0.2.0/pydem/dem_processing.py
-drwxrwxrwx   0        0        0        0 2017-07-26 15:37:17.000000 pyDEM-0.2.0/pydem/examples/
--rw-rw-rw-   0        0        0     2257 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/examples/compare_tile_to_chunk.py
--rw-rw-rw-   0        0        0     7023 2017-07-26 15:25:27.000000 pyDEM-0.2.0/pydem/examples/compare_to_taudem.py
--rw-rw-rw-   0        0        0     8990 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/examples/cross-tile_process_manager_test.py
--rw-rw-rw-   0        0        0     1916 2017-07-26 15:25:27.000000 pyDEM-0.2.0/pydem/examples/process_array.py
--rw-rw-rw-   0        0        0     1739 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/examples/process_manager_directory.py
--rw-rw-rw-   0        0        0    38298 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/processing_manager.py
-drwxrwxrwx   0        0        0        0 2017-07-26 15:37:17.000000 pyDEM-0.2.0/pydem/reader/
--rw-rw-rw-   0        0        0     7373 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/reader/gdal_reader.py
--rw-rw-rw-   0        0        0   352579 2017-06-23 20:30:05.000000 pyDEM-0.2.0/pydem/reader/inpaint.cpp
--rw-rw-rw-   0        0        0     5439 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/reader/inpaint.pyx
--rw-rw-rw-   0        0        0    21561 2017-07-26 15:25:27.000000 pyDEM-0.2.0/pydem/reader/my_types.py
--rw-rw-rw-   0        0        0      598 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/reader/__init__.py
-drwxrwxrwx   0        0        0        0 2017-07-26 15:37:17.000000 pyDEM-0.2.0/pydem/taudem/
--rw-rw-rw-   0        0        0      618 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/README.md
--rw-rw-rw-   0        0        0     1127 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem.py
--rw-rw-rw-   0        0        0     1474 2017-06-23 20:30:29.000000 pyDEM-0.2.0/pydem/taudem/taudem.pyc
-drwxrwxrwx   0        0        0        0 2017-07-26 15:37:17.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/
--rw-rw-rw-   0        0        0   175256 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/aread8
--rw-rw-rw-   0        0        0   175256 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/areadinf
--rw-rw-rw-   0        0        0   183448 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/d8flowdir
--rw-rw-rw-   0        0        0   175256 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/d8flowpathextremeup
--rw-rw-rw-   0        0        0    76696 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/d8hdisttostrm
--rw-rw-rw-   0        0        0    80824 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/dinfavalanche
--rw-rw-rw-   0        0        0   175256 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/dinfconclimaccum
--rw-rw-rw-   0        0        0   175256 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/dinfdecayaccum
--rw-rw-rw-   0        0        0    97208 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/dinfdistdown
--rw-rw-rw-   0        0        0    93112 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/dinfdistup
--rw-rw-rw-   0        0        0   183448 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/dinfflowdir
--rw-rw-rw-   0        0        0    76696 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/dinfrevaccum
--rw-rw-rw-   0        0        0   179352 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/dinftranslimaccum
--rw-rw-rw-   0        0        0    76696 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/dinfupdependence
--rw-rw-rw-   0        0        0   183512 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/dropanalysis
--rw-rw-rw-   0        0        0   179352 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/gridnet
--rw-rw-rw-   0        0        0    72568 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/lengtharea
--rw-rw-rw-   0        0        0    35344 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/license.txt
--rw-rw-rw-   0        0        0   175256 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/moveoutletstostrm
--rw-rw-rw-   0        0        0    72600 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/peukerdouglas
--rw-rw-rw-   0        0        0    80760 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/pitremove
--rw-rw-rw-   0        0        0    72568 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/slopearea
--rw-rw-rw-   0        0        0    72568 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/slopearearatio
--rw-rw-rw-   0        0        0    76664 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/slopeavedown
--rw-rw-rw-   0        0        0   216312 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/streamnet
--rw-rw-rw-   0        0        0    72568 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Linux/threshold
-drwxrwxrwx   0        0        0        0 2017-07-26 15:37:19.000000 pyDEM-0.2.0/pydem/taudem/taudem_Windows/
--rwxrwxrwx   0        0        0    83968 2015-04-17 21:03:18.000000 pyDEM-0.2.0/pydem/taudem/taudem_Windows/AreaD8.exe
--rwxrwxrwx   0        0        0    83968 2015-04-17 21:03:18.000000 pyDEM-0.2.0/pydem/taudem/taudem_Windows/AreaDinf.exe
--rwxrwxrwx   0        0        0    57344 2015-04-17 21:03:18.000000 pyDEM-0.2.0/pydem/taudem/taudem_Windows/D8FlowDir.exe
--rwxrwxrwx   0        0        0    58368 2015-04-17 21:03:18.000000 pyDEM-0.2.0/pydem/taudem/taudem_Windows/DinfFlowDir.exe
--rw-rw-rw-   0        0        0    35344 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Windows/license.txt
--rw-rw-rw-   0        0        0   167936 2015-04-17 21:03:18.000000 pyDEM-0.2.0/pydem/taudem/taudem_Windows/mpich2mpi.dll
--rw-rw-rw-   0        0        0  1617920 2015-04-17 21:03:18.000000 pyDEM-0.2.0/pydem/taudem/taudem_Windows/mpich2nemesis.dll
--rwxrwxrwx   0        0        0    55808 2015-04-17 21:03:18.000000 pyDEM-0.2.0/pydem/taudem/taudem_Windows/PitRemove.exe
--rwxrwxrwx   0        0        0    47104 2015-04-17 21:03:18.000000 pyDEM-0.2.0/pydem/taudem/taudem_Windows/SlopeAreaRatio.exe
--rw-rw-rw-   0        0        0       62 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/taudem_Windows/taudem source.txt
--rw-rw-rw-   0        0        0      598 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/taudem/__init__.py
--rw-rw-rw-   0        0        0      734 2017-06-23 20:30:29.000000 pyDEM-0.2.0/pydem/taudem/__init__.pyc
--rw-rw-rw-   0        0        0    20330 2017-07-26 15:25:27.000000 pyDEM-0.2.0/pydem/test_pydem.py
--rw-rw-rw-   0        0        0    16634 2017-07-26 15:25:27.000000 pyDEM-0.2.0/pydem/utils.py
--rw-rw-rw-   0        0        0      598 2017-06-23 19:14:53.000000 pyDEM-0.2.0/pydem/__init__.py
-drwxrwxrwx   0        0        0        0 2017-07-26 15:37:17.000000 pyDEM-0.2.0/pyDEM.egg-info/
--rw-rw-rw-   0        0        0        1 2017-07-26 15:37:17.000000 pyDEM-0.2.0/pyDEM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2017-07-26 15:37:17.000000 pyDEM-0.2.0/pyDEM.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      553 2017-07-26 15:37:17.000000 pyDEM-0.2.0/pyDEM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       25 2017-07-26 15:37:17.000000 pyDEM-0.2.0/pyDEM.egg-info/requires.txt
--rw-rw-rw-   0        0        0     2339 2017-07-26 15:37:17.000000 pyDEM-0.2.0/pyDEM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        6 2017-07-26 15:37:17.000000 pyDEM-0.2.0/pyDEM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    16079 2017-07-26 15:28:53.000000 pyDEM-0.2.0/README.md
--rw-rw-rw-   0        0        0       92 2017-07-26 15:37:19.000000 pyDEM-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     3336 2017-07-26 15:33:23.000000 pyDEM-0.2.0/setup.py
+drwxrwsr-x   0 mpu       (1002) creare    (1001)        0 2024-05-07 12:05:40.929600 pyDEM-1.0.0/
+drwxrwsr-x   0 mpu       (1002) creare    (1001)        0 2024-05-07 12:05:40.925600 pyDEM-1.0.0/.pytest_cache/
+-rw-rw-r--   0 mpu       (1002) creare    (1001)      302 2024-05-06 19:47:19.000000 pyDEM-1.0.0/.pytest_cache/README.md
+-rw-rw-r--   0 mpu       (1002) creare    (1001)      594 2024-05-07 11:50:34.000000 pyDEM-1.0.0/INSTALL.md
+-rw-rw-r--   0 mpu       (1002) creare    (1001)    10172 2024-02-14 21:01:19.000000 pyDEM-1.0.0/LICENSE.txt
+-rw-rw-r--   0 mpu       (1002) creare    (1001)      130 2024-02-14 21:01:19.000000 pyDEM-1.0.0/MANIFEST.in
+-rw-rw-r--   0 mpu       (1002) creare    (1001)      500 2024-05-07 12:05:40.929600 pyDEM-1.0.0/PKG-INFO
+-rw-rw-r--   0 mpu       (1002) creare    (1001)    15280 2024-05-07 11:51:41.000000 pyDEM-1.0.0/README.md
+drwxrwsr-x   0 mpu       (1002) creare    (1001)        0 2024-05-07 12:05:40.925600 pyDEM-1.0.0/aws/
+-rw-rw-r--   0 mpu       (1002) creare    (1001)     6480 2024-05-07 11:50:34.000000 pyDEM-1.0.0/aws/handler.py
+-rw-rw-r--   0 mpu       (1002) creare    (1001)      899 2024-05-07 11:50:34.000000 pyDEM-1.0.0/aws/link_so.py
+-rw-rw-r--   0 mpu       (1002) creare    (1001)     2312 2024-05-07 11:50:34.000000 pyDEM-1.0.0/aws/mk_dist.py
+drwxrwsr-x   0 mpu       (1002) creare    (1001)        0 2024-05-07 12:05:40.925600 pyDEM-1.0.0/pyDEM.egg-info/
+-rw-rw-r--   0 mpu       (1002) creare    (1001)      500 2024-05-07 12:05:40.000000 pyDEM-1.0.0/pyDEM.egg-info/PKG-INFO
+-rw-rw-r--   0 mpu       (1002) creare    (1001)      706 2024-05-07 12:05:40.000000 pyDEM-1.0.0/pyDEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 mpu       (1002) creare    (1001)        1 2024-05-07 12:05:40.000000 pyDEM-1.0.0/pyDEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 mpu       (1002) creare    (1001)      154 2024-05-07 12:05:40.000000 pyDEM-1.0.0/pyDEM.egg-info/entry_points.txt
+-rw-rw-r--   0 mpu       (1002) creare    (1001)       60 2024-05-07 12:05:40.000000 pyDEM-1.0.0/pyDEM.egg-info/requires.txt
+-rw-rw-r--   0 mpu       (1002) creare    (1001)        6 2024-05-07 12:05:40.000000 pyDEM-1.0.0/pyDEM.egg-info/top_level.txt
+drwxrwsr-x   0 mpu       (1002) creare    (1001)        0 2024-05-07 12:05:40.925600 pyDEM-1.0.0/pydem/
+-rw-rw-r--   0 mpu       (1002) creare    (1001)      871 2024-05-07 11:50:34.000000 pyDEM-1.0.0/pydem/CHANGELOG.md
+-rw-rw-r--   0 mpu       (1002) creare    (1001)      670 2024-05-07 11:50:34.000000 pyDEM-1.0.0/pydem/__init__.py
+-rw-rw-r--   0 mpu       (1002) creare    (1001)     6969 2024-05-07 11:50:34.000000 pyDEM-1.0.0/pydem/commandline_utils.py
+drwxrwsr-x   0 mpu       (1002) creare    (1001)        0 2024-05-07 12:05:40.929600 pyDEM-1.0.0/pydem/cyfuncs/
+-rw-rw-r--   0 mpu       (1002) creare    (1001)      584 2024-02-14 21:01:19.000000 pyDEM-1.0.0/pydem/cyfuncs/__init__.py
+-rw-rw-r--   0 mpu       (1002) creare    (1001)   554822 2024-05-07 12:00:30.000000 pyDEM-1.0.0/pydem/cyfuncs/cyutils.cpp
+-rw-rw-r--   0 mpu       (1002) creare    (1001)     8956 2024-05-07 11:50:34.000000 pyDEM-1.0.0/pydem/cyfuncs/cyutils.pyx
+-rw-rw-r--   0 mpu       (1002) creare    (1001)    79499 2024-05-07 11:50:34.000000 pyDEM-1.0.0/pydem/dem_processing.py
+drwxrwsr-x   0 mpu       (1002) creare    (1001)        0 2024-05-07 12:05:40.929600 pyDEM-1.0.0/pydem/examples/
+-rw-rw-r--   0 mpu       (1002) creare    (1001)     1753 2024-05-07 11:50:34.000000 pyDEM-1.0.0/pydem/examples/process_array.py
+-rw-rw-r--   0 mpu       (1002) creare    (1001)     1452 2024-05-07 11:50:34.000000 pyDEM-1.0.0/pydem/examples/process_manager_directory.py
+-rw-rw-r--   0 mpu       (1002) creare    (1001)    56073 2024-05-07 11:50:34.000000 pyDEM-1.0.0/pydem/process_manager.py
+drwxrwsr-x   0 mpu       (1002) creare    (1001)        0 2024-05-07 12:05:40.929600 pyDEM-1.0.0/pydem/test/
+-rw-rw-r--   0 mpu       (1002) creare    (1001)    10760 2024-05-07 11:50:34.000000 pyDEM-1.0.0/pydem/test/test_end_to_end.py
+-rw-rw-r--   0 mpu       (1002) creare    (1001)    16177 2024-05-07 11:50:34.000000 pyDEM-1.0.0/pydem/utils.py
+-rw-rw-r--   0 mpu       (1002) creare    (1001)    19281 2024-05-07 11:50:34.000000 pyDEM-1.0.0/pydem/utils_test_pydem.py
+-rw-rw-r--   0 mpu       (1002) creare    (1001)       63 2024-05-07 12:05:40.929600 pyDEM-1.0.0/setup.cfg
+-rw-rw-r--   0 mpu       (1002) creare    (1001)     2930 2024-05-07 12:05:36.000000 pyDEM-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyDEM-0.2.0/LICENSE.txt` & `pyDEM-1.0.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,176 +1,176 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
    END OF TERMS AND CONDITIONS
```

### Comparing `pyDEM-0.2.0/pydem/commandline_utils.py` & `pyDEM-1.0.0/pydem/commandline_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-# -*- coding: utf-8 -*-
-"""
-   Copyright 2015 Creare
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
-"""
-
-def DinfFlowDir():
-    import argparse
-
-    parser = argparse.ArgumentParser(
-        description='Assigns a flow direction based on the D-infinity flow'
-        ' method using the steepest slope of a triangular facet (Tarboton, '
-        '1997, "A New Method for the Determination of Flow Directions and '
-        'Contributing Areas in Grid Digital Elevation Models," Water Resources'
-        ' Research, 33(2): 309-319).')
-    parser.add_argument('Input_Pit_Filled_Elevation',
-                        help='The input pit-filled elevation file in '
-                            'geotiff format.',
-                        )
-    parser.add_argument('Input_Number_of_Chunks',
-                        help="The approximate number of chunks that the input "
-                        'file will be divided into for processing (potentially'
-                        ' on multiple processors).', type=int, default=1, nargs='?')
-    parser.add_argument('Output_D_Infinity_Flow_Direction',
-                        help='Output filename for the flow direction. Default'
-                        ' value = ang.tif .', default='ang.tif', nargs='?')
-    parser.add_argument('Output_D_Infinity_Slope',
-                        help='Output filename for the flow direction. Default'
-                        ' value = mag.tif .', default='mag.tif', nargs='?')
-    args = parser.parse_args()
-    fn = args.Input_Pit_Filled_Elevation
-    n_chunks = args.Input_Number_of_Chunks
-    fn_ang = args.Output_D_Infinity_Flow_Direction
-    fn_mag = args.Output_D_Infinity_Slope
-
-    from pydem.dem_processing import DEMProcessor
-    dem_proc = DEMProcessor(fn)
-    shape = dem_proc.data.shape
-    chunk_size = max(shape[0],  shape[1]) / n_chunks
-    dem_proc.chunk_size_slp_dir = chunk_size
-    dem_proc.calc_slopes_directions()
-    dem_proc.save_array(dem_proc.mag, fn_mag, as_int=False)
-    dem_proc.save_array(dem_proc.direction, fn_ang, as_int=False)
-
-def AreaDinf():
-    import argparse
-
-    parser = argparse.ArgumentParser(
-        description='Calculates a grid of specific catchment area which is the'
-        ' contributing area per unit contour length using the multiple flow '
-        'direction D-infinity approach. Note, this is different from the '
-        'equivalent tauDEM function, in that it takes the elevation '
-        '(not the flow direction) as an input, and it calculates the '
-        'slope and direction as intermediate steps.')
-    parser.add_argument('Input_Pit_Filled_Elevation',
-                        help='The input pit-filled elevation file in '
-                            'geotiff format.',
-                        )
-    parser.add_argument('Input_Number_of_Chunks',
-                        help="The approximate number of chunks that the input "
-                        'file will be divided into for processing (potentially'
-                        ' on multiple processors).', type=int, default=1,
-                        nargs='?')
-    parser.add_argument('Output_D_Infinity_Specific_Catchment_Area',
-                        help='Output filename for the flow direction. Default'
-                        ' value = uca.tif .', default='uca.tif', nargs='?')
-    parser.add_argument('--save-all', '--sa',
-                        help='If set, will save all intermediate files as well.',
-                        action='store_true')
-    args = parser.parse_args()
-    fn = args.Input_Pit_Filled_Elevation
-    n_chunks = args.Input_Number_of_Chunks
-    fn_uca = args.Output_D_Infinity_Specific_Catchment_Area
-    sa = args.save_all
-
-    from pydem.dem_processing import DEMProcessor
-    dem_proc = DEMProcessor(fn)
-    shape = dem_proc.data.shape
-    chunk_size = max(shape[0],  shape[1]) / n_chunks
-    dem_proc.chunk_size_slp_dir = chunk_size
-    dem_proc.chunk_size_uca = chunk_size
-    dem_proc.calc_slopes_directions()
-    if sa:
-        dem_proc.save_array(dem_proc.mag, 'mag.tif', as_int=False)
-        dem_proc.save_array(dem_proc.direction, 'ang.tif', as_int=False)
-    dem_proc.calc_uca()
-    dem_proc.save_array(dem_proc.uca, fn_uca, as_int=False)
-
-def TWIDinf():
-    import argparse
-
-    parser = argparse.ArgumentParser(
-        description='Calculates a grid of topographic wetness index '
-        ' which is the log_e(uca / mag), that is, the natural log of the ratio'
-        ' of contributing area per unit contour length and the magnitude of '
-        ' the slope. Note, this function takes the elevation '
-        'as an input, and it calculates the '
-        'slope, direction, and contributing area as intermediate steps.')
-    parser.add_argument('Input_Pit_Filled_Elevation',
-                        help='The input pit-filled elevation file in '
-                            'geotiff format.',
-                        )
-    parser.add_argument('Input_Number_of_Chunks',
-                        help="The approximate number of chunks that the input "
-                        'file will be divided into for processing (potentially'
-                        ' on multiple processors).', type=int, default=1,
-                        nargs='?')
-    parser.add_argument('Output_D_Infinity_TWI',
-                        help='Output filename for the topographic wetness '
-                        'index. Default value = twi.tif .', default='twi.tif',
-                        nargs='?')
-    parser.add_argument('--save-all', '--sa',
-                        help='If set, will save all intermediate files as well.',
-                        action='store_true')
-    args = parser.parse_args()
-    fn = args.Input_Pit_Filled_Elevation
-    n_chunks = args.Input_Number_of_Chunks
-    fn_twi = args.Output_D_Infinity_TWI
-    sa = args.save_all
-
-    from pydem.dem_processing import DEMProcessor
-    dem_proc = DEMProcessor(fn)
-    shape = dem_proc.data.shape
-    chunk_size = max(shape[0],  shape[1]) / n_chunks
-    dem_proc.chunk_size_slp_dir = chunk_size
-    dem_proc.chunk_size_uca = chunk_size
-    dem_proc.calc_slopes_directions()
-    dem_proc.calc_uca()
-    if sa:
-        dem_proc.save_array(dem_proc.mag, 'mag.tif', as_int=False)
-        dem_proc.save_array(dem_proc.direction, 'ang.tif', as_int=False)
-        dem_proc.save_array(dem_proc.uca, 'uca.tif', as_int=False)
-    dem_proc.calc_twi()
-    dem_proc.save_array(dem_proc.twi, fn_twi, as_int=True)
-
-if __name__ == "__main__":
-#    DinfFlowDir()
-#    AreaDinf()
+# -*- coding: utf-8 -*-
+"""
+   Copyright 2015-2024 Creare
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
+"""
+
+def DinfFlowDir():
+    import argparse
+
+    parser = argparse.ArgumentParser(
+        description='Assigns a flow direction based on the D-infinity flow'
+        ' method using the steepest slope of a triangular facet (Tarboton, '
+        '1997, "A New Method for the Determination of Flow Directions and '
+        'Contributing Areas in Grid Digital Elevation Models," Water Resources'
+        ' Research, 33(2): 309-319).')
+    parser.add_argument('Input_Pit_Filled_Elevation',
+                        help='The input pit-filled elevation file in '
+                            'geotiff format.',
+                        )
+    parser.add_argument('Input_Number_of_Chunks',
+                        help="The approximate number of chunks that the input "
+                        'file will be divided into for processing (potentially'
+                        ' on multiple processors).', type=int, default=1, nargs='?')
+    parser.add_argument('Output_D_Infinity_Flow_Direction',
+                        help='Output filename for the flow direction. Default'
+                        ' value = ang.tif .', default='ang.tif', nargs='?')
+    parser.add_argument('Output_D_Infinity_Slope',
+                        help='Output filename for the flow direction. Default'
+                        ' value = mag.tif .', default='mag.tif', nargs='?')
+    args = parser.parse_args()
+    fn = args.Input_Pit_Filled_Elevation
+    n_chunks = args.Input_Number_of_Chunks
+    fn_ang = args.Output_D_Infinity_Flow_Direction
+    fn_mag = args.Output_D_Infinity_Slope
+
+    from pydem.dem_processing import DEMProcessor
+    dem_proc = DEMProcessor(fn)
+    shape = dem_proc.data.shape
+    chunk_size = max(shape[0],  shape[1]) / n_chunks
+    dem_proc.chunk_size_slp_dir = chunk_size
+    dem_proc.calc_slopes_directions()
+    dem_proc.save_array(dem_proc.mag, fn_mag, as_int=False)
+    dem_proc.save_array(dem_proc.direction, fn_ang, as_int=False)
+
+def AreaDinf():
+    import argparse
+
+    parser = argparse.ArgumentParser(
+        description='Calculates a grid of specific catchment area which is the'
+        ' contributing area per unit contour length using the multiple flow '
+        'direction D-infinity approach. Note, this is different from the '
+        'equivalent tauDEM function, in that it takes the elevation '
+        '(not the flow direction) as an input, and it calculates the '
+        'slope and direction as intermediate steps.')
+    parser.add_argument('Input_Pit_Filled_Elevation',
+                        help='The input pit-filled elevation file in '
+                            'geotiff format.',
+                        )
+    parser.add_argument('Input_Number_of_Chunks',
+                        help="The approximate number of chunks that the input "
+                        'file will be divided into for processing (potentially'
+                        ' on multiple processors).', type=int, default=1,
+                        nargs='?')
+    parser.add_argument('Output_D_Infinity_Specific_Catchment_Area',
+                        help='Output filename for the flow direction. Default'
+                        ' value = uca.tif .', default='uca.tif', nargs='?')
+    parser.add_argument('--save-all', '--sa',
+                        help='If set, will save all intermediate files as well.',
+                        action='store_true')
+    args = parser.parse_args()
+    fn = args.Input_Pit_Filled_Elevation
+    n_chunks = args.Input_Number_of_Chunks
+    fn_uca = args.Output_D_Infinity_Specific_Catchment_Area
+    sa = args.save_all
+
+    from pydem.dem_processing import DEMProcessor
+    dem_proc = DEMProcessor(fn)
+    shape = dem_proc.data.shape
+    chunk_size = max(shape[0],  shape[1]) / n_chunks
+    dem_proc.chunk_size_slp_dir = chunk_size
+    dem_proc.chunk_size_uca = chunk_size
+    dem_proc.calc_slopes_directions()
+    if sa:
+        dem_proc.save_array(dem_proc.mag, 'mag.tif', as_int=False)
+        dem_proc.save_array(dem_proc.direction, 'ang.tif', as_int=False)
+    dem_proc.calc_uca()
+    dem_proc.save_array(dem_proc.uca, fn_uca, as_int=False)
+
+def TWIDinf():
+    import argparse
+
+    parser = argparse.ArgumentParser(
+        description='Calculates a grid of topographic wetness index '
+        ' which is the log_e(uca / mag), that is, the natural log of the ratio'
+        ' of contributing area per unit contour length and the magnitude of '
+        ' the slope. Note, this function takes the elevation '
+        'as an input, and it calculates the '
+        'slope, direction, and contributing area as intermediate steps.')
+    parser.add_argument('Input_Pit_Filled_Elevation',
+                        help='The input pit-filled elevation file in '
+                            'geotiff format.',
+                        )
+    parser.add_argument('Input_Number_of_Chunks',
+                        help="The approximate number of chunks that the input "
+                        'file will be divided into for processing (potentially'
+                        ' on multiple processors).', type=int, default=1,
+                        nargs='?')
+    parser.add_argument('Output_D_Infinity_TWI',
+                        help='Output filename for the topographic wetness '
+                        'index. Default value = twi.tif .', default='twi.tif',
+                        nargs='?')
+    parser.add_argument('--save-all', '--sa',
+                        help='If set, will save all intermediate files as well.',
+                        action='store_true')
+    args = parser.parse_args()
+    fn = args.Input_Pit_Filled_Elevation
+    n_chunks = args.Input_Number_of_Chunks
+    fn_twi = args.Output_D_Infinity_TWI
+    sa = args.save_all
+
+    from pydem.dem_processing import DEMProcessor
+    dem_proc = DEMProcessor(fn)
+    shape = dem_proc.data.shape
+    chunk_size = max(shape[0],  shape[1]) / n_chunks
+    dem_proc.chunk_size_slp_dir = chunk_size
+    dem_proc.chunk_size_uca = chunk_size
+    dem_proc.calc_slopes_directions()
+    dem_proc.calc_uca()
+    if sa:
+        dem_proc.save_array(dem_proc.mag, 'mag.tif', as_int=False)
+        dem_proc.save_array(dem_proc.direction, 'ang.tif', as_int=False)
+        dem_proc.save_array(dem_proc.uca, 'uca.tif', as_int=False)
+    dem_proc.calc_twi()
+    dem_proc.save_array(dem_proc.twi, fn_twi, as_int=True)
+
+if __name__ == "__main__":
+#    DinfFlowDir()
+#    AreaDinf()
     TWIDinf()
```

### Comparing `pyDEM-0.2.0/pydem/cyfuncs/cyutils.pyx` & `pyDEM-1.0.0/pydem/cyfuncs/cyutils.pyx`

 * *Files 24% similar despite different names*

```diff
@@ -1,212 +1,226 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Tue Nov 04 17:11:16 2014
-
-@author: mpu
-"""
-
-import numpy as np
-cimport numpy as np
-
-ctypedef np.uint8_t DTYPEb_t
-ctypedef np.int64_t DTYPEi_t
-ctypedef np.int32_t DTYPEi32_t
-
-dtype_bool = 'uint8'
-
-#==============================================================================
-# Drain a single array's connections: If connected to start, change value
-#==============================================================================
-
-def drain_connections(np.ndarray[DTYPEb_t, ndim=1, cast=True] arr,
-                      np.ndarray[DTYPEb_t, ndim=1, cast=True] ids,
-                      np.ndarray[DTYPEi32_t, ndim=1] indptr,
-                      np.ndarray[DTYPEi32_t, ndim=1] indices, DTYPEb_t set_to=0):
-    cdef DTYPEi_t n_ids = ids.size
-    cdef DTYPEi_t n_A = indices.size
-
-    cdef np.ndarray[DTYPEb_t, ndim=1] ids_old = np.zeros(n_ids, dtype=dtype_bool)
-
-    _drain_connections(&(arr[0]), &(ids[0]), &(ids_old[0]),
-                       &(indptr[0]), &(indices[0]), n_ids, n_A, set_to)
-    return arr
-
-
-cdef void _drain_connections(DTYPEb_t *arr,
-                             DTYPEb_t *ids, DTYPEb_t *ids_old, DTYPEi32_t *indptr, DTYPEi32_t *indices,
-                             DTYPEi_t n_ids, DTYPEi_t n_A, DTYPEb_t tf):
-    cdef DTYPEi_t i = 0
-    cdef DTYPEi_t j = 0
-    cdef DTYPEb_t keep_going = 1
-    cdef DTYPEb_t *tmp
-    while keep_going: #If I use ids.sum() > 0 then I might get stuck in circular references.
-#        print "c",
-        # switch pointers
-        tmp = ids_old
-        ids_old = ids
-        ids = tmp
-
-        _zero_arr(ids, n_ids)
-        for i in xrange(n_ids):
-            if ids_old[i] == 0:
-                continue #If this id is not active, just skip the next part
-            for j in xrange(indptr[i], indptr[i + 1]):
-                row_id = indices[j]
-                ids[row_id] += arr[row_id] != tf
-                arr[row_id] = tf
-
-        keep_going = _check_id_changed(ids, ids_old, n_ids)
-
-
-#==============================================================================
-# Update area using the correct weighting factors and not double-dipping
-#==============================================================================
-def drain_area(np.ndarray[double, ndim=1] area,
-               np.ndarray[DTYPEb_t, ndim=1, cast=True] done,
-               np.ndarray[DTYPEb_t, ndim=1, cast=True] ids,
-               np.ndarray[DTYPEi32_t, ndim=1, cast=True] col_indptr,
-               np.ndarray[DTYPEi32_t, ndim=1, cast=True] col_indices,
-               np.ndarray[double, ndim=1] col_data,
-               np.ndarray[DTYPEi32_t, ndim=1, cast=True] row_indptr,
-               np.ndarray[DTYPEi32_t, ndim=1, cast=True] row_indices,
-               DTYPEi_t n_rows, DTYPEi_t n_cols,
-               np.ndarray[double, ndim=1, cast=True] edge_todo=None,
-               np.ndarray[double, ndim=1, cast=True] edge_todo_no_mask=None,
-               skip_edge=0):
-    cdef DTYPEi_t n_ids = ids.size
-    cdef DTYPEi_t n_A = col_indices.size
-
-    cdef DTYPEb_t do_edge_todo
-    if edge_todo is None:
-        edge_todo = np.zeros(1, dtype=float)
-        do_edge_todo = 0
-    else:
-        do_edge_todo = 1
-
-    cdef DTYPEb_t do_edge_todo_no_mask
-    if edge_todo_no_mask is None:
-        edge_todo_no_mask = np.zeros(1, dtype=float)
-        do_edge_todo_no_mask = 0
-    else:
-        do_edge_todo_no_mask = 1
-
-    cdef np.ndarray[DTYPEb_t, ndim=1] ids_old = np.zeros(n_ids, dtype=dtype_bool)
-
-    _drain_area(&(area[0]), &(done[0]), &(ids[0]), &(ids_old[0]),
-                       &(col_indptr[0]), &(col_indices[0]), &(col_data[0]),
-                       &(row_indptr[0]), &(row_indices[0]),
-                       n_rows, n_cols, n_ids, n_A,
-                       &(edge_todo[0]), do_edge_todo,
-                       &(edge_todo_no_mask[0]), do_edge_todo_no_mask,
-                       skip_edge)
-    return area, done, edge_todo.astype('bool'), edge_todo_no_mask.astype('bool')
-
-
-cdef void _drain_area(double *area, DTYPEb_t* done,
-                             DTYPEb_t *ids, DTYPEb_t *ids_old,
-                             DTYPEi32_t *col_indptr, DTYPEi32_t *col_indices, double *col_data,
-                             DTYPEi32_t *row_indptr, DTYPEi32_t *row_indices,
-                             DTYPEi_t n_rows, DTYPEi_t n_cols, DTYPEi_t n_ids, DTYPEi_t n_A,
-                             double* edge_todo, DTYPEb_t do_edge_todo,
-                             double* edge_todo_no_mask, DTYPEb_t do_edge_todo_no_mask,
-                             DTYPEi_t skip_edge):
-    cdef DTYPEi_t i = 0
-    cdef DTYPEi_t j = 0
-    cdef DTYPEb_t keep_going = 1
-    cdef DTYPEb_t *tmp
-    cdef double factor = 0
-    cdef DTYPEb_t wait_for_neighbors = 0
-    while keep_going: # If I use ids.sum() > 0 then I might get stuck in circular references.
-#        print "oc",
-        # Set the points that are about to be drained as done
-        # This has to be done before the next loop because the next candidates
-        # check to make sure that all the points that drain into them are done
-        for i in xrange(n_ids):
-            if ids[i]:
-                done[i] = 1
-#                print i, done[i]
-
-        # switch pointers
-        tmp = ids_old
-        ids_old = ids
-        ids = tmp
-
-        # Initialize array to zero for the points that will be drained next round
-        _zero_arr(ids, n_ids)
-
-        for i in xrange(n_ids):
-            if not ids_old[i]:
-                continue # If this id is not active, just skip the next part
-            for j in xrange(col_indptr[i], col_indptr[i + 1]):
-                row_id = col_indices[j]
-                factor = col_data[j]
-                # check if this is on the edge, if so, do not modify it and go
-                # to the next candidate
-                if ((skip_edge or (done[row_id])) and \
-                        _check_id_on_edge(row_id, n_rows, n_cols)):
-                    continue
-
-                area[row_id] += area[i] * factor
-                
-                if do_edge_todo:
-                    edge_todo[row_id] += edge_todo[i] * factor
-                if do_edge_todo_no_mask:
-                    edge_todo_no_mask[row_id] += edge_todo_no_mask[i] * factor
-
-                # If the point that has just been drained into has all its
-                # source points marked as done, then it can be drained next
-                # round
-                wait_for_neighbors = 0
-                for k in xrange(row_indptr[row_id], row_indptr[row_id+1]):
-                    col_id = row_indices[k]
-#                    print 'row', row_id, 'col', col_id, 'done', done[col_id]
-                    if done[col_id] < 1:
-                        wait_for_neighbors = 1
-                        break
-#                print wait_for_neighbors,
-                if wait_for_neighbors == 0:
-                    ids[row_id] = 1
-
-                if do_edge_todo:
-                    done[i] = 1
-
-        keep_going = _check_id_changed(ids, ids_old, n_ids)
-
-#==============================================================================
-# Helper functions
-#==============================================================================
-
-cdef DTYPEb_t _check_id_changed(DTYPEb_t *ids, DTYPEb_t *ids_old, DTYPEi_t n_ids):
-    cdef DTYPEi_t i
-    cdef DTYPEb_t ret = 0
-    for i in xrange(n_ids):
-        if ids[i] != ids_old[i]:
-            ret = 1
-            break
-    return ret
-
-cdef _zero_arr(DTYPEb_t *arr, DTYPEi_t n):
-    cdef DTYPEi_t i
-    for i in xrange(n):
-        arr[i] = 0
-
-cdef DTYPEi_t _check_id_on_edge(DTYPEi_t row_id, DTYPEi_t n_rows, DTYPEi_t n_cols):
-    # Everything should have been done using c-order.
-    # So, if the id is on the top edge, it will have a value less than n_cols
-    if row_id < n_cols:
-        return 1
-    # if it is on the bottom row, it will have an id greater or equal than
-    # the maximum id minus the number of columns
-    elif row_id >= (n_cols * n_rows - n_cols):
-        return 1
-    # if we divide the id by the number of columns and the remainder is 0,
-    # then the id is in the first column, or the left edge
-    elif (row_id % n_cols) == 0:
-        return 1
-    # if we divide the id by the number of columns and the remainder is one
-    # less than the number of columns, then the id is in the last column, or
-    # the right column
-    elif row_id % n_cols == (n_cols - 1):
-        return 1
-    else: # Otherwise, it's not on an edge
+# -*- coding: utf-8 -*-
+"""
+Created on Tue Nov 04 17:11:16 2014
+
+Copyright 2014-2024 Creare
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+
+@author: mpu
+"""
+
+import numpy as np
+cimport numpy as np
+
+ctypedef np.uint8_t DTYPEb_t
+ctypedef np.int64_t DTYPEi_t
+ctypedef np.int32_t DTYPEi32_t
+
+dtype_bool = 'uint8'
+
+#==============================================================================
+# Drain a single array's connections: If connected to start, change value
+#==============================================================================
+
+def drain_connections(np.ndarray[DTYPEb_t, ndim=1, cast=True] arr,
+                      np.ndarray[DTYPEb_t, ndim=1, cast=True] ids,
+                      np.ndarray[DTYPEi32_t, ndim=1] indptr,
+                      np.ndarray[DTYPEi32_t, ndim=1] indices, DTYPEb_t set_to=0):
+    cdef DTYPEi_t n_ids = ids.size
+    cdef DTYPEi_t n_A = indices.size
+
+    cdef np.ndarray[DTYPEb_t, ndim=1] ids_old = np.zeros(n_ids, dtype=dtype_bool)
+
+    _drain_connections(&(arr[0]), &(ids[0]), &(ids_old[0]),
+                       &(indptr[0]), &(indices[0]), n_ids, n_A, set_to)
+    return arr
+
+
+cdef void _drain_connections(DTYPEb_t *arr,
+                             DTYPEb_t *ids, DTYPEb_t *ids_old, DTYPEi32_t *indptr, DTYPEi32_t *indices,
+                             DTYPEi_t n_ids, DTYPEi_t n_A, DTYPEb_t tf):
+    cdef DTYPEi_t i = 0
+    cdef DTYPEi_t j = 0
+    cdef DTYPEb_t keep_going = 1
+    cdef DTYPEb_t *tmp
+    while keep_going: #If I use ids.sum() > 0 then I might get stuck in circular references.
+#        print "c",
+        # switch pointers
+        tmp = ids_old
+        ids_old = ids
+        ids = tmp
+
+        _zero_arr(ids, n_ids)
+        for i in xrange(n_ids):
+            if ids_old[i] == 0:
+                continue #If this id is not active, just skip the next part
+            for j in xrange(indptr[i], indptr[i + 1]):
+                row_id = indices[j]
+                ids[row_id] += arr[row_id] != tf
+                arr[row_id] = tf
+
+        keep_going = _check_id_changed(ids, ids_old, n_ids)
+
+
+#==============================================================================
+# Update area using the correct weighting factors and not double-dipping
+#==============================================================================
+def drain_area(np.ndarray[double, ndim=1] area,
+               np.ndarray[DTYPEb_t, ndim=1, cast=True] done,
+               np.ndarray[DTYPEb_t, ndim=1, cast=True] ids,
+               np.ndarray[DTYPEi32_t, ndim=1, cast=True] col_indptr,
+               np.ndarray[DTYPEi32_t, ndim=1, cast=True] col_indices,
+               np.ndarray[double, ndim=1] col_data,
+               np.ndarray[DTYPEi32_t, ndim=1, cast=True] row_indptr,
+               np.ndarray[DTYPEi32_t, ndim=1, cast=True] row_indices,
+               DTYPEi_t n_rows, DTYPEi_t n_cols,
+               np.ndarray[double, ndim=1, cast=True] edge_todo=None,
+               np.ndarray[double, ndim=1, cast=True] edge_todo_no_mask=None,
+               skip_edge=0):
+    cdef DTYPEi_t n_ids = ids.size
+    cdef DTYPEi_t n_A = col_indices.size
+
+    cdef DTYPEb_t do_edge_todo
+    if edge_todo is None:
+        edge_todo = np.zeros(1, dtype=float)
+        do_edge_todo = 0
+    else:
+        do_edge_todo = 1
+
+    cdef DTYPEb_t do_edge_todo_no_mask
+    if edge_todo_no_mask is None:
+        edge_todo_no_mask = np.zeros(1, dtype=float)
+        do_edge_todo_no_mask = 0
+    else:
+        do_edge_todo_no_mask = 1
+
+    cdef np.ndarray[DTYPEb_t, ndim=1] ids_old = np.zeros(n_ids, dtype=dtype_bool)
+
+    _drain_area(&(area[0]), &(done[0]), &(ids[0]), &(ids_old[0]),
+                       &(col_indptr[0]), &(col_indices[0]), &(col_data[0]),
+                       &(row_indptr[0]), &(row_indices[0]),
+                       n_rows, n_cols, n_ids, n_A,
+                       &(edge_todo[0]), do_edge_todo,
+                       &(edge_todo_no_mask[0]), do_edge_todo_no_mask,
+                       skip_edge)
+    return area, done, edge_todo, edge_todo_no_mask
+
+
+cdef void _drain_area(double *area, DTYPEb_t* done,
+                             DTYPEb_t *ids, DTYPEb_t *ids_old,
+                             DTYPEi32_t *col_indptr, DTYPEi32_t *col_indices, double *col_data,
+                             DTYPEi32_t *row_indptr, DTYPEi32_t *row_indices,
+                             DTYPEi_t n_rows, DTYPEi_t n_cols, DTYPEi_t n_ids, DTYPEi_t n_A,
+                             double* edge_todo, DTYPEb_t do_edge_todo,
+                             double* edge_todo_no_mask, DTYPEb_t do_edge_todo_no_mask,
+                             DTYPEi_t skip_edge):
+    cdef DTYPEi_t i = 0
+    cdef DTYPEi_t j = 0
+    cdef DTYPEb_t keep_going = 1
+    cdef DTYPEb_t *tmp
+    cdef double factor = 0
+    cdef DTYPEb_t wait_for_neighbors = 0
+    while keep_going: # If I use ids.sum() > 0 then I might get stuck in circular references.
+#        print "oc",
+        # Set the points that are about to be drained as done
+        # This has to be done before the next loop because the next candidates
+        # check to make sure that all the points that drain into them are done
+        for i in xrange(n_ids):
+            if ids[i]:
+                done[i] = 1
+#                print i, done[i]
+
+        # switch pointers
+        tmp = ids_old
+        ids_old = ids
+        ids = tmp
+
+        # Initialize array to zero for the points that will be drained next round
+        _zero_arr(ids, n_ids)
+
+        for i in xrange(n_ids):
+            if not ids_old[i]:
+                continue # If this id is not active, just skip the next part
+            for j in xrange(col_indptr[i], col_indptr[i + 1]):
+                row_id = col_indices[j]
+                factor = col_data[j]
+                # check if this is on the edge, if so, do not modify it and go
+                # to the next candidate
+                if ((skip_edge or (done[row_id])) and \
+                        _check_id_on_edge(row_id, n_rows, n_cols)):
+                    continue
+
+                area[row_id] += area[i] * factor
+
+                if do_edge_todo:
+                    edge_todo[row_id] += edge_todo[i] * factor
+                if do_edge_todo_no_mask:
+                    edge_todo_no_mask[row_id] += edge_todo_no_mask[i] * factor
+
+                # If the point that has just been drained into has all its
+                # source points marked as done, then it can be drained next
+                # round
+                wait_for_neighbors = 0
+                for k in xrange(row_indptr[row_id], row_indptr[row_id+1]):
+                    col_id = row_indices[k]
+#                    print 'row', row_id, 'col', col_id, 'done', done[col_id]
+                    if done[col_id] < 1:
+                        wait_for_neighbors = 1
+                        break
+#                print wait_for_neighbors,
+                if wait_for_neighbors == 0:
+                    ids[row_id] = 1
+
+                if do_edge_todo:
+                    done[i] = 1
+
+        keep_going = _check_id_changed(ids, ids_old, n_ids)
+
+#==============================================================================
+# Helper functions
+#==============================================================================
+
+cdef DTYPEb_t _check_id_changed(DTYPEb_t *ids, DTYPEb_t *ids_old, DTYPEi_t n_ids):
+    cdef DTYPEi_t i
+    cdef DTYPEb_t ret = 0
+    for i in xrange(n_ids):
+        if ids[i] != ids_old[i]:
+            ret = 1
+            break
+    return ret
+
+cdef _zero_arr(DTYPEb_t *arr, DTYPEi_t n):
+    cdef DTYPEi_t i
+    for i in xrange(n):
+        arr[i] = 0
+
+cdef DTYPEi_t _check_id_on_edge(DTYPEi_t row_id, DTYPEi_t n_rows, DTYPEi_t n_cols):
+    # Everything should have been done using c-order.
+    # So, if the id is on the top edge, it will have a value less than n_cols
+    if row_id < n_cols:
+        return 1
+    # if it is on the bottom row, it will have an id greater or equal than
+    # the maximum id minus the number of columns
+    elif row_id >= (n_cols * n_rows - n_cols):
+        return 1
+    # if we divide the id by the number of columns and the remainder is 0,
+    # then the id is in the first column, or the left edge
+    elif (row_id % n_cols) == 0:
+        return 1
+    # if we divide the id by the number of columns and the remainder is one
+    # less than the number of columns, then the id is in the last column, or
+    # the right column
+    elif row_id % n_cols == (n_cols - 1):
+        return 1
+    else: # Otherwise, it's not on an edge
         return 0
```

### Comparing `pyDEM-0.2.0/pydem/cyfuncs/__init__.py` & `pyDEM-1.0.0/pydem/cyfuncs/__init__.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-"""
-   Copyright 2015 Creare
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+"""
+   Copyright 2015 Creare
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
 """
```

### Comparing `pyDEM-0.2.0/pydem/examples/process_array.py` & `pyDEM-1.0.0/pydem/examples/process_array.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,50 @@
-# -*- coding: utf-8 -*-
-"""
-   Copyright 2015 Creare
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
-"""
-if __name__ == "__main__":
-    from pydem.test_pydem import get_test_data
-    from pydem.dem_processing import DEMProcessor
-    from pydem.test_pydem import make_file_names
-
-    import sys, os
-    if len(sys.argv) <= 1:
-        testnum = 13  # Default test number
-
-    NN = 64  # Resolution of tile
-
-    # Get test data and create DEMProcessor
-    elev, ang, test_data = get_test_data(testnum, NN)
-    elev = elev.raster_data
-    
-    dem_proc1 = DEMProcessor(elev)
-    # Calculate TWI
-    twi1 = dem_proc1.calc_twi()
-    
-    # Stretch the latitude direction
-    lats = [0, 2]  # degrees
-    lons = [0, 1]  # degrees
-    dem_proc2 = DEMProcessor((elev, lats, lons))
-    twi2 = dem_proc2.calc_twi()
-
-    # plot results
-    import matplotlib.pyplot as plt
-    plt.matshow(twi1); plt.colorbar()
-    plt.title('TWI calculated from Array, dx/dy determined from array shape')
-    plt.matshow(dem_proc1.data); plt.colorbar()
-    plt.title('Elevation from Array (after fixing flats)')
-    plt.matshow(twi2); plt.colorbar()
-    plt.title('TWI calculated from Array, dx/dy determined from input lat/lon')
-    
-    plt.show()
-    
-    if not os.path.exists('twi'):
-        os.mkdir('twi')
-    dem_proc1.save_twi('.')
-    dem_proc2.save_twi('.')
-    print 'done'
+# -*- coding: utf-8 -*-
+"""
+   Copyright 2015-2024 Creare
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
+"""
+if __name__ == "__main__":
+    from pydem.utils_test_pydem import get_test_data
+    from pydem.dem_processing import DEMProcessor
+    from pydem.utils_test_pydem import make_file_names
+
+    import sys, os
+    if len(sys.argv) <= 1:
+        testnum = 13  # Default test number
+
+    NN = 64  # Resolution of tile
+
+    # Get test data and create DEMProcessor
+    elev, ang, test_data = get_test_data(testnum, NN)
+
+    dem_proc1 = DEMProcessor(elev=elev, fill_flats=False)
+    twi1 = dem_proc1.calc_twi()
+    dem_proc1b = DEMProcessor(elev=elev, fill_flats=True)
+    twi1b = dem_proc1b.calc_twi()
+    # Calculate TWI
+
+    # Stretch the latitude direction
+    dem_proc2 = DEMProcessor(elev=elev, dY=2, dX=1)
+    twi2 = dem_proc2.calc_twi()
+
+    # plot results
+    import matplotlib.pyplot as plt
+    plt.matshow(twi1); plt.colorbar()
+    plt.title('TWI calculated from Array, dx/dy determined from array shape')
+    plt.matshow(twi1b); plt.colorbar()
+    plt.title('Elevation from Array (after fixing flats)')
+    plt.matshow(twi2); plt.colorbar()
+    plt.title('TWI calculated from Array, dx/dy determined from input lat/lon')
+
+    plt.show()
```

### Comparing `pyDEM-0.2.0/pydem/reader/__init__.py` & `pyDEM-1.0.0/pydem/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-"""
-   Copyright 2015 Creare
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
-"""
+"""
+   Copyright 2015-2024 Creare
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
+"""
+
+from pydem.dem_processing import DEMProcessor
+from pydem import process_manager
```

### Comparing `pyDEM-0.2.0/pydem/taudem/__init__.pyc` & `pyDEM-1.0.0/aws/link_so.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,57 @@
-00000000: 03f3 0d0a ad68 4d59 6300 0000 0000 0000  .....hMYc.......
-00000010: 0001 0000 0040 0000 0073 0a00 0000 6400  .....@...s....d.
-00000020: 005a 0000 6401 0053 2802 0000 0073 4202  .Z..d..S(....sB.
-00000030: 0000 0a20 2020 436f 7079 7269 6768 7420  ...   Copyright 
-00000040: 3230 3135 2043 7265 6172 650a 0a20 2020  2015 Creare..   
-00000050: 4c69 6365 6e73 6564 2075 6e64 6572 2074  Licensed under t
-00000060: 6865 2041 7061 6368 6520 4c69 6365 6e73  he Apache Licens
-00000070: 652c 2056 6572 7369 6f6e 2032 2e30 2028  e, Version 2.0 (
-00000080: 7468 6520 224c 6963 656e 7365 2229 3b0a  the "License");.
-00000090: 2020 2079 6f75 206d 6179 206e 6f74 2075     you may not u
-000000a0: 7365 2074 6869 7320 6669 6c65 2065 7863  se this file exc
-000000b0: 6570 7420 696e 2063 6f6d 706c 6961 6e63  ept in complianc
-000000c0: 6520 7769 7468 2074 6865 204c 6963 656e  e with the Licen
-000000d0: 7365 2e0a 2020 2059 6f75 206d 6179 206f  se..   You may o
-000000e0: 6274 6169 6e20 6120 636f 7079 206f 6620  btain a copy of 
-000000f0: 7468 6520 4c69 6365 6e73 6520 6174 0a0a  the License at..
-00000100: 2020 2020 2020 2068 7474 703a 2f2f 7777         http://ww
-00000110: 772e 6170 6163 6865 2e6f 7267 2f6c 6963  w.apache.org/lic
-00000120: 656e 7365 732f 4c49 4345 4e53 452d 322e  enses/LICENSE-2.
-00000130: 300a 0a20 2020 556e 6c65 7373 2072 6571  0..   Unless req
-00000140: 7569 7265 6420 6279 2061 7070 6c69 6361  uired by applica
-00000150: 626c 6520 6c61 7720 6f72 2061 6772 6565  ble law or agree
-00000160: 6420 746f 2069 6e20 7772 6974 696e 672c  d to in writing,
-00000170: 2073 6f66 7477 6172 650a 2020 2064 6973   software.   dis
-00000180: 7472 6962 7574 6564 2075 6e64 6572 2074  tributed under t
-00000190: 6865 204c 6963 656e 7365 2069 7320 6469  he License is di
-000001a0: 7374 7269 6275 7465 6420 6f6e 2061 6e20  stributed on an 
-000001b0: 2241 5320 4953 2220 4241 5349 532c 0a20  "AS IS" BASIS,. 
-000001c0: 2020 5749 5448 4f55 5420 5741 5252 414e    WITHOUT WARRAN
-000001d0: 5449 4553 204f 5220 434f 4e44 4954 494f  TIES OR CONDITIO
-000001e0: 4e53 204f 4620 414e 5920 4b49 4e44 2c20  NS OF ANY KIND, 
-000001f0: 6569 7468 6572 2065 7870 7265 7373 206f  either express o
-00000200: 7220 696d 706c 6965 642e 0a20 2020 5365  r implied..   Se
-00000210: 6520 7468 6520 4c69 6365 6e73 6520 666f  e the License fo
-00000220: 7220 7468 6520 7370 6563 6966 6963 206c  r the specific l
-00000230: 616e 6775 6167 6520 676f 7665 726e 696e  anguage governin
-00000240: 6720 7065 726d 6973 7369 6f6e 7320 616e  g permissions an
-00000250: 640a 2020 206c 696d 6974 6174 696f 6e73  d.   limitations
-00000260: 2075 6e64 6572 2074 6865 204c 6963 656e   under the Licen
-00000270: 7365 2e0a 4e28 0100 0000 7407 0000 005f  se..N(....t...._
-00000280: 5f64 6f63 5f5f 2800 0000 0028 0000 0000  _doc__(....(....
-00000290: 2800 0000 0073 2e00 0000 633a 5c72 6570  (....s....c:\rep
-000002a0: 6f73 6974 6f72 6965 735c 7079 6465 6d5c  ositories\pydem\
-000002b0: 7079 6465 6d5c 7461 7564 656d 5c5f 5f69  pydem\taudem\__i
-000002c0: 6e69 745f 5f2e 7079 7408 0000 003c 6d6f  nit__.pyt....<mo
-000002d0: 6475 6c65 3e0f 0000 0073 0000 0000       dule>....s....
+00000000: 2222 220a 2020 2043 6f70 7972 6967 6874  """.   Copyright
+00000010: 2032 3031 352d 3230 3234 2043 7265 6172   2015-2024 Crear
+00000020: 650a 0a20 2020 4c69 6365 6e73 6564 2075  e..   Licensed u
+00000030: 6e64 6572 2074 6865 2041 7061 6368 6520  nder the Apache 
+00000040: 4c69 6365 6e73 652c 2056 6572 7369 6f6e  License, Version
+00000050: 2032 2e30 2028 7468 6520 224c 6963 656e   2.0 (the "Licen
+00000060: 7365 2229 3b0a 2020 2079 6f75 206d 6179  se");.   you may
+00000070: 206e 6f74 2075 7365 2074 6869 7320 6669   not use this fi
+00000080: 6c65 2065 7863 6570 7420 696e 2063 6f6d  le except in com
+00000090: 706c 6961 6e63 6520 7769 7468 2074 6865  pliance with the
+000000a0: 204c 6963 656e 7365 2e0a 2020 2059 6f75   License..   You
+000000b0: 206d 6179 206f 6274 6169 6e20 6120 636f   may obtain a co
+000000c0: 7079 206f 6620 7468 6520 4c69 6365 6e73  py of the Licens
+000000d0: 6520 6174 0a0a 2020 2020 2020 2068 7474  e at..       htt
+000000e0: 703a 2f2f 7777 772e 6170 6163 6865 2e6f  p://www.apache.o
+000000f0: 7267 2f6c 6963 656e 7365 732f 4c49 4345  rg/licenses/LICE
+00000100: 4e53 452d 322e 300a 0a20 2020 556e 6c65  NSE-2.0..   Unle
+00000110: 7373 2072 6571 7569 7265 6420 6279 2061  ss required by a
+00000120: 7070 6c69 6361 626c 6520 6c61 7720 6f72  pplicable law or
+00000130: 2061 6772 6565 6420 746f 2069 6e20 7772   agreed to in wr
+00000140: 6974 696e 672c 2073 6f66 7477 6172 650a  iting, software.
+00000150: 2020 2064 6973 7472 6962 7574 6564 2075     distributed u
+00000160: 6e64 6572 2074 6865 204c 6963 656e 7365  nder the License
+00000170: 2069 7320 6469 7374 7269 6275 7465 6420   is distributed 
+00000180: 6f6e 2061 6e20 2241 5320 4953 2220 4241  on an "AS IS" BA
+00000190: 5349 532c 0a20 2020 5749 5448 4f55 5420  SIS,.   WITHOUT 
+000001a0: 5741 5252 414e 5449 4553 204f 5220 434f  WARRANTIES OR CO
+000001b0: 4e44 4954 494f 4e53 204f 4620 414e 5920  NDITIONS OF ANY 
+000001c0: 4b49 4e44 2c20 6569 7468 6572 2065 7870  KIND, either exp
+000001d0: 7265 7373 206f 7220 696d 706c 6965 642e  ress or implied.
+000001e0: 0a20 2020 5365 6520 7468 6520 4c69 6365  .   See the Lice
+000001f0: 6e73 6520 666f 7220 7468 6520 7370 6563  nse for the spec
+00000200: 6966 6963 206c 616e 6775 6167 6520 676f  ific language go
+00000210: 7665 726e 696e 6720 7065 726d 6973 7369  verning permissi
+00000220: 6f6e 7320 616e 640a 2020 206c 696d 6974  ons and.   limit
+00000230: 6174 696f 6e73 2075 6e64 6572 2074 6865  ations under the
+00000240: 204c 6963 656e 7365 2e0a 2222 220a 0a69   License.."""..i
+00000250: 6d70 6f72 7420 6f73 0a0a 7769 7468 206f  mport os..with o
+00000260: 7065 6e28 2773 6f5f 6669 6c65 732e 7478  pen('so_files.tx
+00000270: 7427 2c20 2772 2729 2061 7320 6669 643a  t', 'r') as fid:
+00000280: 0a20 2020 2073 6620 3d20 6669 642e 7265  .    sf = fid.re
+00000290: 6164 2829 2e73 706c 6974 2827 5c6e 2729  ad().split('\n')
+000002a0: 0a0a 6c69 6e6b 7320 3d7b 7d0a 666f 7220  ..links ={}.for 
+000002b0: 7320 696e 2073 663a 0a20 2020 206b 6579  s in sf:.    key
+000002c0: 203d 2073 2e73 706c 6974 2827 2f27 295b   = s.split('/')[
+000002d0: 2d31 5d0a 2020 2020 6c69 6e6b 735b 6b65  -1].    links[ke
+000002e0: 795d 203d 206c 696e 6b73 2e67 6574 286b  y] = links.get(k
+000002f0: 6579 2c20 5b5d 2920 2b20 5b73 5d0a 0a66  ey, []) + [s]..f
+00000300: 6f72 206c 2c76 2069 6e20 6c69 7374 286c  or l,v in list(l
+00000310: 696e 6b73 2e69 7465 6d73 2829 293a 0a20  inks.items()):. 
+00000320: 2020 2069 6620 6c65 6e28 7629 203e 2031     if len(v) > 1
+00000330: 3a0a 2020 2020 2020 2020 666f 7220 6620  :.        for f 
+00000340: 696e 2076 5b31 3a5d 3a0a 2020 2020 2020  in v[1:]:.      
+00000350: 2020 2020 2020 6f73 2e72 656d 6f76 6528        os.remove(
+00000360: 6629 0a20 2020 2020 2020 2020 2020 206f  f).            o
+00000370: 732e 7379 6d6c 696e 6b28 765b 305d 2c20  s.symlink(v[0], 
+00000380: 6629 0a                                  f).
```

### Comparing `pyDEM-0.2.0/pydem/test_pydem.py` & `pyDEM-1.0.0/pydem/utils_test_pydem.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,544 +1,525 @@
-# -*- coding: utf-8 -*-
-"""
-   Copyright 2015 Creare
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
-
-Created on Fri Jun 20 11:26:08 2014
-
-@author: mpu
-
-NOTE: x = lat, y = lon -- THIS IS REVERSED FROM THE USUAL IDEA
-"""
-import os
-import gdal
-
-import numpy as np
-from scipy.ndimage.filters import gaussian_filter
-
-from taudem import taudem
-from reader.gdal_reader import GdalReader
-from utils import mk_geotiff_obj, mk_dx_dy_from_geotif_layer, get_fn_from_coords
-PLOT_TESTCASES = True
-
-#if PLOT_TESTCASES:
-#    from matplotlib.pyplot import (figure, subplot, imshow, title,
-#                                       colorbar, clim, draw)
-NO_DATA_VALUE = -9999
-
-
-def make_file_names(testnum, NN, testdir='testtiff'):
-    if type(NN) == list:
-        N = NN[0]
-    else:
-        N = NN
-
-    base = os.path.join(testdir, 'test_NN%03d_%03d' % (N, testnum))
-    return {"elev": base + '_elev.tif', "ang": base + '_ang.tif',
-            "fel": base + '_fel.tif', 'uca': base + '_uca.tif'}
-
-
-def mk_xy_latlon(N):
-    raster = np.zeros((N, N))
-    if os.path.exists('temp.tif'):
-        os.remove('temp.tif')
-    obj, driver = mk_geotiff_obj(raster, 'temp.tif')
-    del obj
-    del driver
-    obj = GdalReader(file_name='temp.tif').raster_layers[0]
-    dx, dy = mk_dx_dy_from_geotif_layer(obj)
-    del obj
-    os.remove('temp.tif')
-    y = np.concatenate([[0], np.cumsum(dx)])
-    x = np.concatenate([[0], np.cumsum(dy)])
-    # Center it on zero
-    x = x - (x.max() - x.min()) / 2.0
-    y = y - (y.max() - y.min()) / 2.0
-    scale = np.sqrt(x**2 + y**2).max()
-    x = x / scale
-    y = y / scale
-    Y, X = np.meshgrid(y, x)
-
-    return X, Y
-
-
-def make_elev_ang(testnum, NN, raster, angle, uca=None, testdir='testtiff'):
-    # Convert masked array to filled array
-    raster = raster.filled()
-    angle = angle.filled()
-    filename = make_file_names(testnum, NN, testdir)
-    try:
-        if not os.path.exists(testdir):
-            os.makedirs(testdir)
-        if not os.path.exists(filename['elev']):
-            elev, driver = mk_geotiff_obj(raster, filename['elev'])
-            del driver
-            del elev
-            print "Created", filename['elev']
-            ang, driver = mk_geotiff_obj(angle, filename['ang'])
-            del ang
-            del driver
-            print "Created", filename['ang']
-        if not os.path.exists(filename['uca']) and uca is not None:
-            ucaf, driver = mk_geotiff_obj(uca, filename['uca'])
-            del ucaf
-            del driver
-            print "Created", filename['uca']
-        else:
-            print "Already exists or None", filename['uca']
-    finally:
-        ucaf = None
-        elev = None
-        ang = None
-        driver = None
-
-
-# Define the inidividual elevation/angles for the test-cases
-def case_cone(x, y, noise=False):
-    # %%Cone
-    NN = x.shape[0]
-    raster = np.ma.masked_array(1 - np.sqrt((y)**2 + (x)**2) / np.sqrt(2.),
-                                mask=np.zeros(x.shape, bool),
-                                fill_value=NO_DATA_VALUE)
-    angle = np.ma.masked_array(np.arctan2(x, -y) + np.pi,
-                               mask=np.zeros(x.shape, bool),
-                               fill_value=NO_DATA_VALUE)
-    ncell = np.round(np.sqrt((y)**2 + (x)**2) / (1.0 / NN))
-    uca = np.ma.masked_array(np.pi * ((y)**2 + (x)**2) / ncell * NN**2 / 4.,
-                             mask=np.zeros(x.shape, bool),
-                             fill_value=NO_DATA_VALUE)
-    # We expect the total upstream contributing area to be the
-    # total area of the data
-    summat = np.zeros_like(uca)
-    summat[:, 0] = 1
-    summat[:, -1] = 1
-    summat[0, :] = 1
-    summat[-1, :] = 1
-    uca = uca * NN ** 2 / np.nansum(summat * uca)
-    if noise:
-        np.random.seed(1773)
-        raster += np.abs(np.random.randn(*raster.shape)**2) * 0.0003
-        raster[:, :] = gaussian_filter(raster, 2, mode='constant')
-#
-    return raster, angle, uca
-
-
-def case_cone_scaled(x, y, noise):
-    raster, angle, uca = case_cone(x, y, noise)
-    raster = raster - raster.ravel().min()  # (make it all positive)
-    return raster, angle, uca
-
-
-def case_line(x, y, line):
-    raster = np.ma.masked_array(line[0] * x + line[1] * y,
-                                mask=np.zeros(x.shape, bool),
-                                fill_value=NO_DATA_VALUE)
-    # normalize
-    raster = raster - raster.min()
-    raster = raster / raster.max()
-
-    angle = np.ma.masked_array(np.arctan2(-line[0], line[1])
-                               * np.ones(raster.shape) + np.pi,
-                               mask=np.zeros(x.shape, bool),
-                               fill_value=NO_DATA_VALUE)
-    NN = x.shape[0]
-
-    if line[0] > 0:
-        x_line = 1
-    else:
-        x_line = -1
-    if line[1] > 0:
-        y_line = 1
-    else:
-        y_line = -1
-
-    tx = (x_line - x) / (line[0] + 1e-17)
-    ty = (y_line - y) / (line[1] + 1e-17)
-    if line[0] == 0:
-        t = ty
-    elif line[1] == 0:
-        t = tx
-    else:
-        t = np.minimum(tx, ty)
-    uca = t  # * (line[0]**2 + line[1]**2)** (0.5)
-    uca = np.ma.masked_array(np.round(t * NN) / 2,
-                             mask=np.zeros(x.shape, bool),
-                             fill_value=NO_DATA_VALUE)
-    return raster, angle, uca
-
-
-def case_opposing_slopes(x, y, line):
-    raster = np.ma.masked_array(line[0] * x + line[1] * y,
-                                mask=np.zeros(x.shape, bool),
-                                fill_value=NO_DATA_VALUE)
-    I = -x * line[1] + y * line[0] > 0
-    raster[I] = -line[0] * x[I] - line[1] * y[I]
-    # normalize
-    raster = raster - raster.min()
-    raster = raster / raster.max()
-
-    angle = np.ma.masked_array(np.arctan2(-line[0], line[1])
-                               * np.ones(raster.shape) + np.pi,
-                               mask=np.zeros(x.shape, bool),
-                               fill_value=NO_DATA_VALUE)
-    angle[I] = np.arctan2(line[0], -line[1]) + np.pi
-    return raster, angle
-
-
-def case_ring_flat(x, y, drains):
-    raster, angle, uca = case_cone(x, y)
-    if type(drains[0]) != list:
-        drains = [drains]
-    # Set the flat
-    I1 = raster >= 0.7
-    I = (raster > 0.5) & (raster < 0.7)
-    angle[I] = -1
-
-    raster2 = raster.copy()
-    for drain in drains:
-        raster[drain[0], drain[1]] -= np.min(raster[drain[0], drain[1]])
-    raster[I] = 0.51
-    raster[I1] = raster2[I1]
-    return raster, angle
-
-
-def case_top_flat(x, y, drains):
-    raster, angle, uca = case_cone(x, y)
-    if type(drains[0]) != list:
-        drains = [drains]
-    # Set the flat
-    I = raster >= 0.7
-    angle[I] = -1
-
-    for drain in drains:
-        raster[drain[0], drain[1]] -= np.min(raster[drain[0], drain[1]])
-    raster[I] = 0.75
-    return raster, angle
-
-
-def case_line_flat(x, y, line):
-    raster, angle, uca = case_line(x, y, line)
-    flat_raster = np.ma.masked_array(1 - np.sqrt((y)**2 + (x)**2) / np.sqrt(2.),
-                                     mask=np.zeros(x.shape, bool),
-                                     fill_value=NO_DATA_VALUE)
-    # normalize
-    raster = raster - raster.min()
-    raster = raster / raster.max()
-
-    # Set the flat
-    I = flat_raster >= 0.7
-    raster[I] = 0.5
-    angle[I] = -1
-
-    return raster, angle
-
-
-def case_pit_of_dispair(x, y, drains):
-    if len(drains) > 0 and type(drains[0]) != list:
-        drains = [drains]
-        # %% The pit of dispair
-    raster = np.ma.masked_array(1 + np.sqrt((y)**2 + (x)**2) / np.sqrt(2.),
-                                mask=np.zeros(x.shape, bool),
-                                fill_value=NO_DATA_VALUE)
-
-    angle = np.ma.masked_array(np.arctan2(-x, y) + np.pi,
-                               mask=np.zeros(x.shape, bool),
-                               fill_value=NO_DATA_VALUE)
-    for drain in drains:
-        N = len(raster[drain[0], drain[1]].ravel())
-        raster[drain[0], drain[1]] = np.linspace(0, 1, N)\
-            .reshape(raster[drain[0], drain[1]].shape)
-
-    return raster, angle
-
-
-def case_trough_of_dispair(x, y, line):
-    # %% The trough of dispair
-    NN = x.shape[0]
-    raster = np.ma.masked_array(line[0] * x + line[1] * y,
-                                mask=np.zeros(x.shape, bool),
-                                fill_value=NO_DATA_VALUE)
-    I = x * line[1] + y * line[0] > 0
-    raster[I] = -line[0] * x[I] - line[1] * y[I]
-    raster += 0.1 * (-line[0] * x + line[1] * y)
-
-    # normalize
-    raster = raster - raster.min()
-    raster = raster / raster.max()
-
-    angle = np.ma.masked_array(np.arctan2(-line[0] * 0.9, line[1] * 1.1)
-                               * np.ones(raster.shape) + np.pi,
-                               mask=np.zeros(x.shape, bool),
-                               fill_value=NO_DATA_VALUE)
-    angle[I] = np.arctan2(line[0] * 1.1, -line[1] * 0.9) + np.pi
-    angle[[np.arange(NN), np.arange(NN)]] = 3 * np.pi / 4
-
-    return raster, angle
-
-
-def case_real_data(x, y, filename='N43W-72_N44W-71_elev.tif', NN=None):
-# def case_real_data(x, y, filename='N72W-112N73W-111_elev.tif', NN=None):
-    if NN is None:
-        NX, NY = x.shape
-        NX0, NY0 = [0, 0]
-    elif type(NN) == list:
-        NX0, NX, NY0, NY = NN
-    else:
-        NX0, NX, NY0, NY = [0, NN, 0, NN]
-    elev_file = GdalReader(file_name=filename)
-    test_data, = elev_file.raster_layers
-    raster = test_data.raster_data[NX0:NX, NY0:NY]
-    del elev_file
-    del test_data
-    angle = -1 + 0 * raster
-    return raster, angle
-
-
-def case_pit_of_carkoon(x, y):
-    raster, angle = case_pit_of_dispair(x, y, [])
-
-    I = np.argmin(raster)
-    raster.mask.ravel()[I] = True
-    angle.mask.ravel()[I] = True
-    return raster, angle
-
-
-def case_sea_of_saw(x, y):
-    raster, angle, uca = case_cone(x, y)
-    I = (raster < 0.4) & (x > 0)
-    raster.mask[I] = True
-    angle.mask[I] = True
-    return raster, angle
-
-
-def spiral(x, y):
-    n, m = x.shape
-    # make the walls
-    raster = np.ma.masked_array((1.0 - np.maximum(np.abs(x), np.abs(y))**2)
-                                * (n * m) / 2 + (n + m) * 2,
-                                mask=np.zeros(x.shape, bool),
-                                fill_value=NO_DATA_VALUE)
-
-    # make the spiral
-    start = [0, 1]
-    stop = [n - 2, m - 2]
-    i, j = start
-    start = [-1, 1]
-    elev = 0
-    count = 0
-    sgn = [1, 1]
-    while count < n*m / 2:
-        count += 1
-        raster[i, j] = elev
-        elev += 1
-        if i < stop[0] and sgn[0] > 0:
-            i += 1
-        elif j < stop[1] and sgn[1] > 0:
-            j += 1
-        elif i == stop[0] and j == stop[1] and sgn[1] > 0:
-            start[0] += 2
-            start[1] += 2
-            sgn = [-1, -1]
-            i -= 1
-        elif i > start[0] and sgn[0] < 0:
-            i -= 1
-        elif j > start[1] and sgn[1] < 0:
-            j -= 1
-        elif i == start[0] and j == start[1] and sgn[1] < 0:
-            stop[0] -= 2
-            stop[1] -= 2
-            sgn = [1, 1]
-            i += 1
-        else:
-            break
-
-    return raster, raster * 0
-
-
-def mk_test_multifile(testnum, NN, testdir, nx_grid=3, ny_grid=4, nx_overlap=16,
-                      ny_overlap=32, lat=[46, 45], lon=[-73, -72]):
-    """
-    Written to make test case for multi-file edge resolution.
-    """
-    path = os.path.split(make_file_names(testnum, NN, os.path.join(
-                                               testdir, 'chunks'))['elev'])[0]
-    try:
-        os.makedirs(path)
-    except:
-        pass
-
-    def _get_chunk_edges(NN, chunk_size, chunk_overlap):
-        left_edge = np.arange(0, NN - chunk_overlap, chunk_size)
-        left_edge[1:] -= chunk_overlap
-        right_edge = np.arange(0, NN - chunk_overlap, chunk_size)
-        right_edge[:-1] = right_edge[1:] + chunk_overlap
-        right_edge[-1] = NN
-        right_edge = np.minimum(right_edge, NN)
-        return left_edge, right_edge
-
-    elev_data, ang_data, fel_data = get_test_data(testnum, NN)
-    try:
-        raster = fel_data.raster_data
-    except:
-        raster = elev_data.raster_data
-
-    ni, nj = raster.shape
-
-    top_edge, bottom_edge = _get_chunk_edges(ni, ni // ny_grid, ny_overlap)
-    left_edge, right_edge = _get_chunk_edges(nj, nj // nx_grid, nx_overlap)
-
-#    gc = elev_data.grid_coordinates
-#    lat = gc.y_axis
-#    lon = gc.x_axis
-    lat = np.linspace(lat[0], lat[1], ni)
-    lon = np.linspace(lon[0], lon[1], nj)
-    count = 0
-    for te, be in zip(top_edge, bottom_edge):
-        for le, re in zip(left_edge, right_edge):
-            count += 1
-            fn = os.path.join(path,
-                              get_fn_from_coords((lat[be-1], lon[le], lat[te],
-                                                  lon[re-1]), 'elev'))
-            print count, ": [%d:%d, %d:%d]" % (te, be, le, re), \
-                '(lat, lon) = (%g to %g, %g to %g)' % (lat[te], lat[be-1],
-                                                       lon[le], lon[re-1]), \
-                'min,max = (%g to %g, %g to %g)' % (lat.min(), lat.max(),
-                                                    lon.min(), lon.max())
-            mk_geotiff_obj(raster[te:be, le:re], fn,
-                           bands=1, gdal_data_type=gdal.GDT_Float32,
-                           lat=[lat[te], lat[be-1]], lon=[lon[le], lon[re-1]])
-
-
-# %% MAKE ALL THE TESTS
-def make_test_files(NN=32, plotflag=False, testdir='testtiff', testnum=None):
-    # Common
-    if plotflag:
-        from matplotlib.pyplot import (figure, subplot, imshow, title,
-                                       colorbar, clim, draw)
-
-    if type(NN) == list:
-        N = np.max(NN)
-    else:
-        N = NN
-    x, y = np.mgrid[-1:1:np.complex(0, N), -1:1:np.complex(0, N)]
-    lat, lon = mk_xy_latlon(N)
-
-    # The first brace it just to avoid the line-continuouation character
-    tests = [[case_cone]  # case 0
-             + [lambda x, y: case_line(x, y, [1, 0]),
-                lambda x, y: case_line(x, y, [-1, 0]),
-                lambda x, y: case_line(x, y, [0, 1]),
-                lambda x, y: case_line(x, y, [0, -1]),
-                lambda x, y: case_line(x, y, [1, 1]),
-                lambda x, y: case_line(x, y, [-1, 1]),
-                lambda x, y: case_line(x, y, [1, -1]),
-                lambda x, y: case_line(x, y, [-1, -1])
-                ]  # cases 1-8, 8 cases in total for the lines
-             + [lambda x, y: case_opposing_slopes(x, y, [1, 0]),
-                lambda x, y: case_opposing_slopes(x, y, [0, 1]),
-                lambda x, y: case_opposing_slopes(x, y, [1, 1]),
-                lambda x, y: case_opposing_slopes(x, y, [-1, 1])
-                ]  # cases 9-12, 4 cases in total for the opposing slopes
-             + [lambda x, y: case_ring_flat(x, y, [slice(NN), slice(NN)]),
-                lambda x, y: case_ring_flat(x, y, [slice(NN//2, NN//2+1),
-                                                   slice(NN//2, NN)]),
-                lambda x, y: case_ring_flat(x, y, [[slice(NN//2, NN//2+1),
-                                                    slice(0, NN//2)],
-                                                   [slice(NN//2, NN//2+1),
-                                                    slice(NN//2, NN)]]),
-                lambda x, y: case_ring_flat(x, y, [[slice(NN//2, NN),
-                                                    slice(NN//2, NN//2+1)],
-                                                   [slice(NN//2, NN//2+1),
-                                                    slice(0, NN//2)],
-                                                   [slice(NN//2, NN//2+1),
-                                                    slice(NN//2, NN)]]),
-                lambda x, y: case_ring_flat(x, y, [[slice(0, NN//2),
-                                                    slice(NN//2, NN//2+1)],
-                                                   [slice(NN//2, NN),
-                                                    slice(NN//2, NN//2+1)],
-                                                   [slice(NN//2, NN//2+1),
-                                                    slice(0, NN//2)],
-                                                   [slice(NN//2, NN//2+1),
-                                                    slice(NN//2, NN)]])
-                ]  # cases 13-17, 5 cases in total for the ring flats
-             + [lambda x, y: case_top_flat(x, y, [slice(NN), slice(NN)]),
-                lambda x, y: case_top_flat(x, y, [slice(NN//2, NN//2+1),
-                                                  slice(NN//2, NN)]),
-                lambda x, y: case_top_flat(x, y, [slice(NN//2, NN//2+1),
-                                                  slice(0, NN//2)]),
-                lambda x, y: case_top_flat(x, y, [slice(NN//2, NN),
-                                                  slice(NN//2, NN//2+1)]),
-                lambda x, y: case_top_flat(x, y, [slice(0, NN//2),
-                                                  slice(NN//2, NN//2+1)])
-                ]  # cases 18-22, 5 cases total for top flats
-             + [lambda x, y: case_line_flat(x, y, [-1, -1])]  # case 23
-             + [lambda x, y: case_pit_of_dispair(x, y, [slice(NN//2, NN//2+1),
-                                                        slice(0, NN//2)]),
-                lambda x, y: case_pit_of_dispair(x, y, [slice(0, NN//2),
-                                                        slice(NN//2, NN//2+1)])
-                ]  # cases 24 and 25
-             + [lambda x, y: case_trough_of_dispair(x, y, [-1, 1])]  # case 26
-             + [lambda x, y: case_real_data(x, y, NN=NN)]  # case 27
-             + [case_pit_of_carkoon]  # Case 28
-             + [case_sea_of_saw]  # case 29
-             + [spiral]  # case 30
-             + [lambda x, y: case_cone(x, y, True)]  # case 31
-             + [lambda x, y: case_cone_scaled(lon, lat, True)]  # case 32
-             ]
-
-    tests = tests[0]  # Remove the outer list
-    if testnum is None:
-        testnum = 0
-    else:
-        tests = [tests[testnum]]
-
-    for test in tests:
-        res = test(x, y)
-        raster, angle = res[:2]
-        if len(res) == 3:
-            uca = res[2]
-        else:
-            uca = None
-        make_elev_ang(testnum, NN, raster, angle, uca, testdir)
-
-        if plotflag:
-            figure(testnum)
-            subplot(121)
-            imshow(raster, interpolation='none'); colorbar()
-            draw()
-            title('Elevation %d' % testnum)
-            subplot(122)
-            imshow(angle / np.pi * 180, interpolation='none'); colorbar(); clim([0, 360])
-            draw()
-            title('Angle %d' % testnum)
-        testnum += 1
-
-
-def get_test_data(test_num, NN, testdir='testtiff'):
-    filenames = make_file_names(test_num, NN, testdir)
-    if not os.path.exists(filenames['elev']):
-        make_test_files(NN, testdir=testdir, testnum=test_num)
-    elev_file = GdalReader(file_name=filenames['elev'])
-    elev_data, = elev_file.raster_layers
-    ang_file = GdalReader(file_name=filenames['ang'])
-    ang_data, = ang_file.raster_layers
-    if not os.path.exists(filenames['fel']):
-        cmd = ('pitremove -z "%s" -fel "%s" ' % (filenames['elev'],
-                                                 filenames['fel']))
-        taudem._run(cmd)
-    fel_file = GdalReader(file_name=filenames['fel'])
-    fel_data,  = fel_file.raster_layers
-    del elev_file
-    del ang_file
-    return elev_data, ang_data, fel_data
-
+# -*- coding: utf-8 -*-
+"""
+   Copyright 2015-2024 Creare
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
+
+Created on Fri Jun 20 11:26:08 2014
+
+@author: mpu
+
+NOTE: x = lat, y = lon -- THIS IS REVERSED FROM THE USUAL IDEA
+"""
+import os
+
+import numpy as np
+from scipy.ndimage import gaussian_filter
+
+from .utils import mk_geotiff_obj, mk_dx_dy_from_geotif_layer, get_fn_from_coords, save_raster, read_raster
+PLOT_TESTCASES = True
+
+#if PLOT_TESTCASES:
+#    from matplotlib.pyplot import (figure, subplot, imshow, title,
+#                                       colorbar, clim, draw)
+NO_DATA_VALUE = -9999
+
+
+def make_file_names(testnum, NN, testdir='testtiff'):
+    if type(NN) == list:
+        N = NN[0]
+    else:
+        N = NN
+
+    base = os.path.join(testdir, 'test_NN%03d_%03d' % (N, testnum))
+    return {"elev": base + '_elev.tif', "ang": base + '_ang.tif',
+            "fel": base + '_fel.tif', 'uca': base + '_uca.tif'}
+
+
+def mk_xy_latlon(N):
+    raster = np.zeros((N, N))
+    if os.path.exists('temp.tif'):
+        os.remove('temp.tif')
+    r, transform = mk_geotiff_obj(raster, 'temp.tif')
+    dx, dy, _, _ = mk_dx_dy_from_geotif_layer(r)
+    y = np.concatenate([[0], np.cumsum(dx)])
+    x = np.concatenate([[0], np.cumsum(dy)])
+    # Center it on zero
+    x = x - (x.max() - x.min()) / 2.0
+    y = y - (y.max() - y.min()) / 2.0
+    scale = np.sqrt(x**2 + y**2).max()
+    x = x / scale
+    y = y / scale
+    Y, X = np.meshgrid(y, x)
+
+    return X, Y
+
+
+def make_elev_ang(testnum, NN, raster, angle, uca=None, testdir='testtiff'):
+    # Convert masked array to filled array
+    raster = raster.filled()
+    angle = angle.filled()
+    filename = make_file_names(testnum, NN, testdir)
+    try:
+        if not os.path.exists(testdir):
+            os.makedirs(testdir)
+        if not os.path.exists(filename['elev']):
+            elev, transform = mk_geotiff_obj(raster, filename['elev'])
+            del transform
+            del elev
+            print("Created", filename['elev'])
+            ang, driver = mk_geotiff_obj(angle, filename['ang'])
+            del ang
+            del driver
+            print("Created", filename['ang'])
+        if not os.path.exists(filename['uca']) and uca is not None:
+            ucaf, driver = mk_geotiff_obj(uca, filename['uca'])
+            del ucaf
+            del driver
+            print("Created", filename['uca'])
+        else:
+            print("Already exists or None", filename['uca'])
+    finally:
+        ucaf = None
+        elev = None
+        ang = None
+        driver = None
+
+# Define the inidividual elevation/angles for the test-cases
+def case_cone(x, y, noise=False):
+    # %%Cone
+    NN = x.shape[0]
+    raster = np.ma.masked_array(1 - np.sqrt((y)**2 + (x)**2) / np.sqrt(2.),
+                                mask=np.zeros(x.shape, bool),
+                                fill_value=NO_DATA_VALUE)
+    angle = np.ma.masked_array(np.arctan2(x, -y) + np.pi,
+                               mask=np.zeros(x.shape, bool),
+                               fill_value=NO_DATA_VALUE)
+    ncell = np.round(np.sqrt((y)**2 + (x)**2) / (1.0 / NN))
+    uca = np.ma.masked_array(np.pi * ((y)**2 + (x)**2) / ncell * NN**2 / 4.,
+                             mask=np.zeros(x.shape, bool),
+                             fill_value=NO_DATA_VALUE)
+    # We expect the total upstream contributing area to be the
+    # total area of the data
+    summat = np.zeros_like(uca)
+    summat[:, 0] = 1
+    summat[:, -1] = 1
+    summat[0, :] = 1
+    summat[-1, :] = 1
+    uca = uca * NN ** 2 / np.nansum(summat * uca)
+    if noise:
+        np.random.seed(1773)
+        raster += np.abs(np.random.randn(*raster.shape)**2) * 0.0003
+        raster[:, :] = gaussian_filter(raster, 2, mode='constant')
+#
+    return raster, angle, uca
+
+
+def case_cone_scaled(x, y, noise):
+    raster, angle, uca = case_cone(x, y, noise)
+    raster = raster - raster.ravel().min()  # (make it all positive)
+    return raster, angle, uca
+
+
+def case_line(x, y, line):
+    raster = np.ma.masked_array(line[0] * x + line[1] * y,
+                                mask=np.zeros(x.shape, bool),
+                                fill_value=NO_DATA_VALUE)
+    # normalize
+    raster = raster - raster.min()
+    raster = raster / raster.max()
+
+    angle = np.ma.masked_array(np.arctan2(-line[0], line[1])
+                               * np.ones(raster.shape) + np.pi,
+                               mask=np.zeros(x.shape, bool),
+                               fill_value=NO_DATA_VALUE)
+    NN = x.shape[0]
+
+    if line[0] > 0:
+        x_line = 1
+    else:
+        x_line = -1
+    if line[1] > 0:
+        y_line = 1
+    else:
+        y_line = -1
+
+    tx = (x_line - x) / (line[0] + 1e-17)
+    ty = (y_line - y) / (line[1] + 1e-17)
+    if line[0] == 0:
+        t = ty
+    elif line[1] == 0:
+        t = tx
+    else:
+        t = np.minimum(tx, ty)
+    uca = t  # * (line[0]**2 + line[1]**2)** (0.5)
+    uca = np.ma.masked_array(np.round(t * NN) / 2,
+                             mask=np.zeros(x.shape, bool),
+                             fill_value=NO_DATA_VALUE)
+    return raster, angle, uca
+
+
+def case_opposing_slopes(x, y, line):
+    raster = np.ma.masked_array(line[0] * x + line[1] * y,
+                                mask=np.zeros(x.shape, bool),
+                                fill_value=NO_DATA_VALUE)
+    I = -x * line[1] + y * line[0] > 0
+    raster[I] = -line[0] * x[I] - line[1] * y[I]
+    # normalize
+    raster = raster - raster.min()
+    raster = raster / raster.max()
+
+    angle = np.ma.masked_array(np.arctan2(-line[0], line[1])
+                               * np.ones(raster.shape) + np.pi,
+                               mask=np.zeros(x.shape, bool),
+                               fill_value=NO_DATA_VALUE)
+    angle[I] = np.arctan2(line[0], -line[1]) + np.pi
+    return raster, angle
+
+
+def case_ring_flat(x, y, drains):
+    raster, angle, uca = case_cone(x, y)
+    if type(drains[0]) != list:
+        drains = [drains]
+    # Set the flat
+    I1 = raster >= 0.7
+    I = (raster > 0.5) & (raster < 0.7)
+    angle[I] = -1
+
+    raster2 = raster.copy()
+    for drain in drains:
+        raster[drain[0], drain[1]] -= np.min(raster[drain[0], drain[1]])
+    raster[I] = 0.51
+    raster[I1] = raster2[I1]
+    return raster, angle
+
+
+def case_top_flat(x, y, drains):
+    raster, angle, uca = case_cone(x, y)
+    if type(drains[0]) != list:
+        drains = [drains]
+    # Set the flat
+    I = raster >= 0.7
+    angle[I] = -1
+
+    for drain in drains:
+        raster[drain[0], drain[1]] -= np.min(raster[drain[0], drain[1]])
+    raster[I] = 0.75
+    return raster, angle
+
+
+def case_line_flat(x, y, line):
+    raster, angle, uca = case_line(x, y, line)
+    flat_raster = np.ma.masked_array(1 - np.sqrt((y)**2 + (x)**2) / np.sqrt(2.),
+                                     mask=np.zeros(x.shape, bool),
+                                     fill_value=NO_DATA_VALUE)
+    # normalize
+    raster = raster - raster.min()
+    raster = raster / raster.max()
+
+    # Set the flat
+    I = flat_raster >= 0.7
+    raster[I] = 0.5
+    angle[I] = -1
+
+    return raster, angle
+
+
+def case_pit_of_dispair(x, y, drains):
+    if len(drains) > 0 and type(drains[0]) != list:
+        drains = [drains]
+        # %% The pit of dispair
+    raster = np.ma.masked_array(1 + np.sqrt((y)**2 + (x)**2) / np.sqrt(2.),
+                                mask=np.zeros(x.shape, bool),
+                                fill_value=NO_DATA_VALUE)
+
+    angle = np.ma.masked_array(np.arctan2(-x, y) + np.pi,
+                               mask=np.zeros(x.shape, bool),
+                               fill_value=NO_DATA_VALUE)
+    for drain in drains:
+        N = len(raster[drain[0], drain[1]].ravel())
+        raster[drain[0], drain[1]] = np.linspace(0, 1, N)\
+            .reshape(raster[drain[0], drain[1]].shape)
+
+    return raster, angle
+
+
+def case_trough_of_dispair(x, y, line):
+    # %% The trough of dispair
+    NN = x.shape[0]
+    raster = np.ma.masked_array(line[0] * x + line[1] * y,
+                                mask=np.zeros(x.shape, bool),
+                                fill_value=NO_DATA_VALUE)
+    I = x * line[1] + y * line[0] > 0
+    raster[I] = -line[0] * x[I] - line[1] * y[I]
+    raster += 0.1 * (-line[0] * x + line[1] * y)
+
+    # normalize
+    raster = raster - raster.min()
+    raster = raster / raster.max()
+
+    angle = np.ma.masked_array(np.arctan2(-line[0] * 0.9, line[1] * 1.1)
+                               * np.ones(raster.shape) + np.pi,
+                               mask=np.zeros(x.shape, bool),
+                               fill_value=NO_DATA_VALUE)
+    angle[I] = np.arctan2(line[0] * 1.1, -line[1] * 0.9) + np.pi
+    angle[[np.arange(NN), np.arange(NN)]] = 3 * np.pi / 4
+
+    return raster, angle
+
+
+def case_real_data(x, y, filename='N43W-72_N44W-71_elev.tif', NN=None):
+# def case_real_data(x, y, filename='N72W-112N73W-111_elev.tif', NN=None):
+    if NN is None:
+        NX, NY = x.shape
+        NX0, NY0 = [0, 0]
+    elif type(NN) == list:
+        NX0, NX, NY0, NY = NN
+    else:
+        NX0, NX, NY0, NY = [0, NN, 0, NN]
+    elev_file = read_raster(file_name=filename)
+    test_data = elev_file.read()
+    raster = test_data[NX0:NX, NY0:NY]
+    del elev_file
+    del test_data
+    angle = -1 + 0 * raster
+    return raster, angle
+
+
+def case_pit_of_carkoon(x, y):
+    raster, angle = case_pit_of_dispair(x, y, [])
+
+    I = np.argmin(raster)
+    raster.mask.ravel()[I] = True
+    angle.mask.ravel()[I] = True
+    return raster, angle
+
+
+def case_sea_of_saw(x, y):
+    raster, angle, uca = case_cone(x, y)
+    I = (raster < 0.4) & (x > 0)
+    raster.mask[I] = True
+    angle.mask[I] = True
+    return raster, angle
+
+
+def spiral(x, y):
+    n, m = x.shape
+    # make the walls
+    raster = np.ma.masked_array((1.0 - np.maximum(np.abs(x), np.abs(y))**2)
+                                * (n * m) / 2 + (n + m) * 2,
+                                mask=np.zeros(x.shape, bool),
+                                fill_value=NO_DATA_VALUE)
+
+    # make the spiral
+    start = [0, 1]
+    stop = [n - 2, m - 2]
+    i, j = start
+    start = [-1, 1]
+    elev = 0
+    count = 0
+    sgn = [1, 1]
+    while count < n*m / 2:
+        count += 1
+        raster[i, j] = elev
+        elev += 1
+        if i < stop[0] and sgn[0] > 0:
+            i += 1
+        elif j < stop[1] and sgn[1] > 0:
+            j += 1
+        elif i == stop[0] and j == stop[1] and sgn[1] > 0:
+            start[0] += 2
+            start[1] += 2
+            sgn = [-1, -1]
+            i -= 1
+        elif i > start[0] and sgn[0] < 0:
+            i -= 1
+        elif j > start[1] and sgn[1] < 0:
+            j -= 1
+        elif i == start[0] and j == start[1] and sgn[1] < 0:
+            stop[0] -= 2
+            stop[1] -= 2
+            sgn = [1, 1]
+            i += 1
+        else:
+            break
+
+    return raster, raster * 0
+
+
+def mk_test_multifile(testnum, NN, testdir, nx_grid=3, ny_grid=4, nx_overlap=16,
+                      ny_overlap=32, lat=[46, 45], lon=[-73, -72]):
+    """
+    Written to make test case for multi-file edge resolution.
+    """
+    path = os.path.split(make_file_names(testnum, NN, os.path.join(
+                                               testdir, 'chunks'))['elev'])[0]
+    try:
+        os.makedirs(path)
+    except:
+        pass
+
+    def _get_chunk_edges(NN, chunk_size, chunk_overlap):
+        chunk_size = int(chunk_size)
+        left_edge = np.arange(0, NN - chunk_overlap, chunk_size)
+        left_edge[1:] -= chunk_overlap // 2
+        right_edge = np.arange(0, NN - chunk_overlap, chunk_size)
+        right_edge[:-1] = right_edge[1:] + int(np.ceil(chunk_overlap / 2))
+        right_edge[-1] = NN
+        right_edge = np.minimum(right_edge, NN)
+        return left_edge, right_edge
+
+    elev_data, ang_data, fel_data = get_test_data(testnum, NN)
+    raster = elev_data
+
+    ni, nj = raster.shape
+
+    top_edge, bottom_edge = _get_chunk_edges(ni, np.ceil(ni / ny_grid), ny_overlap)
+    left_edge, right_edge = _get_chunk_edges(nj, np.ceil(nj / nx_grid), nx_overlap)
+
+#    gc = elev_data.grid_coordinates
+#    lat = gc.y_axis
+#    lon = gc.x_axis
+    lat = np.linspace(lat[0], lat[1], ni)
+    lon = np.linspace(lon[0], lon[1], nj)
+    count = 0
+    for te, be in zip(top_edge, bottom_edge):
+        for le, re in zip(left_edge, right_edge):
+            count += 1
+            fn = os.path.join(path,
+                              get_fn_from_coords((lat[be-1], lon[le], lat[te],
+                                                  lon[re-1]), 'elev'))
+            print(count, ": [%d:%d, %d:%d]" % (te, be, le, re), \
+                '(lat, lon) = (%g to %g, %g to %g)' % (lat[te], lat[be-1],
+                                                       lon[le], lon[re-1]), \
+                'min,max = (%g to %g, %g to %g)' % (lat.min(), lat.max(),
+                                                    lon.min(), lon.max()))
+            mk_geotiff_obj(raster[te:be, le:re], fn,
+                           bands=1,
+                           lat=[lat[te], lat[be-1]], lon=[lon[le], lon[re-1]])
+
+
+# %% MAKE ALL THE TESTS
+def make_test_files(NN=32, plotflag=False, testdir='testtiff', testnum=None):
+    # Common
+    if plotflag:
+        from matplotlib.pyplot import (figure, subplot, imshow, title,
+                                       colorbar, clim, draw)
+
+    if type(NN) == list:
+        N = np.max(NN)
+    else:
+        N = NN
+    x, y = np.mgrid[-1:1:complex(0, N), -1:1:complex(0, N)]
+    lat, lon = mk_xy_latlon(N)
+
+    # The first brace it just to avoid the line-continuouation character
+    tests = [[case_cone]  # case 0
+             + [lambda x, y: case_line(x, y, [1, 0]),
+                lambda x, y: case_line(x, y, [-1, 0]),
+                lambda x, y: case_line(x, y, [0, 1]),
+                lambda x, y: case_line(x, y, [0, -1]),
+                lambda x, y: case_line(x, y, [1, 1]),
+                lambda x, y: case_line(x, y, [-1, 1]),
+                lambda x, y: case_line(x, y, [1, -1]),
+                lambda x, y: case_line(x, y, [-1, -1])
+                ]  # cases 1-8, 8 cases in total for the lines
+             + [lambda x, y: case_opposing_slopes(x, y, [1, 0]),
+                lambda x, y: case_opposing_slopes(x, y, [0, 1]),
+                lambda x, y: case_opposing_slopes(x, y, [1, 1]),
+                lambda x, y: case_opposing_slopes(x, y, [-1, 1])
+                ]  # cases 9-12, 4 cases in total for the opposing slopes
+             + [lambda x, y: case_ring_flat(x, y, [slice(NN), slice(NN)]),
+                lambda x, y: case_ring_flat(x, y, [slice(NN//2, NN//2+1),
+                                                   slice(NN//2, NN)]),
+                lambda x, y: case_ring_flat(x, y, [[slice(NN//2, NN//2+1),
+                                                    slice(0, NN//2)],
+                                                   [slice(NN//2, NN//2+1),
+                                                    slice(NN//2, NN)]]),
+                lambda x, y: case_ring_flat(x, y, [[slice(NN//2, NN),
+                                                    slice(NN//2, NN//2+1)],
+                                                   [slice(NN//2, NN//2+1),
+                                                    slice(0, NN//2)],
+                                                   [slice(NN//2, NN//2+1),
+                                                    slice(NN//2, NN)]]),
+                lambda x, y: case_ring_flat(x, y, [[slice(0, NN//2),
+                                                    slice(NN//2, NN//2+1)],
+                                                   [slice(NN//2, NN),
+                                                    slice(NN//2, NN//2+1)],
+                                                   [slice(NN//2, NN//2+1),
+                                                    slice(0, NN//2)],
+                                                   [slice(NN//2, NN//2+1),
+                                                    slice(NN//2, NN)]])
+                ]  # cases 13-17, 5 cases in total for the ring flats
+             + [lambda x, y: case_top_flat(x, y, [slice(NN), slice(NN)]),
+                lambda x, y: case_top_flat(x, y, [slice(NN//2, NN//2+1),
+                                                  slice(NN//2, NN)]),
+                lambda x, y: case_top_flat(x, y, [slice(NN//2, NN//2+1),
+                                                  slice(0, NN//2)]),
+                lambda x, y: case_top_flat(x, y, [slice(NN//2, NN),
+                                                  slice(NN//2, NN//2+1)]),
+                lambda x, y: case_top_flat(x, y, [slice(0, NN//2),
+                                                  slice(NN//2, NN//2+1)])
+                ]  # cases 18-22, 5 cases total for top flats
+             + [lambda x, y: case_line_flat(x, y, [-1, -1])]  # case 23
+             + [lambda x, y: case_pit_of_dispair(x, y, [slice(NN//2, NN//2+1),
+                                                        slice(0, NN//2)]),
+                lambda x, y: case_pit_of_dispair(x, y, [slice(0, NN//2),
+                                                        slice(NN//2, NN//2+1)])
+                ]  # cases 24 and 25
+             + [lambda x, y: case_trough_of_dispair(x, y, [-1, 1])]  # case 26
+             + [lambda x, y: case_real_data(x, y, NN=NN)]  # case 27
+             + [case_pit_of_carkoon]  # Case 28
+             + [case_sea_of_saw]  # case 29
+             + [spiral]  # case 30
+             + [lambda x, y: case_cone(x, y, True)]  # case 31
+             + [lambda x, y: case_cone_scaled(lon, lat, True)]  # case 32
+             + [lambda x, y: case_cone(x, y, False)]  # case 32
+             + [lambda x, y: case_cone_scaled(lon, lat, False)]  # case 33
+             ]
+
+    tests = tests[0]  # Remove the outer list
+    if testnum is None:
+        testnum = 0
+    else:
+        tests = [tests[testnum]]
+
+    for test in tests:
+        res = test(x, y)
+        raster, angle = res[:2]
+        if len(res) == 3:
+            uca = res[2]
+        else:
+            uca = None
+        make_elev_ang(testnum, NN, raster, angle, uca, testdir)
+
+        if plotflag:
+            figure(testnum)
+            subplot(121)
+            imshow(raster, interpolation='none'); colorbar()
+            draw()
+            title('Elevation %d' % testnum)
+            subplot(122)
+            imshow(angle / np.pi * 180, interpolation='none'); colorbar(); clim([0, 360])
+            draw()
+            title('Angle %d' % testnum)
+        testnum += 1
+
+
+def get_test_data(test_num, NN, testdir='testtiff'):
+    filenames = make_file_names(test_num, NN, testdir)
+    if not os.path.exists(filenames['elev']):
+        make_test_files(NN, testdir=testdir, testnum=test_num)
+    elev_data = read_raster(filenames['elev']).read(1)
+    ang_data = read_raster(filenames['ang']).read(1)
+    return elev_data, ang_data, None
+
```

### Comparing `pyDEM-0.2.0/pydem/utils.py` & `pyDEM-1.0.0/pydem/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,570 +1,552 @@
-# -*- coding: utf-8 -*-
-"""
-   Copyright 2015 Creare
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
-
-
-Helper Utilities
-=================
-The module supplies helper utility functions that may have some more general
-use.
-
-Usage Notes
-------------
-To rename elevation files to the format required by this package use:
-rename_files function.
-
-Developer Notes
-----------------
-
-Created on Tue Oct 14 17:25:50 2014
-
-@author: mpu
-"""
-from geopy.distance import distance
-import os
-import gdal
-import osr
-import re
-from reader.gdal_reader import GdalReader
-
-import numpy as np
-from scipy.ndimage.filters import minimum_filter
-from scipy.ndimage.measurements import center_of_mass
-
-def rename_files(files, name=None):
-    """
-    Given a list of file paths for elevation files, this function will rename
-    those files to the format required by the pyDEM package.
-
-    This assumes a .tif extension.
-
-    Parameters
-    -----------
-    files : list
-        A list of strings of the paths to the elevation files that will be
-        renamed
-    name : str (optional)
-        Default = None. A suffix to the filename. For example
-        <filename>_suffix.tif
-
-    Notes
-    ------
-    The files are renamed in the same directory as the original file locations
-    """
-    for fil in files:
-        elev_file = GdalReader(file_name=fil)
-        elev, = elev_file.raster_layers
-        fn = get_fn(elev, name)
-        del elev_file
-        del elev
-        fn = os.path.join(os.path.split(fil)[0], fn)
-        os.rename(fil, fn)
-        print "Renamed", fil, "to", fn
-
-
-def parse_fn(fn):
-    """ This parses the file name and returns the coordinates of the tile
-
-    Parameters
-    -----------
-    fn : str
-        Filename of a GEOTIFF
-
-    Returns
-    --------
-    coords = [LLC.lat, LLC.lon, URC.lat, URC.lon]
-    """
-    try:
-        parts = os.path.splitext(os.path.split(fn)[-1])[0].replace('o', '.')\
-            .split('_')[:2]
-        coords = [float(crds)
-                  for crds in re.split('[NSEW]', parts[0] + parts[1])[1:]]
-    except:
-        coords = [np.nan] * 4
-    return coords
-
-
-def get_fn(elev, name=None):
-    """
-    Determines the standard filename for a given GeoTIFF Layer.
-
-    Parameters
-    -----------
-    elev : GdalReader.raster_layer
-        A raster layer from the GdalReader object.
-    name : str (optional)
-        An optional suffix to the filename.
-    Returns
-    -------
-    fn : str
-        The standard <filename>_<name>.tif with suffix (if supplied)
-    """
-    gcs = elev.grid_coordinates
-    coords = [gcs.LLC.lat, gcs.LLC.lon, gcs.URC.lat, gcs.URC.lon]
-    return get_fn_from_coords(coords, name)
-
-
-def get_fn_from_coords(coords, name=None):
-    """ Given a set of coordinates, returns the standard filename.
-
-    Parameters
-    -----------
-    coords : list
-        [LLC.lat, LLC.lon, URC.lat, URC.lon]
-    name : str (optional)
-        An optional suffix to the filename.
-
-    Returns
-    -------
-    fn : str
-        The standard <filename>_<name>.tif with suffix (if supplied)
-    """
-    NS1 = ["S", "N"][coords[0] > 0]
-    EW1 = ["W", "E"][coords[1] > 0]
-    NS2 = ["S", "N"][coords[2] > 0]
-    EW2 = ["W", "E"][coords[3] > 0]
-    new_name = "%s%0.3g%s%0.3g_%s%0.3g%s%0.3g" % \
-        (NS1, coords[0], EW1, coords[1], NS2, coords[2], EW2, coords[3])
-    if name is not None:
-        new_name += '_' + name
-    return new_name.replace('.', 'o') + '.tif'
-
-
-def mk_dx_dy_from_geotif_layer(geotif):
-    """
-    Extracts the change in x and y coordinates from the geotiff file. Presently
-    only supports WGS-84 files.
-    """
-    ELLIPSOID_MAP = {'WGS84': 'WGS-84'}
-    ellipsoid = ELLIPSOID_MAP[geotif.grid_coordinates.wkt]
-    d = distance(ellipsoid=ellipsoid)
-    dx = geotif.grid_coordinates.x_axis
-    dy = geotif.grid_coordinates.y_axis
-    dX = np.zeros((dy.shape[0]-1))
-    for j in xrange(len(dX)):
-        dX[j] = d.measure((dy[j+1], dx[1]), (dy[j+1], dx[0])) * 1000  # km2m
-    dY = np.zeros((dy.shape[0]-1))
-    for i in xrange(len(dY)):
-        dY[i] = d.measure((dy[i], 0), (dy[i+1], 0)) * 1000  # km2m
-    return dX, dY
-
-
-def mk_geotiff_obj(raster, fn, bands=1, gdal_data_type=gdal.GDT_Float32,
-                   lat=[46, 45], lon=[-73, -72]):
-    """
-    Creates a new geotiff file objects using the WGS84 coordinate system, saves
-    it to disk, and returns a handle to the python file object and driver
-
-    Parameters
-    ------------
-    raster : array
-        Numpy array of the raster data to be added to the object
-    fn : str
-        Name of the geotiff file
-    bands : int (optional)
-        See :py:func:`gdal.GetDriverByName('Gtiff').Create
-    gdal_data : gdal.GDT_<type>
-        Gdal data type (see gdal.GDT_...)
-    lat : list
-        northern lat, southern lat
-    lon : list
-        [western lon, eastern lon]
-    """
-    NNi, NNj = raster.shape
-    driver = gdal.GetDriverByName('GTiff')
-    obj = driver.Create(fn, NNj, NNi, bands, gdal_data_type)
-    pixel_height = -np.abs(lat[0] - lat[1]) / (NNi - 1.0)
-    pixel_width = np.abs(lon[0] - lon[1]) / (NNj - 1.0)
-    obj.SetGeoTransform([lon[0], pixel_width, 0, lat[0], 0, pixel_height])
-    srs = osr.SpatialReference()
-    srs.SetWellKnownGeogCS('WGS84')
-    obj.SetProjection(srs.ExportToWkt())
-    obj.GetRasterBand(1).WriteArray(raster)
-    return obj, driver
-
-
-def sortrows(a, i=0, index_out=False, recurse=True):
-    """ Sorts array "a" by columns i
-
-    Parameters
-    ------------
-    a : np.ndarray
-        array to be sorted
-    i : int (optional)
-        column to be sorted by, taken as 0 by default
-    index_out : bool (optional)
-        return the index I such that a(I) = sortrows(a,i). Default = False
-    recurse : bool (optional)
-        recursively sort by each of the columns. i.e.
-        once column i is sort, we sort the smallest column number
-        etc. True by default.
-
-    Returns
-    --------
-    a : np.ndarray
-        The array 'a' sorted in descending order by column i
-    I : np.ndarray (optional)
-        The index such that a[I, :] = sortrows(a, i). Only return if
-        index_out = True
-
-    Examples
-    ---------
-    >>> a = array([[1,2],[3,1],[2,3]])
-    >>> b = sortrows(a,0)
-    >>> b
-    array([[1, 2],
-           [2, 3],
-           [3, 1]])
-    c, I = sortrows(a,1,True)
-
-    >>> c
-    array([[3, 1],
-           [1, 2],
-           [2, 3]])
-    >>> I
-    array([1, 0, 2])
-    >>> a[I,:] - c
-    array([[0, 0],
-           [0, 0],
-           [0, 0]])
-    """
-    I = np.argsort(a[:, i])
-    a = a[I, :]
-    # We recursively call sortrows to make sure it is sorted best by every
-    # column
-    if recurse & (len(a[0]) > i + 1):
-        for b in np.unique(a[:, i]):
-            ids = a[:, i] == b
-            colids = range(i) + range(i+1, len(a[0]))
-            a[np.ix_(ids, colids)], I2 = sortrows(a[np.ix_(ids, colids)],
-                                                  0, True, True)
-            I[ids] = I[np.nonzero(ids)[0][I2]]
-
-    if index_out:
-        return a, I
-    else:
-        return a
-
-def get_adjacent_index(I, shape, size):
-    """
-    Find indices 2d-adjacent to those in I. Helper function for get_border*.
-
-    Parameters
-    ----------
-    I : np.ndarray(dtype=int)
-        indices in the flattened region
-    shape : tuple(int, int)
-        region shape
-    size : int
-        region size (technically computable from shape)
-
-    Returns
-    -------
-    J : np.ndarray(dtype=int)
-        indices orthogonally and diagonally adjacent to I
-
-    """
-
-    m, n = shape
-    In = I % n
-    bL = In != 0
-    bR = In != n-1
-    
-    J = np.concatenate([
-        # orthonally adjacent
-        I - n,
-        I[bL] - 1,
-        I[bR] + 1,
-        I + n,
-
-        # diagonally adjacent
-        I[bL] - n-1,
-        I[bR] - n+1,
-        I[bL] + n-1,
-        I[bR] + n+1])
-
-    # remove indices outside the array
-    J = J[(J>=0) & (J<size)]
-
-    return J
-
-def get_border_index(I, shape, size):
-    """
-    Get flattened indices for the border of the region I.
-
-    Parameters
-    ----------
-    I : np.ndarray(dtype=int)
-        indices in the flattened region.
-    size : int
-        region size (technically computable from shape argument)
-    shape : tuple(int, int)
-        region shape
-
-    Returns
-    -------
-    J : np.ndarray(dtype=int)
-        indices orthogonally and diagonally bordering I
-    """
-
-    J = get_adjacent_index(I, shape, size)
-
-    # instead of setdiff?
-    # border = np.zeros(size)
-    # border[J] = 1
-    # border[I] = 0
-    # J, = np.where(border)
-
-    return np.setdiff1d(J, I)
-
-def get_border_mask(region):
-    """
-    Get border of the region as a boolean array mask.
-
-    Parameters
-    ----------
-    region : np.ndarray(shape=(m, n), dtype=bool)
-        mask of the region
-
-    Returns
-    -------
-    border : np.ndarray(shape=(m, n), dtype=bool)
-        mask of the region border (not including region)
-    """
-
-    # common special case (for efficiency)
-    internal = region[1:-1, 1:-1]
-    if internal.all() and internal.any():
-        return ~region
-    
-    I, = np.where(region.ravel())
-    J = get_adjacent_index(I, region.shape, region.size)
-
-    border = np.zeros(region.size, dtype='bool')
-    border[J] = 1
-    border[I] = 0
-    border = border.reshape(region.shape)
-
-    return border
-
-_ORTH2 = np.array([[0, 1, 0], [1, 1, 1], [0, 1, 0]])
-_SQRT2 = np.sqrt(2.0)
-def get_distance(region, src):
-    """
-    Compute within-region distances from the src pixels.
-
-    Parameters
-    ----------
-    region : np.ndarray(shape=(m, n), dtype=bool)
-        mask of the region
-    src : np.ndarray(shape=(m, n), dtype=bool)
-        mask of the source pixels to compute distances from.
-
-    Returns
-    -------
-    d : np.ndarray(shape=(m, n), dtype=float)
-        approximate within-region distance from the nearest src pixel;
-        (distances outside of the region are arbitrary).
-    """
-
-    dmax = float(region.size)
-    d = np.full(region.shape, dmax)
-    d[src] = 0
-    for n in range(region.size):
-        d_orth = minimum_filter(d, footprint=_ORTH2) + 1
-        d_diag = minimum_filter(d, (3, 3)) + _SQRT2
-        d_adj = np.minimum(d_orth[region], d_diag[region])
-        d[region] = np.minimum(d_adj, d[region])
-        if (d[region] < dmax).all():
-            break
-    return d
-
-def make_slice(a, b):
-    if a < b:
-        return slice(a, b)
-    else:
-        return slice(b, a)
-
-def grow_slice(slc, size):
-    """
-    Grow a slice object by 1 in each direction without overreaching the list.
-
-    Parameters
-    ----------
-    slc: slice
-        slice object to grow
-    size: int
-        list length
-
-    Returns
-    -------
-    slc: slice
-       extended slice 
-
-    """
-
-    return slice(max(0, slc.start-1), min(size, slc.stop+1))
-
-def grow_obj(obj, shape):
-    """
-    Grow a 2d object by 1 in all directions without overreaching the array.
-
-    Parameters
-    ----------
-    obj: tuple(slice, slice)
-        Pair of slices (e.g. from scipy.ndimage.measurements.find_objects)
-    shape: tuple(int, int)
-        2d array shape
-
-    Returns
-    -------
-    obj: tuple(slice, slice)
-        extended slice objects
-    """
-
-    return grow_slice(obj[0], shape[0]), grow_slice(obj[1], shape[1])
-
-def is_edge(obj, shape):
-    """
-    Check if a 2d object is on the edge of the array.
-
-    Parameters
-    ----------
-    obj : tuple(slice, slice)
-        Pair of slices (e.g. from scipy.ndimage.measurements.find_objects)
-    shape : tuple(int, int)
-        Array shape.
-
-    Returns
-    -------
-    b : boolean
-        True if the object touches any edge of the array, else False.
-    """
-
-    if obj[0].start == 0: return True
-    if obj[1].start == 0: return True
-    if obj[0].stop == shape[0]: return True
-    if obj[1].stop == shape[1]: return True
-    return False
-
-def find_centroid(region):
-    """
-    Finds an approximate centroid for a region that is within the region.
-    
-    Parameters
-    ----------
-    region : np.ndarray(shape=(m, n), dtype='bool')
-        mask of the region.
-
-    Returns
-    -------
-    i, j : tuple(int, int)
-        2d index within the region nearest the center of mass.
-    """
-
-    x, y = center_of_mass(region)
-    w = np.argwhere(region)
-    i, j = w[np.argmin(np.linalg.norm(w - (x, y), axis=1))]
-    return i, j
-
-def plot_fill_flat(roi, out, region, source, drain, dL, dH):
-    from matplotlib import pyplot
-
-    plot_detail = roi.size < 500
-    cmap = 'Greens'
-
-    pyplot.figure()
-
-    ax = pyplot.subplot(221)
-    pyplot.axis('off')
-    pyplot.title('unfilled')
-    im = pyplot.imshow(roi, interpolation='none')
-    im.set_cmap(cmap)
-    if plot_detail:
-        y, x = np.where(region); pyplot.plot(x, y, 'k.')
-        y, x = np.where(source); pyplot.plot(x, y, lw=0, color='k', marker='$H$', ms=12)
-        y, x = np.where(drain);   pyplot.plot(x, y, lw=0, color='k', marker='$L$', ms=12)
-    
-    pyplot.subplot(222, sharex=ax, sharey=ax)
-    pyplot.axis('off')
-    pyplot.title('filled')
-    im = pyplot.imshow(out, interpolation='none')
-    im.set_cmap(cmap)
-    if plot_detail:
-        for elev in np.unique(out):
-            y, x = np.where(out==elev)
-            pyplot.plot(x, y, lw=0, color='k', marker='$%.3f$' % elev, ms=20)
-
-    if plot_detail:
-        flat = (minimum_filter(out, (3, 3)) >= out) & region
-        y, x = np.where(flat); pyplot.plot(x, y, 'r_', ms=24)
-        
-        pyplot.subplot(223, sharex=ax, sharey=ax)
-        pyplot.axis('off')
-        pyplot.title('dL')
-        im = pyplot.imshow(roi, interpolation='none')
-        im.set_cmap(cmap)
-        for d in np.unique(dL):
-            if d == region.size: continue
-            y, x = np.where(dL==d)
-            pyplot.plot(x, y, lw=0, color='k', marker='$%.2f$' % d, ms=24)
-
-        pyplot.subplot(224, sharex=ax, sharey=ax)
-        pyplot.axis('off')
-        pyplot.title('dH')
-        im = pyplot.imshow(roi, interpolation='none')
-        im.set_cmap(cmap)
-        for d in np.unique(dH):
-            if d == region.size: continue
-            y, x = np.where(dH==d)
-            pyplot.plot(x, y, lw=0, color='k', marker='$%.2f$' % d, ms=24)
-
-    pyplot.tight_layout()
-
-def plot_drain_pit(self, pit, drain, prop, s, elev, area):
-    from matplotlib import pyplot
-    
-    cmap = 'Greens'
-
-    ipit, jpit = np.unravel_index(pit, elev.shape)
-    Idrain, Jdrain = np.unravel_index(drain, elev.shape)
-    Iarea, Jarea = np.unravel_index(area, elev.shape)
-
-    imin = max(0, min(ipit, Idrain.min(), Iarea.min())-1)
-    imax = min(elev.shape[0], max(ipit, Idrain.max(), Iarea.max()) + 2)
-    jmin = max(0, min(jpit, Jdrain.min(), Jarea.min())-1)
-    jmax = min(elev.shape[1], max(jpit, Jdrain.max(), Jarea.max()) + 2)
-    roi = (slice(imin, imax), slice(jmin, jmax))
-
-    pyplot.figure()
-    
-    ax = pyplot.subplot(221);
-    pyplot.axis('off')
-    im = pyplot.imshow(elev[roi], interpolation='none'); im.set_cmap(cmap)
-    pyplot.plot(jpit-jmin, ipit-imin, lw=0, color='k', marker='$P$', ms=10)
-    pyplot.plot(Jarea-jmin, Iarea-imin, 'k.')
-    pyplot.plot(Jdrain-jmin, Idrain-imin, lw=0, color='k', marker='$D$', ms=10)
-
-    pyplot.subplot(223, sharex=ax, sharey=ax); pyplot.axis('off')
-    im = pyplot.imshow(elev[roi], interpolation='none'); im.set_cmap(cmap)
-    for i, j, val in zip(Idrain, Jdrain, prop):
-        pyplot.plot(j-jmin, i-imin, lw=0, color='k', marker='$%.2f$' % val, ms=16)
-
-    pyplot.subplot(224, sharex=ax, sharey=ax); pyplot.axis('off')
-    im = pyplot.imshow(elev[roi], interpolation='none'); im.set_cmap(cmap)
-    for i, j, val in zip(Idrain, Jdrain, s):
-        pyplot.plot(j-jmin, i-imin, lw=0, color='k', marker='$%.2f$' % val, ms=16)
-
-    pyplot.tight_layout()
+# -*- coding: utf-8 -*-
+"""
+   Copyright 2015-2024 Creare
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
+
+
+Helper Utilities
+=================
+The module supplies helper utility functions that may have some more general
+use.
+
+
+Developer Notes
+----------------
+
+Created on Tue Oct 14 17:25:50 2014
+
+@author: mpu
+"""
+from geopy.distance import distance
+import os
+import re
+
+import numpy as np
+from scipy.ndimage import minimum_filter
+from scipy.ndimage import center_of_mass
+import rasterio
+
+def read_raster(fn):
+    return rasterio.open(fn)
+
+def dem_processor_from_raster_kwargs(fn):
+    dataset = read_raster(fn)
+    dx, dy, dx2, dy2 = mk_dx_dy_from_geotif_layer(dataset)
+    elev = dataset.read(1)
+    return dict(dX=dx, dY=dy, elev=elev, bounds=dataset.bounds, transform=dataset.transform,
+                dX2=dx2, dY2=dy2)
+
+def mk_transform(lat_top, lon_left, dlat, dlon, lat_lon_centered=False):
+    if lat_lon_centered:
+        lat_top -= dlat / 2  # expect dlat < 0
+        lon_left -= dlon / 2
+    transform = rasterio.transform.Affine.translation(lon_left, lat_top) \
+            * rasterio.transform.Affine.scale(dlon, dlat)
+    return transform
+
+def save_raster(fn, data, crs, transform=None, affine=None):
+    if transform is not None:
+        transform = rasterio.Affine.from_gdal(*transform)
+    elif affine is not None:
+        transform = affine
+
+    kwargs2 = dict(
+        driver="GTiff",
+        height=data.shape[0],
+        width=data.shape[1],
+        count=1,
+        dtype=data.dtype,
+        crs=crs,
+        transform=transform,
+        mode="w",
+    )
+    with rasterio.open(fn, **kwargs2) as dst:
+        r = dst.write(data, 1)
+    return rasterio.open(fn, mode='r')
+
+def get_fn(elev, name=None):
+    """
+    Determines the standard filename for a given GeoTIFF Layer.
+
+    Parameters
+    -----------
+    elev : GdalReader.raster_layer
+        A raster layer from the GdalReader object.
+    name : str (optional)
+        An optional suffix to the filename.
+    Returns
+    -------
+    fn : str
+        The standard <filename>_<name>.tif with suffix (if supplied)
+    """
+    gcs = elev.grid_coordinates
+    coords = [gcs.LLC.lat, gcs.LLC.lon, gcs.URC.lat, gcs.URC.lon]
+    return get_fn_from_coords(coords, name)
+
+
+def get_fn_from_coords(coords, name=None):
+    """ Given a set of coordinates, returns the standard filename.
+
+    Parameters
+    -----------
+    coords : list
+        [LLC.lat, LLC.lon, URC.lat, URC.lon]
+    name : str (optional)
+        An optional suffix to the filename.
+
+    Returns
+    -------
+    fn : str
+        The standard <filename>_<name>.tif with suffix (if supplied)
+    """
+    NS1 = ["S", "N"][coords[0] > 0]
+    EW1 = ["W", "E"][coords[1] > 0]
+    NS2 = ["S", "N"][coords[2] > 0]
+    EW2 = ["W", "E"][coords[3] > 0]
+    new_name = "%s%0.3g%s%0.3g_%s%0.3g%s%0.3g" % \
+        (NS1, coords[0], EW1, coords[1], NS2, coords[2], EW2, coords[3])
+    if name is not None:
+        new_name += '_' + name
+    return new_name.replace('.', 'o') + '.tif'
+
+
+def mk_dx_dy_from_geotif_layer(dataset):
+    """
+    Extracts the change in x and y coordinates from the geotiff file. Presently
+    only supports WGS-84 files.
+    """
+    if dataset.crs.is_projected:
+        dX = np.ones(dataset.shape[0] - 1) * dataset.transform.a
+        dX2 = np.ones(dataset.shape[0]) * dataset.transform.a
+        dY = np.abs(np.ones(dataset.shape[0] - 1) * dataset.transform.e)
+        dY2 = np.abs(np.ones(dataset.shape[0]) * dataset.transform.e)
+        return dX, dY, dX2, dY2
+
+    wkt = dataset.crs.to_wkt()
+    try:
+        ellipsoid = wkt.split('SPHEROID["')[1].split('"')[0].replace(' ', '-')
+    except Exception as e:
+        print(f"No 'SPHEROID' key in wkt: {e}")
+
+    try:
+        ellipsoid = wkt.split('ELLIPSOID["')[1].split('"')[0].replace(' ', '-')
+    except Exception as e:
+        print(f"No 'ELLIPSOID' key in wkt: {e}")
+
+    d = distance(ellipsoid=ellipsoid)
+    dx = dataset.transform.a
+    lon = dataset.transform.d + dx / 2
+    dy = dataset.transform.e
+    lat = dataset.transform.f + dy / 2
+    dX = np.zeros((dataset.shape[0] - 1))
+    for j in range(len(dX)):
+        dX[j] = d.measure((np.clip(lat + dy * (j + 1), -90, 90), lon + dx), (np.clip(lat + dy * (j + 1), -90, 90), lon)) * 1000  # km2m
+    dY = np.zeros((dataset.shape[0] - 1))
+    for i in range(len(dY)):
+        dY[i] = d.measure((np.clip(lat + dy * i, -90, 90), lon), (np.clip(lat + dy * (i + 1), -90, 90), lon)) * 1000  # km2m
+
+    lon = dataset.transform.d + dx
+    lat = dataset.transform.f + dy
+    dX2 = np.zeros((dataset.shape[0]))
+    for j in range(len(dX2)):
+        dX2[j] = d.measure((np.clip(lat + dy * (j + 1), -90, 90), lon + dx), (np.clip(lat + dy * (j + 1), -90, 90), lon)) * 1000  # km2m
+    dY2 = np.zeros((dataset.shape[0]))
+    for i in range(len(dY2)):
+        dY2[i] = d.measure((np.clip(lat + dy * i, -90, 90), lon), (np.clip(lat + dy * (i + 1), -90, 90), lon)) * 1000  # km2m
+
+    return dX, dY, dX2, dY2
+
+
+def mk_geotiff_obj(raster, fn, bands=1, gdal_data_type=np.float32,
+                   lat=[46, 45], lon=[-73, -72]):
+    """
+    Creates a new geotiff file objects using the WGS84 coordinate system, saves
+    it to disk, and returns a handle to the python file object and driver
+
+    Parameters
+    ------------
+    raster : array
+        Numpy array of the raster data to be added to the object
+    fn : str
+        Name of the geotiff file
+    bands : int (optional)
+        See :py:func:`gdal.GetDriverByName('Gtiff').Create
+    gdal_data : gdal.GDT_<type>
+        Gdal data type (see gdal.GDT_...)
+    lat : list
+        northern lat, southern lat
+    lon : list
+        [western lon, eastern lon]
+    """
+    NNi, NNj = raster.shape
+    pixel_height = -np.abs(lat[0] - lat[1]) / (NNi - 1.0)
+    pixel_width = np.abs(lon[0] - lon[1]) / (NNj - 1.0)
+
+    transform = mk_transform(max(lat), min(lon), pixel_height, pixel_width, lat_lon_centered=True)
+    r = save_raster(fn, data=raster, crs="EPSG:4326", affine=transform)
+
+    return r, transform
+
+
+def sortrows(a, i=0, index_out=False, recurse=True):
+    """ Sorts array "a" by columns i
+
+    Parameters
+    ------------
+    a : np.ndarray
+        array to be sorted
+    i : int (optional)
+        column to be sorted by, taken as 0 by default
+    index_out : bool (optional)
+        return the index I such that a(I) = sortrows(a,i). Default = False
+    recurse : bool (optional)
+        recursively sort by each of the columns. i.e.
+        once column i is sort, we sort the smallest column number
+        etc. True by default.
+
+    Returns
+    --------
+    a : np.ndarray
+        The array 'a' sorted in descending order by column i
+    I : np.ndarray (optional)
+        The index such that a[I, :] = sortrows(a, i). Only return if
+        index_out = True
+
+    Examples
+    ---------
+    >>> a = array([[1,2],[3,1],[2,3]])
+    >>> b = sortrows(a,0)
+    >>> b
+    array([[1, 2],
+           [2, 3],
+           [3, 1]])
+    c, I = sortrows(a,1,True)
+
+    >>> c
+    array([[3, 1],
+           [1, 2],
+           [2, 3]])
+    >>> I
+    array([1, 0, 2])
+    >>> a[I,:] - c
+    array([[0, 0],
+           [0, 0],
+           [0, 0]])
+    """
+    I = np.argsort(a[:, i])
+    a = a[I, :]
+    # We recursively call sortrows to make sure it is sorted best by every
+    # column
+    if recurse & (len(a[0]) > i + 1):
+        for b in np.unique(a[:, i]):
+            ids = a[:, i] == b
+            colids = list(range(i)) + list(range(i+1, len(a[0])))
+            a[np.ix_(ids, colids)], I2 = sortrows(a[np.ix_(ids, colids)],
+                                                  0, True, True)
+            I[ids] = I[np.nonzero(ids)[0][I2]]
+
+    if index_out:
+        return a, I
+    else:
+        return a
+
+def get_adjacent_index(I, shape, size):
+    """
+    Find indices 2d-adjacent to those in I. Helper function for get_border*.
+
+    Parameters
+    ----------
+    I : np.ndarray(dtype=int)
+        indices in the flattened region
+    shape : tuple(int, int)
+        region shape
+    size : int
+        region size (technically computable from shape)
+
+    Returns
+    -------
+    J : np.ndarray(dtype=int)
+        indices orthogonally and diagonally adjacent to I
+
+    """
+
+    m, n = shape
+    In = I % n
+    bL = In != 0
+    bR = In != n-1
+
+    J = np.concatenate([
+        # orthonally adjacent
+        I - n,
+        I[bL] - 1,
+        I[bR] + 1,
+        I + n,
+
+        # diagonally adjacent
+        I[bL] - n-1,
+        I[bR] - n+1,
+        I[bL] + n-1,
+        I[bR] + n+1])
+
+    # remove indices outside the array
+    J = J[(J>=0) & (J<size)]
+
+    return J
+
+def get_border_index(I, shape, size):
+    """
+    Get flattened indices for the border of the region I.
+
+    Parameters
+    ----------
+    I : np.ndarray(dtype=int)
+        indices in the flattened region.
+    size : int
+        region size (technically computable from shape argument)
+    shape : tuple(int, int)
+        region shape
+
+    Returns
+    -------
+    J : np.ndarray(dtype=int)
+        indices orthogonally and diagonally bordering I
+    """
+
+    J = get_adjacent_index(I, shape, size)
+
+    # instead of setdiff?
+    # border = np.zeros(size)
+    # border[J] = 1
+    # border[I] = 0
+    # J, = np.where(border)
+
+    return np.setdiff1d(J, I)
+
+def get_border_mask(region):
+    """
+    Get border of the region as a boolean array mask.
+
+    Parameters
+    ----------
+    region : np.ndarray(shape=(m, n), dtype=bool)
+        mask of the region
+
+    Returns
+    -------
+    border : np.ndarray(shape=(m, n), dtype=bool)
+        mask of the region border (not including region)
+    """
+
+    # common special case (for efficiency)
+    internal = region[1:-1, 1:-1]
+    if internal.all() and internal.any():
+        return ~region
+
+    I, = np.where(region.ravel())
+    J = get_adjacent_index(I, region.shape, region.size)
+
+    border = np.zeros(region.size, dtype='bool')
+    border[J] = 1
+    border[I] = 0
+    border = border.reshape(region.shape)
+
+    return border
+
+_ORTH2 = np.array([[0, 1, 0], [1, 1, 1], [0, 1, 0]])
+_SQRT2 = np.sqrt(2.0)
+def get_distance(region, src):
+    """
+    Compute within-region distances from the src pixels.
+
+    Parameters
+    ----------
+    region : np.ndarray(shape=(m, n), dtype=bool)
+        mask of the region
+    src : np.ndarray(shape=(m, n), dtype=bool)
+        mask of the source pixels to compute distances from.
+
+    Returns
+    -------
+    d : np.ndarray(shape=(m, n), dtype=float)
+        approximate within-region distance from the nearest src pixel;
+        (distances outside of the region are arbitrary).
+    """
+
+    dmax = float(region.size)
+    d = np.full(region.shape, dmax)
+    d[src] = 0
+    for n in range(region.size):
+        d_orth = minimum_filter(d, footprint=_ORTH2) + 1
+        d_diag = minimum_filter(d, (3, 3)) + _SQRT2
+        d_adj = np.minimum(d_orth[region], d_diag[region])
+        d[region] = np.minimum(d_adj, d[region])
+        if (d[region] < dmax).all():
+            break
+    return d
+
+def make_slice(a, b):
+    if a < b:
+        return slice(a, b)
+    else:
+        return slice(b, a)
+
+def grow_slice(slc, size):
+    """
+    Grow a slice object by 1 in each direction without overreaching the list.
+
+    Parameters
+    ----------
+    slc: slice
+        slice object to grow
+    size: int
+        list length
+
+    Returns
+    -------
+    slc: slice
+       extended slice
+
+    """
+
+    return slice(max(0, slc.start-1), min(size, slc.stop+1))
+
+def grow_obj(obj, shape):
+    """
+    Grow a 2d object by 1 in all directions without overreaching the array.
+
+    Parameters
+    ----------
+    obj: tuple(slice, slice)
+        Pair of slices (e.g. from scipy.ndimage.measurements.find_objects)
+    shape: tuple(int, int)
+        2d array shape
+
+    Returns
+    -------
+    obj: tuple(slice, slice)
+        extended slice objects
+    """
+
+    return grow_slice(obj[0], shape[0]), grow_slice(obj[1], shape[1])
+
+
+def find_centroid(region):
+    """
+    Finds an approximate centroid for a region that is within the region.
+
+    Parameters
+    ----------
+    region : np.ndarray(shape=(m, n), dtype='bool')
+        mask of the region.
+
+    Returns
+    -------
+    i, j : tuple(int, int)
+        2d index within the region nearest the center of mass.
+    """
+
+    x, y = center_of_mass(region)
+    w = np.argwhere(region)
+    i, j = w[np.argmin(np.linalg.norm(w - (x, y), axis=1))]
+    return i, j
+
+def plot_fill_flat(roi, out, region, source, drain, dL, dH):
+    from matplotlib import pyplot
+
+    plot_detail = roi.size < 500
+    cmap = 'Greens'
+
+    pyplot.figure()
+
+    ax = pyplot.subplot(221)
+    pyplot.axis('off')
+    pyplot.title('unfilled')
+    im = pyplot.imshow(roi, interpolation='none')
+    im.set_cmap(cmap)
+    if plot_detail:
+        y, x = np.where(region); pyplot.plot(x, y, 'k.')
+        y, x = np.where(source); pyplot.plot(x, y, lw=0, color='k', marker='$H$', ms=12)
+        y, x = np.where(drain);   pyplot.plot(x, y, lw=0, color='k', marker='$L$', ms=12)
+
+    pyplot.subplot(222, sharex=ax, sharey=ax)
+    pyplot.axis('off')
+    pyplot.title('filled')
+    im = pyplot.imshow(out, interpolation='none')
+    im.set_cmap(cmap)
+    if plot_detail:
+        for elev in np.unique(out):
+            y, x = np.where(out==elev)
+            pyplot.plot(x, y, lw=0, color='k', marker='$%.3f$' % elev, ms=20)
+
+    if plot_detail:
+        flat = (minimum_filter(out, (3, 3)) >= out) & region
+        y, x = np.where(flat); pyplot.plot(x, y, 'r_', ms=24)
+
+        pyplot.subplot(223, sharex=ax, sharey=ax)
+        pyplot.axis('off')
+        pyplot.title('dL')
+        im = pyplot.imshow(roi, interpolation='none')
+        im.set_cmap(cmap)
+        for d in np.unique(dL):
+            if d == region.size: continue
+            y, x = np.where(dL==d)
+            pyplot.plot(x, y, lw=0, color='k', marker='$%.2f$' % d, ms=24)
+
+        pyplot.subplot(224, sharex=ax, sharey=ax)
+        pyplot.axis('off')
+        pyplot.title('dH')
+        im = pyplot.imshow(roi, interpolation='none')
+        im.set_cmap(cmap)
+        for d in np.unique(dH):
+            if d == region.size: continue
+            y, x = np.where(dH==d)
+            pyplot.plot(x, y, lw=0, color='k', marker='$%.2f$' % d, ms=24)
+
+    pyplot.tight_layout()
+
+def plot_drain_pit(self, pit, drain, prop, s, elev, area):
+    from matplotlib import pyplot
+
+    cmap = 'Greens'
+
+    ipit, jpit = np.unravel_index(pit, elev.shape)
+    Idrain, Jdrain = np.unravel_index(drain, elev.shape)
+    Iarea, Jarea = np.unravel_index(area, elev.shape)
+
+    imin = max(0, min(ipit, Idrain.min(), Iarea.min())-1)
+    imax = min(elev.shape[0], max(ipit, Idrain.max(), Iarea.max()) + 2)
+    jmin = max(0, min(jpit, Jdrain.min(), Jarea.min())-1)
+    jmax = min(elev.shape[1], max(jpit, Jdrain.max(), Jarea.max()) + 2)
+    roi = (slice(imin, imax), slice(jmin, jmax))
+
+    pyplot.figure()
+
+    ax = pyplot.subplot(221);
+    pyplot.axis('off')
+    im = pyplot.imshow(elev[roi], interpolation='none'); im.set_cmap(cmap)
+    pyplot.plot(jpit-jmin, ipit-imin, lw=0, color='k', marker='$P$', ms=10)
+    pyplot.plot(Jarea-jmin, Iarea-imin, 'k.')
+    pyplot.plot(Jdrain-jmin, Idrain-imin, lw=0, color='k', marker='$D$', ms=10)
+
+    pyplot.subplot(223, sharex=ax, sharey=ax); pyplot.axis('off')
+    im = pyplot.imshow(elev[roi], interpolation='none'); im.set_cmap(cmap)
+    for i, j, val in zip(Idrain, Jdrain, prop):
+        pyplot.plot(j-jmin, i-imin, lw=0, color='k', marker='$%.2f$' % val, ms=16)
+
+    pyplot.subplot(224, sharex=ax, sharey=ax); pyplot.axis('off')
+    im = pyplot.imshow(elev[roi], interpolation='none'); im.set_cmap(cmap)
+    for i, j, val in zip(Idrain, Jdrain, s):
+        pyplot.plot(j-jmin, i-imin, lw=0, color='k', marker='$%.2f$' % val, ms=16)
+
+    pyplot.tight_layout()
```

### Comparing `pyDEM-0.2.0/README.md` & `pyDEM-1.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,258 +1,247 @@
-# pyDEM: A python digital elevation model analysis package
------------------------------------------------------------
-
-PyDEM is a package for topographic (terrain) analysis written in Python (with a
-bit of Cython). It takes in digital elevation model (DEM) rasters, and it 
-outputs quantities like slope, aspect, upstream area, and topographic wetness
-index. PyDEM closely follows the approach taken by TauDEM to calculate these
-quantities. It is designed to be fast, easily extensible, and capable of
-handling very large datasets.
-
-PyDEM can be used both from the command-line, or programmatically via its Python
-API. Examples of both usages are given below and in the examples directory. It
-can operate on individual elevation rasters, or on entire directories
-simultaneously. Most processing steps can be performed in parallel with any
-number of independent pyDEM processes. Note that pyDEM depends on TauDEM for
-certain steps (e.g., pitfilling) and it also makes extensive use of the GDAL
-library for working with geospatial rasters.
-
-## 1. Installation
-For installation notes, see [install.md](INSTALL.md)
-
-## 2. Basic Usage
-Examples and tests can be found in the `pydem\examples` directory.
-
-### 2.1 Python Module Usage
-#### 2.1.1. Calculate quantities on a single elevation tile
-Import the `DEMProcessor` class:
-
-    from pydem.dem_processing import DEMProcessor
-
-Set the path to a pit filled elevation file in WGS84 coordinates:
-
-    filename_to_elevation_geotiff = 'test.tiff'
-
-Instantiate an instance of the `DEMProcessor` class:
-
-    dem_proc = DEMProcessor(filename_to_elevation_geotiff)
-
-The following three commands **do** ***not*** **need to be called in order**.
-
-Calculate the aspect and slope magnitude:
-
-    mag, aspect = dem_proc.calc_slopes_directions()
-
-Calculate the upstream contributing area:
-
-    uca = dem_proc.calc_uca()
-
-Calculate the TWI:
-
-    twi = dem_proc.calc_twi()
-
-#### 2.1.2 Calculate TWI on a directory of elevation tiles
-Import the `ProcessManager` class:
-
-    from pydem.processing_manager import ProcessManager
-
-Set the path to the directory of pit-filled WGS84 geotiff elevation files. ***Important***: The files in this directory needs to follow the naming convention used. See `examples.process_manager_directory.py` for an example of using `utils.rename_files` to rename elevation files.
-
-    elevation_source_path = r'C:\test_directory'
-
-Set the target location (where files will be saved):
-
-    # This is the default location if unspecified. 
-    elevation_target_path = r'C:\test_directory\processed_data'
-
-Instantiate an instance of the `ProcessManager` class:
-
-    pm = ProcessManager(elevation_source_path, elevation_target_path)
-
-Process the elevation files in that directory:
-
-    pm.process()
-
-Topographic wetness index calculated for each elevation file in the supplied directory
-will be located in `C:\test_directory\processed_data\twi`. These TWI files will not have
-edge effects on edges interior to the data set. 
-
-#### 2.1.3 DEMProcessor options
-
-The following options are used by the DEMProcess object. They can be modified by setting the value before processing.
-
-    dem_proc = DEMProcessor(filename_to_elevation_geotiff)
-    dem_proc.fill_flats = False
-    
-
-*Slopes & Directions*
-
- * `chunk_size_slp_dir`: Chunk size for slopes_directions calculation. Default `512`.
- * `chunk_overlap_slp_dir`: Overlap to use for resolving slopes and directions at chunk edges. Default `4`.
- * `fill_flats`: Fill/interpolate the elevation for flat regions before calculating slopes and directions. The direction cannot be calculated in regions where the slope is 0 because the nominal elevation is all the same. This can happen in very gradual terrain or in lake and river beds, particularly when the input elevation is composed of integers. When `True`, the elevation is interpolated in those regions so that a reasonable slope and direction can be calculated. Default `True`.
- * `fill_flats_below_sea`: Interpolate the elevation for flat regions that are below sea level. Water will never flow out of these "pits", so in many cases you can ignore these regions and achieve faster processing times. Default `False`.
- * `fill_flats_source_tol`: When filling flats, the algorithm finds adjacent "source" pixels and "drain" pixels for each flat region and interpolates the elevation using these data points. This sets the tolerance for the elevation of source pixels above the flat region (i.e. shallow sources are used as sources but not steep cliffs). Default `1`.
- * `fill_flats_peaks`: Interpolate the elevation for flat regions that are "peaks" (local maxima). These regions have a higher elevation than all adjacent pixels, so there are no "source" pixels to use for interpolation. When `True`, a single pixel is selected approximately in the center of the flat region as the "peak"/"source". Default `True`.
- * `fill_flats_pits`: Interpolate the elevation for flat regions that are "pits" (local minima). These regions have a lower elevation than all adjacent pixels, so there are no "drain" pixels to use for interpolation. When `True`, a single pixel is selected approximately in the center of the flat region as the "pit"/"drain". Default `True`.
- 
- *UCA*
- 
- * `resolve_edges`: Ensure edge UCA is continuous across chunks. Default `True`.
- * `chunk_size_uca`: Chunk size for uca calculation. Default `512`.
- * `chunk_overlap_uca`: Overlap to use for resolving uca at chunk edges. Default `32`.
- * `drain_pits`: Drain from "pits" to nearby but non-adjacent pixels. Pits have no lower adjacent pixels to drain to directly. *Note that with `fill_flats_pits` off, this setting will still drain each pixel in large flat regions, but it may be slower and produces less reasonable results.* Default `True`.
- * `drain_pits_max_iter`: Maximum number of iterations to look for drain pixels for pits. Generally, "nearby drains" for a pit/flat region are found by expanding the region upward/outward iteratively. Default `100`.
- * `drain_pits_max_dist`: Maximum distance in coordnate-space to (non-adjacent) drains for pits. Pits that are too far from another pixel with a lower elevation will not drain. Default `20`.
- * `drain_pits_max_dist_XY`: Maximum distance in real-space to (non-adjacent) drains for pits. Pits that are too far from another pixel with a lower elevation will not drain. This filter is applied after `drain_pits_max_dist`; if the X and Y resolution are similar, this filter is generally unnecessary. Default `None`.
- * `drain_flats`: *[Deprecated, replaced by `drain_pits`]* Drains flat regions and pits by draining all pixels in the region to an arbitrary pixel in the region and then draining that pixel to the border of the flat region. Ignored if `drain_pits` is `True`. Default `False`.
- * `apply_uca_limit_edges`: Mark edges as completed if the maximum UCA is reached when resolving drainage across edges. Default `False`. If True, it may speed up large calculations.
- * `uca_saturaion_limit`: Default `32`.
- 
- *TWI*
-
- * `apply_twi_limits`: When calculating TWI, limit TWI to max value. Default `False`.
- * `apply_twi_limits_on_uca`: When calculating TWI, limit UCA to max value. Default `False`.
-
- *Other*
- 
-  * `save_projection`: Default `EPSG:4326`.
-
-#### 2.1.4 Calculate a custom quantity on a directory of elevation tiles
-Import and Instantiate a `ProcessManager`:
-    from pydem.processing_manager import ProcessManager
-    # Will save results to default path: 'C:\test_directory\processed_data'
-    pm = ProcessManager(r'C:\test_directory')
-    
-Define a custom command. For example, to calculate hill-shading using gdal:
-
-    def command(source_elevation_file, target_file_save_location):
-        cmd = ['gdaldem', 'hillshade', '-s', '111120',
-               '-compute_edges', '-co',  'BIGTIFF=YES', '-of',
-               'GTiff', '-co', 'compress=lzw', '-co', 'TILED=YES',
-               esfile, fn]
-        print '<'*8, ' '.join(cmd), '>'*8
-        status = subprocess.call(cmd)
-        return status
-
-Process directory of files using custom command:
-    pm.process_command(command, save_name='hillshade_files')
-
-The results of this operation will be found in `C:\test_directory\processed_data\hillshade_files`.
-
-### 2.2 Commandline Usage
-When installing pydem using the provided setup.py file, the commandline utilities `TWIDinf`, `AreaDinf`, and `DinfFlowDir` are registered with the operating system. 
-
-#### TWIDinf : 
-
-    usage: TWIDinf-script.py [-h] [--save-all]
-                         Input_Pit_Filled_Elevation [Input_Number_of_Chunks]
-                         [Output_D_Infinity_TWI]
-    
-    Calculates a grid of topographic wetness index which is the log_e(uca / mag),
-    that is, the natural log of the ratio of contributing area per unit contour
-    length and the magnitude of the slope. Note, this function takes the elevation
-    as an input, and it calculates the slope, direction, and contributing area as
-    intermediate steps.
-    
-    positional arguments:
-      Input_Pit_Filled_Elevation
-                        The input pit-filled elevation file in geotiff format.
-      Input_Number_of_Chunks
-                        The approximate number of chunks that the input file
-                        will be divided into for processing (potentially on
-                        multiple processors).
-      Output_D_Infinity_TWI
-                        Output filename for the topographic wetness index.
-                        Default value = twi.tif .
-    
-    optional arguments:
-      -h, --help            show this help message and exit
-      --save-all, --sa      If set, will save all intermediate files as well.
-
-#### AreaDinf : 
-
-    usage: AreaDinf-script.py [-h] [--save-all]
-                          Input_Pit_Filled_Elevation [Input_Number_of_Chunks]
-                          [Output_D_Infinity_Specific_Catchment_Area]
-    
-    Calculates a grid of specific catchment area which is the contributing area
-    per unit contour length using the multiple flow direction D-infinity approach.
-    Note, this is different from the equivalent tauDEM function, in that it takes
-    the elevation (not the flow direction) as an input, and it calculates the
-    slope and direction as intermediate steps.
-
-    positional arguments:
-      Input_Pit_Filled_Elevation
-                        The input pit-filled elevation file in geotiff format.
-      Input_Number_of_Chunks
-                        The approximate number of chunks that the input file
-                        will be divided into for processing (potentially on
-                        multiple processors).
-      Output_D_Infinity_Specific_Catchment_Area
-                        Output filename for the flow direction. Default value = uca.tif .
-    
-    optional arguments:
-      -h, --help            show this help message and exit
-      --save-all, --sa      If set, will save all intermediate files as well.
-
-
-#### DinfFlowDir : 
-
-    usage: DinfFlowDir-script.py [-h]
-                             Input_Pit_Filled_Elevation
-                             [Input_Number_of_Chunks]
-                             [Output_D_Infinity_Flow_Direction]
-                             [Output_D_Infinity_Slope]
-    
-    Assigns a flow direction based on the D-infinity flow method using the
-    steepest slope of a triangular facet (Tarboton, 1997, "A New Method for the
-    Determination of Flow Directions and Contributing Areas in Grid Digital
-    Elevation Models," Water Resources Research, 33(2): 309-319).
-    
-    positional arguments:
-      Input_Pit_Filled_Elevation
-                        The input pit-filled elevation file in geotiff format.
-      Input_Number_of_Chunks
-                        The approximate number of chunks that the input file
-                        will be divided into for processing (potentially on
-                        multiple processors).
-      Output_D_Infinity_Flow_Direction
-                        Output filename for the flow direction. Default value = ang.tif .
-      Output_D_Infinity_Slope
-                        Output filename for the flow direction. Default value = mag.tif .
-    
-    optional arguments:
-      -h, --help            show this help message and exit
-
-## 3. Description of package Contents
-* `commandline_utils.py` : Contains the functions that wrap the python modules into command line utilities.
-* `dem_processing.py`: Contains the main algorithms. 
-  * Re-implements the D-infinity method from Tarboton (1997).  
-  * Implements a new upstream contributing area algorithm. This performs essentially the same task as previous upstream contributing area algorithms, but with some added functionality. This version deals with areas where the elevation is flat or has no data values and can be updated from the edges without re-calculating the upstream contributing area for the entire tile. 
-  * Re-implements the calculation of the [Topographic Wetness Index](http://en.wikipedia.org/wiki/Topographic_Wetness_Index).
-* `processing_manager.py`: Implements a class that manages the calculation of TWI for a directory of files.
-  * Manages the calculation of the upstream contributing area that drains across tile edges.
-  * Stores errors in the processing.
-  * Allows multiple processes to work on the same directory without causing conflicts.
-* `test_pydem.py`: A few helper utilities that create analytic test-cases used to develop/test pyDEM.
-* `utils.py`: A few helper utility functions.
-  * Renames files in a directory.
-  * Parses file names.
-  * Wraps some `gdal` functions for reading and writing geotiff files.
-  * Sorts the rows in an array.
-* `cyfuncs`: Directory containing cythonized versions of python functions in `dem_processing.py`. 
-  * `cyfuncs.cyutils.pyx`: Computationally efficient implementations of algorithms used to calculate upstream contributing area.
-* `examples`: Directory containing a few examples, along with an end-to-end test of the cross-tile calculations.
-  * `examples.compare_tile_to_chunk.py`: Compares the calculation of the upstream contributing area over a full tile compared to multiple chunks in a file. This tests that the upstream contributing area calculation correctly drains across tile edges.
-  * `examples.compare_to_taudem.py`: This compares the calculation of magnitude and aspect to taudem's algorithms. This validates that the algorithms are correctly implemented from Tarboton (1997), and also shows the differences when taking the change in coordinates into account.
-  * `examples.cross-tile_process_manager_test.py`: End-to-end test to make sure that the cross-tile calculations are correctly performed.
-  * `examples.process_manager_directory.py`: This shows how to use the `ProcessingManager` to calculate all of the elevation files within a directory. 
-* `reader`: Directory containing python code used to deal with opening and closing geotiff files. Essentially wraps `gdal` to provide simpler usage.
-  * `reader.gdal_reader.py`: Contains the `GDALReader class used to read and write geotiff files. 
-  * `reader.inpaint.pyx`: Cython function used to fill no-data values in geotiffs.
-  * `reader.my_types.py`: Defines classes used to deal with different grid coordinate systems.
-* `taudem`: Directory containing a copy of taudem for convenience.
-
-## 4. References
-Tarboton, D. G. (1997). A new method for the determination of flow directions and upslope areas in grid digital elevation models. Water resources research, 33(2), 309-319.
-
-Ueckermann, Mattheus P., et al. (2015). "pyDEM: Global Digital Elevation Model Analysis." In K. Huff & J. Bergstra (Eds.), Scipy 2015: 14th Python in Science Conference. Paper presented at Austin, Texas, 6 - 12 July (pp. 117 - 124). [http://conference.scipy.org/proceedings/scipy2015/mattheus_ueckermann.html](http://conference.scipy.org/proceedings/scipy2015/mattheus_ueckermann.html)
+# pyDEM: A python digital elevation model analysis package
+-----------------------------------------------------------
+
+PyDEM is a package for topographic (terrain) analysis written in Python (with a
+bit of Cython). It takes in digital elevation model (DEM) rasters, and it
+outputs quantities like slope, aspect, upstream area, and topographic wetness
+index. PyDEM closely follows the approach taken by TauDEM to calculate these
+quantities. It is designed to be fast, easily extensible, and capable of
+handling very large datasets.
+
+PyDEM can be used both from the command-line, or programmatically via its Python
+API. Examples of both usages are given below and in the examples directory. It
+can operate on individual elevation rasters, or on entire directories
+simultaneously. Most processing steps can be performed in parallel with any
+number of independent pyDEM processes. Note that pyDEM depends on TauDEM for
+certain steps (e.g., pitfilling) and it also makes extensive use of the GDAL
+library for working with geospatial rasters.
+
+## 1. Installation
+For installation notes, see [install.md](INSTALL.md)
+
+## 2. Basic Usage
+Examples and tests can be found in the `pydem\examples` directory.
+
+### 2.1 Python Module Usage
+#### 2.1.1. Calculate quantities on a single elevation tile
+Import the `DEMProcessor` class:
+
+    from pydem.dem_processing import DEMProcessor
+
+Set the path to a pit filled elevation file in WGS84 coordinates:
+
+    filename_to_elevation_geotiff = 'test.tiff'
+
+Instantiate an instance of the `DEMProcessor` class:
+
+    dem_proc = DEMProcessor(filename_to_elevation_geotiff)
+
+The following three commands **do** ***not*** **need to be called in order**.
+
+Calculate the aspect and slope magnitude:
+
+    mag, aspect = dem_proc.calc_slopes_directions()
+
+Calculate the upstream contributing area:
+
+    uca = dem_proc.calc_uca()
+
+Calculate the TWI:
+
+    twi = dem_proc.calc_twi()
+
+#### 2.1.2 Calculate TWI on a directory of elevation tiles
+The `ProcessManager` class orchestrates multiple processes to compute TWI over multiple tiles in parallel on the same machine. Example usage is as follows:
+```python
+  from pydem.processing_manager import ProcessManager
+  elevation_source_path = r'/home/twi-users/elevation'
+  manager = ProcessManager(
+    n_workers=64, # Number of worker processes to use
+    in_path=elevation_source_path,
+    out_path='/home/twi-users/temporary_compute_storage/'  # Where to save intermediate data
+    dem_proc_kwargs={},  # dictionary of values used to initialize DemProcessor
+  )
+  # Start the processing
+  manager.process_twi()  # If this fails (e.g. machine goes down), can restart to pick up where it left off
+```
+
+You can also call individual parts of the processing:
+```python
+manager.compute_grid()  # Figures out how elevation in folder are tiled
+manager.process_elevation()  # Fills flats, handles pits, fixes artifacts in elevation data
+manager.process_aspect_slope()
+manager.process_uca() # Computes upstream contributing area (UCA) for individual tiles (embarassingly parallel)
+manager.process_uca_edges() # Fixes upstream flow contribution accross tile edges -- iteratively
+manager.process_twi()  # Call all the above functions internally, but skips any work already done
+```
+
+Finally, to export results to a single GeoTiff with overviews, use:
+```python
+manager.save_non_overlap_data_geotiff(
+  'float32',  # Numpy recognized filetype
+  new_path=output_path,
+  keys=['elev', 'uca', 'aspect', 'slope', 'twi'], # list can contain a subset of these
+  overview_type='average')
+```
+
+> Note: The name `non_overlap_data` comes from an implementation quirk. The temporary data is saved as
+    a zarr file. This zarr file OVERLAPS data at the edges of tiles to make it easier to compute UCA
+    across edges
+
+
+#### 2.1.3 DEMProcessor options
+
+The following options are used by the DEMProcess object. They can be modified by setting the value before processing.
+
+    dem_proc = DEMProcessor(filename_to_elevation_geotiff)
+    dem_proc.fill_flats = False
+
+
+*Slopes & Directions*
+
+ * `chunk_size_slp_dir`: Chunk size for slopes_directions calculation. Default `512`.
+ * `chunk_overlap_slp_dir`: Overlap to use for resolving slopes and directions at chunk edges. Default `4`.
+ * `fill_flats`: Fill/interpolate the elevation for flat regions before calculating slopes and directions. The direction cannot be calculated in regions where the slope is 0 because the nominal elevation is all the same. This can happen in very gradual terrain or in lake and river beds, particularly when the input elevation is composed of integers. When `True`, the elevation is interpolated in those regions so that a reasonable slope and direction can be calculated. Default `True`.
+ * `fill_flats_below_sea`: Interpolate the elevation for flat regions that are below sea level. Water will never flow out of these "pits", so in many cases you can ignore these regions and achieve faster processing times. Default `False`.
+ * `fill_flats_source_tol`: When filling flats, the algorithm finds adjacent "source" pixels and "drain" pixels for each flat region and interpolates the elevation using these data points. This sets the tolerance for the elevation of source pixels above the flat region (i.e. shallow sources are used as sources but not steep cliffs). Default `1`.
+ * `fill_flats_peaks`: Interpolate the elevation for flat regions that are "peaks" (local maxima). These regions have a higher elevation than all adjacent pixels, so there are no "source" pixels to use for interpolation. When `True`, a single pixel is selected approximately in the center of the flat region as the "peak"/"source". Default `True`.
+ * `fill_flats_pits`: Interpolate the elevation for flat regions that are "pits" (local minima). These regions have a lower elevation than all adjacent pixels, so there are no "drain" pixels to use for interpolation. When `True`, a single pixel is selected approximately in the center of the flat region as the "pit"/"drain". Default `True`.
+
+ *UCA*
+
+ * `resolve_edges`: Ensure edge UCA is continuous across chunks. Default `True`.
+ * `chunk_size_uca`: Chunk size for uca calculation. Default `512`.
+ * `chunk_overlap_uca`: Overlap to use for resolving uca at chunk edges. Default `32`.
+ * `drain_pits`: Drain from "pits" to nearby but non-adjacent pixels. Pits have no lower adjacent pixels to drain to directly. *Note that with `fill_flats_pits` off, this setting will still drain each pixel in large flat regions, but it may be slower and produces less reasonable results.* Default `True`.
+ * `drain_pits_max_iter`: Maximum number of iterations to look for drain pixels for pits. Generally, "nearby drains" for a pit/flat region are found by expanding the region upward/outward iteratively. Default `100`.
+ * `drain_pits_max_dist`: Maximum distance in coordnate-space to (non-adjacent) drains for pits. Pits that are too far from another pixel with a lower elevation will not drain. Default `20`.
+ * `drain_pits_max_dist_XY`: Maximum distance in real-space to (non-adjacent) drains for pits. Pits that are too far from another pixel with a lower elevation will not drain. This filter is applied after `drain_pits_max_dist`; if the X and Y resolution are similar, this filter is generally unnecessary. Default `None`.
+ * `drain_flats`: *[Deprecated, replaced by `drain_pits`]* Drains flat regions and pits by draining all pixels in the region to an arbitrary pixel in the region and then draining that pixel to the border of the flat region. Ignored if `drain_pits` is `True`. Default `False`.
+ * `apply_uca_limit_edges`: Mark edges as completed if the maximum UCA is reached when resolving drainage across edges. Default `False`. If True, it may speed up large calculations.
+ * `uca_saturaion_limit`: Default `32`.
+
+ *TWI*
+
+ * `apply_twi_limits`: When calculating TWI, limit TWI to max value. Default `False`.
+ * `apply_twi_limits_on_uca`: When calculating TWI, limit UCA to max value. Default `False`.
+
+ *Other*
+
+  * `save_projection`: Default `EPSG:4326`.
+
+### 2.2 Commandline Usage
+When installing pydem using the provided setup.py file, the commandline utilities `TWIDinf`, `AreaDinf`, and `DinfFlowDir` are registered with the operating system.
+
+#### TWIDinf :
+
+    usage: TWIDinf-script.py [-h] [--save-all]
+                         Input_Pit_Filled_Elevation [Input_Number_of_Chunks]
+                         [Output_D_Infinity_TWI]
+
+    Calculates a grid of topographic wetness index which is the log_e(uca / mag),
+    that is, the natural log of the ratio of contributing area per unit contour
+    length and the magnitude of the slope. Note, this function takes the elevation
+    as an input, and it calculates the slope, direction, and contributing area as
+    intermediate steps.
+
+    positional arguments:
+      Input_Pit_Filled_Elevation
+                        The input pit-filled elevation file in geotiff format.
+      Input_Number_of_Chunks
+                        The approximate number of chunks that the input file
+                        will be divided into for processing (potentially on
+                        multiple processors).
+      Output_D_Infinity_TWI
+                        Output filename for the topographic wetness index.
+                        Default value = twi.tif .
+
+    optional arguments:
+      -h, --help            show this help message and exit
+      --save-all, --sa      If set, will save all intermediate files as well.
+
+#### AreaDinf :
+
+    usage: AreaDinf-script.py [-h] [--save-all]
+                          Input_Pit_Filled_Elevation [Input_Number_of_Chunks]
+                          [Output_D_Infinity_Specific_Catchment_Area]
+
+    Calculates a grid of specific catchment area which is the contributing area
+    per unit contour length using the multiple flow direction D-infinity approach.
+    Note, this is different from the equivalent tauDEM function, in that it takes
+    the elevation (not the flow direction) as an input, and it calculates the
+    slope and direction as intermediate steps.
+
+    positional arguments:
+      Input_Pit_Filled_Elevation
+                        The input pit-filled elevation file in geotiff format.
+      Input_Number_of_Chunks
+                        The approximate number of chunks that the input file
+                        will be divided into for processing (potentially on
+                        multiple processors).
+      Output_D_Infinity_Specific_Catchment_Area
+                        Output filename for the flow direction. Default value = uca.tif .
+
+    optional arguments:
+      -h, --help            show this help message and exit
+      --save-all, --sa      If set, will save all intermediate files as well.
+
+
+#### DinfFlowDir :
+
+    usage: DinfFlowDir-script.py [-h]
+                             Input_Pit_Filled_Elevation
+                             [Input_Number_of_Chunks]
+                             [Output_D_Infinity_Flow_Direction]
+                             [Output_D_Infinity_Slope]
+
+    Assigns a flow direction based on the D-infinity flow method using the
+    steepest slope of a triangular facet (Tarboton, 1997, "A New Method for the
+    Determination of Flow Directions and Contributing Areas in Grid Digital
+    Elevation Models," Water Resources Research, 33(2): 309-319).
+
+    positional arguments:
+      Input_Pit_Filled_Elevation
+                        The input pit-filled elevation file in geotiff format.
+      Input_Number_of_Chunks
+                        The approximate number of chunks that the input file
+                        will be divided into for processing (potentially on
+                        multiple processors).
+      Output_D_Infinity_Flow_Direction
+                        Output filename for the flow direction. Default value = ang.tif .
+      Output_D_Infinity_Slope
+                        Output filename for the flow direction. Default value = mag.tif .
+
+    optional arguments:
+      -h, --help            show this help message and exit
+
+## 3. Description of package Contents
+* `commandline_utils.py` : Contains the functions that wrap the python modules into command line utilities.
+* `dem_processing.py`: Contains the main algorithms.
+  * Re-implements the D-infinity method from Tarboton (1997).
+  * Implements a new upstream contributing area algorithm. This performs essentially the same task as previous upstream contributing area algorithms, but with some added functionality. This version deals with areas where the elevation is flat or has no data values and can be updated from the edges without re-calculating the upstream contributing area for the entire tile.
+  * Re-implements the calculation of the [Topographic Wetness Index](http://en.wikipedia.org/wiki/Topographic_Wetness_Index).
+* `process_manager.py`: Implements a class that manages the calculation of TWI for a directory of files.
+  * Manages the calculation of the upstream contributing area that drains across tile edges.
+  * Stores errors in the processing.
+  * Allows multiple processes to work on the same directory without causing conflicts.
+* `test_pydem.py`: A few helper utilities that create analytic test-cases used to develop/test pyDEM.
+* `utils.py`: A few helper utility functions.
+  * Renames files in a directory (deprecated, no longer needed).
+  * Parses file names.
+  * Wraps some `gdal` functions for reading and writing geotiff files.
+  * Sorts the rows in an array.
+* `cyfuncs`: Directory containing cythonized versions of python functions in `dem_processing.py`. These should be compiled during installation.
+  * `cyfuncs.cyutils.pyx`: Computationally efficient implementations of algorithms used to calculate upstream contributing area.
+* `examples`: Directory containing a few examples, along with an end-to-end test of the cross-tile calculations.
+  * `examples.compare_tile_to_chunk.py`: Compares the calculation of the upstream contributing area over a full tile compared to multiple chunks in a file. This tests that the upstream contributing area calculation correctly drains across tile edges.
+    * `examples.process_manager_directory.py`: This shows how to use the `ProcessingManager` to calculate all of the elevation files within a directory.
+* `aws`: Directory containing experiment for running PyDEM on Amazon Web Services
+* `pydem.test.test_end_to_end.py`: A few integration tests. Can be run from the commandline using the `pytest` package: `cd pydem; cd test; pytest .`
+
+## 4. References
+Tarboton, D. G. (1997). A new method for the determination of flow directions and upslope areas in grid digital elevation models. Water resources research, 33(2), 309-319.
+
+Ueckermann, Mattheus P., et al. (2015). "pyDEM: Global Digital Elevation Model Analysis." In K. Huff & J. Bergstra (Eds.), Scipy 2015: 14th Python in Science Conference. Paper presented at Austin, Texas, 6 - 12 July (pp. 117 - 124). [http://conference.scipy.org/proceedings/scipy2015/mattheus_ueckermann.html](http://conference.scipy.org/proceedings/scipy2015/mattheus_ueckermann.html)
+
+## 5. Attributions
+pyDEM uses [lib.pyx](https://github.com/alexlib/openpiv-python/blob/cython_safe_installation/openpiv/c_src/lib.pyx) from the [OpenPIV](https://github.com/alexlib/openpiv-python) project for [inpainting](pydem/pydem/reader/inpaint.pyx) missing values in the final outputs.
```

### Comparing `pyDEM-0.2.0/setup.py` & `pyDEM-1.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,109 +1,101 @@
-"""
-   Copyright 2015 Creare
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
-"""
-
-# Always perfer setuptools over distutils
-from setuptools import setup, find_packages, Extension
-from codecs import open  # To use a consistent encoding
-import platform
-
-from os.path import sep
-from os import path
-import os
-import numpy as np
-
-# Check for python 3
-import sys
-if not sys.version_info[0] == 2:
-    sys.exit("Sorry, Python 3 is not supported.")
-
-from Cython.Build import cythonize
-
-here = os.path.join(path.dirname(__file__), 'pydem')
-
-compile_args = []
-compile_args.append("-O3")
-
-if '32' in platform.architecture()[0]:
-    compile_args.append("-march=i386")
-else:
-    compile_args.append("-march=x86-64")
-
-# Pattern functions
-path_cyfuncs = os.path.join(here, 'cyfuncs')
-path_reader = os.path.join(here, 'reader')
-
-extensions = [
-    Extension("pydem.cyfuncs.cyutils",
-              [os.path.join(path_cyfuncs, "cyutils.pyx")],
-              include_dirs=[np.get_include(), path_cyfuncs],
-              library_dirs=[],
-              extra_compile_args=compile_args,
-              language='c++'),
-    Extension("pydem.reader.inpaint",
-              [path_reader + sep + "inpaint.pyx"],
-              include_dirs=[np.get_include()],
-              library_dirs=[],
-              extra_compile_args=compile_args,
-              language='c++'),
-]
-
-setup(
-    ext_modules=cythonize(extensions),
-
-    name='pyDEM',
-
-    version='0.2.0',
-
-    description="Software for calculating Topographic Wetness Index (TWI)",
-    author='MPU, RXC, JXM',
-    url="https://github.com/creare-com/pydem",
-
-    license="APACHE 2.0",
-
-    classifiers=[
-        # How mature is this project? Common values are
-        # 3 - Alpha
-        # 4 - Beta
-        # 5 - Production/Stable
-        'Development Status :: 3 - Alpha',
-        # Indicate who your project is intended for
-        'Intended Audience :: Developers',
-        'Topic :: Scientific/Engineering :: GIS',
-        # Pick your license as you wish (should match "license" above)
-         'License :: OSI Approved :: Apache Software License',
-        # Specify the Python versions you support here. In particular, ensure
-        # that you indicate whether you support Python 2, Python 3 or both.
-        'Programming Language :: Python :: 2.7',
-    ],
-    packages=find_packages(),
-
-    python_requires='<3',
-
-    install_requires=[
-        #'gdal',
-        'numpy',
-        'scipy',
-        'geopy',
-        'traits',
-        ],
-
-    entry_points = {
-        'console_scripts' : ['TWIDinf=pydem.commandline_utils:TWIDinf',
-                             'AreaDinf=pydem.commandline_utils:AreaDinf',
-                             'DinfFlowDir=pydem.commandline_utils:DinfFlowDir']
-    }
-
-)
+"""
+   Copyright 2015-2024 Creare
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
+"""
+
+# Always perfer setuptools over distutils
+from setuptools import setup, find_packages, Extension
+from codecs import open  # To use a consistent encoding
+import platform
+
+from os.path import sep
+from os import path
+import os
+import numpy as np
+
+from Cython.Build import cythonize
+
+here = os.path.join(path.dirname(__file__), 'pydem')
+
+compile_args = []
+compile_args.append("-O3")
+
+if '32' in platform.architecture()[0]:
+    compile_args.append("-march=i386")
+else:
+    compile_args.append("-march=x86-64")
+
+# Pattern functions
+path_cyfuncs = os.path.join(here, 'cyfuncs')
+path_reader = os.path.join(here, 'reader')
+
+extensions = [
+    Extension("pydem.cyfuncs.cyutils",
+              [os.path.join(path_cyfuncs, "cyutils.pyx")],
+              include_dirs=[np.get_include(), path_cyfuncs],
+              library_dirs=[],
+              extra_compile_args=compile_args,
+              language='c++'),
+]
+
+setup(
+    ext_modules=cythonize(extensions),
+
+    name='pyDEM',
+
+    version='1.0.0',
+
+    description="Software for calculating Topographic Wetness Index (TWI)",
+    author='MPU, RXC, JXM',
+    url="https://github.com/creare-com/pydem",
+
+    license="APACHE 2.0",
+
+    classifiers=[
+        # How mature is this project? Common values are
+        # 3 - Alpha
+        # 4 - Beta
+        # 5 - Production/Stable
+        'Development Status :: 4 - Beta',
+        # Indicate who your project is intended for
+        'Intended Audience :: Developers',
+        'Topic :: Scientific/Engineering :: GIS',
+        # Pick your license as you wish (should match "license" above)
+         'License :: OSI Approved :: Apache Software License',
+        # Specify the Python versions you support here. In particular, ensure
+        # that you indicate whether you support Python 2, Python 3 or both.
+        'Programming Language :: Python :: 3',
+    ],
+    packages=find_packages(),
+
+    python_requires='>=3',
+
+    install_requires=[
+        'rasterio',
+        'numpy',
+        'scipy',
+        'geopy',
+        'traitlets',
+        'traittypes',
+        'zarr',
+        'cython'
+        ],
+
+    entry_points = {
+        'console_scripts' : ['TWIDinf=pydem.commandline_utils:TWIDinf',
+                             'AreaDinf=pydem.commandline_utils:AreaDinf',
+                             'DinfFlowDir=pydem.commandline_utils:DinfFlowDir']
+    }
+
+)
```

