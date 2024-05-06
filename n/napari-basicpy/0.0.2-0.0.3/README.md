# Comparing `tmp/napari_basicpy-0.0.2.tar.gz` & `tmp/napari_basicpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_basicpy-0.0.2.tar", last modified: Fri Jun 24 18:27:07 2022, max compression
+gzip compressed data, was "napari_basicpy-0.0.3.tar", last modified: Mon May  6 23:34:27 2024, max compression
```

## Comparing `napari_basicpy-0.0.2.tar` & `napari_basicpy-0.0.3.tar`

### file list

```diff
@@ -1,45 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 18:27:07.777453 napari_basicpy-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 18:27:07.769453 napari_basicpy-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 18:27:07.773453 napari_basicpy-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2860 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 18:27:07.773453 napari_basicpy-0.0.2/.napari/
--rw-r--r--   0 runner    (1001) docker     (121)     4203 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1484 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3918 2022-06-24 18:27:07.777453 napari_basicpy-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2673 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 18:27:07.773453 napari_basicpy-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 18:27:07.773453 napari_basicpy-0.0.2/resources/
--rw-r--r--   0 runner    (1001) docker     (121)  1244630 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/resources/example.gif
--rw-r--r--   0 runner    (1001) docker     (121)    22358 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/resources/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-06-24 18:27:07.777453 napari_basicpy-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 18:27:07.769453 napari_basicpy-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 18:27:07.777453 napari_basicpy-0.0.2/src/napari_basicpy/
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/src/napari_basicpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 18:27:07.777453 napari_basicpy-0.0.2/src/napari_basicpy/_icons/
--rw-r--r--   0 runner    (1001) docker     (121)    22358 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/src/napari_basicpy/_icons/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)      852 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/src/napari_basicpy/_mock_basic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1789 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/src/napari_basicpy/_sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 18:27:07.777453 napari_basicpy-0.0.2/src/napari_basicpy/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/src/napari_basicpy/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/src/napari_basicpy/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/src/napari_basicpy/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-06-24 18:27:06.000000 napari_basicpy-0.0.2/src/napari_basicpy/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     9338 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/src/napari_basicpy/_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)     2144 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/src/napari_basicpy/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 18:27:07.777453 napari_basicpy-0.0.2/src/napari_basicpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3918 2022-06-24 18:27:06.000000 napari_basicpy-0.0.2/src/napari_basicpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      864 2022-06-24 18:27:07.000000 napari_basicpy-0.0.2/src/napari_basicpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-24 18:27:07.000000 napari_basicpy-0.0.2/src/napari_basicpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-06-24 18:27:07.000000 napari_basicpy-0.0.2/src/napari_basicpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-06-24 18:27:07.000000 napari_basicpy-0.0.2/src/napari_basicpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-06-24 18:27:07.000000 napari_basicpy-0.0.2/src/napari_basicpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-06-24 18:26:56.000000 napari_basicpy-0.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:34:27.826566 napari_basicpy-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:34:27.814566 napari_basicpy-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:34:27.818565 napari_basicpy-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-06 23:34:15.000000 napari_basicpy-0.0.3/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-06 23:34:15.000000 napari_basicpy-0.0.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:34:27.818565 napari_basicpy-0.0.3/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-06 23:34:15.000000 napari_basicpy-0.0.3/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-06 23:34:15.000000 napari_basicpy-0.0.3/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-06 23:34:15.000000 napari_basicpy-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-06 23:34:15.000000 napari_basicpy-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-06 23:34:15.000000 napari_basicpy-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-05-06 23:34:27.826566 napari_basicpy-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-06 23:34:15.000000 napari_basicpy-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-06 23:34:15.000000 napari_basicpy-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:34:27.822565 napari_basicpy-0.0.3/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)  3615389 2024-05-06 23:34:15.000000 napari_basicpy-0.0.3/resources/example.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    22358 2024-05-06 23:34:15.000000 napari_basicpy-0.0.3/resources/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-06 23:34:27.830566 napari_basicpy-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:34:27.814566 napari_basicpy-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:34:27.822565 napari_basicpy-0.0.3/src/napari_basicpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-06 23:34:15.000000 napari_basicpy-0.0.3/src/napari_basicpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:34:27.826566 napari_basicpy-0.0.3/src/napari_basicpy/_icons/
+-rw-r--r--   0 runner    (1001) docker     (127)    22358 2024-05-06 23:34:15.000000 napari_basicpy-0.0.3/src/napari_basicpy/_icons/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-06 23:34:15.000000 napari_basicpy-0.0.3/src/napari_basicpy/_sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:34:27.826566 napari_basicpy-0.0.3/src/napari_basicpy/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:34:15.000000 napari_basicpy-0.0.3/src/napari_basicpy/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-06 23:34:15.000000 napari_basicpy-0.0.3/src/napari_basicpy/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-06 23:34:15.000000 napari_basicpy-0.0.3/src/napari_basicpy/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-06 23:34:27.000000 napari_basicpy-0.0.3/src/napari_basicpy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12490 2024-05-06 23:34:15.000000 napari_basicpy-0.0.3/src/napari_basicpy/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-06 23:34:15.000000 napari_basicpy-0.0.3/src/napari_basicpy/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:34:27.826566 napari_basicpy-0.0.3/src/napari_basicpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-05-06 23:34:27.000000 napari_basicpy-0.0.3/src/napari_basicpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-06 23:34:27.000000 napari_basicpy-0.0.3/src/napari_basicpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 23:34:27.000000 napari_basicpy-0.0.3/src/napari_basicpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-06 23:34:27.000000 napari_basicpy-0.0.3/src/napari_basicpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-06 23:34:27.000000 napari_basicpy-0.0.3/src/napari_basicpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-06 23:34:27.000000 napari_basicpy-0.0.3/src/napari_basicpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-06 23:34:15.000000 napari_basicpy-0.0.3/tox.ini
```

### Comparing `napari_basicpy-0.0.2/.github/workflows/test_and_deploy.yml` & `napari_basicpy-0.0.3/.github/workflows/test_and_deploy.yml`

 * *Files 6% similar despite different names*

```diff
@@ -3,88 +3,89 @@
 
 name: tests
 
 on:
   push:
     branches:
       - main
-      - main
     tags:
       - v[0-9]+.[0-9]+.[0-9]+
       - v[0-9]+.[0-9]+.[0-9]+-dev[0-9]+
   pull_request:
     branches:
       - main
-      - main
   workflow_dispatch:
 
 jobs:
   test:
     name: ${{ matrix.platform }} py${{ matrix.python-version }}
     runs-on: ${{ matrix.platform }}
     strategy:
+      fail-fast: false
       matrix:
-        # platform: [ubuntu-latest, windows-latest, macos-latest]
-        platform: [ubuntu-latest]
-        python-version: [3.8, 3.9, "3.10"]
+        platform: [ubuntu-latest, windows-latest, macos-latest]
+        # python-version: ['3.8', '3.9', '3.10']
+        python-version: ['3.9', '3.10']
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       # these libraries enable testing on Qt on linux
       - uses: tlambert03/setup-qt-libs@v1
 
       # strategy borrowed from vispy for installing opengl libs on windows
       - name: Install Windows OpenGL
         if: runner.os == 'Windows'
         run: |
           git clone --depth 1 https://github.com/pyvista/gl-ci-helpers.git
           powershell gl-ci-helpers/appveyor/install_opengl.ps1
+
       # note: if you need dependencies from conda, considering using
       # setup-miniconda: https://github.com/conda-incubator/setup-miniconda
       # and
       # tox-conda: https://github.com/tox-dev/tox-conda
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install setuptools tox tox-gh-actions
+
       # this runs the platform-specific tests declared in tox.ini
       - name: Test with tox
-        uses: GabrielBB/xvfb-action@v1
+        uses: aganders3/headless-gui@v1
         with:
           run: python -m tox
         env:
           PLATFORM: ${{ matrix.platform }}
 
       - name: Coverage
-        uses: codecov/codecov-action@v2
+        uses: codecov/codecov-action@v3
 
   deploy:
     # this will run when you have tagged a commit, starting with "v*"
     # and requires that you have put your twine API key in your
     # github secrets (see readme for details)
     needs: [test]
     runs-on: ubuntu-latest
     if: contains(github.ref, 'tags')
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: "3.x"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install -U setuptools setuptools_scm wheel twine
+          pip install -U setuptools setuptools_scm wheel twine build
       - name: Build and publish
         env:
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.TWINE_API_KEY }}
         run: |
           git tag
-          python setup.py sdist bdist_wheel
+          python -m build .
           twine upload dist/*
```

### Comparing `napari_basicpy-0.0.2/.gitignore` & `napari_basicpy-0.0.3/.gitignore`

 * *Files 14% similar despite different names*

```diff
@@ -80,7 +80,9 @@
 # OS
 .DS_Store
 
 # written by setuptools_scm
 **/_version.py
 
 scratch/
+
+cov.xml
```

### Comparing `napari_basicpy-0.0.2/.pre-commit-config.yaml` & `napari_basicpy-0.0.3/.pre-commit-config.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,27 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.0.1
+    rev: v4.2.0
     hooks:
       - id: check-docstring-first
       - id: end-of-file-fixer
       - id: trailing-whitespace
-  - repo: https://github.com/asottile/setup-cfg-fmt
-    rev: v1.20.0
+        exclude: ^\.napari-hub/.*
+      - id: check-yaml # checks for correct yaml syntax for github actions ex.
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: v0.0.256
     hooks:
-      - id: setup-cfg-fmt
-  - repo: https://github.com/PyCQA/flake8
-    rev: 4.0.1
-    hooks:
-      - id: flake8
-        additional_dependencies: [flake8-typing-imports==1.7.0]
-  - repo: https://github.com/myint/autoflake
-    rev: v1.4
-    hooks:
-      - id: autoflake
-        args: ["--in-place", "--remove-all-unused-imports"]
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
-    hooks:
-      - id: isort
+      - id: ruff
   - repo: https://github.com/psf/black
     rev: 22.3.0
     hooks:
       - id: black
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v2.29.1
-    hooks:
-      - id: pyupgrade
-        args: [--py37-plus, --keep-runtime-typing]
   - repo: https://github.com/tlambert03/napari-plugin-checks
-    rev: v0.2.0
+    rev: v0.3.0
     hooks:
       - id: napari-plugin-checks
-  - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.910-1
-    hooks:
-      - id: mypy
+  # https://mypy.readthedocs.io/en/stable/introduction.html
+  # you may wish to add this as well!
+  # - repo: https://github.com/pre-commit/mirrors-mypy
+  #   rev: v0.910-1
+  #   hooks:
+  #     - id: mypy
```

### Comparing `napari_basicpy-0.0.2/LICENSE` & `napari_basicpy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_basicpy-0.0.2/resources/logo.png` & `napari_basicpy-0.0.3/resources/logo.png`

 * *Files identical despite different names*

### Comparing `napari_basicpy-0.0.2/src/napari_basicpy/_icons/logo.png` & `napari_basicpy-0.0.3/src/napari_basicpy/_icons/logo.png`

 * *Files identical despite different names*

### Comparing `napari_basicpy-0.0.2/src/napari_basicpy/_sample_data.py` & `napari_basicpy-0.0.3/src/napari_basicpy/_sample_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, List
 
-import basicpy.data
+import basicpy.datasets
 import numpy as np
 
 if TYPE_CHECKING:
     import napari
 
 # TODO logging?
 
@@ -31,29 +31,29 @@
     images = np.moveaxis(images, -1, 0)
     images = 255 - images
 
     return [(images, {"name": "Random"}, "image")]
 
 
 def make_sample_data_cell_culture() -> List[napari.types.LayerData]:
-    data = basicpy.data.cell_culture()
+    data = basicpy.datasets.cell_culture()
     return [(data, {"name": "Cell Culture"}, "image")]
 
 
 def make_sample_data_timelapse_brightfield() -> List[napari.types.LayerData]:
-    data = basicpy.data.timelapse_brightfield()
+    data = basicpy.datasets.timelapse_brightfield()
     return [(data, {"name": "Timelapse Brightfield"}, "image")]
 
 
 def make_sample_data_timelapse_nanog() -> List[napari.types.LayerData]:
-    data = basicpy.data.timelapse_nanog()
+    data = basicpy.datasets.timelapse_nanog()
     return [(data, {"name": "Timelapse Nanog"}, "image")]
 
 
 def make_sample_data_timelapse_pu1() -> List[napari.types.LayerData]:
-    data = basicpy.data.timelapse_pu1()
+    data = basicpy.datasets.timelapse_pu1()
     return [(data, {"name": "Timelapse Pu1"}, "image")]
 
 
 def make_sample_data_wsi_brain():
-    data = basicpy.data.wsi_brain()
+    data = basicpy.datasets.wsi_brain()
     return [(data, {"name": "WSI Brain"}, "image")]
```

### Comparing `napari_basicpy-0.0.2/src/napari_basicpy/_tests/test_sample_data.py` & `napari_basicpy-0.0.3/src/napari_basicpy/_tests/test_sample_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Test sample data."""
 
-
 def test_data(make_napari_viewer):
     samples = [
         "sample_data_random",
         "sample_data_cell_culture",
         "sample_data_timelapse_brightfield",
         "sample_data_timelapse_nanog",
         "sample_data_timelapse_pu1",
```

### Comparing `napari_basicpy-0.0.2/src/napari_basicpy/_tests/test_widget.py` & `napari_basicpy-0.0.3/src/napari_basicpy/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_basicpy-0.0.2/src/napari_basicpy/napari.yaml` & `napari_basicpy-0.0.3/src/napari_basicpy/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari_basicpy-0.0.2/src/napari_basicpy.egg-info/PKG-INFO` & `napari_basicpy-0.0.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,100 +1,87 @@
-Metadata-Version: 2.1
-Name: napari-basicpy
-Version: 0.0.2
-Summary: BaSiCPy illumination correction for napari
-Home-page: https://github.com/tdmorello/napari-basicpy
-Author: Tim Morello
-Author-email: tdmorello@gmail.com
-License: BSD-3-Clause
-Project-URL: Bug Tracker, https://github.com/tdmorello/napari-basicpy/issues
-Project-URL: Documentation, https://github.com/tdmorello/napari-basicpy#README.md
-Project-URL: Source Code, https://github.com/tdmorello/napari-basicpy
-Project-URL: User Support, https://github.com/tdmorello/napari-basicpy/issues
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # napari-basicpy
 
 [![License](https://img.shields.io/pypi/l/napari-basicpy.svg?color=green)](https://github.com/tdmorello/napari-basicpy/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-basicpy.svg?color=green)](https://pypi.org/project/napari-basicpy)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-basicpy.svg?color=green)](https://python.org)
 [![tests](https://github.com/tdmorello/napari-basicpy/workflows/tests/badge.svg)](https://github.com/tdmorello/napari-basicpy/actions)
 [![codecov](https://codecov.io/gh/tdmorello/napari-basicpy/branch/main/graph/badge.svg)](https://codecov.io/gh/tdmorello/napari-basicpy)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-basicpy)](https://napari-hub.org/plugins/napari-basicpy)
 
-BaSiCPy illumination correction for napari
+BaSiCPy illumination correction for [napari]
 
-Example:
+## Example
 
 ![example](resources/example.gif)
 
 ----------------------------------
 
-This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
+## Installation
 
-<!--
-Don't miss the full getting started guide to set up your new package:
-https://github.com/napari/cookiecutter-napari-plugin#getting-started
-
-and review the napari docs for plugin developers:
-https://napari.org/plugins/stable/index.html
--->
+### Recommended Installation Method
 
-## Installation
+We highly recommend using a `conda` virtual environment to install and operate this plugin.
+
+To use Python 3.9, for example:
+
+    conda create -n basicpy -c conda-forge python=3.9 napari pyqt && \
+    conda activate basicpy && \
+    pip install napari-basicpy
+
+For further instructions on installing `napari`, visit their [install guide](https://napari.org/stable/tutorials/fundamentals/installation).
+
+---
+
+**IMPORTANT NOTE FOR APPLE SILICON AND WINDOWS USERS:**
+
+If the above instructions fail with Apple silicon (e.g., M1/M2 chip) or Windows, you may need to install the `jax` and `jaxlib` following the instruction [here](https://github.com/peng-lab/BaSiCPy#installation).
 
-You can install `napari-basicpy` via [pip]:
+---
+
+### Other Installation Methods
+
+You can also install `napari-basicpy` via [pip]:
 
     pip install napari-basicpy
 
 
+To install latest development version:
+
+    pip install git+https://github.com/peng-lab/napari-basicpy.git
 
-To install latest development version :
+or
 
     pip install git+https://github.com/tdmorello/napari-basicpy.git
 
+## Usage
+
+### General Usage
+
+This plugin expects a stack of tiles as input. Mosaic images should be deconstructed into their tiled components before processing. Individual tiles should be two-dimensional.
+
+There are many options to customize the performance of BaSiCPy. Please refer to the BaSiCPy documentation on parameters [here](https://basicpy.readthedocs.io/en/latest/api.html#basicpy.basicpy.BaSiC) for details.
+
+### Batch Processing
+
+Coming soon...
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
 
 Distributed under the terms of the [BSD-3] license,
 "napari-basicpy" is free and open source software
 
 ## Issues
 
-If you encounter any problems, please [file an issue] along with a detailed description.
+If you encounter any problems, please [file an issue](https://github.com/peng-lab/napari-basicpy/issues) along with a detailed description.
 
 [napari]: https://github.com/napari/napari
-[Cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
-[MIT]: http://opensource.org/licenses/MIT
 [BSD-3]: http://opensource.org/licenses/BSD-3-Clause
-[GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
-[GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
-[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
-[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
-[cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
 
-[file an issue]: https://github.com/tdmorello/napari-basicpy/issues
-
-[napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
```

### Comparing `napari_basicpy-0.0.2/src/napari_basicpy.egg-info/SOURCES.txt` & `napari_basicpy-0.0.3/src/napari_basicpy.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,21 @@
-.flake8
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 MANIFEST.in
 README.md
-mkdocs.yml
 pyproject.toml
-requirements.txt
 setup.cfg
-setup.py
 tox.ini
 .github/workflows/test_and_deploy.yml
-.napari/DESCRIPTION.md
-docs/index.md
+.napari-hub/DESCRIPTION.md
+.napari-hub/config.yml
 resources/example.gif
 resources/logo.png
 src/napari_basicpy/__init__.py
-src/napari_basicpy/_mock_basic.py
 src/napari_basicpy/_sample_data.py
 src/napari_basicpy/_version.py
 src/napari_basicpy/_widget.py
 src/napari_basicpy/napari.yaml
 src/napari_basicpy.egg-info/PKG-INFO
 src/napari_basicpy.egg-info/SOURCES.txt
 src/napari_basicpy.egg-info/dependency_links.txt
```

