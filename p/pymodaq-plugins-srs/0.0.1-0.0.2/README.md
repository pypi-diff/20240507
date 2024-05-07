# Comparing `tmp/pymodaq_plugins_srs-0.0.1.tar.gz` & `tmp/pymodaq_plugins_srs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugins_srs-0.0.1.tar", last modified: Mon Nov 20 08:28:39 2023, max compression
+gzip compressed data, was "pymodaq_plugins_srs-0.0.2.tar", last modified: Tue May  7 14:12:55 2024, max compression
```

## Comparing `pymodaq_plugins_srs-0.0.1.tar` & `pymodaq_plugins_srs-0.0.2.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-11-20 08:28:39.039556 pymodaq_plugins_srs-0.0.1/
--rw-rw-rw-   0        0        0     1128 2023-11-20 08:22:53.000000 pymodaq_plugins_srs-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       46 2023-11-20 08:22:53.000000 pymodaq_plugins_srs-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3225 2023-11-20 08:28:39.036640 pymodaq_plugins_srs-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2234 2023-11-20 08:26:35.000000 pymodaq_plugins_srs-0.0.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-11-20 08:28:39.039556 pymodaq_plugins_srs-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     3152 2023-11-20 08:22:53.000000 pymodaq_plugins_srs-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-20 08:28:38.912675 pymodaq_plugins_srs-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-11-20 08:28:38.955547 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/
--rw-rw-rw-   0        0        0      281 2023-11-20 08:22:53.000000 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-20 08:28:38.979462 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/daq_move_plugins/
--rw-rw-rw-   0        0        0      467 2023-11-20 08:22:53.000000 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/daq_move_plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-20 08:28:38.982875 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/daq_viewer_plugins/
--rw-rw-rw-   0        0        0        6 2023-11-20 08:22:53.000000 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/daq_viewer_plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-20 08:28:38.988516 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_0D/
--rw-rw-rw-   0        0        0      472 2023-11-20 08:22:54.000000 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_0D/__init__.py
--rw-rw-rw-   0        0        0     9674 2023-11-20 08:22:54.000000 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_LockInSR830.py
-drwxrwxrwx   0        0        0        0 2023-11-20 08:28:38.992525 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_1D/
--rw-rw-rw-   0        0        0      472 2023-11-20 08:22:54.000000 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_1D/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-20 08:28:38.994463 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_2D/
--rw-rw-rw-   0        0        0      474 2023-11-20 08:22:54.000000 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_2D/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-20 08:28:38.999643 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_ND/
--rw-rw-rw-   0        0        0      472 2023-11-20 08:22:54.000000 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_ND/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-20 08:28:39.002556 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/exporters/
--rw-rw-rw-   0        0        0       87 2023-11-20 08:22:54.000000 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/exporters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-20 08:28:39.005674 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/extensions/
--rw-rw-rw-   0        0        0       87 2023-11-20 08:22:54.000000 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/extensions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-20 08:28:39.008853 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/hardware/
--rw-rw-rw-   0        0        0        0 2023-11-20 08:22:54.000000 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/hardware/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-20 08:28:39.016556 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/models/
--rw-rw-rw-   0        0        0     3167 2023-11-20 08:22:54.000000 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/models/PIDModelTemplate.py
--rw-rw-rw-   0        0        0       87 2023-11-20 08:22:54.000000 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-20 08:28:39.026168 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/resources/
--rw-rw-rw-   0        0        0        5 2023-11-20 08:22:54.000000 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/resources/VERSION
--rw-rw-rw-   0        0        0        0 2023-11-20 08:22:54.000000 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/resources/__init__.py
--rw-rw-rw-   0        0        0       49 2023-11-20 08:22:54.000000 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/resources/config_template.toml
-drwxrwxrwx   0        0        0        0 2023-11-20 08:28:39.028805 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/scanners/
--rw-rw-rw-   0        0        0       87 2023-11-20 08:22:54.000000 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/scanners/__init__.py
--rw-rw-rw-   0        0        0      434 2023-11-20 08:22:54.000000 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/utils.py
-drwxrwxrwx   0        0        0        0 2023-11-20 08:28:38.976463 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs.egg-info/
--rw-rw-rw-   0        0        0     3225 2023-11-20 08:28:38.000000 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1305 2023-11-20 08:28:38.000000 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-20 08:28:38.000000 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-11-20 08:28:38.000000 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-11-20 08:28:38.000000 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-11-20 08:28:38.000000 pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-11-20 08:28:39.032590 pymodaq_plugins_srs-0.0.1/tests/
--rw-rw-rw-   0        0        0     3267 2023-11-20 08:22:54.000000 pymodaq_plugins_srs-0.0.1/tests/test_plugin_package_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:12:55.590761 pymodaq_plugins_srs-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-07 14:12:46.000000 pymodaq_plugins_srs-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 14:12:46.000000 pymodaq_plugins_srs-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-07 14:12:55.590761 pymodaq_plugins_srs-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-07 14:12:46.000000 pymodaq_plugins_srs-0.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:12:55.590761 pymodaq_plugins_srs-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-07 14:12:46.000000 pymodaq_plugins_srs-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:12:55.582761 pymodaq_plugins_srs-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:12:55.586761 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-07 14:12:46.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:12:55.586761 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/daq_move_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-07 14:12:46.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/daq_move_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:12:55.586761 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/daq_viewer_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-07 14:12:46.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/daq_viewer_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:12:55.590761 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_0D/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 14:12:46.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_0D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9443 2024-05-07 14:12:46.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_LockInSR830.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7690 2024-05-07 14:12:46.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_SR830.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:12:55.590761 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_1D/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 14:12:46.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_1D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:12:55.590761 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_2D/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-07 14:12:46.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_2D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:12:55.590761 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_ND/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 14:12:46.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_ND/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:12:55.590761 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 14:12:46.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/exporters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:12:55.590761 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 14:12:46.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:12:55.590761 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:12:46.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/hardware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:12:55.590761 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-07 14:12:46.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/models/PIDModelTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 14:12:46.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:12:55.590761 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 14:12:46.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/resources/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:12:46.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-07 14:12:46.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/resources/config_template.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:12:55.590761 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/scanners/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 14:12:46.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/scanners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-07 14:12:46.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:12:55.590761 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-07 14:12:55.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-07 14:12:55.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:12:55.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-07 14:12:55.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 14:12:55.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 14:12:55.000000 pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:12:55.590761 pymodaq_plugins_srs-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-07 14:12:46.000000 pymodaq_plugins_srs-0.0.2/tests/test_plugin_package_structure.py
```

### Comparing `pymodaq_plugins_srs-0.0.1/LICENSE` & `pymodaq_plugins_srs-0.0.2/LICENSE`

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

### Comparing `pymodaq_plugins_srs-0.0.1/setup.py` & `pymodaq_plugins_srs-0.0.2/setup.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-from setuptools import setup, find_packages
-import toml
-
-config = toml.load('./plugin_info.toml')
-SHORT_PLUGIN_NAME = config['plugin-info']['SHORT_PLUGIN_NAME']
-PLUGIN_NAME = f"pymodaq_plugins_{SHORT_PLUGIN_NAME}"
-
-
-from pathlib import Path
-
-if not SHORT_PLUGIN_NAME.isidentifier():
-    raise ValueError("'SHORT_PLUGIN_NAME = %s' is not a valid python identifier." % SHORT_PLUGIN_NAME)
-
-version_file = Path(__file__).parent.joinpath(f'src/{PLUGIN_NAME}/resources/VERSION')  # new location of the version file
-if not version_file.is_file():
-    version_file = Path(__file__).parent.joinpath(f'src/{PLUGIN_NAME}/VERSION')
-
-with open(str(version_file), 'r') as fvers:
-    version = fvers.read().strip()
-
-
-with open('README.rst') as fd:
-    long_description = fd.read()
-
-setupOpts = dict(
-    name=PLUGIN_NAME,
-    description=config['plugin-info']['description'],
-    long_description=long_description,
-    license=config['plugin-info']['license'],
-    url=config['plugin-info']['package-url'],
-    author=config['plugin-info']['author'],
-    author_email=config['plugin-info']['author-email'],
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "Development Status :: 5 - Production/Stable",
-        "Environment :: Other Environment",
-        "Intended Audience :: Science/Research",
-        "Topic :: Scientific/Engineering :: Human Machine Interfaces",
-        "Topic :: Scientific/Engineering :: Visualization",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-        "Topic :: Software Development :: User Interfaces",
-    ], )
-
-#instrument
-#extension = false  # true if plugins contains dashboard extensions
-#pid_models = false  # true if plugins contains pid models
-#h5exporters = false  # true if plugin contains custom h5 file exporters
-#scans
-
-entrypoints = {}
-if 'features' in config:
-    if config['features'].get('instruments', False):
-        entrypoints['pymodaq.instruments'] = f'{SHORT_PLUGIN_NAME} = {PLUGIN_NAME}'
-    if config['features'].get('extensions', False):
-        entrypoints['pymodaq.extensions'] = f'{SHORT_PLUGIN_NAME} = {PLUGIN_NAME}'
-    if config['features'].get('pid_models', False):
-        entrypoints['pymodaq.pid_models'] = f'{SHORT_PLUGIN_NAME} = {PLUGIN_NAME}'
-    if config['features'].get('h5exporters', False):
-        entrypoints['pymodaq.h5exporters'] = f'{SHORT_PLUGIN_NAME} = {PLUGIN_NAME}'
-    if config['features'].get('scanners', False):
-        entrypoints['pymodaq.scanners'] = f'{SHORT_PLUGIN_NAME} = {PLUGIN_NAME}'
-else:
-    entrypoints['pymodaq.instruments'] = f'{SHORT_PLUGIN_NAME} = {PLUGIN_NAME}'
-entrypoints['pymodaq.plugins'] = f'{SHORT_PLUGIN_NAME} = {PLUGIN_NAME}'  # generic plugin, usefull for the plugin manager
-setup(
-    version=version,
-    packages=find_packages(where='./src'),
-    package_dir={'': 'src'},
-    include_package_data=True,
-    entry_points=entrypoints,
-    install_requires=['toml', ]+config['plugin-install']['packages-required'],
-    **setupOpts
-)
+from setuptools import setup, find_packages
+import toml
+
+config = toml.load('./plugin_info.toml')
+SHORT_PLUGIN_NAME = config['plugin-info']['SHORT_PLUGIN_NAME']
+PLUGIN_NAME = f"pymodaq_plugins_{SHORT_PLUGIN_NAME}"
+
+
+from pathlib import Path
+
+if not SHORT_PLUGIN_NAME.isidentifier():
+    raise ValueError("'SHORT_PLUGIN_NAME = %s' is not a valid python identifier." % SHORT_PLUGIN_NAME)
+
+version_file = Path(__file__).parent.joinpath(f'src/{PLUGIN_NAME}/resources/VERSION')  # new location of the version file
+if not version_file.is_file():
+    version_file = Path(__file__).parent.joinpath(f'src/{PLUGIN_NAME}/VERSION')
+
+with open(str(version_file), 'r') as fvers:
+    version = fvers.read().strip()
+
+
+with open('README.rst') as fd:
+    long_description = fd.read()
+
+setupOpts = dict(
+    name=PLUGIN_NAME,
+    description=config['plugin-info']['description'],
+    long_description=long_description,
+    license=config['plugin-info']['license'],
+    url=config['plugin-info']['package-url'],
+    author=config['plugin-info']['author'],
+    author_email=config['plugin-info']['author-email'],
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "Development Status :: 5 - Production/Stable",
+        "Environment :: Other Environment",
+        "Intended Audience :: Science/Research",
+        "Topic :: Scientific/Engineering :: Human Machine Interfaces",
+        "Topic :: Scientific/Engineering :: Visualization",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Topic :: Software Development :: User Interfaces",
+    ], )
+
+#instrument
+#extension = false  # true if plugins contains dashboard extensions
+#pid_models = false  # true if plugins contains pid models
+#h5exporters = false  # true if plugin contains custom h5 file exporters
+#scans
+
+entrypoints = {}
+if 'features' in config:
+    if config['features'].get('instruments', False):
+        entrypoints['pymodaq.instruments'] = f'{SHORT_PLUGIN_NAME} = {PLUGIN_NAME}'
+    if config['features'].get('extensions', False):
+        entrypoints['pymodaq.extensions'] = f'{SHORT_PLUGIN_NAME} = {PLUGIN_NAME}'
+    if config['features'].get('pid_models', False):
+        entrypoints['pymodaq.pid_models'] = f'{SHORT_PLUGIN_NAME} = {PLUGIN_NAME}'
+    if config['features'].get('h5exporters', False):
+        entrypoints['pymodaq.h5exporters'] = f'{SHORT_PLUGIN_NAME} = {PLUGIN_NAME}'
+    if config['features'].get('scanners', False):
+        entrypoints['pymodaq.scanners'] = f'{SHORT_PLUGIN_NAME} = {PLUGIN_NAME}'
+else:
+    entrypoints['pymodaq.instruments'] = f'{SHORT_PLUGIN_NAME} = {PLUGIN_NAME}'
+entrypoints['pymodaq.plugins'] = f'{SHORT_PLUGIN_NAME} = {PLUGIN_NAME}'  # generic plugin, usefull for the plugin manager
+setup(
+    version=version,
+    packages=find_packages(where='./src'),
+    package_dir={'': 'src'},
+    include_package_data=True,
+    entry_points=entrypoints,
+    install_requires=['toml', ]+config['plugin-install']['packages-required'],
+    **setupOpts
+)
```

### Comparing `pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_LockInSR830.py` & `pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_LockInSR830.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,232 +1,232 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Thu Jun 14 15:14:54 2018
-
-@author: Weber Sébastien
-@email: seba.weber@gmail.com
-"""
-from qtpy.QtCore import Signal
-from easydict import EasyDict as edict
-
-from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
-from pymodaq.utils.data import DataFromPlugins
-from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base, main, comon_parameters
-from collections import OrderedDict
-
-import numpy as np
-import re
-
-
-class DAQ_0DViewer_LockInSR830(DAQ_Viewer_base):
-    """
-        ==================== ========================
-        **Attributes**        **Type**
-        *data_grabed_signal*  instance of Signal
-        *VISA_rm*             ResourceManager
-        *com_ports*           
-        *params*              dictionnary list
-        *inst*
-        *settings*
-        ==================== ========================
-    """
-    data_grabed_signal=Signal(list)
-    channels=['X', 'Y', 'MAG', 'PHA', 'Aux In 1', 'Aux In 2', 'Aux In 3', 'Aux In 4', 'Ref frequency', 'CH1 display', 'CH2 display']
-
-    ##checking VISA ressources
-    try:
-        from pyvisa import ResourceManager
-        VISA_rm = ResourceManager()
-        devices = list(VISA_rm.list_resources())
-        device = ''
-        for dev in devices:
-            if 'GPIB' in dev:
-                device = dev
-                break
-    except Exception as e:
-        devices = []
-        device = ''
-        raise e
-
-    params = comon_parameters + [
-        {'title': 'VISA:', 'name': 'VISA_ressources', 'type': 'list', 'limits': devices, 'value': device},
-        {'title': 'Manufacturer:', 'name': 'manufacturer', 'type': 'str', 'value': ""},
-        {'title': 'Serial number:', 'name': 'serial_number', 'type': 'str', 'value': ""},
-        {'title': 'Model:', 'name': 'model', 'type': 'str', 'value': ""},
-        {'title': 'Timeout (ms):', 'name': 'timeout', 'type': 'int', 'value': 2000, 'default': 2000, 'min': 1000},
-        {'title': 'Configuration:', 'name': 'config', 'type': 'group', 'children': [
-            {'title': 'Reset:', 'name': 'reset', 'type': 'bool_push', 'value': False},
-            {'title': 'Channels in separate viewer:', 'name': 'separate_viewers', 'type': 'bool', 'value': True},
-            {'title': 'Channels:', 'name': 'channels', 'type': 'itemselect',
-             'value': dict(all_items=channels, selected=['MAG', 'PHA'])},
-            {'title': 'Setup:', 'name': 'setup', 'type': 'group', 'children': [
-                {'title': 'Setup number:', 'name': 'setup_number', 'type': 'int', 'value': 0},
-                {'title': 'Save setup:', 'name': 'save_setup', 'type': 'bool', 'value': False},
-                {'title': 'Load setup:', 'name': 'load_setup', 'type': 'bool', 'value': False}, ]}
-        ]},
-    ]
-
-    def __init__(self, parent=None, params_state=None):
-        super().__init__(parent, params_state)
-        self.controller = None
-
-    def query_data(self, cmd):
-        try:
-            res = self.controller.query(cmd)
-            searched = re.search('\n', res)
-            status_byte = res[searched.start() + 1]
-            overload_byte = res[searched.start() + 3]
-            if searched.start != 0:
-                data = np.array([float(x) for x in res[0:searched.start()].split(",")])
-            else:
-                data = None
-            return (status_byte, overload_byte, data)
-        except:
-            return ('\x01', '\x00', None)
-
-    def query_string(self, cmd):
-        try:
-            res = self.controller.query(cmd)
-            searched = re.search('\n', res)
-            status_byte = res[searched.start() + 1]
-            overload_byte = res[searched.start() + 3]
-            if searched.start != 0:
-                str = res[0:searched.start()]
-            else:
-                str = ""
-            return (status_byte, overload_byte, str)
-        except:
-            return ('\x01', '\x00', "")
-
-    def ini_detector(self, controller=None):
-        """
-            Initialisation procedure of the detector.
-
-            Returns
-            -------
-
-                The initialized status.
-
-            See Also
-            --------
-            daq_utils.ThreadCommand
-        """
-        self.status.update(edict(initialized=False, info="", x_axis=None, y_axis=None, controller=None))
-        try:
-
-            if self.settings.child(('controller_status')).value() == "Slave":
-                if controller is None:
-                    raise Exception('no controller has been defined externally while this detector is a slave one')
-                else:
-                    self.controller = controller
-            else:
-                self.controller = self.VISA_rm.open_resource(self.settings.child(('VISA_ressources')).value())
-
-            self.controller.timeout = self.settings.child(('timeout')).value()
-            idn = self.controller.query('OUTX1;*IDN?;')
-            idn = idn.rstrip('\n')
-            idn = idn.rsplit(',')
-            if len(idn) >= 0:
-                self.settings.child(('manufacturer')).setValue(idn[0])
-            if len(idn) >= 1:
-                self.settings.child(('model')).setValue(idn[1])
-            if len(idn) >= 2:
-                self.settings.child(('serial_number')).setValue(idn[2])
-
-            # self.reset()
-
-            self.status.controller = self.controller
-            self.status.initialized = True
-            return self.status
-
-        except Exception as e:
-            self.emit_status(ThreadCommand('Update_Status', [getLineInfo() + str(e), 'log']))
-            self.status.info = getLineInfo() + str(e)
-            self.status.initialized = False
-            return self.status
-
-    def reset(self):
-        self.controller.write('*RST')
-
-    def grab_data(self, Naverage=1, **kwargs):
-        """
-            | Start new acquisition.
-            | grab the current values.
-            | Send the data_grabed_signal once done.
-
-            =============== ======== ===============================================
-            **Parameters**  **Type**  **Description**
-            *Naverage*      int       Number of values to average
-            =============== ======== ===============================================
-        """
-        data_tot = []
-        data = self.controller.query_ascii_values('SNAP ? 1,2,3,4,5,6')
-        data.extend(self.controller.query_ascii_values('SNAP ? 7,8,9,10,11'))
-        selected_channels = self.settings.child('config', 'channels').value()['selected']
-        data_to_export = [np.array([data[ind]]) for ind in [self.channels.index(sel) for sel in selected_channels]]
-
-        if self.settings.child('config', 'separate_viewers').value():
-            for ind_channel, dat in enumerate(data_to_export):
-                data_tot.append(DataFromPlugins(name=selected_channels[ind_channel], data=[dat], dim='Data0D',
-                                                labels=[selected_channels[ind_channel]]))
-            self.data_grabed_signal.emit(data_tot)
-        else:
-            self.data_grabed_signal.emit(
-                [DataFromPlugins(name='SR830', data=data_to_export, dim='Data0D', labels=selected_channels)])
-
-    def commit_settings(self, param):
-        """
-            Activate the parameters changes in the hardware.
-
-            =============== ================================= ============================
-            **Parameters**   **Type**                         **Description**
-            *param*         instance of pyqtgraph.parameter   The parameter to be checked.
-            =============== ================================= ============================
-
-            See Also
-            --------
-            daq_utils.ThreadCommand
-        """
-        try:
-            if param.name() == 'timeout':
-                self.controller.timeout = self.settings.child(('timeout')).value()
-
-            if param.name() == 'load_setup':
-                self.controller.write(
-                    'RSET{:d};'.format(self.settings.child('config', 'setup', 'setup_number').value()))
-                param.setValue(False)
-
-            if param.name() == 'save_setup':
-                self.controller.write(
-                    'SSET{:d};'.format(self.settings.child('config', 'setup', 'setup_number').value()))
-                param.setValue(False)
-
-            elif param.name() == 'channels':
-                data_init = []
-                for channel in param.value()['selected']:
-                    if self.settings.child('config', 'separate_viewers').value():
-                        data_init.append(DataFromPlugins(name=channel, data=[np.array([0])], dim='Data0D'))
-                    else:
-                        data_init.append(np.array([0]))
-                if self.settings.child('config', 'separate_viewers').value():
-                    self.data_grabed_signal_temp.emit(data_init)
-                else:
-                    self.data_grabed_signal_temp.emit([DataFromPlugins(name='SR830', data=data_init, dim='Data0D')])
-            elif param.name() == 'reset':
-                self.reset()
-                param.setValue(False)
-
-        except Exception as e:
-            self.emit_status(ThreadCommand('Update_Status', [getLineInfo() + str(e), 'log']))
-
-    def close(self):
-        """
-            close the current instance of the visa session.
-        """
-        self.controller.close()
-
-    def stop(self):
-        pass
-
-
-if __name__ == '__main__':
+# -*- coding: utf-8 -*-
+"""
+Created on Thu Jun 14 15:14:54 2018
+
+@author: Weber Sébastien
+@email: seba.weber@gmail.com
+"""
+from qtpy.QtCore import Signal
+from easydict import EasyDict as edict
+
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
+from pymodaq.utils.data import DataFromPlugins
+from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base, main, comon_parameters
+from collections import OrderedDict
+
+import numpy as np
+import re
+
+
+class DAQ_0DViewer_LockInSR830(DAQ_Viewer_base):
+    """
+        ==================== ========================
+        **Attributes**        **Type**
+        *data_grabed_signal*  instance of Signal
+        *VISA_rm*             ResourceManager
+        *com_ports*           
+        *params*              dictionnary list
+        *inst*
+        *settings*
+        ==================== ========================
+    """
+    data_grabed_signal=Signal(list)
+    channels=['X', 'Y', 'MAG', 'PHA', 'Aux In 1', 'Aux In 2', 'Aux In 3', 'Aux In 4', 'Ref frequency', 'CH1 display', 'CH2 display']
+
+    ##checking VISA ressources
+    try:
+        from pyvisa import ResourceManager
+        VISA_rm = ResourceManager()
+        devices = list(VISA_rm.list_resources())
+        device = ''
+        for dev in devices:
+            if 'GPIB' in dev:
+                device = dev
+                break
+    except Exception as e:
+        devices = []
+        device = ''
+        raise e
+
+    params = comon_parameters + [
+        {'title': 'VISA:', 'name': 'VISA_ressources', 'type': 'list', 'limits': devices, 'value': device},
+        {'title': 'Manufacturer:', 'name': 'manufacturer', 'type': 'str', 'value': ""},
+        {'title': 'Serial number:', 'name': 'serial_number', 'type': 'str', 'value': ""},
+        {'title': 'Model:', 'name': 'model', 'type': 'str', 'value': ""},
+        {'title': 'Timeout (ms):', 'name': 'timeout', 'type': 'int', 'value': 2000, 'default': 2000, 'min': 1000},
+        {'title': 'Configuration:', 'name': 'config', 'type': 'group', 'children': [
+            {'title': 'Reset:', 'name': 'reset', 'type': 'bool_push', 'value': False},
+            {'title': 'Channels in separate viewer:', 'name': 'separate_viewers', 'type': 'bool', 'value': True},
+            {'title': 'Channels:', 'name': 'channels', 'type': 'itemselect',
+             'value': dict(all_items=channels, selected=['MAG', 'PHA'])},
+            {'title': 'Setup:', 'name': 'setup', 'type': 'group', 'children': [
+                {'title': 'Setup number:', 'name': 'setup_number', 'type': 'int', 'value': 0},
+                {'title': 'Save setup:', 'name': 'save_setup', 'type': 'bool', 'value': False},
+                {'title': 'Load setup:', 'name': 'load_setup', 'type': 'bool', 'value': False}, ]}
+        ]},
+    ]
+
+    def __init__(self, parent=None, params_state=None):
+        super().__init__(parent, params_state)
+        self.controller = None
+
+    def query_data(self, cmd):
+        try:
+            res = self.controller.query(cmd)
+            searched = re.search('\n', res)
+            status_byte = res[searched.start() + 1]
+            overload_byte = res[searched.start() + 3]
+            if searched.start != 0:
+                data = np.array([float(x) for x in res[0:searched.start()].split(",")])
+            else:
+                data = None
+            return (status_byte, overload_byte, data)
+        except:
+            return ('\x01', '\x00', None)
+
+    def query_string(self, cmd):
+        try:
+            res = self.controller.query(cmd)
+            searched = re.search('\n', res)
+            status_byte = res[searched.start() + 1]
+            overload_byte = res[searched.start() + 3]
+            if searched.start != 0:
+                str = res[0:searched.start()]
+            else:
+                str = ""
+            return (status_byte, overload_byte, str)
+        except:
+            return ('\x01', '\x00', "")
+
+    def ini_detector(self, controller=None):
+        """
+            Initialisation procedure of the detector.
+
+            Returns
+            -------
+
+                The initialized status.
+
+            See Also
+            --------
+            daq_utils.ThreadCommand
+        """
+        self.status.update(edict(initialized=False, info="", x_axis=None, y_axis=None, controller=None))
+        try:
+
+            if self.settings.child(('controller_status')).value() == "Slave":
+                if controller is None:
+                    raise Exception('no controller has been defined externally while this detector is a slave one')
+                else:
+                    self.controller = controller
+            else:
+                self.controller = self.VISA_rm.open_resource(self.settings.child(('VISA_ressources')).value())
+
+            self.controller.timeout = self.settings.child(('timeout')).value()
+            idn = self.controller.query('OUTX1;*IDN?;')
+            idn = idn.rstrip('\n')
+            idn = idn.rsplit(',')
+            if len(idn) >= 0:
+                self.settings.child(('manufacturer')).setValue(idn[0])
+            if len(idn) >= 1:
+                self.settings.child(('model')).setValue(idn[1])
+            if len(idn) >= 2:
+                self.settings.child(('serial_number')).setValue(idn[2])
+
+            # self.reset()
+
+            self.status.controller = self.controller
+            self.status.initialized = True
+            return self.status
+
+        except Exception as e:
+            self.emit_status(ThreadCommand('Update_Status', [getLineInfo() + str(e), 'log']))
+            self.status.info = getLineInfo() + str(e)
+            self.status.initialized = False
+            return self.status
+
+    def reset(self):
+        self.controller.write('*RST')
+
+    def grab_data(self, Naverage=1, **kwargs):
+        """
+            | Start new acquisition.
+            | grab the current values.
+            | Send the data_grabed_signal once done.
+
+            =============== ======== ===============================================
+            **Parameters**  **Type**  **Description**
+            *Naverage*      int       Number of values to average
+            =============== ======== ===============================================
+        """
+        data_tot = []
+        data = self.controller.query_ascii_values('SNAP ? 1,2,3,4,5,6')
+        data.extend(self.controller.query_ascii_values('SNAP ? 7,8,9,10,11'))
+        selected_channels = self.settings.child('config', 'channels').value()['selected']
+        data_to_export = [np.array([data[ind]]) for ind in [self.channels.index(sel) for sel in selected_channels]]
+
+        if self.settings.child('config', 'separate_viewers').value():
+            for ind_channel, dat in enumerate(data_to_export):
+                data_tot.append(DataFromPlugins(name=selected_channels[ind_channel], data=[dat], dim='Data0D',
+                                                labels=[selected_channels[ind_channel]]))
+            self.data_grabed_signal.emit(data_tot)
+        else:
+            self.data_grabed_signal.emit(
+                [DataFromPlugins(name='SR830', data=data_to_export, dim='Data0D', labels=selected_channels)])
+
+    def commit_settings(self, param):
+        """
+            Activate the parameters changes in the hardware.
+
+            =============== ================================= ============================
+            **Parameters**   **Type**                         **Description**
+            *param*         instance of pyqtgraph.parameter   The parameter to be checked.
+            =============== ================================= ============================
+
+            See Also
+            --------
+            daq_utils.ThreadCommand
+        """
+        try:
+            if param.name() == 'timeout':
+                self.controller.timeout = self.settings.child(('timeout')).value()
+
+            if param.name() == 'load_setup':
+                self.controller.write(
+                    'RSET{:d};'.format(self.settings.child('config', 'setup', 'setup_number').value()))
+                param.setValue(False)
+
+            if param.name() == 'save_setup':
+                self.controller.write(
+                    'SSET{:d};'.format(self.settings.child('config', 'setup', 'setup_number').value()))
+                param.setValue(False)
+
+            elif param.name() == 'channels':
+                data_init = []
+                for channel in param.value()['selected']:
+                    if self.settings.child('config', 'separate_viewers').value():
+                        data_init.append(DataFromPlugins(name=channel, data=[np.array([0])], dim='Data0D'))
+                    else:
+                        data_init.append(np.array([0]))
+                if self.settings.child('config', 'separate_viewers').value():
+                    self.data_grabed_signal_temp.emit(data_init)
+                else:
+                    self.data_grabed_signal_temp.emit([DataFromPlugins(name='SR830', data=data_init, dim='Data0D')])
+            elif param.name() == 'reset':
+                self.reset()
+                param.setValue(False)
+
+        except Exception as e:
+            self.emit_status(ThreadCommand('Update_Status', [getLineInfo() + str(e), 'log']))
+
+    def close(self):
+        """
+            close the current instance of the visa session.
+        """
+        self.controller.close()
+
+    def stop(self):
+        pass
+
+
+if __name__ == '__main__':
     main(__file__, init=False)
```

### Comparing `pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs/models/PIDModelTemplate.py` & `pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs/models/PIDModelTemplate.py`

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

### Comparing `pymodaq_plugins_srs-0.0.1/src/pymodaq_plugins_srs.egg-info/SOURCES.txt` & `pymodaq_plugins_srs-0.0.2/src/pymodaq_plugins_srs.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 src/pymodaq_plugins_srs.egg-info/entry_points.txt
 src/pymodaq_plugins_srs.egg-info/requires.txt
 src/pymodaq_plugins_srs.egg-info/top_level.txt
 src/pymodaq_plugins_srs/daq_move_plugins/__init__.py
 src/pymodaq_plugins_srs/daq_viewer_plugins/__init__.py
 src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_0D/__init__.py
 src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_LockInSR830.py
+src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_SR830.py
 src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_1D/__init__.py
 src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_2D/__init__.py
 src/pymodaq_plugins_srs/daq_viewer_plugins/plugins_ND/__init__.py
 src/pymodaq_plugins_srs/exporters/__init__.py
 src/pymodaq_plugins_srs/extensions/__init__.py
 src/pymodaq_plugins_srs/hardware/__init__.py
 src/pymodaq_plugins_srs/models/PIDModelTemplate.py
```

### Comparing `pymodaq_plugins_srs-0.0.1/tests/test_plugin_package_structure.py` & `pymodaq_plugins_srs-0.0.2/tests/test_plugin_package_structure.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-# -*- coding: utf-8 -*-
-"""
-Created the 17/10/2023
-
-@author: Sebastien Weber
-"""
-import pytest
-from pathlib import Path
-import importlib
-import pkgutil
-
-
-MANDATORY_MOVE_METHODS = ['ini_attributes', 'get_actuator_value', 'close', 'commit_settings',
-                          'ini_stage', 'move_abs', 'move_home', 'move_rel', 'stop_motion']
-MANDATORY_VIEWER_METHODS = ['ini_attributes', 'grab_data', 'close', 'commit_settings',
-                          'ini_detector', ]
-
-
-def get_package_name():
-    here = Path(__file__).parent
-    package_name = here.parent.stem
-    return package_name
-
-
-def get_move_plugins():
-    pkg_name = get_package_name()
-    move_mod = importlib.import_module(f'{pkg_name}.daq_move_plugins')
-
-    plugin_list = [mod for mod in [mod[1] for mod in
-                                   pkgutil.iter_modules([str(move_mod.path.parent)])]
-                   if 'daq_move_' in mod]
-    return plugin_list, move_mod
-
-
-def get_viewer_plugins(dim='0D'):
-    pkg_name = get_package_name()
-    viewer_mod = importlib.import_module(f'{pkg_name}.daq_viewer_plugins.plugins_{dim}')
-
-    plugin_list = [mod for mod in [mod[1] for mod in
-                                   pkgutil.iter_modules([str(viewer_mod.path.parent)])]
-                   if f'daq_{dim}viewer_' in mod]
-    return plugin_list, viewer_mod
-
-
-def test_package_name_ok():
-    assert 'pymodaq_plugins_' in get_package_name()[0:16]
-
-
-def test_imports():
-    pkg_name = get_package_name()
-    mod = importlib.import_module(pkg_name)
-    assert hasattr(mod, 'config')
-    assert hasattr(mod, '__version__')
-    move_mod = importlib.import_module(f'{pkg_name}', 'daq_move_plugins')
-    importlib.import_module(f'{pkg_name}', 'daq_viewer_plugins')
-    importlib.import_module(f'{pkg_name}', 'extensions')
-    importlib.import_module(f'{pkg_name}', 'models')
-    importlib.import_module(f'{pkg_name}.daq_viewer_plugins', 'plugins_0D')
-    importlib.import_module(f'{pkg_name}.daq_viewer_plugins', 'plugins_1D')
-    importlib.import_module(f'{pkg_name}.daq_viewer_plugins', 'plugins_2D')
-    importlib.import_module(f'{pkg_name}.daq_viewer_plugins', 'plugins_ND')
-
-
-def test_move_inst_plugins_name():
-    plugin_list, move_mod = get_move_plugins()
-    for plug in plugin_list:
-        name = plug.split('daq_move_')[1]
-        assert hasattr(getattr(move_mod, plug), f'DAQ_Move_{name}')
-
-
-def test_move_has_mandatory_methods():
-    plugin_list, move_mod = get_move_plugins()
-    for plug in plugin_list:
-        name = plug.split('daq_move_')[1]
-        klass = getattr(getattr(move_mod, plug), f'DAQ_Move_{name}')
-        for meth in MANDATORY_MOVE_METHODS:
-            assert hasattr(klass, meth)
-
-
-@pytest.mark.parametrize('dim', ('0D', '1D', '2D', 'ND'))
-def test_viewer_has_mandatory_methods(dim):
-    plugin_list, mod = get_viewer_plugins(dim)
-    for plug in plugin_list:
-        name = plug.split(f'daq_{dim}viewer_')[1]
-        try:
-            module = importlib.import_module(f'.{plug}', mod.__package__)
-        except Exception:
-            break
-        klass = getattr(module, f'DAQ_{dim}Viewer_{name}')
-        for meth in MANDATORY_VIEWER_METHODS:
-            assert hasattr(klass, meth)
+# -*- coding: utf-8 -*-
+"""
+Created the 17/10/2023
+
+@author: Sebastien Weber
+"""
+import pytest
+from pathlib import Path
+import importlib
+import pkgutil
+
+
+MANDATORY_MOVE_METHODS = ['ini_attributes', 'get_actuator_value', 'close', 'commit_settings',
+                          'ini_stage', 'move_abs', 'move_home', 'move_rel', 'stop_motion']
+MANDATORY_VIEWER_METHODS = ['ini_attributes', 'grab_data', 'close', 'commit_settings',
+                          'ini_detector', ]
+
+
+def get_package_name():
+    here = Path(__file__).parent
+    package_name = here.parent.stem
+    return package_name
+
+
+def get_move_plugins():
+    pkg_name = get_package_name()
+    move_mod = importlib.import_module(f'{pkg_name}.daq_move_plugins')
+
+    plugin_list = [mod for mod in [mod[1] for mod in
+                                   pkgutil.iter_modules([str(move_mod.path.parent)])]
+                   if 'daq_move_' in mod]
+    return plugin_list, move_mod
+
+
+def get_viewer_plugins(dim='0D'):
+    pkg_name = get_package_name()
+    viewer_mod = importlib.import_module(f'{pkg_name}.daq_viewer_plugins.plugins_{dim}')
+
+    plugin_list = [mod for mod in [mod[1] for mod in
+                                   pkgutil.iter_modules([str(viewer_mod.path.parent)])]
+                   if f'daq_{dim}viewer_' in mod]
+    return plugin_list, viewer_mod
+
+
+def test_package_name_ok():
+    assert 'pymodaq_plugins_' in get_package_name()[0:16]
+
+
+def test_imports():
+    pkg_name = get_package_name()
+    mod = importlib.import_module(pkg_name)
+    assert hasattr(mod, 'config')
+    assert hasattr(mod, '__version__')
+    move_mod = importlib.import_module(f'{pkg_name}', 'daq_move_plugins')
+    importlib.import_module(f'{pkg_name}', 'daq_viewer_plugins')
+    importlib.import_module(f'{pkg_name}', 'extensions')
+    importlib.import_module(f'{pkg_name}', 'models')
+    importlib.import_module(f'{pkg_name}.daq_viewer_plugins', 'plugins_0D')
+    importlib.import_module(f'{pkg_name}.daq_viewer_plugins', 'plugins_1D')
+    importlib.import_module(f'{pkg_name}.daq_viewer_plugins', 'plugins_2D')
+    importlib.import_module(f'{pkg_name}.daq_viewer_plugins', 'plugins_ND')
+
+
+def test_move_inst_plugins_name():
+    plugin_list, move_mod = get_move_plugins()
+    for plug in plugin_list:
+        name = plug.split('daq_move_')[1]
+        assert hasattr(getattr(move_mod, plug), f'DAQ_Move_{name}')
+
+
+def test_move_has_mandatory_methods():
+    plugin_list, move_mod = get_move_plugins()
+    for plug in plugin_list:
+        name = plug.split('daq_move_')[1]
+        klass = getattr(getattr(move_mod, plug), f'DAQ_Move_{name}')
+        for meth in MANDATORY_MOVE_METHODS:
+            assert hasattr(klass, meth)
+
+
+@pytest.mark.parametrize('dim', ('0D', '1D', '2D', 'ND'))
+def test_viewer_has_mandatory_methods(dim):
+    plugin_list, mod = get_viewer_plugins(dim)
+    for plug in plugin_list:
+        name = plug.split(f'daq_{dim}viewer_')[1]
+        try:
+            module = importlib.import_module(f'.{plug}', mod.__package__)
+        except Exception:
+            break
+        klass = getattr(module, f'DAQ_{dim}Viewer_{name}')
+        for meth in MANDATORY_VIEWER_METHODS:
+            assert hasattr(klass, meth)
```

