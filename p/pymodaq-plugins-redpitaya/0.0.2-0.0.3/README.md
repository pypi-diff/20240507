# Comparing `tmp/pymodaq_plugins_redpitaya-0.0.2.tar.gz` & `tmp/pymodaq_plugins_redpitaya-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugins_redpitaya-0.0.2.tar", last modified: Mon Jan 29 15:16:07 2024, max compression
+gzip compressed data, was "pymodaq_plugins_redpitaya-0.0.3.tar", last modified: Tue May  7 14:11:02 2024, max compression
```

## Comparing `pymodaq_plugins_redpitaya-0.0.2.tar` & `pymodaq_plugins_redpitaya-0.0.3.tar`

### file list

```diff
@@ -1,69 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-01-29 15:16:07.078621 pymodaq_plugins_redpitaya-0.0.2/
--rw-rw-rw-   0        0        0     1128 2024-01-25 13:47:56.000000 pymodaq_plugins_redpitaya-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       46 2024-01-25 13:47:56.000000 pymodaq_plugins_redpitaya-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2445 2024-01-29 15:16:07.076621 pymodaq_plugins_redpitaya-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1476 2024-01-29 15:15:40.000000 pymodaq_plugins_redpitaya-0.0.2/README.rst
--rw-rw-rw-   0        0        0       42 2024-01-29 15:16:07.079623 pymodaq_plugins_redpitaya-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      106 2024-01-25 13:47:56.000000 pymodaq_plugins_redpitaya-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-29 15:16:06.962999 pymodaq_plugins_redpitaya-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-01-29 15:16:06.993525 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/
--rw-rw-rw-   0        0        0      281 2024-01-25 13:47:56.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-29 15:16:07.009593 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/__pycache__/
--rw-rw-rw-   0        0        0      553 2024-01-26 12:46:04.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      823 2024-01-26 12:46:04.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/__pycache__/utils.cpython-310.pyc
-drwxrwxrwx   0        0        0        0 2024-01-29 15:16:07.010523 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_move_plugins/
--rw-rw-rw-   0        0        0      467 2024-01-25 13:47:56.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_move_plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-29 15:16:07.014068 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_move_plugins/__pycache__/
--rw-rw-rw-   0        0        0      729 2024-01-26 12:46:05.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_move_plugins/__pycache__/__init__.cpython-310.pyc
-drwxrwxrwx   0        0        0        0 2024-01-29 15:16:07.015524 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/
--rw-rw-rw-   0        0        0        6 2024-01-25 13:47:56.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-29 15:16:07.018084 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/__pycache__/
--rw-rw-rw-   0        0        0      252 2024-01-26 12:46:05.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/__pycache__/__init__.cpython-310.pyc
-drwxrwxrwx   0        0        0        0 2024-01-29 15:16:07.019621 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_0D/
--rw-rw-rw-   0        0        0      472 2024-01-25 13:47:56.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_0D/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-29 15:16:07.021527 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_0D/__pycache__/
--rw-rw-rw-   0        0        0      746 2024-01-26 12:46:05.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_0D/__pycache__/__init__.cpython-310.pyc
-drwxrwxrwx   0        0        0        0 2024-01-29 15:16:07.030526 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_1D/
--rw-rw-rw-   0        0        0      472 2024-01-25 13:47:56.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_1D/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-29 15:16:07.040527 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_1D/__pycache__/
--rw-rw-rw-   0        0        0      746 2024-01-26 12:46:06.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_1D/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     6172 2024-01-26 13:02:42.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_1D/__pycache__/daq_1Dviewer_RedPitayaSCPI.cpython-310.pyc
--rw-rw-rw-   0        0        0     6661 2024-01-26 12:54:37.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_1D/__pycache__/lextab.cpython-310.pyc
--rw-rw-rw-   0        0        0   180884 2024-01-26 12:54:37.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_1D/__pycache__/yacctab.cpython-310.pyc
--rw-rw-rw-   0        0        0     8360 2024-01-29 15:06:53.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_1D/daq_1Dviewer_RedPitayaSCPI.py
--rw-rw-rw-   0        0        0     8553 2024-01-29 15:07:13.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_1D/lextab.py
--rw-rw-rw-   0        0        0   210417 2024-01-29 15:07:15.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_1D/yacctab.py
-drwxrwxrwx   0        0        0        0 2024-01-29 15:16:07.043738 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_2D/
--rw-rw-rw-   0        0        0      474 2024-01-25 13:47:56.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_2D/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-29 15:16:07.045547 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_2D/__pycache__/
--rw-rw-rw-   0        0        0      746 2024-01-26 12:46:06.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_2D/__pycache__/__init__.cpython-310.pyc
-drwxrwxrwx   0        0        0        0 2024-01-29 15:16:07.047529 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_ND/
--rw-rw-rw-   0        0        0      472 2024-01-25 13:47:56.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_ND/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-29 15:16:07.050524 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_ND/__pycache__/
--rw-rw-rw-   0        0        0      746 2024-01-26 12:46:06.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_ND/__pycache__/__init__.cpython-310.pyc
-drwxrwxrwx   0        0        0        0 2024-01-29 15:16:07.051527 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/exporters/
--rw-rw-rw-   0        0        0       87 2024-01-25 13:47:56.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/exporters/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-29 15:16:07.057169 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/extensions/
--rw-rw-rw-   0        0        0       87 2024-01-25 13:47:56.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/extensions/__init__.py
--rw-rw-rw-   0        0        0     7559 2024-01-25 13:47:56.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/extensions/myextension.py
-drwxrwxrwx   0        0        0        0 2024-01-29 15:16:07.059876 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/hardware/
--rw-rw-rw-   0        0        0        0 2024-01-25 13:47:56.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/hardware/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-29 15:16:07.063643 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/models/
--rw-rw-rw-   0        0        0     3167 2024-01-25 13:47:56.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/models/PIDModelTemplate.py
--rw-rw-rw-   0        0        0       87 2024-01-25 13:47:56.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-29 15:16:07.069869 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/resources/
--rw-rw-rw-   0        0        0        7 2024-01-29 15:15:56.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/resources/VERSION
--rw-rw-rw-   0        0        0        0 2024-01-25 13:47:56.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/resources/__init__.py
--rw-rw-rw-   0        0        0      338 2024-01-29 14:39:18.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/resources/config_template.toml
-drwxrwxrwx   0        0        0        0 2024-01-29 15:16:07.072621 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/scanners/
--rw-rw-rw-   0        0        0       87 2024-01-25 13:47:56.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/scanners/__init__.py
--rw-rw-rw-   0        0        0      434 2024-01-25 13:47:56.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-29 15:16:07.005547 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya.egg-info/
--rw-rw-rw-   0        0        0     2445 2024-01-29 15:16:06.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2643 2024-01-29 15:16:06.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-29 15:16:06.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2024-01-29 15:16:06.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2024-01-29 15:16:06.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-01-29 15:16:06.000000 pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-01-29 15:16:07.074621 pymodaq_plugins_redpitaya-0.0.2/tests/
--rw-rw-rw-   0        0        0     3267 2024-01-25 13:47:56.000000 pymodaq_plugins_redpitaya-0.0.2/tests/test_plugin_package_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:11:02.272780 pymodaq_plugins_redpitaya-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-07 14:10:29.000000 pymodaq_plugins_redpitaya-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 14:10:29.000000 pymodaq_plugins_redpitaya-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-07 14:11:02.272780 pymodaq_plugins_redpitaya-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-07 14:10:29.000000 pymodaq_plugins_redpitaya-0.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:11:02.272780 pymodaq_plugins_redpitaya-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 14:10:29.000000 pymodaq_plugins_redpitaya-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:11:02.264780 pymodaq_plugins_redpitaya-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:11:02.268780 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-07 14:10:29.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:11:02.268780 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/daq_move_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-07 14:10:29.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/daq_move_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:11:02.268780 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-07 14:10:29.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:11:02.268780 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_0D/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 14:10:29.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_0D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:11:02.268780 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_1D/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 14:10:29.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_1D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8170 2024-05-07 14:10:29.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_1D/daq_1Dviewer_RedPitayaSCPI.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:11:02.268780 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_2D/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-07 14:10:29.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_2D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:11:02.268780 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_ND/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 14:10:29.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/daq_viewer_plugins/plugins_ND/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:11:02.268780 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 14:10:29.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/exporters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:11:02.268780 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 14:10:29.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-05-07 14:10:29.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/extensions/myextension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:11:02.268780 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:10:29.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/hardware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:11:02.272780 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-07 14:10:29.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/models/PIDModelTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 14:10:29.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:11:02.272780 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 14:10:29.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/resources/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:10:29.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-07 14:10:29.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/resources/config_template.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:11:02.272780 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/scanners/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 14:10:29.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/scanners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-07 14:10:29.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:11:02.268780 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-07 14:11:02.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-07 14:11:02.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:11:02.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-07 14:11:02.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 14:11:02.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 14:11:02.000000 pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya.egg-info/top_level.txt
```

### Comparing `pymodaq_plugins_redpitaya-0.0.2/LICENSE` & `pymodaq_plugins_redpitaya-0.0.3/LICENSE`

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

### Comparing `pymodaq_plugins_redpitaya-0.0.2/PKG-INFO` & `pymodaq_plugins_redpitaya-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,72 +1,71 @@
-Metadata-Version: 2.1
-Name: pymodaq_plugins_redpitaya
-Version: 0.0.2
-Summary: PyMoDAQ Plugin to use the Redpitaya electronic board
-Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_redpitaya
-Author: Sebastien J. Weber
-Author-email: sebastien.weber@cemes.fr
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
-Requires-Dist: pymeasure
-
-pymodaq_plugins_redpitaya
-#########################
-
-.. the following must be adapted to your developed package, links to pypi, github  description...
-
-.. image:: https://img.shields.io/pypi/v/pymodaq_plugins_redpitaya.svg
-   :target: https://pypi.org/project/pymodaq_plugins_redpitaya/
-   :alt: Latest Version
-
-.. image:: https://readthedocs.org/projects/pymodaq/badge/?version=latest
-   :target: https://pymodaq.readthedocs.io/en/stable/?badge=latest
-   :alt: Documentation Status
-
-.. image:: https://github.com/PyMoDAQ/pymodaq_plugins_redpitaya/workflows/Upload%20Python%20Package/badge.svg
-   :target: https://github.com/PyMoDAQ/pymodaq_plugins_redpitaya
-   :alt: Publication Status
-
-.. image:: https://github.com/PyMoDAQ/pymodaq_plugins_redpitaya/actions/workflows/Test.yml/badge.svg
-    :target: https://github.com/PyMoDAQ/pymodaq_plugins_redpitaya/actions/workflows/Test.yml
-
-
-PyMoDAQ Plugin to use the Redpitaya electronic board
-
-https://redpitaya.readthedocs.io/en/latest/
-
-
-Authors
-=======
-
-* Sebastien J. Weber  (sebastien.weber@cemes.fr)
-
-Instruments
-===========
-
-Below is the list of instruments included in this plugin
-
-
-Viewer1D
-++++++++
-
-* **RedPitayaSCPI**: perform analog data acquisition using one of the fast channels
-
-
-Installation instructions
-=========================
-
-* PyMoDAQâ€™s version: >= 4.1.0
-* Operating systemâ€™s version: any
-* For the SCPI version, use the driver from the pymeasure package
+Metadata-Version: 2.1
+Name: pymodaq_plugins_redpitaya
+Version: 0.0.3
+Summary: PyMoDAQ Plugin to use the Redpitaya electronic board
+Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_redpitaya
+Author: Sebastien J. Weber
+Author-email: sebastien.weber@cemes.fr
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
+
+pymodaq_plugins_redpitaya
+#########################
+
+.. the following must be adapted to your developed package, links to pypi, github  description...
+
+.. image:: https://img.shields.io/pypi/v/pymodaq_plugins_redpitaya.svg
+   :target: https://pypi.org/project/pymodaq_plugins_redpitaya/
+   :alt: Latest Version
+
+.. image:: https://readthedocs.org/projects/pymodaq/badge/?version=latest
+   :target: https://pymodaq.readthedocs.io/en/stable/?badge=latest
+   :alt: Documentation Status
+
+.. image:: https://github.com/PyMoDAQ/pymodaq_plugins_redpitaya/workflows/Upload%20Python%20Package/badge.svg
+   :target: https://github.com/PyMoDAQ/pymodaq_plugins_redpitaya
+   :alt: Publication Status
+
+.. image:: https://github.com/PyMoDAQ/pymodaq_plugins_redpitaya/actions/workflows/Test.yml/badge.svg
+    :target: https://github.com/PyMoDAQ/pymodaq_plugins_redpitaya/actions/workflows/Test.yml
+
+
+PyMoDAQ Plugin to use the Redpitaya electronic board
+
+https://redpitaya.readthedocs.io/en/latest/
+
+
+Authors
+=======
+
+* Sebastien J. Weber  (sebastien.weber@cemes.fr)
+
+
+Instruments
+===========
+
+Below is the list of instruments included in this plugin
+
+
+Viewer1D
+++++++++
+
+* **RedPitayaSCPI**: perform analog data acquisition using one of the fast channels
+
+
+
+Installation instructions
+=========================
+
+* PyMoDAQ’s version: >= 4.1.0
+* Operating system’s version: any
+* For the SCPI version, use the driver from the pymeasure package
```

### Comparing `pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/extensions/myextension.py` & `pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/extensions/myextension.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,195 +1,195 @@
-from pymodaq.utils import gui_utils as gutils
-from pymodaq.utils import daq_utils as utils
-from pyqtgraph.parametertree import Parameter, ParameterTree
-from pymodaq.utils.parameter import pymodaq_ptypes
-from qtpy import QtWidgets, QtCore
-
-from pymodaq.utils.plotting.data_viewers.viewer1D import Viewer1D
-from pymodaq.utils.plotting.data_viewers.viewer2D import Viewer2D
-
-
-config = utils.load_config()
-logger = utils.set_logger(utils.get_module_name(__file__))
-
-EXTENSION_NAME = 'MY_EXTENSION_NAME'
-CLASS_NAME = 'MyExtension'
-
-
-class MyExtension(gutils.CustomApp):
-    # list of dicts enabling the settings tree on the user interface
-    params = [
-        {'title': 'Main settings:', 'name': 'main_settings', 'type': 'group', 'children': [
-            {'title': 'Save base path:', 'name': 'base_path', 'type': 'browsepath',
-             'value': config['data_saving']['h5file']['save_path']},
-            {'title': 'File name:', 'name': 'target_filename', 'type': 'str', 'value': "", 'readonly': True},
-            {'title': 'Date:', 'name': 'date', 'type': 'date', 'value': QtCore.QDate.currentDate()},
-            {'title': 'Do something, such as showing data:', 'name': 'do_something', 'type': 'bool', 'value': False},
-            {'title': 'Something done:', 'name': 'something_done', 'type': 'led', 'value': False, 'readonly': True},
-            {'title': 'Infos:', 'name': 'info', 'type': 'text', 'value': ""},
-            {'title': 'push:', 'name': 'push', 'type': 'bool_push', 'value': False}
-        ]},
-        {'title': 'Other settings:', 'name': 'other_settings', 'type': 'group', 'children': [
-            {'title': 'List of stuffs:', 'name': 'list_stuff', 'type': 'list', 'value': 'first',
-             'limits': ['first', 'second', 'third'], 'tip': 'choose a stuff from the list'},
-            {'title': 'List of integers:', 'name': 'list_int', 'type': 'list', 'value': 0,
-             'limits': [0, 256, 512], 'tip': 'choose a stuff from this int list'},
-            {'title': 'one integer:', 'name': 'an_integer', 'type': 'int', 'value': 500, },
-            {'title': 'one float:', 'name': 'a_float', 'type': 'float', 'value': 2.7, },
-        ]},
-    ]
-
-    def __init__(self, dockarea, dashboard):
-        super().__init__(dockarea, dashboard)
-        self.setup_ui()
-
-    def connect_things(self):
-        pass
-
-    def setup_docks(self):
-        """
-        to be subclassed to setup the docks layout
-        for instance:
-
-        self.docks['ADock'] = gutils.Dock('ADock name)
-        self.dockarea.addDock(self.docks['ADock"])
-        self.docks['AnotherDock'] = gutils.Dock('AnotherDock name)
-        self.dockarea.addDock(self.docks['AnotherDock"], 'bottom', self.docks['ADock"])
-
-        See Also
-        ########
-        pyqtgraph.dockarea.Dock
-        """
-        self.docks['settings'] = gutils.Dock('Settings')
-        self.dockarea.addDock(self.docks['settings'])
-        self.docks['settings'].addWidget(self.settings_tree)
-
-        self.docks['modmanager'] = gutils.Dock('Module Manager')
-        self.dockarea.addDock(self.docks['modmanager'], 'right', self.docks['settings'])
-        self.docks['modmanager'].addWidget(self.modules_manager.settings_tree)
-
-        self.docks['viewer1D'] = gutils.Dock('Viewers')
-        self.dockarea.addDock(self.docks['viewer1D'], 'right', self.docks['modmanager'])
-
-        self.docks['viewer2D'] = gutils.Dock('Viewers')
-        self.dockarea.addDock(self.docks['viewer2D'], 'bottom', self.docks['viewer1D'])
-
-        widg = QtWidgets.QWidget()
-        self.viewer1D = Viewer1D(widg)
-        self.docks['viewer1D'].addWidget(widg)
-
-        widg1 = QtWidgets.QWidget()
-        self.viewer2D = Viewer2D(widg1)
-        self.docks['viewer2D'].addWidget(widg1)
-
-    def setup_menu(self):
-        '''
-        to be subclassed
-        create menu for actions contained into the self.actions_manager, for instance:
-
-        For instance:
-
-        file_menu = self.menubar.addMenu('File')
-        self.actions_manager.affect_to('load', file_menu)
-        self.actions_manager.affect_to('save', file_menu)
-
-        file_menu.addSeparator()
-        self.actions_manager.affect_to('quit', file_menu)
-        '''
-        pass
-
-    def value_changed(self, param):
-        ''' to be subclassed for actions to perform when one of the param's value in self.settings is changed
-
-        For instance:
-        if param.name() == 'do_something':
-            if param.value():
-                print('Do something')
-                self.settings.child('main_settings', 'something_done').setValue(False)
-
-        Parameters
-        ----------
-        param: (Parameter) the parameter whose value just changed
-        '''
-        if param.name() == 'do_something':
-            if param.value():
-                self.modules_manager.det_done_signal.connect(self.show_data)
-            else:
-                self.modules_manager.det_done_signal.disconnect()
-
-    def param_deleted(self, param):
-        ''' to be subclassed for actions to perform when one of the param in self.settings has been deleted
-
-        Parameters
-        ----------
-        param: (Parameter) the parameter that has been deleted
-        '''
-        raise NotImplementedError
-
-    def child_added(self, param):
-        ''' to be subclassed for actions to perform when a param  has been added in self.settings
-
-        Parameters
-        ----------
-        param: (Parameter) the parameter that has been deleted
-        '''
-        raise NotImplementedError
-
-    def setup_actions(self):
-        pass
-
-    def show_data(self, data_all):
-        data1D = []
-        data2D = []
-        labels1D = []
-        labels2D = []
-        dims = ['data1D', 'data2D']
-        for det in data_all:
-            for dim in dims:
-                if len(data_all[det][dim]) != 0:
-                    for channel in data_all[det][dim]:
-                        if dim == 'data1D':
-                            labels1D.append(channel)
-                            data1D.append(data_all[det][dim][channel]['data'])
-                        else:
-                            labels2D.append(channel)
-                            data2D.append(data_all[det][dim][channel]['data'])
-        self.viewer1D.show_data(data1D)
-        self.viewer2D.setImage(*data2D[:min(3, len(data2D))])
-
-
-
-def main():
-    import sys
-    from pymodaq.dashboard import DashBoard
-    from pathlib import Path
-    app = QtWidgets.QApplication(sys.argv)
-    mainwindow = QtWidgets.QMainWindow()
-    dockarea = gutils.DockArea()
-    mainwindow.setCentralWidget(dockarea)
-
-    #  init the dashboard
-    mainwindow_dash = QtWidgets.QMainWindow()
-    area_dash = gutils.DockArea()
-    mainwindow_dash.setCentralWidget(area_dash)
-    dashboard = DashBoard(area_dash)
-    file = Path(utils.get_set_preset_path()).joinpath(f"{config['presets']['default_preset_for_scan']}.xml")
-    if file.exists():
-        dashboard.set_preset_mode(file)
-    else:
-        msgBox = QtWidgets.QMessageBox()
-        msgBox.setText(f"The default file specified in the configuration file does not exists!\n"
-                       f"{file}\n"
-                       f"Impossible to load the DAQ_Scan Module")
-        msgBox.setStandardButtons(msgBox.Ok)
-        ret = msgBox.exec()
-
-    prog = MyExtension(dockarea, dashboard)
-
-    mainwindow.show()
-    sys.exit(app.exec_())
-
-
-if __name__ == '__main__':
-    main()
-
-
+from pymodaq.utils import gui_utils as gutils
+from pymodaq.utils import daq_utils as utils
+from pyqtgraph.parametertree import Parameter, ParameterTree
+from pymodaq.utils.parameter import pymodaq_ptypes
+from qtpy import QtWidgets, QtCore
+
+from pymodaq.utils.plotting.data_viewers.viewer1D import Viewer1D
+from pymodaq.utils.plotting.data_viewers.viewer2D import Viewer2D
+
+
+config = utils.load_config()
+logger = utils.set_logger(utils.get_module_name(__file__))
+
+EXTENSION_NAME = 'MY_EXTENSION_NAME'
+CLASS_NAME = 'MyExtension'
+
+
+class MyExtension(gutils.CustomApp):
+    # list of dicts enabling the settings tree on the user interface
+    params = [
+        {'title': 'Main settings:', 'name': 'main_settings', 'type': 'group', 'children': [
+            {'title': 'Save base path:', 'name': 'base_path', 'type': 'browsepath',
+             'value': config['data_saving']['h5file']['save_path']},
+            {'title': 'File name:', 'name': 'target_filename', 'type': 'str', 'value': "", 'readonly': True},
+            {'title': 'Date:', 'name': 'date', 'type': 'date', 'value': QtCore.QDate.currentDate()},
+            {'title': 'Do something, such as showing data:', 'name': 'do_something', 'type': 'bool', 'value': False},
+            {'title': 'Something done:', 'name': 'something_done', 'type': 'led', 'value': False, 'readonly': True},
+            {'title': 'Infos:', 'name': 'info', 'type': 'text', 'value': ""},
+            {'title': 'push:', 'name': 'push', 'type': 'bool_push', 'value': False}
+        ]},
+        {'title': 'Other settings:', 'name': 'other_settings', 'type': 'group', 'children': [
+            {'title': 'List of stuffs:', 'name': 'list_stuff', 'type': 'list', 'value': 'first',
+             'limits': ['first', 'second', 'third'], 'tip': 'choose a stuff from the list'},
+            {'title': 'List of integers:', 'name': 'list_int', 'type': 'list', 'value': 0,
+             'limits': [0, 256, 512], 'tip': 'choose a stuff from this int list'},
+            {'title': 'one integer:', 'name': 'an_integer', 'type': 'int', 'value': 500, },
+            {'title': 'one float:', 'name': 'a_float', 'type': 'float', 'value': 2.7, },
+        ]},
+    ]
+
+    def __init__(self, dockarea, dashboard):
+        super().__init__(dockarea, dashboard)
+        self.setup_ui()
+
+    def connect_things(self):
+        pass
+
+    def setup_docks(self):
+        """
+        to be subclassed to setup the docks layout
+        for instance:
+
+        self.docks['ADock'] = gutils.Dock('ADock name)
+        self.dockarea.addDock(self.docks['ADock"])
+        self.docks['AnotherDock'] = gutils.Dock('AnotherDock name)
+        self.dockarea.addDock(self.docks['AnotherDock"], 'bottom', self.docks['ADock"])
+
+        See Also
+        ########
+        pyqtgraph.dockarea.Dock
+        """
+        self.docks['settings'] = gutils.Dock('Settings')
+        self.dockarea.addDock(self.docks['settings'])
+        self.docks['settings'].addWidget(self.settings_tree)
+
+        self.docks['modmanager'] = gutils.Dock('Module Manager')
+        self.dockarea.addDock(self.docks['modmanager'], 'right', self.docks['settings'])
+        self.docks['modmanager'].addWidget(self.modules_manager.settings_tree)
+
+        self.docks['viewer1D'] = gutils.Dock('Viewers')
+        self.dockarea.addDock(self.docks['viewer1D'], 'right', self.docks['modmanager'])
+
+        self.docks['viewer2D'] = gutils.Dock('Viewers')
+        self.dockarea.addDock(self.docks['viewer2D'], 'bottom', self.docks['viewer1D'])
+
+        widg = QtWidgets.QWidget()
+        self.viewer1D = Viewer1D(widg)
+        self.docks['viewer1D'].addWidget(widg)
+
+        widg1 = QtWidgets.QWidget()
+        self.viewer2D = Viewer2D(widg1)
+        self.docks['viewer2D'].addWidget(widg1)
+
+    def setup_menu(self):
+        '''
+        to be subclassed
+        create menu for actions contained into the self.actions_manager, for instance:
+
+        For instance:
+
+        file_menu = self.menubar.addMenu('File')
+        self.actions_manager.affect_to('load', file_menu)
+        self.actions_manager.affect_to('save', file_menu)
+
+        file_menu.addSeparator()
+        self.actions_manager.affect_to('quit', file_menu)
+        '''
+        pass
+
+    def value_changed(self, param):
+        ''' to be subclassed for actions to perform when one of the param's value in self.settings is changed
+
+        For instance:
+        if param.name() == 'do_something':
+            if param.value():
+                print('Do something')
+                self.settings.child('main_settings', 'something_done').setValue(False)
+
+        Parameters
+        ----------
+        param: (Parameter) the parameter whose value just changed
+        '''
+        if param.name() == 'do_something':
+            if param.value():
+                self.modules_manager.det_done_signal.connect(self.show_data)
+            else:
+                self.modules_manager.det_done_signal.disconnect()
+
+    def param_deleted(self, param):
+        ''' to be subclassed for actions to perform when one of the param in self.settings has been deleted
+
+        Parameters
+        ----------
+        param: (Parameter) the parameter that has been deleted
+        '''
+        raise NotImplementedError
+
+    def child_added(self, param):
+        ''' to be subclassed for actions to perform when a param  has been added in self.settings
+
+        Parameters
+        ----------
+        param: (Parameter) the parameter that has been deleted
+        '''
+        raise NotImplementedError
+
+    def setup_actions(self):
+        pass
+
+    def show_data(self, data_all):
+        data1D = []
+        data2D = []
+        labels1D = []
+        labels2D = []
+        dims = ['data1D', 'data2D']
+        for det in data_all:
+            for dim in dims:
+                if len(data_all[det][dim]) != 0:
+                    for channel in data_all[det][dim]:
+                        if dim == 'data1D':
+                            labels1D.append(channel)
+                            data1D.append(data_all[det][dim][channel]['data'])
+                        else:
+                            labels2D.append(channel)
+                            data2D.append(data_all[det][dim][channel]['data'])
+        self.viewer1D.show_data(data1D)
+        self.viewer2D.setImage(*data2D[:min(3, len(data2D))])
+
+
+
+def main():
+    import sys
+    from pymodaq.dashboard import DashBoard
+    from pathlib import Path
+    app = QtWidgets.QApplication(sys.argv)
+    mainwindow = QtWidgets.QMainWindow()
+    dockarea = gutils.DockArea()
+    mainwindow.setCentralWidget(dockarea)
+
+    #  init the dashboard
+    mainwindow_dash = QtWidgets.QMainWindow()
+    area_dash = gutils.DockArea()
+    mainwindow_dash.setCentralWidget(area_dash)
+    dashboard = DashBoard(area_dash)
+    file = Path(utils.get_set_preset_path()).joinpath(f"{config['presets']['default_preset_for_scan']}.xml")
+    if file.exists():
+        dashboard.set_preset_mode(file)
+    else:
+        msgBox = QtWidgets.QMessageBox()
+        msgBox.setText(f"The default file specified in the configuration file does not exists!\n"
+                       f"{file}\n"
+                       f"Impossible to load the DAQ_Scan Module")
+        msgBox.setStandardButtons(msgBox.Ok)
+        ret = msgBox.exec()
+
+    prog = MyExtension(dockarea, dashboard)
+
+    mainwindow.show()
+    sys.exit(app.exec_())
+
+
+if __name__ == '__main__':
+    main()
+
+
```

### Comparing `pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya/models/PIDModelTemplate.py` & `pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya/models/PIDModelTemplate.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-from pymodaq.extensions.pid.utils import PIDModelGeneric, OutputToActuator, InputFromDetector, main
-from pymodaq.utils.data import DataToExport
-from typing import List
-
-
-def some_function_to_convert_the_pid_outputs(outputs: List[float], dt: float, stab=True):
-    """ Should be replaced here or in the model class to process the outputs """
-    return outputs
-
-
-def some_function_to_convert_the_data(measurements: DataToExport):
-    """ Should be replaced here or in the model class to process the measurement """
-    a = 0
-    b = 1
-    return [a, b]
-
-
-class PIDModelTemplate(PIDModelGeneric):
-    limits = dict(max=dict(state=False, value=100),
-                  min=dict(state=False, value=-100),)
-    konstants = dict(kp=0.1, ki=0.000, kd=0.0000)
-
-    Nsetpoints = 2  # number of setpoints
-    setpoint_ini = [128, 128]  # number and values of initial setpoints
-    setpoints_names = ['Xaxis', 'Yaxis']  # number and names of setpoints
-
-    actuators_name = ["Xpiezo", "Ypiezo"]  # names of actuator's control modules involved in the PID
-    detectors_name = ['Camera']  # names of detector's control modules involved in the PID
-
-    params = []  # list of dict to initialize specific Parameters
-
-    def __init__(self, pid_controller):
-        super().__init__(pid_controller)
-
-    def update_settings(self, param):
-        """
-        Get a parameter instance whose value has been modified by a user on the UI
-        Parameters
-        ----------
-        param: (Parameter) instance of Parameter object
-        """
-        if param.name() == '':
-            pass
-
-    def ini_model(self):
-        super().ini_model()
-
-        # add here other specifics initialization if needed
-
-    def convert_input(self, measurements: DataToExport):
-        """
-        Convert the measurements in the units to be fed to the PID (same dimensionality as the setpoint)
-        Parameters
-        ----------
-        measurements: DataToExport
-            Data from the declared detectors from which the model extract a value of the same units as the setpoint
-
-        Returns
-        -------
-        InputFromDetector: the converted input in the setpoints units
-
-        """
-
-        x, y = some_function_to_convert_the_data(measurements)
-        return InputFromDetector([y, x])
-
-    def convert_output(self, outputs: List[float], dt: float, stab=True):
-        """
-        Convert the output of the PID in units to be fed into the actuator
-        Parameters
-        ----------
-        outputs: List of float
-            output value from the PID from which the model extract a value of the same units as the actuator
-        dt: float
-            Ellapsed time since the last call to this function
-        stab: bool
-
-        Returns
-        -------
-        OutputToActuator: the converted output
-
-        """
-        outputs = some_function_to_convert_the_pid_outputs(outputs, dt, stab)
-        return OutputToActuator(mode='rel', values=outputs)
-
-
-if __name__ == '__main__':
-    main("BeamSteeringMockNoModel.xml")  # some preset configured with the right actuators and detectors
-
-
+from pymodaq.extensions.pid.utils import PIDModelGeneric, OutputToActuator, InputFromDetector, main
+from pymodaq.utils.data import DataToExport
+from typing import List
+
+
+def some_function_to_convert_the_pid_outputs(outputs: List[float], dt: float, stab=True):
+    """ Should be replaced here or in the model class to process the outputs """
+    return outputs
+
+
+def some_function_to_convert_the_data(measurements: DataToExport):
+    """ Should be replaced here or in the model class to process the measurement """
+    a = 0
+    b = 1
+    return [a, b]
+
+
+class PIDModelTemplate(PIDModelGeneric):
+    limits = dict(max=dict(state=False, value=100),
+                  min=dict(state=False, value=-100),)
+    konstants = dict(kp=0.1, ki=0.000, kd=0.0000)
+
+    Nsetpoints = 2  # number of setpoints
+    setpoint_ini = [128, 128]  # number and values of initial setpoints
+    setpoints_names = ['Xaxis', 'Yaxis']  # number and names of setpoints
+
+    actuators_name = ["Xpiezo", "Ypiezo"]  # names of actuator's control modules involved in the PID
+    detectors_name = ['Camera']  # names of detector's control modules involved in the PID
+
+    params = []  # list of dict to initialize specific Parameters
+
+    def __init__(self, pid_controller):
+        super().__init__(pid_controller)
+
+    def update_settings(self, param):
+        """
+        Get a parameter instance whose value has been modified by a user on the UI
+        Parameters
+        ----------
+        param: (Parameter) instance of Parameter object
+        """
+        if param.name() == '':
+            pass
+
+    def ini_model(self):
+        super().ini_model()
+
+        # add here other specifics initialization if needed
+
+    def convert_input(self, measurements: DataToExport):
+        """
+        Convert the measurements in the units to be fed to the PID (same dimensionality as the setpoint)
+        Parameters
+        ----------
+        measurements: DataToExport
+            Data from the declared detectors from which the model extract a value of the same units as the setpoint
+
+        Returns
+        -------
+        InputFromDetector: the converted input in the setpoints units
+
+        """
+
+        x, y = some_function_to_convert_the_data(measurements)
+        return InputFromDetector([y, x])
+
+    def convert_output(self, outputs: List[float], dt: float, stab=True):
+        """
+        Convert the output of the PID in units to be fed into the actuator
+        Parameters
+        ----------
+        outputs: List of float
+            output value from the PID from which the model extract a value of the same units as the actuator
+        dt: float
+            Ellapsed time since the last call to this function
+        stab: bool
+
+        Returns
+        -------
+        OutputToActuator: the converted output
+
+        """
+        outputs = some_function_to_convert_the_pid_outputs(outputs, dt, stab)
+        return OutputToActuator(mode='rel', values=outputs)
+
+
+if __name__ == '__main__':
+    main("BeamSteeringMockNoModel.xml")  # some preset configured with the right actuators and detectors
+
+
```

### Comparing `pymodaq_plugins_redpitaya-0.0.2/src/pymodaq_plugins_redpitaya.egg-info/PKG-INFO` & `pymodaq_plugins_redpitaya-0.0.3/src/pymodaq_plugins_redpitaya.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,71 @@
-Metadata-Version: 2.1
-Name: pymodaq-plugins-redpitaya
-Version: 0.0.2
-Summary: PyMoDAQ Plugin to use the Redpitaya electronic board
-Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_redpitaya
-Author: Sebastien J. Weber
-Author-email: sebastien.weber@cemes.fr
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
-Requires-Dist: pymeasure
-
-pymodaq_plugins_redpitaya
-#########################
-
-.. the following must be adapted to your developed package, links to pypi, github  description...
-
-.. image:: https://img.shields.io/pypi/v/pymodaq_plugins_redpitaya.svg
-   :target: https://pypi.org/project/pymodaq_plugins_redpitaya/
-   :alt: Latest Version
-
-.. image:: https://readthedocs.org/projects/pymodaq/badge/?version=latest
-   :target: https://pymodaq.readthedocs.io/en/stable/?badge=latest
-   :alt: Documentation Status
-
-.. image:: https://github.com/PyMoDAQ/pymodaq_plugins_redpitaya/workflows/Upload%20Python%20Package/badge.svg
-   :target: https://github.com/PyMoDAQ/pymodaq_plugins_redpitaya
-   :alt: Publication Status
-
-.. image:: https://github.com/PyMoDAQ/pymodaq_plugins_redpitaya/actions/workflows/Test.yml/badge.svg
-    :target: https://github.com/PyMoDAQ/pymodaq_plugins_redpitaya/actions/workflows/Test.yml
-
-
-PyMoDAQ Plugin to use the Redpitaya electronic board
-
-https://redpitaya.readthedocs.io/en/latest/
-
-
-Authors
-=======
-
-* Sebastien J. Weber  (sebastien.weber@cemes.fr)
-
-Instruments
-===========
-
-Below is the list of instruments included in this plugin
-
-
-Viewer1D
-++++++++
-
-* **RedPitayaSCPI**: perform analog data acquisition using one of the fast channels
-
-
-Installation instructions
-=========================
-
-* PyMoDAQâ€™s version: >= 4.1.0
-* Operating systemâ€™s version: any
-* For the SCPI version, use the driver from the pymeasure package
+Metadata-Version: 2.1
+Name: pymodaq-plugins-redpitaya
+Version: 0.0.3
+Summary: PyMoDAQ Plugin to use the Redpitaya electronic board
+Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_redpitaya
+Author: Sebastien J. Weber
+Author-email: sebastien.weber@cemes.fr
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
+
+pymodaq_plugins_redpitaya
+#########################
+
+.. the following must be adapted to your developed package, links to pypi, github  description...
+
+.. image:: https://img.shields.io/pypi/v/pymodaq_plugins_redpitaya.svg
+   :target: https://pypi.org/project/pymodaq_plugins_redpitaya/
+   :alt: Latest Version
+
+.. image:: https://readthedocs.org/projects/pymodaq/badge/?version=latest
+   :target: https://pymodaq.readthedocs.io/en/stable/?badge=latest
+   :alt: Documentation Status
+
+.. image:: https://github.com/PyMoDAQ/pymodaq_plugins_redpitaya/workflows/Upload%20Python%20Package/badge.svg
+   :target: https://github.com/PyMoDAQ/pymodaq_plugins_redpitaya
+   :alt: Publication Status
+
+.. image:: https://github.com/PyMoDAQ/pymodaq_plugins_redpitaya/actions/workflows/Test.yml/badge.svg
+    :target: https://github.com/PyMoDAQ/pymodaq_plugins_redpitaya/actions/workflows/Test.yml
+
+
+PyMoDAQ Plugin to use the Redpitaya electronic board
+
+https://redpitaya.readthedocs.io/en/latest/
+
+
+Authors
+=======
+
+* Sebastien J. Weber  (sebastien.weber@cemes.fr)
+
+
+Instruments
+===========
+
+Below is the list of instruments included in this plugin
+
+
+Viewer1D
+++++++++
+
+* **RedPitayaSCPI**: perform analog data acquisition using one of the fast channels
+
+
+
+Installation instructions
+=========================
+
+* PyMoDAQ’s version: >= 4.1.0
+* Operating system’s version: any
+* For the SCPI version, use the driver from the pymeasure package
```

