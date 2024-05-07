# Comparing `tmp/pymodaq_plugins_bnc-0.0.3.tar.gz` & `tmp/pymodaq_plugins_bnc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugins_bnc-0.0.3.tar", last modified: Thu Feb 29 21:37:53 2024, max compression
+gzip compressed data, was "pymodaq_plugins_bnc-0.0.4.tar", last modified: Tue May  7 07:33:12 2024, max compression
```

## Comparing `pymodaq_plugins_bnc-0.0.3.tar` & `pymodaq_plugins_bnc-0.0.4.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-02-29 21:37:53.670322 pymodaq_plugins_bnc-0.0.3/
--rw-rw-rw-   0        0        0     1128 2024-02-29 09:24:34.000000 pymodaq_plugins_bnc-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       72 2024-02-29 09:24:34.000000 pymodaq_plugins_bnc-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2128 2024-02-29 21:37:53.667888 pymodaq_plugins_bnc-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1176 2024-02-29 21:35:53.000000 pymodaq_plugins_bnc-0.0.3/README.rst
--rw-rw-rw-   0        0        0     1101 2024-02-29 11:07:30.000000 pymodaq_plugins_bnc-0.0.3/plugin_info.toml
--rw-rw-rw-   0        0        0       42 2024-02-29 21:37:53.670322 pymodaq_plugins_bnc-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      106 2024-02-29 09:24:34.000000 pymodaq_plugins_bnc-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-29 21:37:53.591414 pymodaq_plugins_bnc-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-02-29 21:37:53.616187 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/
--rw-rw-rw-   0        0        0      281 2024-02-29 09:24:34.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-29 21:37:53.643535 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/daq_move_plugins/
--rw-rw-rw-   0        0        0      467 2024-02-29 09:24:34.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/daq_move_plugins/__init__.py
--rw-rw-rw-   0        0        0    14069 2024-02-29 21:30:11.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/daq_move_plugins/daq_move_bnc.py
-drwxrwxrwx   0        0        0        0 2024-02-29 21:37:53.645701 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/daq_viewer_plugins/
--rw-rw-rw-   0        0        0        6 2024-02-29 09:24:34.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/daq_viewer_plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-29 21:37:53.647712 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_0D/
--rw-rw-rw-   0        0        0      472 2024-02-29 09:24:34.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_0D/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-29 21:37:53.648709 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_1D/
--rw-rw-rw-   0        0        0      472 2024-02-29 09:24:34.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_1D/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-29 21:37:53.650055 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_2D/
--rw-rw-rw-   0        0        0      474 2024-02-29 09:24:34.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_2D/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-29 21:37:53.650603 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_ND/
--rw-rw-rw-   0        0        0      472 2024-02-29 09:24:34.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_ND/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-29 21:37:53.653634 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/exporters/
--rw-rw-rw-   0        0        0       87 2024-02-29 09:24:34.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/exporters/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-29 21:37:53.655645 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/extensions/
--rw-rw-rw-   0        0        0       87 2024-02-29 09:24:34.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/extensions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-29 21:37:53.659468 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/hardware/
--rw-rw-rw-   0        0        0        0 2024-02-29 09:24:34.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/hardware/__init__.py
--rw-rw-rw-   0        0        0    10671 2024-02-29 21:26:10.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/hardware/bnc_commands.py
--rw-rw-rw-   0        0        0      962 2024-02-29 09:24:34.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/hardware/device.py
-drwxrwxrwx   0        0        0        0 2024-02-29 21:37:53.661759 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/models/
--rw-rw-rw-   0        0        0       87 2024-02-29 09:24:34.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-29 21:37:53.665086 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/resources/
--rw-rw-rw-   0        0        0        5 2024-02-29 21:32:03.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/resources/VERSION
--rw-rw-rw-   0        0        0        0 2024-02-29 09:24:34.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/resources/__init__.py
--rw-rw-rw-   0        0        0       49 2024-02-29 09:24:34.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/resources/config_template.toml
-drwxrwxrwx   0        0        0        0 2024-02-29 21:37:53.665757 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/scanners/
--rw-rw-rw-   0        0        0       87 2024-02-29 09:24:34.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/scanners/__init__.py
--rw-rw-rw-   0        0        0      434 2024-02-29 09:24:34.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-29 21:37:53.667888 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc.egg-info/
--rw-rw-rw-   0        0        0     2128 2024-02-29 21:37:53.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1299 2024-02-29 21:37:53.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-29 21:37:53.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2024-02-29 21:37:53.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2024-02-29 21:37:53.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-02-29 21:37:53.000000 pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/plugin_info.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.578198 pymodaq_plugins_bnc-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.582198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.582198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_move_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_move_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14593 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_move_plugins/daq_move_bnc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.582198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_viewer_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_viewer_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.582198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_0D/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_0D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.582198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_1D/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_1D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_2D/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_2D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_ND/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_ND/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/exporters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10537 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/hardware/bnc_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/hardware/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/resources/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/resources/config_template.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/scanners/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/scanners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-07 07:33:12.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-07 07:33:12.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:33:12.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-07 07:33:12.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 07:33:12.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 07:33:12.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/tests/test_plugin_package_structure.py
```

### Comparing `pymodaq_plugins_bnc-0.0.3/LICENSE` & `pymodaq_plugins_bnc-0.0.4/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) 2021 Sebastien Weber <sebastien.weber@cemes.fr>
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+The MIT License (MIT)
+
+Copyright (c) 2021 Sebastien Weber <sebastien.weber@cemes.fr>
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
```

### Comparing `pymodaq_plugins_bnc-0.0.3/PKG-INFO` & `pymodaq_plugins_bnc-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,62 @@
-Metadata-Version: 2.1
-Name: pymodaq_plugins_bnc
-Version: 0.0.3
-Summary: PyMoDAQ module for communication and readout from BNC575 delay/signal generator
-Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_bnc
-Author: Christian Cabello
-Author-email: christian.cabello@ip-paris.fr
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Other Environment
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: User Interfaces
-License-File: LICENSE
-Requires-Dist: toml
-Requires-Dist: pymodaq>=4.1.0
-
-pymodaq_plugins_bnc
-
-
-.. image:: https://img.shields.io/pypi/v/pymodaq_plugins_template.svg
-   :target: https://pypi.org/project/pymodaq_plugins_template/
-   :alt: Latest Version
-
-.. image:: https://readthedocs.org/projects/pymodaq/badge/?version=latest
-   :target: https://pymodaq.readthedocs.io/en/stable/?badge=latest
-   :alt: Documentation Status
-
-.. image:: https://github.com/PyMoDAQ/pymodaq_plugins_template/workflows/Upload%20Python%20Package/badge.svg
-   :target: https://github.com/PyMoDAQ/pymodaq_plugins_template
-   :alt: Publication Status
-
-.. image:: https://github.com/PyMoDAQ/pymodaq_plugins_template/actions/workflows/Test.yml/badge.svg
-    :target: https://github.com/PyMoDAQ/pymodaq_plugins_template/actions/workflows/Test.yml
-
-
-Authors
-=======
-
-* First Author  (christian.cabello@ip-paris.fr)
-
-
-Instruments
-===========
-
-Below is the list of instruments included in this plugin
-
-Actuator
-++++++++
-
-BNC575 Delay/Pulse Generator Interface with Delay Scan Capability
-
-
-
-Installation instructions
-=========================
-
-* Tested on PyMoDAQ version 4.1.1
-* Tested on Python 3.8.18
-* No additional drivers necessary
+Metadata-Version: 2.1
+Name: pymodaq_plugins_bnc
+Version: 0.0.4
+Summary: PyMoDAQ module for communication and readout from BNC575 delay/signal generator
+Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_bnc
+Author: Christian Cabello
+Author-email: christian.cabello@ip-paris.fr
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Other Environment
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: User Interfaces
+License-File: LICENSE
+Requires-Dist: toml
+Requires-Dist: pymodaq>=4.1.0
+
+pymodaq_plugins_bnc
+
+
+.. image:: https://img.shields.io/pypi/v/pymodaq_plugins_bnc.svg
+   :target: https://pypi.org/project/pymodaq-plugins-bnc
+   :alt: Latest Version
+
+.. image:: https://github.com/ccabello99/pymodaq_plugins_bnc/workflows/Upload%20Python%20Package/badge.svg
+   :target: https://github.com/ccabello99/pymodaq_plugins_bnc
+   :alt: Publication Status
+
+.. image:: https://github.com/ccabello99/pymodaq_plugins_bnc/actions/workflows/Test.yml/badge.svg
+    :target: https://github.com/ccabello99/pymodaq_plugins_bnc/actions/workflows/Test.yml
+
+
+Authors
+=======
+
+* First Author  (christian.cabello@ip-paris.fr)
+
+
+Instruments
+===========
+
+Below is the list of instruments included in this plugin
+
+Actuator
+++++++++
+
+BNC575 Delay/Pulse Generator Interface with Delay Scan Capability
+
+
+
+Installation instructions
+=========================
+
+* Tested on PyMoDAQ version 4.1.1
+* Tested on Python 3.8.18
+* No additional drivers necessary
+* To install plugin, run: pip install pymodaq-plugins-bnc
```

### Comparing `pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/daq_move_plugins/daq_move_bnc.py` & `pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_move_plugins/daq_move_bnc.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,294 +1,312 @@
-from pymodaq.control_modules.move_utility_classes import DAQ_Move_base, comon_parameters_fun, main, DataActuatorType,\
-    DataActuator  # common set of parameters for all actuators
-from pymodaq.utils.daq_utils import ThreadCommand # object used to send info back to the main thread
-from pymodaq.utils.parameter import Parameter
-from pymodaq_plugins_bnc.hardware.bnc_commands import BNC575
-import time
-
-
-class DAQ_Move_bnc(DAQ_Move_base):
-    """ Instrument plugin class for an actuator.
-    
-    This object inherits all functionalities to communicate with PyMoDAQ’s DAQ_Move module through inheritance via
-    DAQ_Move_base. It makes a bridge between the DAQ_Move module and the Python wrapper of a particular instrument.
-
-        * This is compatible with the BNC 575 Delay/Pulse Generator
-        * Tested on PyMoDAQ 4.1.1
-        * Tested on Python 3.8.18
-        * No additional drivers necessary
-
-    Attributes:
-    -----------
-    controller: object
-        The particular object that allow the communication with the hardware, in general a python wrapper around the
-         hardware library.
-
-    """
-    _controller_units = 'ns'
-    is_multiaxes = False
-    _axis_names = ['Delay']
-    _epsilon = 0.25
-    #data_actuator_type = DataActuatorType['DataActuator']  # wether you use the new data style for actuator otherwise set this
-    # as  DataActuatorType['float']  (or entirely remove the line)
-
-    params = [
-    {'title': 'Connection', 'name': 'connection', 'type': 'group', 'children': [
-        {'title': 'Controller', 'name': 'id', 'type': 'str', 'value': 'BNC,575-4,31309,2.4.1-1.2.2', 'readonly': True},
-        {'title': 'IP', 'name': 'ip', 'type': 'str', 'value': '', 'readonly': True},
-        {'title': 'Port', 'name': 'port', 'type': 'str', 'value': '', 'readonly': True}
-    ]},
-
-    {'title': 'Device Configuration State', 'name': 'config', 'type': 'group', 'children': [
-        {'title': 'Configuration Label', 'name': 'label', 'type': 'str', 'value': ""},
-        {'title': 'Local Memory Slot', 'name': 'slot', 'type': 'list', 'value': 1, 'limits': [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]},
-        {'title': 'Save Current Configuration?', 'name': 'save', 'type': 'bool_push', 'label': 'Save', 'value': False},
-        {'title': 'Restore Previous Configuration?', 'name': 'restore', 'type': 'bool_push', 'label': 'Restore', 'value': False},
-        {'title': 'Reset Device?', 'name': 'reset', 'type': 'bool_push', 'label': 'Reset', 'value': False}
-    ]},
-
-    {'title': 'Global State', 'name': 'global_state', 'type': 'list', 'value': "OFF", 'limits': ['ON', 'OFF']},
-    
-    {'title': 'Global Mode', 'name': 'global_mode', 'type': 'list', 'value': 'NORM', 'limits': ['NORM', 'SING', 'BURS', 'DCYC']},
-
-    {'title': 'Channel', 'name': 'channel_label', 'type': 'list', 'value': "A", 'limits': ['A', 'B', 'C', 'D']},
-
-    {'title': 'Channel Mode', 'name': 'channel_mode', 'type': 'list', 'value': 'NORM', 'limits': ['NORM', 'SING', 'BURS', 'DCYC']},
-
-    {'title': 'Channel State', 'name': 'channel_state', 'type': 'list', 'value': "OFF", 'limits': ['ON', 'OFF']},
-
-    {'title': 'Width (s)', 'name': 'width', 'type': 'float', 'value': 10e-9, 'default': 10e-9, 'min': 10e-9, 'max': 999.0},
-
-    {'title': 'Amplitude Mode', 'name': 'amplitude_mode', 'type': 'list', 'value': "ADJ", 'limits': ['ADJ', 'TTL']},
-        
-    {'title': 'Amplitude (V)', 'name': 'amplitude', 'type': 'float', 'value': 2.0, 'default': 2.0, 'min': 2.0, 'max': 20.0},
-
-    {'title': 'Polarity', 'name': 'polarity', 'type': 'list', 'value': "NORM", 'limits': ['NORM', 'COMP', 'INV']},
-
-    {'title': 'Delay (s)', 'name': 'delay', 'type': 'float', 'value': 0, 'default': 0, 'min': 0, 'max': 999.0},
-
-    {'title': 'Continuous Mode', 'name': 'continuous_mode', 'type': 'group', 'children': [
-        {'title': 'Period (s)', 'name': 'period', 'type': 'float', 'value': 1e-3, 'default': 1e-3, 'min': 100e-9, 'max': 5000.0},
-        {'title': 'Repetition Rate (Hz)', 'name': 'rep_rate', 'type': 'float', 'value': 1e3, 'default': 1e3, 'min': 2e-4, 'max': 10e6}
-    ]},
-
-    {'title': 'Trigger Mode', 'name': 'trigger_mode', 'type': 'group', 'children': [
-        {'title': 'Trigger Mode', 'name': 'trig_mode', 'type': 'list', 'value': 'DIS', 'limits': ['DIS', 'TRIG']},
-        {'title': 'Trigger Threshold (V)', 'name': 'trig_thresh', 'type': 'float', 'value': 2.5, 'default': 2.5, 'min': 0.2, 'max': 15.0},
-        {'title': 'Trigger Edge', 'name': 'trig_edge', 'type': 'list', 'value': 'HIGH', 'limits': ['HIGH', 'LOW']}
-    ]},
-
-    {'title': 'Gating', 'name': 'gating', 'type': 'group', 'children': [
-        {'title': 'Global Gate Mode', 'name': 'gate_mode', 'type': 'list', 'value': "DIS", 'limits': ['DIS', 'PULS', 'OUTP', 'CHAN']},
-        {'title': 'Channel Gate Mode', 'name': 'channel_gate_mode', 'type': 'list', 'value': "DIS", 'limits': ['DIS', 'PULS', 'OUTP']},
-        {'title': 'Gate Threshold (V)', 'name': 'gate_thresh', 'type': 'float', 'value': 2.5, 'default': 2.5, 'min': 0.2, 'max': 15.0},
-        {'title': 'Gate Logic', 'name': 'gate_logic', 'type': 'list', 'value': 'HIGH', 'limits': ['HIGH', 'LOW']}
-
-    ]}] + comon_parameters_fun(is_multiaxes, axis_names=_axis_names, epsilon=_epsilon)
-    # _epsilon is the initial default value for the epsilon parameter allowing pymodaq to know if the controller reached
-    # the target value. It is the developer responsibility to put here a meaningful value
-
-    def ini_attributes(self):
-        self.controller: BNC575 = None
-
-    def get_actuator_value(self):
-        """Get the current value from the hardware with scaling conversion.
-
-        Returns
-        -------
-        float: The delay obtained after scaling conversion.
-        """
-        delay = DataActuator(data=self.controller.delay*1e9)
-        self.current_value = delay
-        return delay
-
-    def close(self):
-        """Terminate the communication protocol"""
-        self.controller.close()
-
-    def grab_data(self):
-        """Start a grab from the detector"""
-        
-        data_dict = self.controller.output()
-
-        self.settings.child('config',  'label').setValue(data_dict['Configuration Label'])
-        time.sleep(0.075)
-        self.settings.param('global_state').setValue(data_dict['Global State'])
-        time.sleep(0.075)
-        self.settings.param('global_mode').setValue(data_dict['Global Mode'])
-        time.sleep(0.075)
-        self.settings.param('channel_label').setValue(data_dict['Channel'])
-        time.sleep(0.075)
-        self.settings.param('channel_mode').setValue(data_dict['Channel Mode'])
-        time.sleep(0.075)
-        self.settings.param('channel_state').setValue(data_dict['Channel State'])
-        time.sleep(0.075)
-        self.settings.param('width').setValue(data_dict['Width (s)'])
-        time.sleep(0.075)
-        self.settings.param('amplitude_mode').setValue(data_dict['Amplitude Mode'])
-        time.sleep(0.075)
-        self.settings.param('amplitude').setValue(data_dict['Amplitude (V)'])
-        time.sleep(0.075)
-        self.settings.param('polarity').setValue(data_dict['Polarity'])
-        time.sleep(0.075)
-        self.settings.param('delay').setValue(data_dict['Delay (s)'])
-        time.sleep(0.075)
-        self.get_actuator_value()
-        self.settings.child('continuous_mode',  'period').setValue(data_dict['Period (s)'])
-        time.sleep(0.075)
-        self.settings.child('continuous_mode',  'rep_rate').setValue(1 / data_dict['Period (s)'])
-        time.sleep(0.075)
-        self.settings.child('trigger_mode',  'trig_mode').setValue(data_dict['Trigger Mode'])
-        time.sleep(0.075)
-        self.settings.child('trigger_mode',  'trig_thresh').setValue(data_dict['Trigger Threshold (V)'])
-        time.sleep(0.075)
-        self.settings.child('trigger_mode',  'trig_edge').setValue(data_dict['Trigger Edge'])
-        time.sleep(0.075)
-        self.settings.child('gating',  'gate_mode').setValue(data_dict['Global Gate Mode'])
-        time.sleep(0.075)
-        self.settings.child('gating',  'channel_gate_mode').setValue(data_dict['Channel Gate Mode'])
-        time.sleep(0.075)
-        self.settings.child('gating',  'gate_thresh').setValue(data_dict['Gate Threshold (V)'])
-        time.sleep(0.075)
-        self.settings.child('gating',  'gate_logic').setValue(data_dict['Gate Logic'])
-        time.sleep(0.075)
-
-
-    def commit_settings(self, param: Parameter):
-        """Apply the consequences of a change of value in the detector settings
-
-        Parameters
-        ----------
-        param: Parameter
-            A given parameter (within detector_settings) whose value has been changed by the user
-        """
-        if param.name() == "label":
-            self.controller.label = param.value()
-        elif param.name() == "slot":
-           self.controller.slot = param.value()
-        elif param.name() == "save":
-            if param.value:
-                self.controller.save_state()
-                time.sleep(0.05)
-        elif param.name() == "restore":
-            if param.value:
-                self.controller.restore_state()
-                time.sleep(0.05)
-                self.grab_data()
-        elif param.name() == "reset":
-            if param.value:
-                self.controller.reset()
-                time.sleep(0.05)
-                self.grab_data()
-        elif param.name() == "global_state":
-            self.controller.global_state = param.value()
-        elif param.name() == "global_mode":
-            self.controller.global_mode = param.value()
-        elif param.name() == "channel_label":
-           self.controller.channel_label = param.value()
-           self.grab_data()
-        elif param.name() == "channel_state":
-            self.controller.channel_state = param.value()
-        elif param.name() == "channel_mode":
-            self.controller.channel_mode = param.value()
-        elif param.name() == "delay":
-            self.controller.delay = param.value()
-            self.get_actuator_value()
-        elif param.name() == "width":
-            self.controller.width = param.value()
-        elif param.name() == "amplitude_mode":
-            self.controller.amplitude_mode = param.value()
-        elif param.name() == "amplitude":
-            self.controller.amplitude = param.value()
-        elif param.name() == "polarity":
-            self.controller.polarity = param.value()            
-        elif param.name() == "period":
-            self.controller.period = param.value()
-            self.settings.child('continuous_mode',  'rep_rate').setValue(1 / self.controller.period)
-            time.sleep(0.075)
-        elif param.name() == "rep_rate":
-            self.controller.period = 1 / param.value()
-            self.settings.child('continuous_mode',  'period').setValue(self.controller.period)
-            time.sleep(0.075)
-        elif param.name() == "trig_mode":
-            self.controller.trig_mode = param.value()
-        elif param.name() == "trig_thresh":
-            self.controller.trig_thresh = param.value()
-        elif param.name() == "trig_edge":
-            self.controller.trig_edge = param.value()
-        elif param.name() == "gate_mode":
-            self.controller.gate_mode = param.value()
-        elif param.name() == "channel_gate_mode":
-            self.controller.channel_gate_mode = param.value()
-            self.settings.child('gating',  'gate_mode').setValue(self.controller.gate_mode)
-            time.sleep(0.075)
-        elif param.name() == "gate_thresh":
-            self.controller.gate_thresh = param.value()
-        elif param.name() == "gate_logic":            
-            self.controller.gate_logic = param.value()
-
-    def ini_stage(self, controller=None):
-        """Actuator communication initialization
-
-        Parameters
-        ----------
-        controller: (object)
-            custom object of a PyMoDAQ plugin (Slave case). None if only one actuator by controller (Master case)
-
-        Returns
-        -------
-        info: str
-        initialized: bool
-            False if initialization failed otherwise True
-        """
-
-        self.controller = self.ini_stage_init(old_controller=controller,
-                                              new_controller=BNC575("192.168.178.146", 2001))
-        
-        self.settings.child('connection',  'ip').setValue(self.controller.ip)
-        time.sleep(0.05)
-        self.settings.child('connection',  'port').setValue(self.controller.port)
-        time.sleep(0.05)
-        self.controller.restore_state()
-        time.sleep(0.05)
-        self.grab_data()
-        
-
-        info = "Whatever info you want to log"
-        initialized = True
-        return info, initialized
-
-
-    def move_abs(self, value: DataActuator):
-        """ Move the actuator to the absolute target defined by value
-        Parameters
-        ----------
-        value: (float) value of the absolute target positioning
-        """
-        self.target_value = value
-        self.controller.delay = self.target_value * 1e-9
-        self.get_actuator_value()
-
-    def move_rel(self, value: DataActuator):
-        """ Move the actuator to the relative target actuator value defined by value
-        Parameters
-        ----------
-        value: (float) value of the relative target positioning
-        """
-        self.target_value = self.current_value + value
-        self.controller.delay = self.target_value * 1e-9
-        self.get_actuator_value()
-
-    def move_home(self):
-        """Call the reference method of the controller"""
-        self.controller.delay = 0
-        self.get_actuator_value()
-
-    def stop_motion(self):
-      """Stop the actuator and emits move_done signal"""
-      self.controller.stop()
-      self.move_done()
-      self.get_actuator_value()
-
-
-if __name__ == '__main__':
-    main(__file__)
+from pymodaq.control_modules.move_utility_classes import DAQ_Move_base, comon_parameters_fun, main, DataActuatorType,\
+    DataActuator  # common set of parameters for all actuators
+from pymodaq.utils.daq_utils import ThreadCommand # object used to send info back to the main thread
+from pymodaq.utils.parameter import Parameter
+from pymodaq_plugins_bnc.hardware.bnc_commands import BNC575
+import time
+
+
+class DAQ_Move_bnc(DAQ_Move_base):
+    """ Instrument plugin class for an actuator.
+    
+    This object inherits all functionalities to communicate with PyMoDAQ’s DAQ_Move module through inheritance via
+    DAQ_Move_base. It makes a bridge between the DAQ_Move module and the Python wrapper of a particular instrument.
+
+        * This is compatible with the BNC 575 Delay/Pulse Generator
+        * Tested on PyMoDAQ 4.1.1
+        * Tested on Python 3.8.18
+        * No additional drivers necessary
+
+    Attributes:
+    -----------
+    controller: object
+        The particular object that allow the communication with the hardware, in general a python wrapper around the
+         hardware library.
+
+    """
+    _controller_units = 'ns'
+    is_multiaxes = False
+    _axis_names = ['Delay']
+    _epsilon = 0.25
+    #data_actuator_type = DataActuatorType['DataActuator']  # wether you use the new data style for actuator otherwise set this
+    # as  DataActuatorType['float']  (or entirely remove the line)
+
+    params = [
+    {'title': 'Connection', 'name': 'connection', 'type': 'group', 'children': [
+        {'title': 'Controller', 'name': 'id', 'type': 'str', 'value': 'BNC,575-4,31309,2.4.1-1.2.2', 'readonly': True},
+        {'title': 'IP', 'name': 'ip', 'type': 'str', 'value': ''},
+        {'title': 'Port', 'name': 'port', 'type': 'str', 'value': ''}
+    ]},
+
+    {'title': 'Device Configuration State', 'name': 'config', 'type': 'group', 'children': [
+        {'title': 'Configuration Label', 'name': 'label', 'type': 'str', 'value': ""},
+        {'title': 'Local Memory Slot', 'name': 'slot', 'type': 'list', 'value': 1, 'limits': [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]},
+        {'title': 'Save Current Configuration?', 'name': 'save', 'type': 'bool_push', 'label': 'Save', 'value': False},
+        {'title': 'Restore Previous Configuration?', 'name': 'restore', 'type': 'bool_push', 'label': 'Restore', 'value': False},
+        {'title': 'Reset Device?', 'name': 'reset', 'type': 'bool_push', 'label': 'Reset', 'value': False}
+    ]},
+
+    {'title': 'Global State', 'name': 'global_state', 'type': 'list', 'value': "OFF", 'limits': ['ON', 'OFF']},
+    
+    {'title': 'Global Mode', 'name': 'global_mode', 'type': 'list', 'value': 'NORM', 'limits': ['NORM', 'SING', 'BURS', 'DCYC']},
+
+    {'title': 'Channel', 'name': 'channel_label', 'type': 'list', 'value': "A", 'limits': ['A', 'B', 'C', 'D']},
+
+    {'title': 'Channel Mode', 'name': 'channel_mode', 'type': 'list', 'value': 'NORM', 'limits': ['NORM', 'SING', 'BURS', 'DCYC']},
+
+    {'title': 'Channel State', 'name': 'channel_state', 'type': 'list', 'value': "OFF", 'limits': ['ON', 'OFF']},
+
+    {'title': 'Width (s)', 'name': 'width', 'type': 'float', 'value': 10e-9, 'default': 10e-9, 'min': 10e-9, 'max': 999.0},
+
+    {'title': 'Amplitude Mode', 'name': 'amplitude_mode', 'type': 'list', 'value': "ADJ", 'limits': ['ADJ', 'TTL']},
+        
+    {'title': 'Amplitude (V)', 'name': 'amplitude', 'type': 'float', 'value': 2.0, 'default': 2.0, 'min': 2.0, 'max': 20.0},
+
+    {'title': 'Polarity', 'name': 'polarity', 'type': 'list', 'value': "NORM", 'limits': ['NORM', 'COMP', 'INV']},
+
+    {'title': 'Delay (s)', 'name': 'delay', 'type': 'float', 'value': 0, 'default': 0, 'min': 0, 'max': 999.0},
+
+    {'title': 'Continuous Mode', 'name': 'continuous_mode', 'type': 'group', 'children': [
+        {'title': 'Period (s)', 'name': 'period', 'type': 'float', 'value': 1e-3, 'default': 1e-3, 'min': 100e-9, 'max': 5000.0},
+        {'title': 'Repetition Rate (Hz)', 'name': 'rep_rate', 'type': 'float', 'value': 1e3, 'default': 1e3, 'min': 2e-4, 'max': 10e6}
+    ]},
+
+    {'title': 'Trigger Mode', 'name': 'trigger_mode', 'type': 'group', 'children': [
+        {'title': 'Trigger Mode', 'name': 'trig_mode', 'type': 'list', 'value': 'DIS', 'limits': ['DIS', 'TRIG']},
+        {'title': 'Trigger Threshold (V)', 'name': 'trig_thresh', 'type': 'float', 'value': 2.5, 'default': 2.5, 'min': 0.2, 'max': 15.0},
+        {'title': 'Trigger Edge', 'name': 'trig_edge', 'type': 'list', 'value': 'HIGH', 'limits': ['HIGH', 'LOW']}
+    ]},
+
+    {'title': 'Gating', 'name': 'gating', 'type': 'group', 'children': [
+        {'title': 'Global Gate Mode', 'name': 'gate_mode', 'type': 'list', 'value': "DIS", 'limits': ['DIS', 'PULS', 'OUTP', 'CHAN']},
+        {'title': 'Channel Gate Mode', 'name': 'channel_gate_mode', 'type': 'list', 'value': "DIS", 'limits': ['DIS', 'PULS', 'OUTP']},
+        {'title': 'Gate Threshold (V)', 'name': 'gate_thresh', 'type': 'float', 'value': 2.5, 'default': 2.5, 'min': 0.2, 'max': 15.0},
+        {'title': 'Gate Logic', 'name': 'gate_logic', 'type': 'list', 'value': 'HIGH', 'limits': ['HIGH', 'LOW']}
+
+    ]}] + comon_parameters_fun(is_multiaxes, axis_names=_axis_names, epsilon=_epsilon)
+    # _epsilon is the initial default value for the epsilon parameter allowing pymodaq to know if the controller reached
+    # the target value. It is the developer responsibility to put here a meaningful value
+
+    def ini_attributes(self):
+        self.controller: BNC575 = None
+
+    def get_actuator_value(self):
+        """Get the current value from the hardware with scaling conversion.
+
+        Returns
+        -------
+        float: The delay obtained after scaling conversion.
+        """
+        delay = DataActuator(data=self.controller.delay*1e9)
+        self.current_value = delay
+        return delay
+
+    def close(self):
+        """Terminate the communication protocol"""
+        self.controller.close()
+
+    def grab_data(self):
+        """Start a grab from the detector"""
+        
+        data_dict = self.controller.output()
+        
+        self.settings.child('connection',  'ip').setValue(data_dict['IP Address'])
+        time.sleep(0.075)
+        self.settings.child('connection',  'port').setValue(data_dict['Port'])
+        time.sleep(0.075)
+        self.settings.child('config',  'label').setValue(data_dict['Configuration Label'])
+        time.sleep(0.075)
+        self.settings.param('global_state').setValue(data_dict['Global State'])
+        time.sleep(0.075)
+        self.settings.param('global_mode').setValue(data_dict['Global Mode'])
+        time.sleep(0.075)
+        self.settings.param('channel_label').setValue(data_dict['Channel'])
+        time.sleep(0.075)
+        self.settings.param('channel_mode').setValue(data_dict['Channel Mode'])
+        time.sleep(0.075)
+        self.settings.param('channel_state').setValue(data_dict['Channel State'])
+        time.sleep(0.075)
+        self.settings.param('width').setValue(data_dict['Width (s)'])
+        time.sleep(0.075)
+        self.settings.param('amplitude_mode').setValue(data_dict['Amplitude Mode'])
+        time.sleep(0.075)
+        self.settings.param('amplitude').setValue(data_dict['Amplitude (V)'])
+        time.sleep(0.075)
+        self.settings.param('polarity').setValue(data_dict['Polarity'])
+        time.sleep(0.075)
+        self.settings.param('delay').setValue(data_dict['Delay (s)'])
+        time.sleep(0.075)
+        self.get_actuator_value()
+        self.settings.child('continuous_mode',  'period').setValue(data_dict['Period (s)'])
+        time.sleep(0.075)
+        self.settings.child('continuous_mode',  'rep_rate').setValue(1 / data_dict['Period (s)'])
+        time.sleep(0.075)
+        self.settings.child('trigger_mode',  'trig_mode').setValue(data_dict['Trigger Mode'])
+        time.sleep(0.075)
+        self.settings.child('trigger_mode',  'trig_thresh').setValue(data_dict['Trigger Threshold (V)'])
+        time.sleep(0.075)
+        self.settings.child('trigger_mode',  'trig_edge').setValue(data_dict['Trigger Edge'])
+        time.sleep(0.075)
+        self.settings.child('gating',  'gate_mode').setValue(data_dict['Global Gate Mode'])
+        time.sleep(0.075)
+        self.settings.child('gating',  'channel_gate_mode').setValue(data_dict['Channel Gate Mode'])
+        time.sleep(0.075)
+        self.settings.child('gating',  'gate_thresh').setValue(data_dict['Gate Threshold (V)'])
+        time.sleep(0.075)
+        self.settings.child('gating',  'gate_logic').setValue(data_dict['Gate Logic'])
+        time.sleep(0.075)
+
+
+    def commit_settings(self, param: Parameter):
+        """Apply the consequences of a change of value in the detector settings
+
+        Parameters
+        ----------
+        param: Parameter
+            A given parameter (within detector_settings) whose value has been changed by the user
+        """
+        if param.name() == "ip":
+            port = self.controller.port
+            self.close()
+            time.sleep(0.05)
+            self.controller = self.ini_stage_init(old_controller=None,
+                                              new_controller=BNC575(param.value(), port))
+            time.sleep(0.05)
+        if param.name() == "port":
+            ip = self.controller.ip
+            self.close()
+            time.sleep(0.05)
+            self.controller = self.ini_stage_init(old_controller=None,
+                                              new_controller=BNC575(ip, param.value()))
+            time.sleep(0.05)
+        elif param.name() == "label":
+            self.controller.label = param.value()
+        elif param.name() == "slot":
+           self.controller.slot = param.value()
+        elif param.name() == "save":
+            if param.value:
+                self.controller.save_state()
+                time.sleep(0.05)
+        elif param.name() == "restore":
+            if param.value:
+                self.controller.restore_state()
+                time.sleep(0.05)
+                self.grab_data()
+        elif param.name() == "reset":
+            if param.value:
+                self.controller.reset()
+                time.sleep(0.05)
+                self.grab_data()
+        elif param.name() == "global_state":
+            self.controller.global_state = param.value()
+        elif param.name() == "global_mode":
+            self.controller.global_mode = param.value()
+        elif param.name() == "channel_label":
+           self.controller.channel_label = param.value()
+           self.grab_data()
+        elif param.name() == "channel_state":
+            self.controller.channel_state = param.value()
+        elif param.name() == "channel_mode":
+            self.controller.channel_mode = param.value()
+        elif param.name() == "delay":
+            self.controller.delay = param.value()
+            self.get_actuator_value()
+        elif param.name() == "width":
+            self.controller.width = param.value()
+        elif param.name() == "amplitude_mode":
+            self.controller.amplitude_mode = param.value()
+        elif param.name() == "amplitude":
+            self.controller.amplitude = param.value()
+        elif param.name() == "polarity":
+            self.controller.polarity = param.value()            
+        elif param.name() == "period":
+            self.controller.period = param.value()
+            self.settings.child('continuous_mode',  'rep_rate').setValue(1 / self.controller.period)
+            time.sleep(0.075)
+        elif param.name() == "rep_rate":
+            self.controller.period = 1 / param.value()
+            self.settings.child('continuous_mode',  'period').setValue(self.controller.period)
+            time.sleep(0.075)
+        elif param.name() == "trig_mode":
+            self.controller.trig_mode = param.value()
+        elif param.name() == "trig_thresh":
+            self.controller.trig_thresh = param.value()
+        elif param.name() == "trig_edge":
+            self.controller.trig_edge = param.value()
+        elif param.name() == "gate_mode":
+            self.controller.gate_mode = param.value()
+        elif param.name() == "channel_gate_mode":
+            self.controller.channel_gate_mode = param.value()
+            self.settings.child('gating',  'gate_mode').setValue(self.controller.gate_mode)
+            time.sleep(0.075)
+        elif param.name() == "gate_thresh":
+            self.controller.gate_thresh = param.value()
+        elif param.name() == "gate_logic":            
+            self.controller.gate_logic = param.value()
+
+    def ini_stage(self, controller=None):
+        """Actuator communication initialization
+
+        Parameters
+        ----------
+        controller: (object)
+            custom object of a PyMoDAQ plugin (Slave case). None if only one actuator by controller (Master case)
+
+        Returns
+        -------
+        info: str
+        initialized: bool
+            False if initialization failed otherwise True
+        """
+
+        self.controller = self.ini_stage_init(old_controller=controller,
+                                              new_controller=BNC575("192.168.178.146", 2001))
+        
+        self.settings.child('connection',  'ip').setValue(self.controller.ip)
+        time.sleep(0.05)
+        self.settings.child('connection',  'port').setValue(self.controller.port)
+        time.sleep(0.05)
+        self.controller.restore_state()
+        time.sleep(0.05)
+        self.grab_data()
+        
+
+        info = "Whatever info you want to log"
+        initialized = True
+        return info, initialized
+
+
+    def move_abs(self, value: DataActuator):
+        """ Move the actuator to the absolute target defined by value
+        Parameters
+        ----------
+        value: (float) value of the absolute target positioning
+        """
+        self.target_value = value
+        self.controller.delay = self.target_value * 1e-9
+        self.get_actuator_value()
+
+    def move_rel(self, value: DataActuator):
+        """ Move the actuator to the relative target actuator value defined by value
+        Parameters
+        ----------
+        value: (float) value of the relative target positioning
+        """
+        self.target_value = self.current_value + value
+        self.controller.delay = self.target_value * 1e-9
+        self.get_actuator_value()
+
+    def move_home(self):
+        """Call the reference method of the controller"""
+        self.controller.delay = 0
+        self.get_actuator_value()
+
+    def stop_motion(self):
+      """Stop the actuator and emits move_done signal"""
+      self.controller.stop()
+      self.move_done()
+      self.get_actuator_value()
+
+
+if __name__ == '__main__':
+    main(__file__)
```

### Comparing `pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc/hardware/bnc_commands.py` & `pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/hardware/bnc_commands.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,370 +1,382 @@
-import time
-from pymodaq_plugins_bnc.hardware.device import Device
-
-class BNC575(Device):
-
-    def __init__(self, ip, port):
-        super().__init__(ip, port)
-        self.channel_label = "A"
-        self.slot = 1
-
-    def idn(self):
-        idn = self.query("*IDN").strip()
-        time.sleep(0.25)
-        return idn
-
-    def reset(self):
-        self.send("*RST")
-        time.sleep(0.05)
-
-    def stop(self):
-        pass
-    
-    @property
-    def slot(self):
-        return self._slot
-    
-    @slot.setter
-    def slot(self, slot):
-        self._slot = slot
-    
-    def save_state(self):
-        self.set("*SAV", str(self.slot))
-        time.sleep(0.05)
-    
-    def restore_state(self):
-        self.set("*RCL", str(self.slot))
-        time.sleep(0.05)
-    
-    def trig(self):
-        self.send("*TRG")
-        time.sleep(0.05)
-    
-    @property
-    def label(self):
-        lbl = self.query("*LBL").strip()
-        time.sleep(0.05)
-        return lbl
-    
-    @label.setter
-    def label(self, label):
-        self.set("*LBL", "\"" + label + "\"")
-        time.sleep(0.05)
-        
-    @property
-    def global_state(self):
-        state = self.query(":INST:STATE").strip()
-        time.sleep(0.05)
-        if state == "1":
-            return "ON"
-        else:
-            return "OFF"
-
-    @global_state.setter
-    def global_state(self, state):
-        if state == "ON":
-            self.set(":INST:STATE", "ON")
-        else:
-            self.set(":INST:STATE", "OFF")
-        time.sleep(0.05)
-    
-    @property
-    def global_mode(self):
-        mode = self.query(":PULSE0:MODE")
-        time.sleep(0.05)
-        return mode
-    
-    @global_mode.setter
-    def global_mode(self, mode):
-        self.set(":PULSE0:MODE", mode)
-        time.sleep(0.05)
-        
-    def close(self):
-        self.com.close()
-    
-    def set_channel(self):
-        if self.channel_label == "A":
-            channel = 1
-            return channel
-        elif self.channel_label == "B":
-            channel = 2
-            return channel
-        elif self.channel_label == "C":
-            channel = 3
-            return channel
-        elif self.channel_label == "D":
-            channel = 4
-            return channel
-
-    @property
-    def channel_label(self):
-        return self._channel_label
-
-    @channel_label.setter
-    def channel_label(self, channel_label):
-        self._channel_label = channel_label
-        
-    @property
-    def channel_mode(self):
-        channel = self.set_channel()
-        mode = self.query(f":PULSE{channel}:CMOD").strip()
-        time.sleep(0.05)
-        return mode
-
-    @channel_mode.setter
-    def channel_mode(self, mode):
-        channel = self.set_channel()
-        self.set(f":PULSE{channel}:CMOD", mode)
-        time.sleep(0.05)
-        
-    @property
-    def channel_state(self):
-        channel = self.set_channel()
-        state = self.query(f":PULSE{channel}:STATE").strip()
-        time.sleep(0.05)
-        if state == "1":
-            return "ON"
-        else:
-            return "OFF"
-
-    @channel_state.setter    
-    def channel_state(self, state):
-        channel = self.set_channel()
-        self.set(f":PULSE{channel}:STATE", state)
-        time.sleep(0.05)
-
-    @property
-    def trig_mode(self):
-        trig_mode = self.query(":PULSE0:TRIG:MODE").strip()
-        time.sleep(0.05)
-        return trig_mode
-
-    @trig_mode.setter
-    def trig_mode(self, mode):
-        self.set(f":PULSE0:TRIG:MODE", mode)
-        time.sleep(0.05)
-        
-    @property        
-    def trig_thresh(self):
-        thresh = float(self.query(":PULSE0:TRIG:LEV").strip())
-        time.sleep(0.05)
-        return thresh
-    
-    @trig_thresh.setter
-    def trig_thresh(self, thresh):
-        self.set(f":PULSE0:TRIG:LEV", str(thresh))
-        time.sleep(0.05)
-
-    @property
-    def trig_edge(self):
-        edge = self.query(":PULSE0:TRIG:EDGE").strip()
-        time.sleep(0.05)
-        if edge == "RIS":
-            return "RISING"
-        else:
-            return "FALLING"
-    
-    @trig_edge.setter
-    def trig_edge(self, edge):
-        self.set(f":PULSE0:TRIG:EDGE", edge)
-        time.sleep(0.05)
-
-    @property
-    def gate_mode(self):
-        gate_mode = self.query(":PULSE0:GATE:MODE").strip()
-        time.sleep(0.05)
-        return gate_mode
-
-    @gate_mode.setter
-    def gate_mode(self, mode):
-        self.set(f":PULSE0:GATE:MODE", mode)
-
-    @property        
-    def gate_thresh(self):
-        thresh = float(self.query(":PULSE0:GATE:LEV").strip())
-        time.sleep(0.05)
-        return thresh
-    
-    @gate_thresh.setter
-    def gate_thresh(self, thresh):
-        self.set(f":PULSE0:GATE:LEV", str(thresh))
-        time.sleep(0.05)
-
-    @property
-    def gate_logic(self):
-        global_gate_mode = self.query(":PULSE0:GATE:MODE").strip()
-        time.sleep(0.05)
-        if global_gate_mode == "CHAN":
-            channel = self.set_channel()
-            logic = self.query(f":PULSE{channel}:CLOGIC").strip()
-            time.sleep(0.05)
-            return logic
-        else:
-            logic = self.query(f":PULSE0:GATE:LOGIC").strip()
-            time.sleep(0.05)
-            return logic
-        
-    @gate_logic.setter
-    def gate_logic(self, logic):
-        global_gate_mode = self.query(":PULSE0:GATE:MODE").strip()
-        time.sleep(0.05)
-        if global_gate_mode == "CHAN":
-            channel = self.set_channel()
-            self.set(f":PULSE{channel}:CLOGIC", logic)
-            time.sleep(0.05)
-        else:
-            self.set(f":PULSE0:GATE:LOGIC", logic)
-            time.sleep(0.05)
-
-    @property
-    def channel_gate_mode(self):
-        global_gate_mode = self.query(":PULSE0:GATE:MODE").strip()
-        time.sleep(0.05)
-        if global_gate_mode == "CHAN":
-            channel = self.set_channel()
-            mode = self.query(f":PULSE{channel}:CGATE").strip()
-            time.sleep(0.05)
-            return mode
-        else:
-            return "DIS"
-        
-    @channel_gate_mode.setter
-    def channel_gate_mode(self, channel_gate_mode):
-        global_gate_mode = self.query(":PULSE0:GATE:MODE").strip()
-        channel = self.set_channel()
-        time.sleep(0.05)
-        if global_gate_mode == "CHAN":
-            channel = self.set_channel()
-            self.set(f":PULSE{channel}:CGATE", channel_gate_mode)
-            time.sleep(0.05)
-        else:
-            self.set(f":PULSE0:GATE:MODE", "CHAN")
-            time.sleep(0.05)
-            self.set(f":PULSE{channel}:CGATE", channel_gate_mode)
-            time.sleep(0.05)
-
-    @property
-    def period(self):
-        period = float(self.query(":PULSE0:PER").strip())
-        time.sleep(0.05)
-        return period
-    
-    @period.setter
-    def period(self, period):
-        self.set(f":PULSE0:PER", str(period))
-        time.sleep(0.05)
-
-    @property
-    def delay(self):
-        channel = self.set_channel()
-        delay = float(self.query(f":PULSE{channel}:DELAY").strip())
-        time.sleep(0.05)
-        return delay
-
-    @delay.setter
-    def delay(self, delay):
-        channel = self.set_channel()
-        self.set(f":PULSE{channel}:DELAY", "{:10.9f}".format(delay))
-        time.sleep(0.05)
-
-    @property
-    def width(self):
-        channel = self.set_channel()
-        width = float(self.query(f":PULSE{channel}:WIDT").strip())
-        time.sleep(0.05)
-        return width
-    
-    @width.setter
-    def width(self, width):
-        channel = self.set_channel()
-        self.set(f":PULSE{channel}:WIDT", "{:10.9f}".format(width))
-        time.sleep(0.05)
-
-    @property
-    def amplitude_mode(self):
-        channel = self.set_channel()
-        mode = self.query(f":PULSE{channel}:OUTP:MODE").strip()
-        time.sleep(0.05)
-        return mode
-    
-    @amplitude_mode.setter
-    def amplitude_mode(self, mode):
-        channel = self.set_channel()
-        self.set(f":PULSE{channel}:OUTP:MODE", mode)
-        time.sleep(0.05)
-
-    @property
-    def amplitude(self):
-        channel = self.set_channel()
-        amp = float(self.query(f":PULSE{channel}:OUTP:AMPL").strip())
-        time.sleep(0.05)
-        return amp
-    
-    @amplitude.setter
-    def amplitude(self, amplitude):
-        amp_mode = self.amplitude_mode
-        if amp_mode == "ADJ":
-            channel = self.set_channel()
-            self.set(f":PULSE{channel}:OUTP:AMPL", str(amplitude))
-            time.sleep(0.05)
-        else:
-            return "In TTL mode. First, switch to ADJ mode."
-
-    @property
-    def polarity(self):
-        channel = self.set_channel()
-        pol = self.query(f":PULSE{channel}:POL").strip()
-        time.sleep(0.05)
-        return pol
-    
-    @polarity.setter
-    def polarity(self, pol):
-        channel = self.set_channel()
-        self.set(f":PULSE{channel}:POL", pol)
-        time.sleep(0.05)
-
-    def output(self):
-        out = {}
-        out['Configuration Label'] = self.label
-        time.sleep(0.075)
-        out['Local Memory Slot'] = self.slot
-        time.sleep(0.075)
-        out['Global State'] = self.global_state
-        time.sleep(0.075)
-        out['Global Mode'] = self.global_mode
-        time.sleep(0.075)
-        out['Channel'] = self.channel_label
-        time.sleep(0.075)
-        out['Channel Mode'] = self.channel_mode
-        time.sleep(0.075)
-        out['Channel State'] = self.channel_state
-        time.sleep(0.075)
-        out['Width (s)'] = self.width
-        time.sleep(0.075)
-        out['Amplitude Mode'] = self.amplitude_mode
-        time.sleep(0.075)
-        out['Amplitude (V)'] = self.amplitude
-        time.sleep(0.075)
-        out['Polarity'] = self.polarity
-        time.sleep(0.075)
-        out['Delay (s)'] = self.delay
-        time.sleep(0.075)
-        out['Period (s)'] = self.period
-        time.sleep(0.075)
-        out['Trigger Mode'] = self.trig_mode
-        time.sleep(0.075)
-        out['Trigger Threshold (V)'] = self.trig_thresh
-        time.sleep(0.075)
-        out['Trigger Edge'] = self.trig_edge
-        time.sleep(0.075)
-        out['Global Gate Mode'] = self.gate_mode
-        time.sleep(0.075)
-        out['Channel Gate Mode'] = self.channel_gate_mode
-        time.sleep(0.075)
-        out['Gate Threshold (V)'] = self.gate_thresh
-        time.sleep(0.075)
-        out['Gate Logic'] = self.gate_logic
-        time.sleep(0.075)
-
-        return out
-        
+import time
+from pymodaq_plugins_bnc.hardware.device import Device
+
+class BNC575(Device):
+
+    def __init__(self, ip, port):
+        super().__init__(ip, port)
+        self.channel_label = "A"
+        self.slot = 1
+
+    def idn(self):
+        idn = self.query("*IDN").strip()
+        time.sleep(0.25)
+        return idn
+
+    @property
+    def ip(self):
+        return self.ip
+
+    @property
+    def port(self):
+        return self.port
+
+    def reset(self):
+        self.send("*RST")
+        time.sleep(0.05)
+
+    def stop(self):
+        pass
+    
+    @property
+    def slot(self):
+        return self._slot
+    
+    @slot.setter
+    def slot(self, slot):
+        self._slot = slot
+    
+    def save_state(self):
+        self.set("*SAV", str(self.slot))
+        time.sleep(0.05)
+    
+    def restore_state(self):
+        self.set("*RCL", str(self.slot))
+        time.sleep(0.05)
+    
+    def trig(self):
+        self.send("*TRG")
+        time.sleep(0.05)
+    
+    @property
+    def label(self):
+        lbl = self.query("*LBL").strip()
+        time.sleep(0.05)
+        return lbl
+    
+    @label.setter
+    def label(self, label):
+        self.set("*LBL", "\"" + label + "\"")
+        time.sleep(0.05)
+        
+    @property
+    def global_state(self):
+        state = self.query(":INST:STATE").strip()
+        time.sleep(0.05)
+        if state == "1":
+            return "ON"
+        else:
+            return "OFF"
+
+    @global_state.setter
+    def global_state(self, state):
+        if state == "ON":
+            self.set(":INST:STATE", "ON")
+        else:
+            self.set(":INST:STATE", "OFF")
+        time.sleep(0.05)
+    
+    @property
+    def global_mode(self):
+        mode = self.query(":PULSE0:MODE")
+        time.sleep(0.05)
+        return mode
+    
+    @global_mode.setter
+    def global_mode(self, mode):
+        self.set(":PULSE0:MODE", mode)
+        time.sleep(0.05)
+        
+    def close(self):
+        self.com.close()
+    
+    def set_channel(self):
+        if self.channel_label == "A":
+            channel = 1
+            return channel
+        elif self.channel_label == "B":
+            channel = 2
+            return channel
+        elif self.channel_label == "C":
+            channel = 3
+            return channel
+        elif self.channel_label == "D":
+            channel = 4
+            return channel
+
+    @property
+    def channel_label(self):
+        return self._channel_label
+
+    @channel_label.setter
+    def channel_label(self, channel_label):
+        self._channel_label = channel_label
+        
+    @property
+    def channel_mode(self):
+        channel = self.set_channel()
+        mode = self.query(f":PULSE{channel}:CMOD").strip()
+        time.sleep(0.05)
+        return mode
+
+    @channel_mode.setter
+    def channel_mode(self, mode):
+        channel = self.set_channel()
+        self.set(f":PULSE{channel}:CMOD", mode)
+        time.sleep(0.05)
+        
+    @property
+    def channel_state(self):
+        channel = self.set_channel()
+        state = self.query(f":PULSE{channel}:STATE").strip()
+        time.sleep(0.05)
+        if state == "1":
+            return "ON"
+        else:
+            return "OFF"
+
+    @channel_state.setter    
+    def channel_state(self, state):
+        channel = self.set_channel()
+        self.set(f":PULSE{channel}:STATE", state)
+        time.sleep(0.05)
+
+    @property
+    def trig_mode(self):
+        trig_mode = self.query(":PULSE0:TRIG:MODE").strip()
+        time.sleep(0.05)
+        return trig_mode
+
+    @trig_mode.setter
+    def trig_mode(self, mode):
+        self.set(f":PULSE0:TRIG:MODE", mode)
+        time.sleep(0.05)
+        
+    @property        
+    def trig_thresh(self):
+        thresh = float(self.query(":PULSE0:TRIG:LEV").strip())
+        time.sleep(0.05)
+        return thresh
+    
+    @trig_thresh.setter
+    def trig_thresh(self, thresh):
+        self.set(f":PULSE0:TRIG:LEV", str(thresh))
+        time.sleep(0.05)
+
+    @property
+    def trig_edge(self):
+        edge = self.query(":PULSE0:TRIG:EDGE").strip()
+        time.sleep(0.05)
+        if edge == "RIS":
+            return "RISING"
+        else:
+            return "FALLING"
+    
+    @trig_edge.setter
+    def trig_edge(self, edge):
+        self.set(f":PULSE0:TRIG:EDGE", edge)
+        time.sleep(0.05)
+
+    @property
+    def gate_mode(self):
+        gate_mode = self.query(":PULSE0:GATE:MODE").strip()
+        time.sleep(0.05)
+        return gate_mode
+
+    @gate_mode.setter
+    def gate_mode(self, mode):
+        self.set(f":PULSE0:GATE:MODE", mode)
+
+    @property        
+    def gate_thresh(self):
+        thresh = float(self.query(":PULSE0:GATE:LEV").strip())
+        time.sleep(0.05)
+        return thresh
+    
+    @gate_thresh.setter
+    def gate_thresh(self, thresh):
+        self.set(f":PULSE0:GATE:LEV", str(thresh))
+        time.sleep(0.05)
+
+    @property
+    def gate_logic(self):
+        global_gate_mode = self.query(":PULSE0:GATE:MODE").strip()
+        time.sleep(0.05)
+        if global_gate_mode == "CHAN":
+            channel = self.set_channel()
+            logic = self.query(f":PULSE{channel}:CLOGIC").strip()
+            time.sleep(0.05)
+            return logic
+        else:
+            logic = self.query(f":PULSE0:GATE:LOGIC").strip()
+            time.sleep(0.05)
+            return logic
+        
+    @gate_logic.setter
+    def gate_logic(self, logic):
+        global_gate_mode = self.query(":PULSE0:GATE:MODE").strip()
+        time.sleep(0.05)
+        if global_gate_mode == "CHAN":
+            channel = self.set_channel()
+            self.set(f":PULSE{channel}:CLOGIC", logic)
+            time.sleep(0.05)
+        else:
+            self.set(f":PULSE0:GATE:LOGIC", logic)
+            time.sleep(0.05)
+
+    @property
+    def channel_gate_mode(self):
+        global_gate_mode = self.query(":PULSE0:GATE:MODE").strip()
+        time.sleep(0.05)
+        if global_gate_mode == "CHAN":
+            channel = self.set_channel()
+            mode = self.query(f":PULSE{channel}:CGATE").strip()
+            time.sleep(0.05)
+            return mode
+        else:
+            return "DIS"
+        
+    @channel_gate_mode.setter
+    def channel_gate_mode(self, channel_gate_mode):
+        global_gate_mode = self.query(":PULSE0:GATE:MODE").strip()
+        channel = self.set_channel()
+        time.sleep(0.05)
+        if global_gate_mode == "CHAN":
+            channel = self.set_channel()
+            self.set(f":PULSE{channel}:CGATE", channel_gate_mode)
+            time.sleep(0.05)
+        else:
+            self.set(f":PULSE0:GATE:MODE", "CHAN")
+            time.sleep(0.05)
+            self.set(f":PULSE{channel}:CGATE", channel_gate_mode)
+            time.sleep(0.05)
+
+    @property
+    def period(self):
+        period = float(self.query(":PULSE0:PER").strip())
+        time.sleep(0.05)
+        return period
+    
+    @period.setter
+    def period(self, period):
+        self.set(f":PULSE0:PER", str(period))
+        time.sleep(0.05)
+
+    @property
+    def delay(self):
+        channel = self.set_channel()
+        delay = float(self.query(f":PULSE{channel}:DELAY").strip())
+        time.sleep(0.05)
+        return delay
+
+    @delay.setter
+    def delay(self, delay):
+        channel = self.set_channel()
+        self.set(f":PULSE{channel}:DELAY", "{:10.9f}".format(delay))
+        time.sleep(0.05)
+
+    @property
+    def width(self):
+        channel = self.set_channel()
+        width = float(self.query(f":PULSE{channel}:WIDT").strip())
+        time.sleep(0.05)
+        return width
+    
+    @width.setter
+    def width(self, width):
+        channel = self.set_channel()
+        self.set(f":PULSE{channel}:WIDT", "{:10.9f}".format(width))
+        time.sleep(0.05)
+
+    @property
+    def amplitude_mode(self):
+        channel = self.set_channel()
+        mode = self.query(f":PULSE{channel}:OUTP:MODE").strip()
+        time.sleep(0.05)
+        return mode
+    
+    @amplitude_mode.setter
+    def amplitude_mode(self, mode):
+        channel = self.set_channel()
+        self.set(f":PULSE{channel}:OUTP:MODE", mode)
+        time.sleep(0.05)
+
+    @property
+    def amplitude(self):
+        channel = self.set_channel()
+        amp = float(self.query(f":PULSE{channel}:OUTP:AMPL").strip())
+        time.sleep(0.05)
+        return amp
+    
+    @amplitude.setter
+    def amplitude(self, amplitude):
+        amp_mode = self.amplitude_mode
+        if amp_mode == "ADJ":
+            channel = self.set_channel()
+            self.set(f":PULSE{channel}:OUTP:AMPL", str(amplitude))
+            time.sleep(0.05)
+        else:
+            return "In TTL mode. First, switch to ADJ mode."
+
+    @property
+    def polarity(self):
+        channel = self.set_channel()
+        pol = self.query(f":PULSE{channel}:POL").strip()
+        time.sleep(0.05)
+        return pol
+    
+    @polarity.setter
+    def polarity(self, pol):
+        channel = self.set_channel()
+        self.set(f":PULSE{channel}:POL", pol)
+        time.sleep(0.05)
+
+    def output(self):
+        out = {}
+        out['IP Address'] = self.ip
+        time.sleep(0.075)
+        out['Port'] = self.port
+        time.sleep(0.075)
+        out['Configuration Label'] = self.label
+        time.sleep(0.075)
+        out['Local Memory Slot'] = self.slot
+        time.sleep(0.075)
+        out['Global State'] = self.global_state
+        time.sleep(0.075)
+        out['Global Mode'] = self.global_mode
+        time.sleep(0.075)
+        out['Channel'] = self.channel_label
+        time.sleep(0.075)
+        out['Channel Mode'] = self.channel_mode
+        time.sleep(0.075)
+        out['Channel State'] = self.channel_state
+        time.sleep(0.075)
+        out['Width (s)'] = self.width
+        time.sleep(0.075)
+        out['Amplitude Mode'] = self.amplitude_mode
+        time.sleep(0.075)
+        out['Amplitude (V)'] = self.amplitude
+        time.sleep(0.075)
+        out['Polarity'] = self.polarity
+        time.sleep(0.075)
+        out['Delay (s)'] = self.delay
+        time.sleep(0.075)
+        out['Period (s)'] = self.period
+        time.sleep(0.075)
+        out['Trigger Mode'] = self.trig_mode
+        time.sleep(0.075)
+        out['Trigger Threshold (V)'] = self.trig_thresh
+        time.sleep(0.075)
+        out['Trigger Edge'] = self.trig_edge
+        time.sleep(0.075)
+        out['Global Gate Mode'] = self.gate_mode
+        time.sleep(0.075)
+        out['Channel Gate Mode'] = self.channel_gate_mode
+        time.sleep(0.075)
+        out['Gate Threshold (V)'] = self.gate_thresh
+        time.sleep(0.075)
+        out['Gate Logic'] = self.gate_logic
+        time.sleep(0.075)
+
+        return out
+
```

### Comparing `pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc.egg-info/PKG-INFO` & `pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,62 @@
-Metadata-Version: 2.1
-Name: pymodaq_plugins_bnc
-Version: 0.0.3
-Summary: PyMoDAQ module for communication and readout from BNC575 delay/signal generator
-Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_bnc
-Author: Christian Cabello
-Author-email: christian.cabello@ip-paris.fr
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Other Environment
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: User Interfaces
-License-File: LICENSE
-Requires-Dist: toml
-Requires-Dist: pymodaq>=4.1.0
-
-pymodaq_plugins_bnc
-
-
-.. image:: https://img.shields.io/pypi/v/pymodaq_plugins_template.svg
-   :target: https://pypi.org/project/pymodaq_plugins_template/
-   :alt: Latest Version
-
-.. image:: https://readthedocs.org/projects/pymodaq/badge/?version=latest
-   :target: https://pymodaq.readthedocs.io/en/stable/?badge=latest
-   :alt: Documentation Status
-
-.. image:: https://github.com/PyMoDAQ/pymodaq_plugins_template/workflows/Upload%20Python%20Package/badge.svg
-   :target: https://github.com/PyMoDAQ/pymodaq_plugins_template
-   :alt: Publication Status
-
-.. image:: https://github.com/PyMoDAQ/pymodaq_plugins_template/actions/workflows/Test.yml/badge.svg
-    :target: https://github.com/PyMoDAQ/pymodaq_plugins_template/actions/workflows/Test.yml
-
-
-Authors
-=======
-
-* First Author  (christian.cabello@ip-paris.fr)
-
-
-Instruments
-===========
-
-Below is the list of instruments included in this plugin
-
-Actuator
-++++++++
-
-BNC575 Delay/Pulse Generator Interface with Delay Scan Capability
-
-
-
-Installation instructions
-=========================
-
-* Tested on PyMoDAQ version 4.1.1
-* Tested on Python 3.8.18
-* No additional drivers necessary
+Metadata-Version: 2.1
+Name: pymodaq_plugins_bnc
+Version: 0.0.4
+Summary: PyMoDAQ module for communication and readout from BNC575 delay/signal generator
+Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_bnc
+Author: Christian Cabello
+Author-email: christian.cabello@ip-paris.fr
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Other Environment
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: User Interfaces
+License-File: LICENSE
+Requires-Dist: toml
+Requires-Dist: pymodaq>=4.1.0
+
+pymodaq_plugins_bnc
+
+
+.. image:: https://img.shields.io/pypi/v/pymodaq_plugins_bnc.svg
+   :target: https://pypi.org/project/pymodaq-plugins-bnc
+   :alt: Latest Version
+
+.. image:: https://github.com/ccabello99/pymodaq_plugins_bnc/workflows/Upload%20Python%20Package/badge.svg
+   :target: https://github.com/ccabello99/pymodaq_plugins_bnc
+   :alt: Publication Status
+
+.. image:: https://github.com/ccabello99/pymodaq_plugins_bnc/actions/workflows/Test.yml/badge.svg
+    :target: https://github.com/ccabello99/pymodaq_plugins_bnc/actions/workflows/Test.yml
+
+
+Authors
+=======
+
+* First Author  (christian.cabello@ip-paris.fr)
+
+
+Instruments
+===========
+
+Below is the list of instruments included in this plugin
+
+Actuator
+++++++++
+
+BNC575 Delay/Pulse Generator Interface with Delay Scan Capability
+
+
+
+Installation instructions
+=========================
+
+* Tested on PyMoDAQ version 4.1.1
+* Tested on Python 3.8.18
+* No additional drivers necessary
+* To install plugin, run: pip install pymodaq-plugins-bnc
```

### Comparing `pymodaq_plugins_bnc-0.0.3/src/pymodaq_plugins_bnc.egg-info/SOURCES.txt` & `pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 src/pymodaq_plugins_bnc/hardware/__init__.py
 src/pymodaq_plugins_bnc/hardware/bnc_commands.py
 src/pymodaq_plugins_bnc/hardware/device.py
 src/pymodaq_plugins_bnc/models/__init__.py
 src/pymodaq_plugins_bnc/resources/VERSION
 src/pymodaq_plugins_bnc/resources/__init__.py
 src/pymodaq_plugins_bnc/resources/config_template.toml
-src/pymodaq_plugins_bnc/scanners/__init__.py
+src/pymodaq_plugins_bnc/scanners/__init__.py
+tests/test_plugin_package_structure.py
```

