# Comparing `tmp/error-manager-1.3.3.tar.gz` & `tmp/error_manager-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error-manager-1.3.3.tar", last modified: Mon Oct 23 10:24:14 2023, max compression
+gzip compressed data, was "error_manager-1.3.4.tar", last modified: Tue May  7 20:02:53 2024, max compression
```

## Comparing `error-manager-1.3.3.tar` & `error_manager-1.3.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2023-10-23 10:24:14.093881 error-manager-1.3.3/
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      353 2023-04-17 09:35:16.000000 error-manager-1.3.3/.editorconfig
--rw-r--r--   0 maartenderuyter   (501) staff       (20)       30 2023-04-17 09:35:16.000000 error-manager-1.3.3/.isort.cfg
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      284 2023-04-17 09:35:16.000000 error-manager-1.3.3/.readthedocs.yml
--rw-r--r--   0 maartenderuyter   (501) staff       (20)       38 2023-04-17 09:35:16.000000 error-manager-1.3.3/AUTHORS.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     1667 2023-10-23 10:12:52.000000 error-manager-1.3.3/CHANGELOG.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     2620 2023-10-18 10:45:03.000000 error-manager-1.3.3/CONTRIBUTING.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)    43710 2023-04-17 09:35:16.000000 error-manager-1.3.3/LICENSE
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      290 2023-10-18 12:47:22.000000 error-manager-1.3.3/MANIFEST.in
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     5272 2023-10-23 10:24:14.093798 error-manager-1.3.3/PKG-INFO
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     3190 2023-04-17 09:35:16.000000 error-manager-1.3.3/README.rst
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2023-10-23 10:24:14.091216 error-manager-1.3.3/docs/
--rw-r--r--   0 maartenderuyter   (501) staff       (20)       28 2023-04-17 09:35:16.000000 error-manager-1.3.3/docs/authors.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)       30 2023-04-17 09:35:16.000000 error-manager-1.3.3/docs/changelog.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     1233 2023-04-17 09:35:16.000000 error-manager-1.3.3/docs/conf.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)       33 2023-04-17 09:35:16.000000 error-manager-1.3.3/docs/contributing.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     2849 2023-04-17 09:35:16.000000 error-manager-1.3.3/docs/index.rst
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2023-10-23 10:24:14.091540 error-manager-1.3.3/docs/reference/
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      110 2023-04-17 09:35:16.000000 error-manager-1.3.3/docs/reference/base.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)       72 2023-04-17 09:35:16.000000 error-manager-1.3.3/docs/reference/index.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)       77 2023-04-17 09:35:16.000000 error-manager-1.3.3/docs/reference/listerrors.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)       29 2023-04-17 09:35:16.000000 error-manager-1.3.3/docs/requirements.txt
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     4262 2023-04-17 09:35:16.000000 error-manager-1.3.3/docs/return_value.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      109 2023-04-17 09:35:16.000000 error-manager-1.3.3/docs/spelling_wordlist.txt
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     3662 2023-04-17 09:35:16.000000 error-manager-1.3.3/docs/usage.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)       89 2023-10-18 12:11:24.000000 error-manager-1.3.3/pyproject.toml
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     1515 2023-10-23 10:24:14.094250 error-manager-1.3.3/setup.cfg
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2023-10-23 10:24:14.088910 error-manager-1.3.3/src/
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2023-10-23 10:24:14.092330 error-manager-1.3.3/src/error_manager.egg-info/
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     5272 2023-10-23 10:24:14.000000 error-manager-1.3.3/src/error_manager.egg-info/PKG-INFO
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      799 2023-10-23 10:24:14.000000 error-manager-1.3.3/src/error_manager.egg-info/SOURCES.txt
--rw-r--r--   0 maartenderuyter   (501) staff       (20)        1 2023-10-23 10:24:14.000000 error-manager-1.3.3/src/error_manager.egg-info/dependency_links.txt
--rw-r--r--   0 maartenderuyter   (501) staff       (20)        7 2023-10-23 10:24:14.000000 error-manager-1.3.3/src/error_manager.egg-info/top_level.txt
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2023-10-23 10:24:14.093162 error-manager-1.3.3/src/errors/
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      315 2023-10-18 13:30:07.000000 error-manager-1.3.3/src/errors/__init__.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      380 2023-04-17 09:35:16.000000 error-manager-1.3.3/src/errors/__main__.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     3022 2023-10-18 13:30:07.000000 error-manager-1.3.3/src/errors/base.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      844 2023-04-17 09:35:16.000000 error-manager-1.3.3/src/errors/cli.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     1627 2023-10-18 13:30:07.000000 error-manager-1.3.3/src/errors/data_classes.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     1964 2023-10-18 13:30:07.000000 error-manager-1.3.3/src/errors/error.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      401 2023-10-18 13:30:07.000000 error-manager-1.3.3/src/errors/settings.py
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2023-10-23 10:24:14.093571 error-manager-1.3.3/tests/
--rw-r--r--   0 maartenderuyter   (501) staff       (20)        0 2023-04-17 09:35:16.000000 error-manager-1.3.3/tests/__init__.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     1920 2023-10-18 20:51:30.000000 error-manager-1.3.3/tests/test_enumerator.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     2627 2023-10-18 20:51:33.000000 error-manager-1.3.3/tests/test_errors.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     3602 2023-10-18 20:48:20.000000 error-manager-1.3.3/tests/test_return_value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:53.163318 error_manager-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-07 20:02:49.000000 error_manager-1.3.4/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 20:02:49.000000 error_manager-1.3.4/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-07 20:02:49.000000 error_manager-1.3.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 20:02:49.000000 error_manager-1.3.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-07 20:02:49.000000 error_manager-1.3.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-07 20:02:49.000000 error_manager-1.3.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    43710 2024-05-07 20:02:49.000000 error_manager-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-07 20:02:49.000000 error_manager-1.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-07 20:02:53.163318 error_manager-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-07 20:02:49.000000 error_manager-1.3.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:53.159319 error_manager-1.3.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:53.159319 error_manager-1.3.4/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/reference/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/reference/listerrors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/return_value.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 20:02:49.000000 error_manager-1.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-07 20:02:53.163318 error_manager-1.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:53.155319 error_manager-1.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:53.163318 error_manager-1.3.4/src/error_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-07 20:02:53.000000 error_manager-1.3.4/src/error_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-07 20:02:53.000000 error_manager-1.3.4/src/error_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:02:53.000000 error_manager-1.3.4/src/error_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 20:02:53.000000 error_manager-1.3.4/src/error_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:53.163318 error_manager-1.3.4/src/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-07 20:02:49.000000 error_manager-1.3.4/src/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-07 20:02:49.000000 error_manager-1.3.4/src/errors/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-07 20:02:49.000000 error_manager-1.3.4/src/errors/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-07 20:02:49.000000 error_manager-1.3.4/src/errors/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-07 20:02:49.000000 error_manager-1.3.4/src/errors/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:53.163318 error_manager-1.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:49.000000 error_manager-1.3.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-07 20:02:49.000000 error_manager-1.3.4/tests/test_enumerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-07 20:02:49.000000 error_manager-1.3.4/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-07 20:02:49.000000 error_manager-1.3.4/tests/test_return_value.py
```

### Comparing `error-manager-1.3.3/CHANGELOG.rst` & `error_manager-1.3.4/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `error-manager-1.3.3/CONTRIBUTING.rst` & `error_manager-1.3.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `error-manager-1.3.3/LICENSE` & `error_manager-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `error-manager-1.3.3/PKG-INFO` & `error_manager-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-manager
-Version: 1.3.3
+Version: 1.3.4
 Summary: Manage error codes, descriptions and data in a unified way throughout a project
 Home-page: https://github.com/MaartendeRuyter/errors
 Author: Maarten de Ruyter
 Author-email: "Maarten de Ruyter" <maarten@geodatagarden.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `error-manager-1.3.3/README.rst` & `error_manager-1.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `error-manager-1.3.3/docs/index.rst` & `error_manager-1.3.4/docs/index.rst`

 * *Files 24% similar despite different names*

```diff
@@ -57,31 +57,38 @@
 
 -------------------
 
 **error-manager main use cases**::
 
     # retrieve customer defined ErrorCode object form ``ListErrors`` class
     >>> from errors.error import ListErrors
-    >>> error = ListErrors.COULD_NOT_FIND_ERROR_CODE
+    >>> error = ListErrors.API_GET_RETURNED_404
     >>> error
-    ErrorCode(code='ER_GETERROR_00001', description='Could not find requested 
-    error code', error_data=<class 'dict'>)
+    ErrorCode(code='ER_API404_00001', description='API get request returned 404', error_data=<class 'dict'>)
     
-    # add custom error data to error message when you want to persist or log
-    # the error
-    >>> from errors.base import add_error_data   
-    >>> error_with_data = add_error_data(error, {'key': 'Example error data'})
+    # add custom error data to error message when you want to persist or log the error
+    >>> from errors.base import add_error_data
+    >>> error_without_data = ListErrors.API_GET_RETURNED_404
+    >>> error_with_data = add_error_data(error_without_data, {'url': 'www.bad_url.com'})
     >>> error_with_data 
-    ErrorCode(code='ER_GETERROR_00001', description='Could not find requested error code', error_data={'key': 'Example error data'})
+    ErrorCode(code='ER_API404_00001', description='API get request returned 404', error_data={'url': 'www.bad_url.com'})
+    
+    # This ErrorCode could be returned by the method performing the request so that
+    # the logic calling this method is aware of the failing request.
+    
+    # In order to use a single type as return value the error-manager package introduces a `ReturnValue` class
+    # that can hold the actual response, any possible downstream errors and the status of the return value. See 
+    # ReturnValue documentation.
     
 see :doc:`usage section <usage>` on how to create and
 register custom error codes for your project
 
 .. toctree::
    :maxdepth: 2
+   :caption: Contents:
 
    usage
    return_value
    reference/index
    contributing
    authors
    changelog
```

### Comparing `error-manager-1.3.3/docs/return_value.rst` & `error_manager-1.3.4/docs/return_value.rst`

 * *Files identical despite different names*

### Comparing `error-manager-1.3.3/docs/usage.rst` & `error_manager-1.3.4/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `error-manager-1.3.3/setup.cfg` & `error_manager-1.3.4/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = error-manager
-version = 1.3.3
+version = 1.3.4
 description = Manage error codes, descriptions and data in a unified way throughout a project
 long_description = file: README.rst, CHANGELOG.rst
 long_description_content_type = text/markdown
 url = https://github.com/MaartendeRuyter/errors
 author = Maarten de Ruyter
 author_email = "Maarten de Ruyter" <maarten@geodatagarden.com>
 license = MIT
@@ -13,14 +13,15 @@
 	License :: OSI Approved :: MIT License
 
 [options]
 package_dir = 
 	=src
 packages = find:
 include_package_data = True
+install_requires = 
 
 [options.packages.find]
 where = src
 exclude = 
 	test*
 
 [mypy]
@@ -31,15 +32,15 @@
 namespace_packages = True
 check_untyped_defs = True
 
 [flake8]
 max-line-length = 120
 
 [tool:pytest]
-testpaths = test
+testpaths = tests
 addopts = --cov --strict-markers
 xfail_strict = True
 
 [coverage:run]
 source = errors
 branch = True
 
@@ -49,43 +50,52 @@
 
 [coverage:paths]
 source = 
 	src/errors
 	*/site-packages/errors
 
 [tox:tox]
-envlist = py312
+envlist = py310, py311, py312
 isolated_build = True
 
 [testenv]
 deps = 
 	pytest
 	pytest-cov
 commands = 
 	pytest {posargs}
 
 [testenv:typecheck]
 deps = 
-	mypy
-	pytest
+	mypy==1.10.0
+	pytest==8.2.0
 commands = 
 	mypy --ignore-missing-imports {posargs:src tests}
 
 [testenv:format]
 skip_install = True
 deps = 
-	black
+	black==24.4.2
 commands = 
 	black {posargs:--check --diff src tests}
 
 [testenv:lint]
 skip_install = True
 deps = 
-	flake8
-	flake8-bugbear
+	flake8==7.0.0
+	flake8-bugbear==24.4.26
 commands = 
 	flake8 {posargs:src tests}
 
+[testenv:docs]
+basepython = python3
+deps = 
+	sphinx
+	sphinx-rtd-theme
+allowlist_externals = sphinx-build
+commands = 
+	sphinx-build -n -W --keep-going -b html docs/ docs/_build/
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `error-manager-1.3.3/src/error_manager.egg-info/PKG-INFO` & `error_manager-1.3.4/src/error_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-manager
-Version: 1.3.3
+Version: 1.3.4
 Summary: Manage error codes, descriptions and data in a unified way throughout a project
 Home-page: https://github.com/MaartendeRuyter/errors
 Author: Maarten de Ruyter
 Author-email: "Maarten de Ruyter" <maarten@geodatagarden.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `error-manager-1.3.3/src/error_manager.egg-info/SOURCES.txt` & `error_manager-1.3.4/src/error_manager.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,34 +5,34 @@
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
+docs/Makefile
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
+docs/make.bat
 docs/requirements.txt
 docs/return_value.rst
 docs/spelling_wordlist.txt
 docs/usage.rst
 docs/reference/base.rst
 docs/reference/index.rst
 docs/reference/listerrors.rst
 src/error_manager.egg-info/PKG-INFO
 src/error_manager.egg-info/SOURCES.txt
 src/error_manager.egg-info/dependency_links.txt
 src/error_manager.egg-info/top_level.txt
 src/errors/__init__.py
-src/errors/__main__.py
 src/errors/base.py
-src/errors/cli.py
 src/errors/data_classes.py
 src/errors/error.py
 src/errors/settings.py
 tests/__init__.py
 tests/test_enumerator.py
 tests/test_errors.py
 tests/test_return_value.py
```

### Comparing `error-manager-1.3.3/src/errors/base.py` & `error_manager-1.3.4/src/errors/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 ---------------------
 This method returns a new ErrorCode object with added error data.
 
 enumerator FunctionalErrorsBaseClass
 ------------------------------------
 Enumerator class that can be used to add errors and the register these error againts
 """
+
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Any, Dict, Union
 
 
 @dataclass(frozen=True)
 class ErrorCode:
```

### Comparing `error-manager-1.3.3/src/errors/data_classes.py` & `error_manager-1.3.4/src/errors/data_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """_summary_
 """
+
 from dataclasses import dataclass, field
 from typing import Any, List
 
 import errors.settings as st
 
 from .base import ErrorCode
```

### Comparing `error-manager-1.3.3/src/errors/error.py` & `error_manager-1.3.4/src/errors/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module to define ListErrors class."""
+
 from typing import Dict, Type
 
 from errors.base import ErrorCode, ErrorsClassErrors, FunctionalErrorsBaseClass
 
 
 class ListErrors:
     """Singleton Class for registering and retrieving error codes"""
```

### Comparing `error-manager-1.3.3/tests/test_enumerator.py` & `error_manager-1.3.4/tests/test_enumerator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module to provide test methods for errors.enumerator module."""
+
 import pytest
 
 from errors.base import BaseEnumerator, ErrorCode, ErrorsClassErrors, add_error_data
 
 
 def test_base_enumerators_class_exists():
     """Ensure ErrorsClassErrors class exists."""
```

### Comparing `error-manager-1.3.3/tests/test_errors.py` & `error_manager-1.3.4/tests/test_errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 """Module to provide test methods for errors.error module."""
+
 import pytest
 
 from errors.base import BaseEnumerator, ErrorCode, ErrorsClassErrors, is_error
-from errors.cli import main
 from errors.error import ListErrors
 
 
-def test_main():
-    assert main([]) == 0
-
-
 def test_list_errors_class_exists():
     """Ensure ErrorsClassErrors class exists."""
     assert ListErrors  # type: ignore
 
 
 def test_list_error_is_singleton_class():
     """Ensure ErrorsClassErrors class is a singleton class."""
```

### Comparing `error-manager-1.3.3/tests/test_return_value.py` & `error_manager-1.3.4/tests/test_return_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Module to provide test methods for ReturnValue dataclass of the errors module.
 """
+
 import pytest
 
 from errors.base import ErrorCode
 from errors.data_classes import ReturnValueWithErrorStatus, ReturnValueWithStatus
 
 
 def test_return_value_with_status_class_exists():
```

