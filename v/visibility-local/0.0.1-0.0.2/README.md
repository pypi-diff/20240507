# Comparing `tmp/visibility-local-0.0.1.tar.gz` & `tmp/visibility_local-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visibility-local-0.0.1.tar", last modified: Tue Jan 23 07:01:39 2024, max compression
+gzip compressed data, was "visibility_local-0.0.2.tar", last modified: Tue May  7 02:42:08 2024, max compression
```

## Comparing `visibility-local-0.0.1.tar` & `visibility_local-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 07:01:39.420000 visibility-local-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-01-23 07:01:39.420000 visibility-local-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-01-23 07:01:10.000000 visibility-local-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-01-23 07:01:10.000000 visibility-local-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-23 07:01:39.420000 visibility-local-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-01-23 07:01:10.000000 visibility-local-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 07:01:39.416000 visibility-local-0.0.1/visibility_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 07:01:39.416000 visibility-local-0.0.1/visibility_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 07:01:10.000000 visibility-local-0.0.1/visibility_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-01-23 07:01:10.000000 visibility-local-0.0.1/visibility_local/src/visibilities_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 07:01:39.416000 visibility-local-0.0.1/visibility_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-01-23 07:01:39.000000 visibility-local-0.0.1/visibility_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-01-23 07:01:39.000000 visibility-local-0.0.1/visibility_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 07:01:39.000000 visibility-local-0.0.1/visibility_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-23 07:01:39.000000 visibility-local-0.0.1/visibility_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-23 07:01:39.000000 visibility-local-0.0.1/visibility_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:42:08.985637 visibility_local-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-07 02:42:08.985637 visibility_local-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-07 02:41:49.000000 visibility_local-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-07 02:41:49.000000 visibility_local-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 02:42:08.985637 visibility_local-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-07 02:41:49.000000 visibility_local-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:42:08.981637 visibility_local-0.0.2/visibility_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:42:08.981637 visibility_local-0.0.2/visibility_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:41:49.000000 visibility_local-0.0.2/visibility_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-07 02:41:49.000000 visibility_local-0.0.2/visibility_local/src/visibilities_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:42:08.981637 visibility_local-0.0.2/visibility_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-07 02:42:08.000000 visibility_local-0.0.2/visibility_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-07 02:42:08.000000 visibility_local-0.0.2/visibility_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 02:42:08.000000 visibility_local-0.0.2/visibility_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 02:42:08.000000 visibility_local-0.0.2/visibility_local.egg-info/top_level.txt
```

### Comparing `visibility-local-0.0.1/README.md` & `visibility_local-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `visibility-local-0.0.1/pyproject.toml` & `visibility_local-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `visibility-local-0.0.1/setup.py` & `visibility_local-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 PACKAGE_NAME = "visibility-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     # TODO: Please update the name and delete this line i.e. XXX-local or XXX-remote
     #  (without the -python-package suffix). Only lowercase, no underlines.
     name=PACKAGE_NAME,
-    version='0.0.1',  # update only the minor version each time # https://pypi.org/project/<short-project-name-with-underscores>/
+    version='0.0.2',  # update only the minor version each time # https://pypi.org/project/<short-project-name-with-underscores>/
     author="Circles",
     author_email="info@circlez.ai",
     # TODO: Please update the description and long_description with no sensitive information as it is exposed in pypi.org
     description="PyPI Package for Circles visibility-local Python",
     long_description="PyPI Package for Circles visibility-local Python",
     long_description_content_type='text/markdown',
     # TODO: Please update the URL below
@@ -33,17 +33,10 @@
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ],
-    # TODO: Update which packages to include with this package
     install_requires=[
-        'PyMySQL>=1.0.2',
-        'pytest>=7.4.0',
-        'mysql-connector>=2.2.9',
-        'logzio-python-handler>= 4.1.0',
-        'user-context-remote>=0.0.17',
-        'python-sdk-local>=0.0.27'
     ],
 )
```

