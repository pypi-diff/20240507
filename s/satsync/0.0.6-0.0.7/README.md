# Comparing `tmp/satsync-0.0.6.tar.gz` & `tmp/satsync-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsync-0.0.6.tar", max compression
+gzip compressed data, was "satsync-0.0.7.tar", max compression
```

## Comparing `satsync-0.0.6.tar` & `satsync-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1070 2024-05-05 16:14:00.568999 satsync-0.0.6/LICENSE
--rw-r--r--   0        0        0     2490 2024-05-05 16:14:00.576999 satsync-0.0.6/README.md
--rw-r--r--   0        0        0     1987 2024-05-06 09:44:04.552490 satsync-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      122 2024-05-06 08:10:33.368528 satsync-0.0.6/satsync/__init__.py
--rw-r--r--   0        0        0     3005 2024-05-06 08:10:29.848629 satsync-0.0.6/satsync/ecc.py
--rw-r--r--   0        0        0     7609 2024-05-06 08:10:33.364529 satsync-0.0.6/satsync/lgm.py
--rw-r--r--   0        0        0      263 2024-03-27 16:40:42.000000 satsync-0.0.6/satsync/lightglue/__init__.py
--rw-r--r--   0        0        0    26803 2024-05-05 19:07:59.747047 satsync-0.0.6/satsync/lightglue/aliked.py
--rw-r--r--   0        0        0     1751 2024-03-27 16:40:42.000000 satsync-0.0.6/satsync/lightglue/disk.py
--rw-r--r--   0        0        0     1500 2024-03-27 16:40:42.000000 satsync-0.0.6/satsync/lightglue/dog_hardnet.py
--rw-r--r--   0        0        0    25997 2024-05-05 19:08:04.722906 satsync-0.0.6/satsync/lightglue/lightglue.py
--rw-r--r--   0        0        0     8194 2024-03-27 16:40:42.000000 satsync-0.0.6/satsync/lightglue/sift.py
--rw-r--r--   0        0        0     8618 2024-03-27 16:40:42.000000 satsync-0.0.6/satsync/lightglue/superpoint.py
--rw-r--r--   0        0        0     5510 2024-05-05 19:08:04.722906 satsync-0.0.6/satsync/lightglue/utils.py
--rw-r--r--   0        0        0     5949 2024-05-05 19:07:59.631050 satsync-0.0.6/satsync/lightglue/viz2d.py
--rw-r--r--   0        0        0    14350 2024-05-06 09:16:25.363915 satsync-0.0.6/satsync/main.py
--rw-r--r--   0        0        0     4111 2024-05-06 08:10:29.856629 satsync-0.0.6/satsync/pcc.py
--rw-r--r--   0        0        0    13642 2024-05-06 09:31:34.186154 satsync-0.0.6/satsync/utils.py
--rw-r--r--   0        0        0     3361 1970-01-01 00:00:00.000000 satsync-0.0.6/setup.py
--rw-r--r--   0        0        0     3264 1970-01-01 00:00:00.000000 satsync-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-05 16:14:00.568999 satsync-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2490 2024-05-05 16:14:00.576999 satsync-0.0.7/README.md
+-rw-r--r--   0        0        0     1994 2024-05-07 14:05:45.984415 satsync-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-05-06 08:10:33.368528 satsync-0.0.7/satsync/__init__.py
+-rw-r--r--   0        0        0     3005 2024-05-06 08:10:29.848629 satsync-0.0.7/satsync/ecc.py
+-rw-r--r--   0        0        0     7609 2024-05-06 08:10:33.364529 satsync-0.0.7/satsync/lgm.py
+-rw-r--r--   0        0        0      263 2024-03-27 16:40:42.000000 satsync-0.0.7/satsync/lightglue/__init__.py
+-rw-r--r--   0        0        0    26803 2024-05-05 19:07:59.747047 satsync-0.0.7/satsync/lightglue/aliked.py
+-rw-r--r--   0        0        0     1751 2024-03-27 16:40:42.000000 satsync-0.0.7/satsync/lightglue/disk.py
+-rw-r--r--   0        0        0     1500 2024-03-27 16:40:42.000000 satsync-0.0.7/satsync/lightglue/dog_hardnet.py
+-rw-r--r--   0        0        0    25997 2024-05-05 19:08:04.722906 satsync-0.0.7/satsync/lightglue/lightglue.py
+-rw-r--r--   0        0        0     8194 2024-03-27 16:40:42.000000 satsync-0.0.7/satsync/lightglue/sift.py
+-rw-r--r--   0        0        0     8618 2024-03-27 16:40:42.000000 satsync-0.0.7/satsync/lightglue/superpoint.py
+-rw-r--r--   0        0        0     5510 2024-05-05 19:08:04.722906 satsync-0.0.7/satsync/lightglue/utils.py
+-rw-r--r--   0        0        0     5949 2024-05-05 19:07:59.631050 satsync-0.0.7/satsync/lightglue/viz2d.py
+-rw-r--r--   0        0        0    14350 2024-05-06 09:16:25.363915 satsync-0.0.7/satsync/main.py
+-rw-r--r--   0        0        0     4111 2024-05-06 08:10:29.856629 satsync-0.0.7/satsync/pcc.py
+-rw-r--r--   0        0        0    13642 2024-05-06 09:31:34.186154 satsync-0.0.7/satsync/utils.py
+-rw-r--r--   0        0        0     3368 1970-01-01 00:00:00.000000 satsync-0.0.7/setup.py
+-rw-r--r--   0        0        0     3271 1970-01-01 00:00:00.000000 satsync-0.0.7/PKG-INFO
```

### Comparing `satsync-0.0.6/LICENSE` & `satsync-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `satsync-0.0.6/README.md` & `satsync-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `satsync-0.0.6/pyproject.toml` & `satsync-0.0.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "satsync"
-version = "0.0.6"
-description = "A python package to align satellite images."
+version = "0.0.7"
+description = "Methods for spatial alignment of satellite imagery"
 authors = ["Cesar Aybar <fcesar.aybar@uv.es>"]
 repository = "https://github.com/csaybar/satsync"
 documentation = "https://csaybar.github.io/satsync/"
 readme = "README.md"
 packages = [
   {include = "satsync"}
 ]
@@ -15,15 +15,15 @@
 numpy = ">=1.25.2"
 xarray = ">=2023.7.0"
 rasterio = ">=1.3.10"
 scikit-image = ">=0.23.1"
 opencv-python = ">=4.8.0.76"
 pandas = ">=2.0.3"
 kornia = ">=0.7.2"
-torch = ">=2.2.0"
+torch = ">=2.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 deptry = "^0.12.0"
 mypy = "^1.5.1"
 pre-commit = "^3.4.0"
```

### Comparing `satsync-0.0.6/satsync/ecc.py` & `satsync-0.0.7/satsync/ecc.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.6/satsync/lgm.py` & `satsync-0.0.7/satsync/lgm.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.6/satsync/lightglue/aliked.py` & `satsync-0.0.7/satsync/lightglue/aliked.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.6/satsync/lightglue/disk.py` & `satsync-0.0.7/satsync/lightglue/disk.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.6/satsync/lightglue/dog_hardnet.py` & `satsync-0.0.7/satsync/lightglue/dog_hardnet.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.6/satsync/lightglue/lightglue.py` & `satsync-0.0.7/satsync/lightglue/lightglue.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.6/satsync/lightglue/sift.py` & `satsync-0.0.7/satsync/lightglue/sift.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.6/satsync/lightglue/superpoint.py` & `satsync-0.0.7/satsync/lightglue/superpoint.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.6/satsync/lightglue/utils.py` & `satsync-0.0.7/satsync/lightglue/utils.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.6/satsync/lightglue/viz2d.py` & `satsync-0.0.7/satsync/lightglue/viz2d.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.6/satsync/main.py` & `satsync-0.0.7/satsync/main.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.6/satsync/pcc.py` & `satsync-0.0.7/satsync/pcc.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.6/satsync/utils.py` & `satsync-0.0.7/satsync/utils.py`

 * *Files identical despite different names*

### Comparing `satsync-0.0.6/setup.py` & `satsync-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 install_requires = \
 ['kornia>=0.7.2',
  'numpy>=1.25.2',
  'opencv-python>=4.8.0.76',
  'pandas>=2.0.3',
  'rasterio>=1.3.10',
  'scikit-image>=0.23.1',
- 'torch>=2.2.0',
+ 'torch>=2.0.0',
  'xarray>=2023.7.0']
 
 setup_kwargs = {
     'name': 'satsync',
-    'version': '0.0.6',
-    'description': 'A python package to align satellite images.',
+    'version': '0.0.7',
+    'description': 'Methods for spatial alignment of satellite imagery',
     'long_description': '# satsync\n\n[![Release](https://img.shields.io/github/v/release/csaybar/satsync)](https://img.shields.io/github/v/release/csaybar/satsync)\n[![Build status](https://img.shields.io/github/actions/workflow/status/csaybar/satsync/main.yml?branch=main)](https://github.com/csaybar/satsync/actions/workflows/main.yml?query=branch%3Amain)\n[![codecov](https://codecov.io/gh/csaybar/satsync/branch/main/graph/badge.svg)](https://codecov.io/gh/csaybar/satsync)\n[![Commit activity](https://img.shields.io/github/commit-activity/m/csaybar/satsync)](https://img.shields.io/github/commit-activity/m/csaybar/satsync)\n[![License](https://img.shields.io/github/license/csaybar/satsync)](https://img.shields.io/github/license/csaybar/satsync)\n\nA python package to align satellite images.\n\n- **Github repository**: <https://github.com/csaybar/satsync/>\n- **Documentation** <https://csaybar.github.io/satsync/>\n\n## Getting started with your project\n\nFirst, create a repository on GitHub with the same name as this project, and then run the following commands:\n\n```bash\ngit init -b main\ngit add .\ngit commit -m "init commit"\ngit remote add origin git@github.com:csaybar/satsync.git\ngit push -u origin main\n```\n\nFinally, install the environment and the pre-commit hooks with\n\n```bash\nmake install\n```\n\nYou are now ready to start development on your project!\nThe CI/CD pipeline will be triggered when you open a pull request, merge to main, or when you create a new release.\n\nTo finalize the set-up for publishing to PyPi or Artifactory, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/publishing/#set-up-for-pypi).\nFor activating the automatic documentation with MkDocs, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/mkdocs/#enabling-the-documentation-on-github).\nTo enable the code coverage reports, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/codecov/).\n\n## Releasing a new version\n\n- Create an API Token on [Pypi](https://pypi.org/).\n- Add the API Token to your projects secrets with the name `PYPI_TOKEN` by visiting [this page](https://github.com/csaybar/satsync/settings/secrets/actions/new).\n- Create a [new release](https://github.com/csaybar/satsync/releases/new) on Github.\n- Create a new tag in the form `*.*.*`.\n\nFor more details, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/cicd/#how-to-trigger-a-release).\n\n---\n\nRepository initiated with [fpgmaas/cookiecutter-poetry](https://github.com/fpgmaas/cookiecutter-poetry).\n',
     'author': 'Cesar Aybar',
     'author_email': 'fcesar.aybar@uv.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/csaybar/satsync',
     'packages': packages,
```

### Comparing `satsync-0.0.6/PKG-INFO` & `satsync-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: satsync
-Version: 0.0.6
-Summary: A python package to align satellite images.
+Version: 0.0.7
+Summary: Methods for spatial alignment of satellite imagery
 Home-page: https://github.com/csaybar/satsync
 Author: Cesar Aybar
 Author-email: fcesar.aybar@uv.es
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: kornia (>=0.7.2)
 Requires-Dist: numpy (>=1.25.2)
 Requires-Dist: opencv-python (>=4.8.0.76)
 Requires-Dist: pandas (>=2.0.3)
 Requires-Dist: rasterio (>=1.3.10)
 Requires-Dist: scikit-image (>=0.23.1)
-Requires-Dist: torch (>=2.2.0)
+Requires-Dist: torch (>=2.0.0)
 Requires-Dist: xarray (>=2023.7.0)
 Project-URL: Documentation, https://csaybar.github.io/satsync/
 Project-URL: Repository, https://github.com/csaybar/satsync
 Description-Content-Type: text/markdown
 
 # satsync
```

