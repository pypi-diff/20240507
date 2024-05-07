# Comparing `tmp/pypular-0.1.tar.gz` & `tmp/pypular-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypular-0.1.tar", last modified: Sun May  5 19:04:52 2024, max compression
+gzip compressed data, was "pypular-0.2.tar", last modified: Tue May  7 20:41:22 2024, max compression
```

## Comparing `pypular-0.1.tar` & `pypular-0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 salvo     (1000) salvo     (1000)        0 2024-05-05 19:04:52.266886 pypular-0.1/
--rw-rw-r--   0 salvo     (1000) salvo     (1000)    34523 2024-05-02 18:16:31.000000 pypular-0.1/LICENSE
--rw-rw-r--   0 salvo     (1000) salvo     (1000)      580 2024-05-05 19:04:52.266886 pypular-0.1/PKG-INFO
--rw-rw-r--   0 salvo     (1000) salvo     (1000)      981 2024-05-05 18:21:34.000000 pypular-0.1/README.md
-drwxrwxr-x   0 salvo     (1000) salvo     (1000)        0 2024-05-05 19:04:52.266886 pypular-0.1/pypular/
--rw-rw-r--   0 salvo     (1000) salvo     (1000)        0 2024-05-03 06:59:27.000000 pypular-0.1/pypular/__init__.py
--rw-rw-r--   0 salvo     (1000) salvo     (1000)     1559 2024-05-04 12:26:01.000000 pypular-0.1/pypular/__main__.py
-drwxrwxr-x   0 salvo     (1000) salvo     (1000)        0 2024-05-05 19:04:52.266886 pypular-0.1/pypular.egg-info/
--rw-rw-r--   0 salvo     (1000) salvo     (1000)      580 2024-05-05 19:04:52.000000 pypular-0.1/pypular.egg-info/PKG-INFO
--rw-rw-r--   0 salvo     (1000) salvo     (1000)      224 2024-05-05 19:04:52.000000 pypular-0.1/pypular.egg-info/SOURCES.txt
--rw-rw-r--   0 salvo     (1000) salvo     (1000)        1 2024-05-05 19:04:52.000000 pypular-0.1/pypular.egg-info/dependency_links.txt
--rw-rw-r--   0 salvo     (1000) salvo     (1000)       50 2024-05-05 19:04:52.000000 pypular-0.1/pypular.egg-info/entry_points.txt
--rw-rw-r--   0 salvo     (1000) salvo     (1000)        8 2024-05-05 19:04:52.000000 pypular-0.1/pypular.egg-info/top_level.txt
--rw-rw-r--   0 salvo     (1000) salvo     (1000)       38 2024-05-05 19:04:52.266886 pypular-0.1/setup.cfg
--rwxrw-r--   0 salvo     (1000) salvo     (1000)      849 2024-05-05 19:04:52.000000 pypular-0.1/setup.py
+drwxrwxr-x   0 salvo     (1000) salvo     (1000)        0 2024-05-07 20:41:22.813984 pypular-0.2/
+-rw-rw-r--   0 salvo     (1000) salvo     (1000)    34523 2024-05-02 18:16:31.000000 pypular-0.2/LICENSE
+-rw-rw-r--   0 salvo     (1000) salvo     (1000)    42332 2024-05-07 20:41:22.813984 pypular-0.2/PKG-INFO
+-rw-rw-r--   0 salvo     (1000) salvo     (1000)     1724 2024-05-07 20:39:36.000000 pypular-0.2/README.md
+-rw-rw-r--   0 salvo     (1000) salvo     (1000)      804 2024-05-07 20:41:22.000000 pypular-0.2/pyproject.toml
+drwxrwxr-x   0 salvo     (1000) salvo     (1000)        0 2024-05-07 20:41:22.813984 pypular-0.2/pypular/
+-rw-rw-r--   0 salvo     (1000) salvo     (1000)        0 2024-05-03 06:59:27.000000 pypular-0.2/pypular/__init__.py
+-rw-rw-r--   0 salvo     (1000) salvo     (1000)     1559 2024-05-04 12:26:01.000000 pypular-0.2/pypular/__main__.py
+drwxrwxr-x   0 salvo     (1000) salvo     (1000)        0 2024-05-07 20:41:22.813984 pypular-0.2/pypular.egg-info/
+-rw-rw-r--   0 salvo     (1000) salvo     (1000)    42332 2024-05-07 20:41:22.000000 pypular-0.2/pypular.egg-info/PKG-INFO
+-rw-rw-r--   0 salvo     (1000) salvo     (1000)      239 2024-05-07 20:41:22.000000 pypular-0.2/pypular.egg-info/SOURCES.txt
+-rw-rw-r--   0 salvo     (1000) salvo     (1000)        1 2024-05-07 20:41:22.000000 pypular-0.2/pypular.egg-info/dependency_links.txt
+-rw-rw-r--   0 salvo     (1000) salvo     (1000)       50 2024-05-07 20:41:22.000000 pypular-0.2/pypular.egg-info/entry_points.txt
+-rw-rw-r--   0 salvo     (1000) salvo     (1000)        8 2024-05-07 20:41:22.000000 pypular-0.2/pypular.egg-info/top_level.txt
+-rw-rw-r--   0 salvo     (1000) salvo     (1000)       38 2024-05-07 20:41:22.813984 pypular-0.2/setup.cfg
+-rwxrw-r--   0 salvo     (1000) salvo     (1000)      849 2024-05-07 20:41:22.000000 pypular-0.2/setup.py
```

### Comparing `pypular-0.1/LICENSE` & `pypular-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypular-0.1/pypular/__main__.py` & `pypular-0.2/pypular/__main__.py`

 * *Files identical despite different names*

### Comparing `pypular-0.1/setup.py` & `pypular-0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/python3
 # This file is auto generated. Do not modify
 from setuptools import setup
 setup(
     name='pypular',
-    version='0.1',
+    version='0.2',
     description='Increase the popularity of your PYPI package by downloading it many times.',
     readme='README.md',
     url='https://codeberg.org/ltworf/pypular/',
     author="Salvo 'LtWorf' Tomaselli",
     author_email='tiposchi@tiscali.it',
     license='AGPL3',
     classifiers=['Development Status :: 2 - Pre-Alpha', 'Environment :: Console', 'License :: OSI Approved :: GNU Affero General Public License v3', 'Programming Language :: Python :: 3.11', 'Programming Language :: Python :: 3.12'],
```

