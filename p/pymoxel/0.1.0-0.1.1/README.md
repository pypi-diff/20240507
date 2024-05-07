# Comparing `tmp/pymoxel-0.1.0.tar.gz` & `tmp/pymoxel-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymoxel-0.1.0.tar", last modified: Wed May  1 15:41:42 2024, max compression
+gzip compressed data, was "pymoxel-0.1.1.tar", last modified: Tue May  7 11:14:41 2024, max compression
```

## Comparing `pymoxel-0.1.0.tar` & `pymoxel-0.1.1.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:42.903982 pymoxel-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:42.887982 pymoxel-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:42.891982 pymoxel-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-01 15:41:38.000000 pymoxel-0.1.0/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-01 15:41:38.000000 pymoxel-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-01 15:41:38.000000 pymoxel-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 15:41:38.000000 pymoxel-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-01 15:41:42.903982 pymoxel-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-01 15:41:38.000000 pymoxel-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:42.891982 pymoxel-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:42.891982 pymoxel-0.1.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:42.891982 pymoxel-0.1.0/docs/source/down/
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/down/CIFs.zip
--rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/down/IRMOF-1.cif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:42.895982 pymoxel-0.1.0/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (127)   101913 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/images/moxel_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)  1955651 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/images/moxel_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   423802 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/images/plot_voxels.png
--rw-r--r--   0 runner    (1001) docker     (127)   347027 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/images/voxels.gif
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/moxel.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-01 15:41:38.000000 pymoxel-0.1.0/docs/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-01 15:41:38.000000 pymoxel-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 15:41:42.903982 pymoxel-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:42.891982 pymoxel-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:42.899982 pymoxel-0.1.0/src/moxel/
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-01 15:41:38.000000 pymoxel-0.1.0/src/moxel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-01 15:41:38.000000 pymoxel-0.1.0/src/moxel/_params.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-01 15:41:38.000000 pymoxel-0.1.0/src/moxel/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    15346 2024-05-01 15:41:38.000000 pymoxel-0.1.0/src/moxel/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-01 15:41:38.000000 pymoxel-0.1.0/src/moxel/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:42.903982 pymoxel-0.1.0/src/pymoxel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-01 15:41:42.000000 pymoxel-0.1.0/src/pymoxel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-01 15:41:42.000000 pymoxel-0.1.0/src/pymoxel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 15:41:42.000000 pymoxel-0.1.0/src/pymoxel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-01 15:41:42.000000 pymoxel-0.1.0/src/pymoxel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 15:41:42.000000 pymoxel-0.1.0/src/pymoxel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 15:41:42.000000 pymoxel-0.1.0/src/pymoxel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:42.899982 pymoxel-0.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:42.903982 pymoxel-0.1.0/tests/CIFs/
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-01 15:41:38.000000 pymoxel-0.1.0/tests/CIFs/COF-5.cif
--rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-05-01 15:41:38.000000 pymoxel-0.1.0/tests/CIFs/IRMOF-1.cif
--rw-r--r--   0 runner    (1001) docker     (127)    32325 2024-05-01 15:41:38.000000 pymoxel-0.1.0/tests/CIFs/ZIF-69.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-01 15:41:38.000000 pymoxel-0.1.0/tests/CIFs/ZnHBDC.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-01 15:41:38.000000 pymoxel-0.1.0/tests/CIFs/ZnMOF-74.cif
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:38.000000 pymoxel-0.1.0/tests/CIFs/corrupted_1.cif
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:38.000000 pymoxel-0.1.0/tests/CIFs/corrupted_2.cif
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:38.000000 pymoxel-0.1.0/tests/CIFs/corrupted_3.cif
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:38.000000 pymoxel-0.1.0/tests/CIFs/corrupted_4.cif
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:41:38.000000 pymoxel-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-01 15:41:38.000000 pymoxel-0.1.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-05-01 15:41:38.000000 pymoxel-0.1.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:41.766997 pymoxel-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:41.750997 pymoxel-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:41.754997 pymoxel-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-07 11:14:37.000000 pymoxel-0.1.1/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-07 11:14:37.000000 pymoxel-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-07 11:14:37.000000 pymoxel-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-07 11:14:37.000000 pymoxel-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-07 11:14:41.766997 pymoxel-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-07 11:14:37.000000 pymoxel-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:41.754997 pymoxel-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:41.754997 pymoxel-0.1.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:41.754997 pymoxel-0.1.1/docs/source/down/
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/down/CIFs.zip
+-rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/down/IRMOF-1.cif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:41.758997 pymoxel-0.1.1/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   101913 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/images/moxel_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1955651 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/images/moxel_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   423802 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/images/plot_voxels.png
+-rw-r--r--   0 runner    (1001) docker     (127)   347027 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/images/voxels.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/moxel.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-07 11:14:37.000000 pymoxel-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 11:14:41.766997 pymoxel-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:41.750997 pymoxel-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:41.762997 pymoxel-0.1.1/src/moxel/
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-07 11:14:37.000000 pymoxel-0.1.1/src/moxel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-07 11:14:37.000000 pymoxel-0.1.1/src/moxel/_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-07 11:14:37.000000 pymoxel-0.1.1/src/moxel/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16380 2024-05-07 11:14:37.000000 pymoxel-0.1.1/src/moxel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-07 11:14:37.000000 pymoxel-0.1.1/src/moxel/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:41.766997 pymoxel-0.1.1/src/pymoxel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-07 11:14:41.000000 pymoxel-0.1.1/src/pymoxel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-07 11:14:41.000000 pymoxel-0.1.1/src/pymoxel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 11:14:41.000000 pymoxel-0.1.1/src/pymoxel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-07 11:14:41.000000 pymoxel-0.1.1/src/pymoxel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 11:14:41.000000 pymoxel-0.1.1/src/pymoxel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 11:14:41.000000 pymoxel-0.1.1/src/pymoxel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:41.762997 pymoxel-0.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:41.766997 pymoxel-0.1.1/tests/CIFs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/CIFs/COF-5.cif
+-rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/CIFs/IRMOF-1.cif
+-rw-r--r--   0 runner    (1001) docker     (127)   113146 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/CIFs/MnH28C26(N2Cl)2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    32325 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/CIFs/ZIF-69.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/CIFs/ZnHBDC.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/CIFs/ZnMOF-74.cif
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/CIFs/corrupted_1.cif
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/CIFs/corrupted_2.cif
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/CIFs/corrupted_3.cif
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/CIFs/corrupted_4.cif
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/test_visualize.py
```

### Comparing `pymoxel-0.1.0/.github/workflows/python-publish.yaml` & `pymoxel-0.1.1/.github/workflows/python-publish.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-name: Publish Python 🐍 distribution 📦 to PyPI and TestPyPI
+name: Publish Python 🐍 distribution 📦 to PyPI
 
 on: push
 
 jobs:
   build:
     name: Build distribution 📦
+    if: startsWith(github.ref, 'refs/tags/')  # only build on tag pushes
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
@@ -24,16 +25,15 @@
     - name: Store the distribution packages
       uses: actions/upload-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
 
   publish-to-pypi:
-    name: >-
-      Publish Python 🐍 distribution 📦 to PyPI
+    name: Publish Python 🐍 distribution 📦 to PyPI
     if: startsWith(github.ref, 'refs/tags/')  # only publish to PyPI on tag pushes
     needs:
     - build
     runs-on: ubuntu-latest
     environment:
       name: pypi
       url: https://pypi.org/p/pymoxel  # Replace <package-name> with your PyPI project name
```

### Comparing `pymoxel-0.1.0/.readthedocs.yaml` & `pymoxel-0.1.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.0/LICENSE` & `pymoxel-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.0/PKG-INFO` & `pymoxel-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymoxel
-Version: 0.1.0
+Version: 0.1.1
 Summary: Package for parallel calculation of energy voxels.
 Author-email: "Antonios P. Sarikas" <antonios.sarikas@gmail.com>
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/adosar/moxel
 Project-URL: Documentation, https://moxel.readthedocs.io
 Project-URL: Changelog, https://moxel.readthedocs.io/en/stable/changes.html
 Classifier: Programming Language :: Python :: 3
@@ -72,17 +72,18 @@
     url = {http://dx.doi.org/10.1038/s41598-023-50309-8},
     DOI = {10.1038/s41598-023-50309-8},
     number = {1},
     journal = {Scientific Reports},
     publisher = {Springer Science and Business Media LLC},
     author = {Sarikas,  Antonios P. and Gkagkas,  Konstantinos and Froudakis,  George E.},
     year = {2024},
-    month = jan 
+    month = jan
     }
 
 ## 📇 TODO
-* Improve modeling of interactions
-* Improve voxelization scheme
-* Improve performance
+1. CLI for training [RetNet](https://www.nature.com/articles/s41598-023-50309-8).
+2. Improve performance
+3. Improve voxelization scheme
+4. Improve modeling of interactions
 
 ## 📑 License
 MOXελ is released under the [GNU General Public License v3.0 only](https://spdx.org/licenses/GPL-3.0-only.html).
```

### Comparing `pymoxel-0.1.0/README.md` & `pymoxel-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,17 +50,18 @@
     url = {http://dx.doi.org/10.1038/s41598-023-50309-8},
     DOI = {10.1038/s41598-023-50309-8},
     number = {1},
     journal = {Scientific Reports},
     publisher = {Springer Science and Business Media LLC},
     author = {Sarikas,  Antonios P. and Gkagkas,  Konstantinos and Froudakis,  George E.},
     year = {2024},
-    month = jan 
+    month = jan
     }
 
 ## 📇 TODO
-* Improve modeling of interactions
-* Improve voxelization scheme
-* Improve performance
+1. CLI for training [RetNet](https://www.nature.com/articles/s41598-023-50309-8).
+2. Improve performance
+3. Improve voxelization scheme
+4. Improve modeling of interactions
 
 ## 📑 License
 MOXελ is released under the [GNU General Public License v3.0 only](https://spdx.org/licenses/GPL-3.0-only.html).
```

### Comparing `pymoxel-0.1.0/docs/Makefile` & `pymoxel-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.0/docs/make.bat` & `pymoxel-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.0/docs/source/down/CIFs.zip` & `pymoxel-0.1.1/docs/source/down/CIFs.zip`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.0/docs/source/down/IRMOF-1.cif` & `pymoxel-0.1.1/docs/source/down/IRMOF-1.cif`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.0/docs/source/images/moxel_logo.png` & `pymoxel-0.1.1/docs/source/images/moxel_logo.png`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.0/docs/source/images/moxel_logo.svg` & `pymoxel-0.1.1/docs/source/images/moxel_logo.svg`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.0/docs/source/images/plot_voxels.png` & `pymoxel-0.1.1/docs/source/images/plot_voxels.png`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.0/docs/source/images/voxels.gif` & `pymoxel-0.1.1/docs/source/images/voxels.gif`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.0/docs/source/index.rst` & `pymoxel-0.1.1/docs/source/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -71,16 +71,16 @@
     year = {2024},
     month = jan 
     }
 
 TODO
 ----
 
-1. Improve performance
-2. CLI for training `RetNet <https://www.nature.com/articles/s41598-023-50309-8>`_
+1. CLI for training `RetNet <https://www.nature.com/articles/s41598-023-50309-8>`_
+2. Improve performance
 3. Improve voxelization scheme
 4. Improve modeling of interactions
 
 License
 -------
 MOXελ is released under the `GNU General Public License v3.0 only <https://spdx.org/licenses/GPL-3.0-only.html>`_.
```

### Comparing `pymoxel-0.1.0/docs/source/tutorial.rst` & `pymoxel-0.1.1/docs/source/tutorial.rst`

 * *Files 11% similar despite different names*

```diff
@@ -43,14 +43,28 @@
 * :func:`moxel.utils.voxels_from_files`
 * :func:`moxel.utils.voxels_from_dir`
 
 In all cases, :func:`moxel.utils.Grid.calculate` is used under the hood to calculate the
 voxels (all other functions are just wrappers). To better understand how to use
 them: :ref:`documentation`.
 
+.. attention::
+    Consider playing with the ``n_jobs`` parameter to get the best performance
+    for your system::
+
+        from timeit import timeit
+
+        setup = 'from moxel.utils import voxels_from_file'
+        n_jobs = [1, 2, 8, 16]  # Modify this according to your system.
+
+        for n in n_jobs:
+            stmt = f'voxels_from_file("path/to/cif", n_jobs={n})'
+            time = timeit(stmt=stmt, setup=setup, number=1)
+            print(f'Time with {n} jobs: {time:.3f} s')
+
 Visualization
 ^^^^^^^^^^^^^
 
 .. code-block::
 
    >>> from moxel.visualize import plot_voxels_mpl
    >>> import matplotlib.pyplot as plt
```

### Comparing `pymoxel-0.1.0/pyproject.toml` & `pymoxel-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.0/src/moxel/__init__.py` & `pymoxel-0.1.1/src/moxel/__init__.py`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.0/src/moxel/_params.py` & `pymoxel-0.1.1/src/moxel/_params.py`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.0/src/moxel/cli.py` & `pymoxel-0.1.1/src/moxel/cli.py`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.0/src/moxel/utils.py` & `pymoxel-0.1.1/src/moxel/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,28 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 r"""
 This module provides helper functions for creating voxels.
 
 .. note::
     Currently, interactions are modelled with the Lennard-Jones (LJ) potential.
+
+.. attention::
+    Consider playing with the ``n_jobs`` parameter to get the best performance
+    for your system::
+
+        from timeit import timeit
+
+        setup = 'from moxel.utils import voxels_from_file'
+        n_jobs = [1, 2, 8, 16]  # Modify this according to your system.
+
+        for n in n_jobs:
+            stmt = f'voxels_from_file("path/to/cif", n_jobs={n})'
+            time = timeit(stmt=stmt, setup=setup, number=1)
+            print(f'Time with {n} jobs: {time:.3f} s')
 """
 
 import os
 import json
 import itertools
 from pathlib import Path
 from multiprocessing import Pool
@@ -113,25 +127,26 @@
     """
     def __init__(self, grid_size=25, cutoff=10, epsilon=50, sigma=2.5):
         self.grid_size = grid_size
         self.cutoff = cutoff
         self.epsilon = epsilon
         self.sigma = sigma
 
-    def load_structure(self, cif_pathname):
+    def load_structure(self, pathname):
         r"""
-        Load a crystal structure from a ``.cif`` file.
+        Load a crystal structure from a file in a format supported by
+        :meth:`pymatgen.core.Structure.from_file`.
 
         Parameters
         ----------
-        cif_pathname : str
-           Pathname to the ``.cif`` file.
+        pathname : str
+           Pathname to the file.
         """
-        self.structure = Structure.from_file(cif_pathname)
-        self.structure_name = Path(cif_pathname).stem
+        self.structure = Structure.from_file(pathname)
+        self.structure_name = Path(pathname).stem
 
     def calculate(self, cubic_box=False, length=30, potential='lj', n_jobs=None):
         r"""
         Iterate over the grid and return voxels.
 
         For computational efficiency and to assure (approximately) the same
         spatial resolution, the grid is overlayed over a supercell scaled
@@ -174,14 +189,20 @@
             self._simulation_box = self.structure
         else:
             probe_coords = np.linspace(0, 1, self.grid_size)  # Fractional.
             scale = mic_scale_factors(self.cutoff, self.structure.lattice.matrix)
             self._simulation_box = self.structure * scale
         
         if potential == 'lj':
+            # Cache LJ parameters for all atoms in the simulation box.
+            self._lj_params = np.array([lj_params[atom.species_string] for atom in self._simulation_box])
+
+            # Cache fractional coordinates since this is a slow function in pymatgen.
+            self._frac_coords = self._simulation_box.frac_coords
+
             # Embarrassingly parallel.
             with Pool(processes=n_jobs) as p:
                 energies = p.map(
                         self.lj_potential, itertools.product(*(probe_coords,)*3)
                         )
 
         self.voxels = np.array(energies, dtype=np.float32).reshape((self.grid_size,)*3)
@@ -201,29 +222,36 @@
         Returns
         -------
         energy : float
             Energy as :math:`e^{-\beta \mathcal{V}}`, to ensure numerical stability.
         """
         if self.cubic_box:
             cartesian_coords = coords
-            neighbors = self._simulation_box.get_sites_in_sphere(cartesian_coords, self.cutoff)
         else:
             cartesian_coords = self._simulation_box.lattice.get_cartesian_coords(coords)
-            neighbors = self._simulation_box.get_sites_in_sphere(cartesian_coords, self.cutoff)
 
-        energy = 0
-        if len(neighbors) != 0:
-            for atom in neighbors:
-                r_ij = np.linalg.norm(cartesian_coords - atom.coords)
-                if r_ij <= 1e-3:
-                    energy += 1000
-                else:
-                    e_j, s_j = lj_params[atom.species_string]
-                    x = (0.5 * (s_j + self.sigma)) / r_ij
-                    energy += 4 * np.sqrt(e_j * self.epsilon) * (x**12 - x**6)
+        _, r_ij, indices, _ = self._simulation_box._lattice.get_points_in_sphere(
+                self._frac_coords, cartesian_coords,
+                self.cutoff, zip_results=False,
+                )
+
+        '''
+        Need to check for length of r_ij because of
+        https://github.com/materialsproject/pymatgen/issues/3794
+        '''
+        if len(r_ij) == 0:  # No neighbor, zero energy.
+            return 1.
+
+        if np.any(r_ij < 1e-3):  # Close contact, infinite energy.
+            return 0.
+
+        es_j = self._lj_params[indices]
+        x = (0.5 * (es_j[:, 1] + self.sigma)) / r_ij
+        e = 4 * np.sqrt(es_j[:, 0] * self.epsilon)
+        energy = sum(e * (x**12 - x**6))
 
         # This should be changed with clipping in future versions.
         return np.exp(-(1 / 298) * energy)  # For numerical stability.
 
 
 def voxels_from_file(
         cif_pathname, grid_size=25, cutoff=10,
@@ -290,16 +318,16 @@
 
     After processing the following files are created::
 
         out_pathname
             ├──voxels.npy
             └──names.json
 
-    The file ``names.json`` stores the names of the materials, which might be
-    useful for later indexing.
+    The file ``names.json`` stores the names of the materials as a
+    :class:`list`, which might be useful for later indexing.
 
     Parameters
     ----------
     cif_pathnames : list
        List of pathnames to the ``.cif`` files.
     out_pathname : str
         Pathname to the directory under which voxels are stored.
@@ -312,16 +340,17 @@
     sigma : float, default=25
         Sigma value (σ/Å) of the probe atom.
     cubic_box : bool, default=False
         If ``True``, the simulation box is cubic.
     length : float, default=30
         The size of the cubic box in Å. Takes effect only if ``cubic_box == True``.
     n_jobs : int, optional
-        Number of jobs to run in parallel. If ``None``, all processors are used.
-    
+        Number of jobs to run in parallel. If ``None``, then the number returned
+        by ``os.cpu_count()`` is used.
+
     Notes
     -----
     * Samples in output array follow the order in ``cif_pathnames``.
     * For structures that can not be processsed, their voxels are filled with zeros.
     """
     n_samples = len(cif_pathnames)
     names = [Path(i).stem for i in cif_pathnames]
@@ -363,16 +392,16 @@
 
     After processing the following files are created::
 
         out_pathname
             ├──voxels.npy
             └──names.json
 
-    The file ``names.json`` stores the names of the materials, which might be
-    useful for later indexing.
+    The file ``names.json`` stores the names of the materials as a
+    :class:`list`, which might be useful for later indexing.
 
     Parameters
     ----------
     cif_dirname : str
        Pathname to the directory containing the ``.cif`` files.
     out_pathname : str
         Pathname to the directory under which voxels are stored.
@@ -385,15 +414,16 @@
     sigma : float, default=25
         Sigma value (σ/Å) of the probe atom.
     cubic_box : bool, default=False
         If ``True``, the simulation box is cubic.
     length : float, default=30
         The size of the cubic box in Å. Takes effect only if ``cubic_box == True``.
     n_jobs : int, optional
-        Number of jobs to run in parallel. If ``None``, all processors are used.
+        Number of jobs to run in parallel. If ``None``, then the number returned
+        by ``os.cpu_count()`` is used.
 
     Notes
     -----
     * Samples in output array follow the order in ``sorted(os.listdir(cif_dirname))``.
     * For structures that can not be processsed, their voxels are filled with zeros.
     """
     files = [os.path.join(cif_dirname, f) for f in sorted(os.listdir(cif_dirname))]
```

### Comparing `pymoxel-0.1.0/src/moxel/visualize.py` & `pymoxel-0.1.1/src/moxel/visualize.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 .. tip::
     For faster rendering you should prefer :func:`plot_voxels_pv`.
 """
 
 import numpy as np
 import pyvista as pv
 import matplotlib as mpl
+import matplotlib.pyplot as plt
 
 
 def plot_voxels_mpl(voxels, *, fill_pattern=None, colorbar=True, cmap='viridis', **kwargs):
     r"""
     Visualize voxels with `Axes3d.voxels`_.
 
     .. _Axes3d.voxels: https://matplotlib.org/stable/api/_as_gen/mpl_toolkits.mplot3d.axes3d.Axes3D.voxels.html#mpl_toolkits.mplot3d.axes3d.Axes3D.voxels
@@ -54,29 +55,31 @@
 
     Returns
     -------
     fig : `Figure <https://matplotlib.org/stable/api/figure_api.html#matplotlib.figure.Figure>`_
 
     Examples
     --------
+    >>> voxels = np.random.randn(5, 5, 5)
     >>> fig = plot_voxels_mpl(voxels, cmap='coolwarm')
+    >>> plt.show()  # Not needed for Jupyter.
     """
 
     if np.all(fill_pattern) == None:
         fill_pattern = np.full(voxels.shape, True)
 
     cmap = plt.get_cmap(cmap)
     norm = mpl.colors.Normalize()
     colors = cmap((voxels - voxels.min()) / (voxels.max() - voxels.min()))
 
     fig, ax = plt.subplots(subplot_kw={'projection': '3d'})
     _ = ax.voxels(filled=fill_pattern, facecolors=colors, **kwargs)
 
     if colorbar:
-        mappable = mpl.cm.ScalarMappable(norm=mpl.colors.Normalize(), cmap=cmap) 
+        mappable = mpl.cm.ScalarMappable(norm=norm, cmap=cmap)
         cbar = fig.colorbar(
             mappable, ax=ax, ticks=[], extend='max',
             shrink=0.7, pad=0.1,
             )
         cbar.ax.set_ylabel(r'$e^{-\beta \mathcal{V}}$', fontsize=12)
     
     return fig
@@ -95,12 +98,13 @@
     ----------
     voxels : 3D array
     **kwargs : dict, optional
         Valid keyword arguments for `Plotter.add_volume`_.
 
     Examples
     --------
+    >>> voxels = np.random.randn(5, 5, 5)
     >>> plot_voxels_pv(voxels, cmap='coolwarm')
     """
     pl = pv.Plotter()
     pl.add_volume(voxels, **kwargs)
     pl.show()
```

### Comparing `pymoxel-0.1.0/src/pymoxel.egg-info/PKG-INFO` & `pymoxel-0.1.1/src/pymoxel.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymoxel
-Version: 0.1.0
+Version: 0.1.1
 Summary: Package for parallel calculation of energy voxels.
 Author-email: "Antonios P. Sarikas" <antonios.sarikas@gmail.com>
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/adosar/moxel
 Project-URL: Documentation, https://moxel.readthedocs.io
 Project-URL: Changelog, https://moxel.readthedocs.io/en/stable/changes.html
 Classifier: Programming Language :: Python :: 3
@@ -72,17 +72,18 @@
     url = {http://dx.doi.org/10.1038/s41598-023-50309-8},
     DOI = {10.1038/s41598-023-50309-8},
     number = {1},
     journal = {Scientific Reports},
     publisher = {Springer Science and Business Media LLC},
     author = {Sarikas,  Antonios P. and Gkagkas,  Konstantinos and Froudakis,  George E.},
     year = {2024},
-    month = jan 
+    month = jan
     }
 
 ## 📇 TODO
-* Improve modeling of interactions
-* Improve voxelization scheme
-* Improve performance
+1. CLI for training [RetNet](https://www.nature.com/articles/s41598-023-50309-8).
+2. Improve performance
+3. Improve voxelization scheme
+4. Improve modeling of interactions
 
 ## 📑 License
 MOXελ is released under the [GNU General Public License v3.0 only](https://spdx.org/licenses/GPL-3.0-only.html).
```

### Comparing `pymoxel-0.1.0/src/pymoxel.egg-info/SOURCES.txt` & `pymoxel-0.1.1/src/pymoxel.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -29,18 +29,19 @@
 src/pymoxel.egg-info/PKG-INFO
 src/pymoxel.egg-info/SOURCES.txt
 src/pymoxel.egg-info/dependency_links.txt
 src/pymoxel.egg-info/entry_points.txt
 src/pymoxel.egg-info/requires.txt
 src/pymoxel.egg-info/top_level.txt
 tests/__init__.py
-tests/test_cli.py
 tests/test_utils.py
+tests/test_visualize.py
 tests/CIFs/COF-5.cif
 tests/CIFs/IRMOF-1.cif
+tests/CIFs/MnH28C26(N2Cl)2.json
 tests/CIFs/ZIF-69.cif
 tests/CIFs/ZnHBDC.cif
 tests/CIFs/ZnMOF-74.cif
 tests/CIFs/corrupted_1.cif
 tests/CIFs/corrupted_2.cif
 tests/CIFs/corrupted_3.cif
 tests/CIFs/corrupted_4.cif
```

### Comparing `pymoxel-0.1.0/tests/CIFs/COF-5.cif` & `pymoxel-0.1.1/tests/CIFs/COF-5.cif`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.0/tests/CIFs/IRMOF-1.cif` & `pymoxel-0.1.1/tests/CIFs/IRMOF-1.cif`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.0/tests/CIFs/ZIF-69.cif` & `pymoxel-0.1.1/tests/CIFs/ZIF-69.cif`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.0/tests/CIFs/ZnHBDC.cif` & `pymoxel-0.1.1/tests/CIFs/ZnHBDC.cif`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.0/tests/CIFs/ZnMOF-74.cif` & `pymoxel-0.1.1/tests/CIFs/ZnMOF-74.cif`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.0/tests/test_utils.py` & `pymoxel-0.1.1/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -155,10 +155,19 @@
 
             # Check that the voxels have been cleaned.
             self.assertTrue(np.all(voxels[filled_idx] == clean_voxels))
 
             # Check that the names have been correctly stored.
             self.assertEqual([names[i] for i in filled_idx], clean_names)
 
+    def test_load_file(self):
+        cif_dir = 'tests/CIFs'
+
+        grid = Grid()
+        grid.load_structure(f'{cif_dir}/IRMOF-1.cif')
+
+        grid = Grid()
+        grid.load_structure(f'{cif_dir}/MnH28C26(N2Cl)2.json')
+
 
 if __name__ == '__main__':
     unittest.main()
```

