# Comparing `tmp/dataidea-0.1.2.tar.gz` & `tmp/dataidea-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataidea-0.1.2.tar", last modified: Mon May  6 17:36:49 2024, max compression
+gzip compressed data, was "dataidea-0.1.3.tar", last modified: Tue May  7 14:28:23 2024, max compression
```

## Comparing `dataidea-0.1.2.tar` & `dataidea-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,38 @@
-drwxrwxr-x   0 jumashafara  (1000) jumashafara  (1000)        0 2024-05-06 17:36:49.331774 dataidea-0.1.2/
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)    11337 2024-04-25 15:06:39.000000 dataidea-0.1.2/LICENSE
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      111 2024-04-25 15:06:39.000000 dataidea-0.1.2/MANIFEST.in
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     2864 2024-05-06 17:36:49.327774 dataidea-0.1.2/PKG-INFO
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     2009 2024-04-30 16:38:32.000000 dataidea-0.1.2/README.md
-drwxrwxr-x   0 jumashafara  (1000) jumashafara  (1000)        0 2024-05-06 17:36:49.327774 dataidea-0.1.2/dataidea/
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)       22 2024-05-06 17:34:47.000000 dataidea-0.1.2/dataidea/__init__.py
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     1030 2024-05-06 17:34:47.000000 dataidea-0.1.2/dataidea/_modidx.py
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     1030 2024-04-27 09:51:24.000000 dataidea-0.1.2/dataidea/datasets.py
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      167 2024-04-27 09:39:06.000000 dataidea-0.1.2/dataidea/packages.py
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     1230 2024-05-06 17:34:47.000000 dataidea-0.1.2/dataidea/statistics.py
-drwxrwxr-x   0 jumashafara  (1000) jumashafara  (1000)        0 2024-05-06 17:36:49.327774 dataidea-0.1.2/dataidea.egg-info/
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     2864 2024-05-06 17:36:49.000000 dataidea-0.1.2/dataidea.egg-info/PKG-INFO
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      382 2024-05-06 17:36:49.000000 dataidea-0.1.2/dataidea.egg-info/SOURCES.txt
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)        1 2024-05-06 17:36:49.000000 dataidea-0.1.2/dataidea.egg-info/dependency_links.txt
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)       59 2024-05-06 17:36:49.000000 dataidea-0.1.2/dataidea.egg-info/entry_points.txt
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)        1 2024-05-05 12:55:26.000000 dataidea-0.1.2/dataidea.egg-info/not-zip-safe
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)        7 2024-05-06 17:36:49.000000 dataidea-0.1.2/dataidea.egg-info/requires.txt
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)        9 2024-05-06 17:36:49.000000 dataidea-0.1.2/dataidea.egg-info/top_level.txt
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     1093 2024-05-06 17:34:34.000000 dataidea-0.1.2/settings.ini
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)       38 2024-05-06 17:36:49.331774 dataidea-0.1.2/setup.cfg
--rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     2596 2024-04-25 15:06:39.000000 dataidea-0.1.2/setup.py
+drwxrwxr-x   0 jumashafara  (1000) jumashafara  (1000)        0 2024-05-07 14:28:23.834132 dataidea-0.1.3/
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)    11337 2024-04-25 15:06:39.000000 dataidea-0.1.3/LICENSE
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      137 2024-05-07 13:55:08.000000 dataidea-0.1.3/MANIFEST.in
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     2864 2024-05-07 14:28:23.834132 dataidea-0.1.3/PKG-INFO
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     2009 2024-04-30 16:38:32.000000 dataidea-0.1.3/README.md
+drwxrwxr-x   0 jumashafara  (1000) jumashafara  (1000)        0 2024-05-07 14:28:23.822132 dataidea-0.1.3/dataidea/
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)       22 2024-05-07 14:13:39.000000 dataidea-0.1.3/dataidea/__init__.py
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     1030 2024-05-07 14:13:39.000000 dataidea-0.1.3/dataidea/_modidx.py
+drwxrwxr-x   0 jumashafara  (1000) jumashafara  (1000)        0 2024-05-07 14:28:23.830132 dataidea-0.1.3/dataidea/datasets/
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     1745 2024-05-06 10:01:07.000000 dataidea-0.1.3/dataidea/datasets/air_passengers.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)    37145 2024-05-03 07:05:30.000000 dataidea-0.1.3/dataidea/datasets/boston.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      229 2024-04-19 06:31:05.000000 dataidea-0.1.3/dataidea/datasets/cluster.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     4645 2024-04-19 06:33:56.000000 dataidea-0.1.3/dataidea/datasets/demo.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)    47391 2024-04-19 06:31:05.000000 dataidea-0.1.3/dataidea/datasets/fpl.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      370 2024-04-19 06:31:05.000000 dataidea-0.1.3/dataidea/datasets/homeprices.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     3780 2024-04-27 09:00:34.000000 dataidea-0.1.3/dataidea/datasets/mall.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)  2091239 2024-04-19 06:31:05.000000 dataidea-0.1.3/dataidea/datasets/melbourne.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      302 2024-04-19 06:31:05.000000 dataidea-0.1.3/dataidea/datasets/music.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      656 2024-04-19 06:31:05.000000 dataidea-0.1.3/dataidea/datasets/salaries.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)    41983 2024-04-27 09:39:55.000000 dataidea-0.1.3/dataidea/datasets/student-mat.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)    68558 2024-04-27 09:39:44.000000 dataidea-0.1.3/dataidea/datasets/student-por.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)   108285 2024-04-19 06:31:05.000000 dataidea-0.1.3/dataidea/datasets/titanic.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)  1355781 2024-04-19 06:31:05.000000 dataidea-0.1.3/dataidea/datasets/vgsales.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      217 2024-04-19 06:31:05.000000 dataidea-0.1.3/dataidea/datasets/weather.csv
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     1030 2024-04-27 09:51:24.000000 dataidea-0.1.3/dataidea/datasets.py
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      167 2024-04-27 09:39:06.000000 dataidea-0.1.3/dataidea/packages.py
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     1230 2024-05-07 14:13:39.000000 dataidea-0.1.3/dataidea/statistics.py
+drwxrwxr-x   0 jumashafara  (1000) jumashafara  (1000)        0 2024-05-07 14:28:23.822132 dataidea-0.1.3/dataidea.egg-info/
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     2864 2024-05-07 14:28:23.000000 dataidea-0.1.3/dataidea.egg-info/PKG-INFO
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)      840 2024-05-07 14:28:23.000000 dataidea-0.1.3/dataidea.egg-info/SOURCES.txt
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)        1 2024-05-07 14:28:23.000000 dataidea-0.1.3/dataidea.egg-info/dependency_links.txt
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)       59 2024-05-07 14:28:23.000000 dataidea-0.1.3/dataidea.egg-info/entry_points.txt
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)        1 2024-05-05 12:55:26.000000 dataidea-0.1.3/dataidea.egg-info/not-zip-safe
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)        7 2024-05-07 14:28:23.000000 dataidea-0.1.3/dataidea.egg-info/requires.txt
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)        9 2024-05-07 14:28:23.000000 dataidea-0.1.3/dataidea.egg-info/top_level.txt
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     1093 2024-05-07 14:13:17.000000 dataidea-0.1.3/settings.ini
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)       38 2024-05-07 14:28:23.834132 dataidea-0.1.3/setup.cfg
+-rw-rw-r--   0 jumashafara  (1000) jumashafara  (1000)     2641 2024-05-07 14:28:14.000000 dataidea-0.1.3/setup.py
```

### Comparing `dataidea-0.1.2/LICENSE` & `dataidea-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dataidea-0.1.2/PKG-INFO` & `dataidea-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataidea
-Version: 0.1.2
+Version: 0.1.3
 Summary: Learn Programming For Data Science
 Home-page: https://github.com/dataidea/dataidea
 Author: jumashafara
 Author-email: jumashafara0@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev,jupyter,jupyter notebook,python,dataidea,machine learning,data,data science,science
 Platform: UNKNOWN
```

### Comparing `dataidea-0.1.2/README.md` & `dataidea-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dataidea-0.1.2/dataidea/_modidx.py` & `dataidea-0.1.3/dataidea/_modidx.py`

 * *Files identical despite different names*

### Comparing `dataidea-0.1.2/dataidea/datasets.py` & `dataidea-0.1.3/dataidea/datasets.py`

 * *Files identical despite different names*

### Comparing `dataidea-0.1.2/dataidea/statistics.py` & `dataidea-0.1.3/dataidea/statistics.py`

 * *Files identical despite different names*

### Comparing `dataidea-0.1.2/dataidea.egg-info/PKG-INFO` & `dataidea-0.1.3/dataidea.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataidea
-Version: 0.1.2
+Version: 0.1.3
 Summary: Learn Programming For Data Science
 Home-page: https://github.com/dataidea/dataidea
 Author: jumashafara
 Author-email: jumashafara0@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev,jupyter,jupyter notebook,python,dataidea,machine learning,data,data science,science
 Platform: UNKNOWN
```

### Comparing `dataidea-0.1.2/settings.ini` & `dataidea-0.1.3/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = dataidea
 lib_name = %(repo)s
-version = 0.1.2
+version = 0.1.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = dataidea
```

### Comparing `dataidea-0.1.2/setup.py` & `dataidea-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from pkg_resources import parse_version
 from configparser import ConfigParser
 import setuptools, shlex
+
+
 assert parse_version(setuptools.__version__)>=parse_version('36.2')
 
 # note: all settings are in settings.ini; edit there, not here
 config = ConfigParser(delimiters=['='])
 config.read('settings.ini', encoding='utf-8')
 cfg = config['DEFAULT']
 
@@ -37,14 +39,15 @@
         'Development Status :: ' + statuses[int(cfg['status'])],
         'Intended Audience :: ' + cfg['audience'].title(),
         'Natural Language :: ' + cfg['language'].title(),
     ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]] + (['License :: ' + lic[1] ] if lic[1] else []),
     url = cfg['git_url'],
     packages = setuptools.find_packages(),
     include_package_data = True,
+    package_data={'': ['datasets/*.csv']},
     install_requires = requirements,
     extras_require={ 'dev': dev_requirements },
     dependency_links = cfg.get('dep_links','').split(),
     python_requires  = '>=' + cfg['min_python'],
     long_description = open('README.md', encoding='utf-8').read(),
     long_description_content_type = 'text/markdown',
     zip_safe = False,
```

