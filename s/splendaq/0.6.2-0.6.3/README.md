# Comparing `tmp/splendaq-0.6.2.tar.gz` & `tmp/splendaq-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splendaq-0.6.2.tar", last modified: Wed Apr 10 18:58:52 2024, max compression
+gzip compressed data, was "splendaq-0.6.3.tar", last modified: Tue May  7 18:27:48 2024, max compression
```

## Comparing `splendaq-0.6.2.tar` & `splendaq-0.6.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.896850 splendaq-0.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.884850 splendaq-0.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.888850 splendaq-0.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-10 18:58:47.000000 splendaq-0.6.2/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-10 18:58:47.000000 splendaq-0.6.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-10 18:58:47.000000 splendaq-0.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-10 18:58:47.000000 splendaq-0.6.2/CITATION.bib
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-10 18:58:47.000000 splendaq-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-10 18:58:47.000000 splendaq-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-10 18:58:52.896850 splendaq-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-10 18:58:47.000000 splendaq-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-10 18:58:47.000000 splendaq-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-10 18:58:52.896850 splendaq-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-10 18:58:47.000000 splendaq-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.884850 splendaq-0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.888850 splendaq-0.6.2/src/splendaq/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-10 18:58:52.000000 splendaq-0.6.2/src/splendaq/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.888850 splendaq-0.6.2/src/splendaq/control/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/control/_hps.py
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/control/_sr560.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.892850 splendaq-0.6.2/src/splendaq/daq/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/daq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19827 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/daq/_log_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    25592 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/daq/_offline_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/daq/_oscilloscope.py
--rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/daq/_sequencer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.892850 splendaq-0.6.2/src/splendaq/io/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/io/_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.892850 splendaq-0.6.2/src/splendaq/io/_liconvert/
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/io/_liconvert/COPYING.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)   716536 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/io/_liconvert/liconvert_linux
--rwxr-xr-x   0 runner    (1001) docker     (127)   629104 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/io/_liconvert/liconvert_macos
--rw-r--r--   0 runner    (1001) docker     (127)   689928 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/io/_liconvert/liconvert_windows.exe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.896850 splendaq-0.6.2/src/splendaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-10 18:58:52.000000 splendaq-0.6.2/src/splendaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-10 18:58:52.000000 splendaq-0.6.2/src/splendaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 18:58:52.000000 splendaq-0.6.2/src/splendaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 18:58:52.000000 splendaq-0.6.2/src/splendaq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 18:58:52.000000 splendaq-0.6.2/src/splendaq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 18:58:52.000000 splendaq-0.6.2/src/splendaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 18:58:52.000000 splendaq-0.6.2/src/splendaq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.884850 splendaq-0.6.2/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.896850 splendaq-0.6.2/tutorials/daq/
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-10 18:58:47.000000 splendaq-0.6.2/tutorials/daq/dc_oscilloscope.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12596 2024-04-10 18:58:47.000000 splendaq-0.6.2/tutorials/daq/event_building.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-10 18:58:47.000000 splendaq-0.6.2/tutorials/daq/logging_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-04-10 18:58:47.000000 splendaq-0.6.2/tutorials/daq/running_the_sequencer.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-10 18:58:47.000000 splendaq-0.6.2/tutorials/daq/sequencer_settings.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.896850 splendaq-0.6.2/tutorials/io/
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-10 18:58:47.000000 splendaq-0.6.2/tutorials/io/read_files.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-04-10 18:58:47.000000 splendaq-0.6.2/tutorials/io/write_files.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:27:48.568452 splendaq-0.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:27:48.556451 splendaq-0.6.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:27:48.560452 splendaq-0.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-07 18:27:43.000000 splendaq-0.6.3/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-07 18:27:43.000000 splendaq-0.6.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-07 18:27:43.000000 splendaq-0.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 18:27:43.000000 splendaq-0.6.3/CITATION.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-07 18:27:43.000000 splendaq-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-07 18:27:43.000000 splendaq-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-07 18:27:48.568452 splendaq-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-07 18:27:43.000000 splendaq-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-07 18:27:43.000000 splendaq-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-07 18:27:48.568452 splendaq-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-07 18:27:43.000000 splendaq-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:27:48.556451 splendaq-0.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:27:48.560452 splendaq-0.6.3/src/splendaq/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-07 18:27:43.000000 splendaq-0.6.3/src/splendaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-07 18:27:43.000000 splendaq-0.6.3/src/splendaq/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 18:27:48.000000 splendaq-0.6.3/src/splendaq/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:27:48.560452 splendaq-0.6.3/src/splendaq/control/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 18:27:43.000000 splendaq-0.6.3/src/splendaq/control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-07 18:27:43.000000 splendaq-0.6.3/src/splendaq/control/_hps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-05-07 18:27:43.000000 splendaq-0.6.3/src/splendaq/control/_sr560.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:27:48.564452 splendaq-0.6.3/src/splendaq/daq/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-07 18:27:43.000000 splendaq-0.6.3/src/splendaq/daq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19750 2024-05-07 18:27:43.000000 splendaq-0.6.3/src/splendaq/daq/_log_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25592 2024-05-07 18:27:43.000000 splendaq-0.6.3/src/splendaq/daq/_offline_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-05-07 18:27:43.000000 splendaq-0.6.3/src/splendaq/daq/_oscilloscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-05-07 18:27:43.000000 splendaq-0.6.3/src/splendaq/daq/_sequencer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:27:48.564452 splendaq-0.6.3/src/splendaq/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 18:27:43.000000 splendaq-0.6.3/src/splendaq/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-05-07 18:27:43.000000 splendaq-0.6.3/src/splendaq/io/_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:27:48.564452 splendaq-0.6.3/src/splendaq/io/_liconvert/
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-07 18:27:43.000000 splendaq-0.6.3/src/splendaq/io/_liconvert/COPYING.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)   716536 2024-05-07 18:27:43.000000 splendaq-0.6.3/src/splendaq/io/_liconvert/liconvert_linux
+-rwxr-xr-x   0 runner    (1001) docker     (127)   629104 2024-05-07 18:27:43.000000 splendaq-0.6.3/src/splendaq/io/_liconvert/liconvert_macos
+-rw-r--r--   0 runner    (1001) docker     (127)   689928 2024-05-07 18:27:43.000000 splendaq-0.6.3/src/splendaq/io/_liconvert/liconvert_windows.exe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:27:48.568452 splendaq-0.6.3/src/splendaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-07 18:27:48.000000 splendaq-0.6.3/src/splendaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-07 18:27:48.000000 splendaq-0.6.3/src/splendaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:27:48.000000 splendaq-0.6.3/src/splendaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-07 18:27:48.000000 splendaq-0.6.3/src/splendaq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:27:48.000000 splendaq-0.6.3/src/splendaq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-07 18:27:48.000000 splendaq-0.6.3/src/splendaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 18:27:48.000000 splendaq-0.6.3/src/splendaq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:27:48.556451 splendaq-0.6.3/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:27:48.568452 splendaq-0.6.3/tutorials/daq/
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-05-07 18:27:43.000000 splendaq-0.6.3/tutorials/daq/dc_oscilloscope.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12596 2024-05-07 18:27:43.000000 splendaq-0.6.3/tutorials/daq/event_building.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-05-07 18:27:43.000000 splendaq-0.6.3/tutorials/daq/logging_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-05-07 18:27:43.000000 splendaq-0.6.3/tutorials/daq/running_the_sequencer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-07 18:27:43.000000 splendaq-0.6.3/tutorials/daq/sequencer_settings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:27:48.568452 splendaq-0.6.3/tutorials/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-05-07 18:27:43.000000 splendaq-0.6.3/tutorials/io/read_files.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-05-07 18:27:43.000000 splendaq-0.6.3/tutorials/io/write_files.ipynb
```

### Comparing `splendaq-0.6.2/.github/workflows/python-package.yml` & `splendaq-0.6.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.2/.github/workflows/python-publish.yml` & `splendaq-0.6.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.2/.gitignore` & `splendaq-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.2/LICENSE` & `splendaq-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.2/PKG-INFO` & `splendaq-0.6.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: splendaq
-Version: 0.6.2
+Version: 0.6.3
 Summary: Generalized offline data acquisition with a focus on the Moku
 Home-page: https://github.com/splendor-collab/splendaq
 Author: SPLENDOR Collaboration
 Maintainer: SPLENDOR Collaboration
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: matplotlib
-Requires-Dist: moku>=3.0.0
+Requires-Dist: moku>=3.2.0
 Requires-Dist: h5py
 Requires-Dist: pyyaml
 Requires-Dist: pyserial
 
 # `splendaq`
 
 [![Python package](https://github.com/splendor-collab/splendaq/actions/workflows/python-package.yml/badge.svg)](https://github.com/splendor-collab/splendaq/actions/workflows/python-package.yml) [![PyPI](https://img.shields.io/pypi/v/splendaq)](https://pypi.org/project/splendaq/) [![Python 3.6](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/) [![GitHub](https://img.shields.io/github/license/splendor-collab/splendaq)](https://github.com/splendor-collab/splendaq/blob/main/LICENSE) [![arXiv](https://img.shields.io/badge/arXiv-2310.01279-<COLOR>.svg)](https://arxiv.org/abs/2310.01279)
```

### Comparing `splendaq-0.6.2/README.md` & `splendaq-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.2/setup.cfg` & `splendaq-0.6.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 [options]
 packages = find:
 install_requires = 
 	numpy
 	scipy
 	matplotlib
-	moku>=3.0.0
+	moku>=3.2.0
 	h5py
 	pyyaml
 	pyserial
 python_requires = >=3.6
 include_package_data = True
 package_dir = 
 	= src
```

### Comparing `splendaq-0.6.2/src/splendaq/_cli.py` & `splendaq-0.6.3/src/splendaq/_cli.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.2/src/splendaq/control/_hps.py` & `splendaq-0.6.3/src/splendaq/control/_hps.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.2/src/splendaq/control/_sr560.py` & `splendaq-0.6.3/src/splendaq/control/_sr560.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.2/src/splendaq/daq/_log_data.py` & `splendaq-0.6.3/src/splendaq/daq/_log_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,16 +97,16 @@
 
         if self._device == "Moku:Pro":
             chan_list = [1, 2, 3, 4]
         elif self._device in ["Moku:Lab", "Moku:Go"]:
             chan_list = [1, 2]
 
         for chan in chan_list:
+            self.DL.enable_input(chan, False) # disable inputs
             self.DL.generate_waveform(chan, 'Off') # disable outputs
-            self.DL.disable_channel(chan) # disable inputs
 
         self.DL.relinquish_ownership()
 
     def set_input_channels(self, channels, impedance="1MOhm", coupling="DC",
                            vrange=None):
         """
         Set which channels to save data from and which settings to use.
@@ -160,15 +160,15 @@
             coupling = [coupling] * len(channels)
         if np.isscalar(vrange):
             vrange = [vrange] * len(channels)
 
         disable_chans = [chan not in channels for chan in chan_list]
         for chan, disable in zip(chan_list, disable_chans):
             if disable:
-                self.DL.disable_channel(chan)
+                self.DL.enable_input(chan, False)
             else:
                 ind = channels.index(chan)
                 self.DL.set_frontend(
                     channel=chan,
                     impedance=impedance[ind],
                     coupling=coupling[ind],
                     range=vrange[ind],
@@ -401,15 +401,15 @@
 
         """
 
         return {
             'dc_level': dc_level,
         }
 
-    def set_output_channel(self, channel, waveformtype, load="1MOhm",
+    def set_output_channel(self, channel, waveformtype, load="HiZ",
                            **settings):
         """
         Method to turn on an output channel and generate the speicified
         waveform. Use the various self.*_settings() methods to
         generate the various valid settings. Can only set one channel
         at a time.
 
@@ -419,27 +419,27 @@
             The output channel to generate a waveform on. With a
             Moku:Pro, this must be an integer of 1, 2, 3 or 4. With a
             Moku:Go or Moku:Lab, this must be an integer of 1 or 2.
         waveformtype : str
             The waveform type to generate, must be one of 'Sine',
             'Square', 'Ramp', 'Pulse', 'DC'. Can also be set to 'Off'
             to turn the channel off.
-        load : str, optional
-            The load impedance to use for the output channel. For a
-            Moku:Pro or Moku:Lab, this must be one of '1MOhm' or
-            '50Ohm'. For a Moku:Go, this can only be '1MOhm'. Default
-            is '1MOhm'.
+        termination : str, optional
+            The waveform termination to use for the output channel.
+            For a Moku:Pro or Moku:Lab, this must be one of 'HiZ' or
+            '50Ohm'. For a Moku:Go, this can only be 'HiZ'. Default
+            is 'HiZ'.
         settings : dict
             The dictionary containing all of the settings needed for
             the specified waveform type.
 
         """
 
         if self._device in ["Moku:Pro", "Moku:Lab"]:
-            self.DL.set_output_load(channel, load)
+            self.DL.set_output_termination(channel, load)
         self.DL.generate_waveform(
             channel,
             waveformtype,
             **settings,
         )
 
 
@@ -485,20 +485,17 @@
             )
             # Track progress percentage of the data logging session
             is_logging = True
             while is_logging:
                 # Wait for the logging session to progress by sleeping 0.5sec
                 time.sleep(0.5)
                 # Get current progress percentage and check if it's complete
-                try:
-                    progress = self.DL.logging_progress()
-                    remaining_time = progress['time_remaining']
-                    is_logging = remaining_time >= 0
-                except:
-                    is_logging = False
+                progress = self.DL.logging_progress()
+                remaining_time = progress['time_remaining']
+                is_logging = remaining_time > 0
 
             filenames.append(logfile['file_name'])
 
         if self._device == "Moku:Pro":
             target = "ssd"
         elif self._device == "Moku:Lab":
             target = "media"
```

### Comparing `splendaq-0.6.2/src/splendaq/daq/_offline_trigger.py` & `splendaq-0.6.3/src/splendaq/daq/_offline_trigger.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.2/src/splendaq/daq/_oscilloscope.py` & `splendaq-0.6.3/src/splendaq/daq/_oscilloscope.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.2/src/splendaq/daq/_sequencer.py` & `splendaq-0.6.3/src/splendaq/daq/_sequencer.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.2/src/splendaq/io/_io.py` & `splendaq-0.6.3/src/splendaq/io/_io.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.2/src/splendaq/io/_liconvert/COPYING.txt` & `splendaq-0.6.3/src/splendaq/io/_liconvert/COPYING.txt`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.2/src/splendaq/io/_liconvert/liconvert_linux` & `splendaq-0.6.3/src/splendaq/io/_liconvert/liconvert_linux`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.2/src/splendaq/io/_liconvert/liconvert_macos` & `splendaq-0.6.3/src/splendaq/io/_liconvert/liconvert_macos`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.2/src/splendaq/io/_liconvert/liconvert_windows.exe` & `splendaq-0.6.3/src/splendaq/io/_liconvert/liconvert_windows.exe`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.2/src/splendaq.egg-info/PKG-INFO` & `splendaq-0.6.3/src/splendaq.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: splendaq
-Version: 0.6.2
+Version: 0.6.3
 Summary: Generalized offline data acquisition with a focus on the Moku
 Home-page: https://github.com/splendor-collab/splendaq
 Author: SPLENDOR Collaboration
 Maintainer: SPLENDOR Collaboration
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: matplotlib
-Requires-Dist: moku>=3.0.0
+Requires-Dist: moku>=3.2.0
 Requires-Dist: h5py
 Requires-Dist: pyyaml
 Requires-Dist: pyserial
 
 # `splendaq`
 
 [![Python package](https://github.com/splendor-collab/splendaq/actions/workflows/python-package.yml/badge.svg)](https://github.com/splendor-collab/splendaq/actions/workflows/python-package.yml) [![PyPI](https://img.shields.io/pypi/v/splendaq)](https://pypi.org/project/splendaq/) [![Python 3.6](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/) [![GitHub](https://img.shields.io/github/license/splendor-collab/splendaq)](https://github.com/splendor-collab/splendaq/blob/main/LICENSE) [![arXiv](https://img.shields.io/badge/arXiv-2310.01279-<COLOR>.svg)](https://arxiv.org/abs/2310.01279)
```

### Comparing `splendaq-0.6.2/src/splendaq.egg-info/SOURCES.txt` & `splendaq-0.6.3/src/splendaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.2/tutorials/daq/dc_oscilloscope.ipynb` & `splendaq-0.6.3/tutorials/daq/dc_oscilloscope.ipynb`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.2/tutorials/daq/event_building.ipynb` & `splendaq-0.6.3/tutorials/daq/event_building.ipynb`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.2/tutorials/daq/logging_data.ipynb` & `splendaq-0.6.3/tutorials/daq/logging_data.ipynb`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.2/tutorials/daq/running_the_sequencer.ipynb` & `splendaq-0.6.3/tutorials/daq/running_the_sequencer.ipynb`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.2/tutorials/daq/sequencer_settings.yaml` & `splendaq-0.6.3/tutorials/daq/sequencer_settings.yaml`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.2/tutorials/io/read_files.ipynb` & `splendaq-0.6.3/tutorials/io/read_files.ipynb`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.2/tutorials/io/write_files.ipynb` & `splendaq-0.6.3/tutorials/io/write_files.ipynb`

 * *Files identical despite different names*

