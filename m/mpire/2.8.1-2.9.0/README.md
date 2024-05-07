# Comparing `tmp/mpire-2.8.1.tar.gz` & `tmp/mpire-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mpire-2.8.1.tar", last modified: Wed Nov  8 13:46:16 2023, max compression
+gzip compressed data, was "dist/mpire-2.9.0.tar", last modified: Mon Jan  8 21:28:47 2024, max compression
```

## Comparing `mpire-2.8.1.tar` & `mpire-2.9.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 13:46:16.000000 mpire-2.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2023-11-08 13:46:00.000000 mpire-2.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 13:46:16.000000 mpire-2.8.1/bin/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2023-11-08 13:46:00.000000 mpire-2.8.1/bin/mpire-dashboard
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-11-08 13:46:00.000000 mpire-2.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-11-08 13:46:00.000000 mpire-2.8.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 13:46:16.000000 mpire-2.8.1/mpire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-08 13:46:16.000000 mpire-2.8.1/mpire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2023-11-08 13:46:16.000000 mpire-2.8.1/mpire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-08 13:46:16.000000 mpire-2.8.1/mpire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15341 2023-11-08 13:46:16.000000 mpire-2.8.1/mpire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      815 2023-11-08 13:46:16.000000 mpire-2.8.1/mpire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15341 2023-11-08 13:46:16.000000 mpire-2.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-11-08 13:46:00.000000 mpire-2.8.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 13:46:16.000000 mpire-2.8.1/mpire/
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    10730 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14409 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     9657 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/async_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)    16630 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/params.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72103 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/pool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 13:46:16.000000 mpire-2.8.1/mpire/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/dashboard/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 13:46:16.000000 mpire-2.8.1/mpire/dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (127)    88145 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/dashboard/static/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   155756 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/dashboard/static/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/dashboard/static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)    16857 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/dashboard/static/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    78635 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/dashboard/static/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    13740 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/dashboard/static/glyphicons.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 13:46:16.000000 mpire-2.8.1/mpire/dashboard/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    45404 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/dashboard/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    23424 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/dashboard/static/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)   108738 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/dashboard/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (127)    20127 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/dashboard/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (127)    18028 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/dashboard/static/fonts/glyphicons-halflings-regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10579 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/dashboard/static/refresh.js
--rw-r--r--   0 runner    (1001) docker     (127)      396 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8789 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 13:46:16.000000 mpire-2.8.1/mpire/dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/dashboard/templates/mpire.html
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/dashboard/templates/menu_top_right.html
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     9516 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/dashboard/templates/progress_bar.html
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/dashboard/connection_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/dashboard/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    13340 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/insights.py
--rw-r--r--   0 runner    (1001) docker     (127)    30541 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/comms.py
--rw-r--r--   0 runner    (1001) docker     (127)     7967 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/tqdm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    32545 2023-11-08 13:46:00.000000 mpire-2.8.1/mpire/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-11-08 13:46:16.000000 mpire-2.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    12070 2023-11-08 13:46:00.000000 mpire-2.8.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:28:47.000000 mpire-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-01-08 21:28:35.000000 mpire-2.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-08 21:28:35.000000 mpire-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-01-08 21:28:35.000000 mpire-2.9.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:28:47.000000 mpire-2.9.0/mpire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-01-08 21:28:47.000000 mpire-2.9.0/mpire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-08 21:28:47.000000 mpire-2.9.0/mpire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 21:28:47.000000 mpire-2.9.0/mpire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15387 2024-01-08 21:28:47.000000 mpire-2.9.0/mpire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-01-08 21:28:47.000000 mpire-2.9.0/mpire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15387 2024-01-08 21:28:47.000000 mpire-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12116 2024-01-08 21:28:35.000000 mpire-2.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:28:47.000000 mpire-2.9.0/mpire/
+-rw-r--r--   0 runner    (1001) docker     (127)    16533 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72100 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/tqdm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/async_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12480 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12212 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:28:47.000000 mpire-2.9.0/mpire/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/dashboard/connection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8849 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/dashboard/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/dashboard/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/dashboard/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:28:47.000000 mpire-2.9.0/mpire/dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/dashboard/templates/menu_top_right.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/dashboard/templates/progress_bar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/dashboard/templates/mpire.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:28:47.000000 mpire-2.9.0/mpire/dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    78635 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/dashboard/static/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    88145 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/dashboard/static/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10579 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/dashboard/static/refresh.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:28:47.000000 mpire-2.9.0/mpire/dashboard/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   108738 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/dashboard/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/dashboard/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/dashboard/static/fonts/glyphicons-halflings-regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    45404 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/dashboard/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/dashboard/static/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   155756 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/dashboard/static/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    13740 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/dashboard/static/glyphicons.css
+-rw-r--r--   0 runner    (1001) docker     (127)    16857 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/dashboard/static/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/dashboard/static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12451 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/insights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30541 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/comms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32545 2024-01-08 21:28:35.000000 mpire-2.9.0/mpire/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-01-08 21:28:35.000000 mpire-2.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-08 21:28:47.000000 mpire-2.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:28:47.000000 mpire-2.9.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-01-08 21:28:35.000000 mpire-2.9.0/bin/mpire-dashboard
```

### Comparing `mpire-2.8.1/setup.py` & `mpire-2.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,44 +5,42 @@
     with open('README.rst') as file:
         return file.read()
 
 
 if __name__ == '__main__':
     setup(
         name='mpire',
-        version='2.8.1',
+        version='2.9.0',
         author='Sybren Jansen',
         description='A Python package for easy multiprocessing, but faster than multiprocessing',
         long_description=read_description(),
         url='https://github.com/sybrenjansen/mpire',
         license='MIT',
         packages=find_packages(exclude=['*tests*']),
         scripts=['bin/mpire-dashboard'],
-        install_requires=['dataclasses; python_version<"3.7"',
-                          'pywin32==225; platform_system=="Windows" and python_version=="3.6"',
-                          'pywin32>=301; platform_system=="Windows" and python_version>"3.6"',
+        install_requires=['pywin32>=301; platform_system=="Windows"',
                           'pygments>=2.0',
                           'tqdm>=4.27'],
         include_package_data=True,
         extras_require={
             'dashboard': ['flask'],
             'dill': ['multiprocess; python_version<"3.11"',
                      'multiprocess>=0.70.15; python_version>="3.11"'],
             'docs': ['docutils==0.17.1',
                      'sphinx==3.2.1',
                      'sphinx-rtd-theme==0.5.0',
                      'sphinx-autodoc-typehints==1.11.0',
                      'sphinxcontrib-images==0.9.2',
                      'sphinx-versions==1.0.1'],
-            'testing': ['dataclasses; python_version<"3.7"',
+            'testing': ['ipywidgets',
                         'multiprocess; python_version<"3.11"',
                         'multiprocess>=0.70.15; python_version>="3.11"',
                         'numpy',
-                        'pywin32==225; platform_system=="Windows" and python_version=="3.6"',
-                        'pywin32>=301; platform_system=="Windows" and python_version>"3.6"'],
+                        'pywin32>=301; platform_system=="Windows"',
+                        'rich'],
         },
         test_suite='tests',
         tests_require=['multiprocess', 'numpy'],
         classifiers=[
             # Development status
             'Development Status :: 5 - Production/Stable',
```

### Comparing `mpire-2.8.1/bin/mpire-dashboard` & `mpire-2.9.0/bin/mpire-dashboard`

 * *Files identical despite different names*

### Comparing `mpire-2.8.1/mpire.egg-info/SOURCES.txt` & `mpire-2.9.0/mpire.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 mpire/comms.py
 mpire/context.py
 mpire/exception.py
 mpire/insights.py
 mpire/params.py
 mpire/pool.py
 mpire/progress_bar.py
+mpire/py.typed
 mpire/signal.py
 mpire/tqdm_utils.py
 mpire/utils.py
 mpire/worker.py
 mpire.egg-info/PKG-INFO
 mpire.egg-info/SOURCES.txt
 mpire.egg-info/dependency_links.txt
```

### Comparing `mpire-2.8.1/mpire.egg-info/PKG-INFO` & `mpire-2.9.0/mpire.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpire
-Version: 2.8.1
+Version: 2.9.0
 Summary: A Python package for easy multiprocessing, but faster than multiprocessing
 Home-page: https://github.com/sybrenjansen/mpire
 Author: Sybren Jansen
 License: MIT
 Description: MPIRE (MultiProcessing Is Really Easy)
         ======================================
         
@@ -38,15 +38,15 @@
         - Intuitive, Pythonic syntax
         - Multiprocessing with ``map``/``map_unordered``/``imap``/``imap_unordered``/``apply``/``apply_async`` functions
         - Easy use of copy-on-write shared objects with a pool of workers (copy-on-write is only available for start method
           ``fork``)
         - Each worker can have its own state and with convenient worker init and exit functionality this state can be easily
           manipulated (e.g., to load a memory-intensive model only once for each worker without the need of sending it through a
           queue)
-        - Progress bar support using tqdm_
+        - Progress bar support using tqdm_ (``rich`` and notebook widgets are supported)
         - Progress dashboard support
         - Worker insights to provide insight into your multiprocessing efficiency
         - Graceful and user-friendly exception handling
         - Timeouts, including for worker init and exit functions
         - Automatic task chunking for all available map functions to speed up processing of small task queues (including numpy
           arrays)
         - Adjustable maximum number of active tasks to avoid memory problems
@@ -313,11 +313,11 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: docs
 Provides-Extra: dashboard
-Provides-Extra: testing
 Provides-Extra: dill
-Provides-Extra: docs
+Provides-Extra: testing
```

### Comparing `mpire-2.8.1/PKG-INFO` & `mpire-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpire
-Version: 2.8.1
+Version: 2.9.0
 Summary: A Python package for easy multiprocessing, but faster than multiprocessing
 Home-page: https://github.com/sybrenjansen/mpire
 Author: Sybren Jansen
 License: MIT
 Description: MPIRE (MultiProcessing Is Really Easy)
         ======================================
         
@@ -38,15 +38,15 @@
         - Intuitive, Pythonic syntax
         - Multiprocessing with ``map``/``map_unordered``/``imap``/``imap_unordered``/``apply``/``apply_async`` functions
         - Easy use of copy-on-write shared objects with a pool of workers (copy-on-write is only available for start method
           ``fork``)
         - Each worker can have its own state and with convenient worker init and exit functionality this state can be easily
           manipulated (e.g., to load a memory-intensive model only once for each worker without the need of sending it through a
           queue)
-        - Progress bar support using tqdm_
+        - Progress bar support using tqdm_ (``rich`` and notebook widgets are supported)
         - Progress dashboard support
         - Worker insights to provide insight into your multiprocessing efficiency
         - Graceful and user-friendly exception handling
         - Timeouts, including for worker init and exit functions
         - Automatic task chunking for all available map functions to speed up processing of small task queues (including numpy
           arrays)
         - Adjustable maximum number of active tasks to avoid memory problems
@@ -313,11 +313,11 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: docs
 Provides-Extra: dashboard
-Provides-Extra: testing
 Provides-Extra: dill
-Provides-Extra: docs
+Provides-Extra: testing
```

### Comparing `mpire-2.8.1/LICENSE` & `mpire-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpire-2.8.1/mpire/exception.py` & `mpire-2.9.0/mpire/exception.py`

 * *Files identical despite different names*

### Comparing `mpire-2.8.1/mpire/utils.py` & `mpire-2.9.0/mpire/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import heapq
 import itertools
 import math
+import multiprocessing
 import os
 from datetime import datetime, timedelta
 from multiprocessing import Array, cpu_count
+from multiprocessing.managers import SyncManager
 from typing import Callable, Collection, Generator, Iterable, List, Optional, Tuple, Union
 
 try:
     import numpy as np
     NUMPY_INSTALLED = True
 except ImportError:
     np = None
@@ -237,7 +239,46 @@
     def __exit__(self, exc_type, exc_val, exc_tb) -> None:
         duration = (datetime.now() - self.start_dt).total_seconds()
         if self.cum_time_array is not None:
             self.cum_time_array[self.array_idx] += duration
         if self.max_time_array is not None and duration > self.max_time_array[0][0]:
             heapq.heappushpop(self.max_time_array,
                               (duration, self.format_args_func() if self.format_args_func is not None else None))
+
+    
+class PicklableSyncManager:
+    """ SyncManager wrapper that can be pickled """
+    
+    def __init__(self, authkey: bytes) -> None:
+        self.authkey = authkey
+        self.manager = SyncManager(authkey=authkey)
+        
+    def __getattr__(self, item):
+        return getattr(self.manager, item)
+
+    def __getstate__(self) -> dict:
+        """
+        Returns the state excluding the manager object, as this is not picklable. The address of the manager is added
+        to the state instead, which can be used to reconnect to the manager.
+        
+        :return: State dict
+        """
+        state = self.__dict__.copy()
+        state["manager_address"] = self.manager.address
+        del state["manager"]
+        return state
+
+    def __setstate__(self, state: dict) -> None:
+        """
+        Set the state and reconnect to the manager using the stored address.
+        
+        :param state: State dict
+        """
+        address = state.pop("manager_address")
+        self.__dict__ = state
+        
+        # This line is needed because otherwise we can get "multiprocessing.context.AuthenticationError: digest sent 
+        # was rejected" errors. See https://bugs.python.org/issue7503 for more information
+        multiprocessing.current_process().authkey = self.authkey
+        
+        self.manager = SyncManager(address=address, authkey=self.authkey)
+        self.manager.connect()
```

### Comparing `mpire-2.8.1/mpire/progress_bar.py` & `mpire-2.9.0/mpire/progress_bar.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import threading
 import traceback
 from datetime import datetime, timedelta
 from threading import Event, Thread
 from typing import Any, Dict, Optional, Type
+import warnings
 
-from tqdm import tqdm as tqdm_type
+from tqdm import TqdmExperimentalWarning, tqdm as tqdm_type
 
 from mpire.comms import WorkerComms, POISON_PILL
-from mpire.dashboard.connection_utils import (DashboardConnectionDetails, get_dashboard_connection_details,
-                                              set_dashboard_connection)
 from mpire.exception import remove_highlighting
 from mpire.insights import WorkerInsights
 from mpire.params import WorkerMapParams, WorkerPoolParams
 from mpire.signal import DisableKeyboardInterruptSignal
-from mpire.tqdm_utils import get_tqdm, TqdmConnectionDetails, TqdmManager
+from mpire.tqdm_utils import get_tqdm, TqdmManager
 from mpire.utils import format_seconds
 
 # If a user has not installed the dashboard dependencies than the imports below will fail
 try:
     from mpire.dashboard.dashboard import DASHBOARD_STARTED_EVENT
     from mpire.dashboard.utils import get_function_details
     from mpire.dashboard.manager import get_manager_client_dicts
@@ -77,16 +76,15 @@
 
         :return: self
         """
         if self.show_progress_bar:
 
             # Disable the interrupt signal. We let the thread die gracefully
             with DisableKeyboardInterruptSignal():
-                self.thread = Thread(target=self._progress_bar_handler, args=(TqdmManager.get_connection_details(),
-                                                                              get_dashboard_connection_details()))
+                self.thread = Thread(target=self._progress_bar_handler)
                 self.thread.start()
                 self.thread_started.wait()
 
         return self
 
     def __exit__(self, exc_type: Type, *_) -> None:
         """
@@ -100,45 +98,34 @@
                 self.worker_comms.signal_kill_signal_received()
 
             # Signal shutdown and close the handling thread
             if not self.worker_comms.exception_thrown():
                 self.worker_comms.signal_progress_bar_shutdown()
             self.thread.join()
 
-    def _progress_bar_handler(self, tqdm_connection_details: TqdmConnectionDetails,
-                              dashboard_connection_details: DashboardConnectionDetails) -> None:
+    def _progress_bar_handler(self) -> None:
         """
         Keeps track of the progress made by the workers and updates the progress bar accordingly
-
-        :param tqdm_connection_details: Tqdm manager host, and whether the manager is started/connected
-        :param dashboard_connection_details: Dashboard manager host, port_nr and whether a dashboard is
-            started/connected
         """
         # Obtain the progress bar tqdm class
-        tqdm, in_notebook = get_tqdm(self.progress_bar_style)
-
-        # Set tqdm and dashboard connection details. This is needed for nested pools and in the case forkserver or
-        # spawn is used as start method
-        TqdmManager.set_connection_details(tqdm_connection_details)
-        set_dashboard_connection(dashboard_connection_details)
+        tqdm = get_tqdm(self.progress_bar_style)
 
         # Connect to the tqdm manager
         tqdm_manager = TqdmManager()
         tqdm_lock, tqdm_position_register = tqdm_manager.get_lock_and_position_register()
         tqdm.set_lock(tqdm_lock)
-        main_progress_bar = tqdm_position_register.register_progress_bar_position(self.progress_bar_options["position"])
-
-        # In case we're running tqdm in a notebook we need to apply a dirty hack to get progress bars working.
-        # Solution adapted from https://github.com/tqdm/tqdm/issues/485#issuecomment-473338308
-        if in_notebook and not main_progress_bar:
-            print(' ', end='', flush=True)
-
-        # Create progress bar and register the start time
-        tqdm.monitor_interval = False
-        progress_bar = tqdm(**self.progress_bar_options)
+        tqdm.set_main_progress_bar(
+            tqdm_position_register.register_progress_bar_position(self.progress_bar_options["position"])
+        )
+
+        # Create progress bar and register the start time. Ignore the experimental warning for rich progress bars
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore", TqdmExperimentalWarning)
+            tqdm.monitor_interval = False
+            progress_bar = tqdm(**self.progress_bar_options)
         self.start_t = datetime.fromtimestamp(progress_bar.start_t)
 
         # Notify that the main process can continue working. We set it after the progress bar has been created, instead
         # of right after this thread has started, for a better user experience
         self.thread_started.set()
 
         # Register progress bar to dashboard in case a dashboard is started
@@ -161,48 +148,32 @@
                             if self.exception_traceback_str is None:
                                 self.exception_traceback_str_set_condition.wait()
                         self._send_dashboard_update(progress_bar, failed=True,
                                                     traceback_str=self.exception_traceback_str)
                     elif self.worker_comms.kill_signal_received():
                         self._send_dashboard_update(progress_bar, failed=True, traceback_str='Kill signal received')
 
-                # Final update of the progress bar. When we're not in a notebook and this is the main progress bar, we
-                # add as many newlines as the highest progress bar position, such that new output is added after the
-                # progress bars.
-                progress_bar.refresh()
-                if in_notebook:
-                    progress_bar.close()
-                else:
-                    progress_bar.disable = True
-                    if main_progress_bar:
-                        progress_bar.fp.write('\n' * (tqdm_position_register.get_highest_progress_bar_position() + 1))
+                # Final update of the progress bar
+                progress_bar.final_refresh(tqdm_position_register.get_highest_progress_bar_position())
                 break
 
             # Check if the total has been updated. It could be that we didn't know the total number of tasks at the
-            # beginning, but we do now. In a notebook we also need to update the max value of the progress bar widget.
+            # beginning, but we do now.
             if self.total_updated.is_set():
-                progress_bar.total = self.total
-                if in_notebook:
-                    progress_bar.container.children[1].max = self.total
-                progress_bar.refresh()
+                progress_bar.update_total(self.total)
                 self._send_dashboard_update(progress_bar)
                 self.total_updated.clear()
 
             # Check if there's an actual update
             if tasks_completed > 0 and tasks_completed == progress_bar.n:
                 continue
 
             # Update progress bar
             progress_bar.update(tasks_completed - progress_bar.n)
-
-            # Force a refresh when we're at 100%
             if progress_bar.n == progress_bar.total:
-                if in_notebook:
-                    progress_bar.close()
-                progress_bar.refresh()
                 self.worker_comms.signal_progress_bar_complete()
                 self.worker_comms.wait_until_progress_bar_is_complete()
                 self._send_dashboard_update(progress_bar)
 
             # Send update to dashboard in case a dashboard is started, but only when tqdm updated its view as well. This
             # will make the dashboard a lot more responsive
             if progress_bar.n == progress_bar.last_print_n:
```

### Comparing `mpire-2.8.1/mpire/async_result.py` & `mpire-2.9.0/mpire/async_result.py`

 * *Files identical despite different names*

### Comparing `mpire-2.8.1/mpire/context.py` & `mpire-2.9.0/mpire/context.py`

 * *Files identical despite different names*

### Comparing `mpire-2.8.1/mpire/signal.py` & `mpire-2.9.0/mpire/signal.py`

 * *Files identical despite different names*

### Comparing `mpire-2.8.1/mpire/params.py` & `mpire-2.9.0/mpire/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import itertools
 import math
 import multiprocessing as mp
 import warnings
-from io import StringIO
+from dataclasses import dataclass, field
 from typing import Any, Callable, Dict, Iterable, List, Optional, Sized, Tuple, Type, Union
 
-from dataclasses import dataclass, field
-from unittest.mock import patch
-from tqdm import tqdm, TqdmKeyError
+from tqdm import TqdmKeyError
 
-from mpire.context import DEFAULT_START_METHOD, RUNNING_WINDOWS
+from mpire.context import DEFAULT_START_METHOD
 from mpire.tqdm_utils import get_tqdm
 
 # Typedefs
 CPUList = List[Union[int, List[int]]]
 
 
 @dataclass(init=True, frozen=False)
@@ -203,19 +201,14 @@
         max_tasks_active = pool_params.n_jobs * int(math.ceil(chunk_size)) * 2
     else:
         check_number(max_tasks_active, 'max_tasks_active', allowed_types=(int,), none_allowed=True, min_=1)
 
     # If worker lifespan is not None or not a positive integer, raise
     check_number(worker_lifespan, 'worker_lifespan', allowed_types=(int,), none_allowed=True, min_=1)
 
-    # Progress bar is currently not supported on Windows when using threading as start method. For reasons still
-    # unknown we get a TypeError: cannot pickle '_thread.Lock' object.
-    if RUNNING_WINDOWS and progress_bar and pool_params.start_method == "threading":
-        raise ValueError("Progress bar is currently not supported on Windows when using start_method='threading'")
-
     # Check progress bar parameters and set default values
     progress_bar_options = check_progress_bar_options(progress_bar_options, progress_bar_position, n_tasks,
                                                       progress_bar_style)
 
     # Timeout parameters can't be negative
     for timeout_var, timeout_var_name in [(task_timeout, 'task_timeout'),
                                           (worker_init_timeout, 'worker_init_timeout'),
@@ -296,30 +289,34 @@
                       "progress bar position using 'progress_bar_options' instead", DeprecationWarning, stacklevel=2)
         check_number(progress_bar_position, "progress_bar_position", (int,), False, min_=0)
         if "position" in progress_bar_options:
             warnings.warn("The 'progress_bar_position' is already provided in 'progress_bar_options', which will take "
                           "precedence", RuntimeWarning, stacklevel=2)
         else:
             progress_bar_options["position"] = progress_bar_position
+            
+    # We currently do not support the position parameter for rich progress bars. Although this can be implemented by
+    # using a single rich progress bar for all workers and using `add_task`, but this is not trivial to implement.
+    if progress_bar_style == "rich" and "position" in progress_bar_options:
+        raise NotImplementedError("The 'position' parameter is currently not supported for rich progress bars")
 
     # Set some defaults and overwrite others
     progress_bar_options["total"] = n_tasks
     progress_bar_options["leave"] = True
     progress_bar_options.setdefault("position", 0)
     progress_bar_options.setdefault("dynamic_ncols", True)
     progress_bar_options.setdefault("mininterval", 0.1)
     progress_bar_options.setdefault("maxinterval", 0.5)
 
     # Check if the tqdm progress bar style is valid
-    get_tqdm(progress_bar_style)
+    tqdm = get_tqdm(progress_bar_style)
 
-    # Check that all progress bar options are properly formatted. We need to that here, because when an error occurs
+    # Check that all progress bar options are properly formatted. We need to do that here, because when an error occurs
     # within the progress bar handler it will deadlock (it's not technically impossible to do it there, but might as
     # well do it here)
     try:
-        with patch(progress_bar_options.get('file', 'sys.stderr'), new=StringIO()):
-            tqdm(**progress_bar_options)
+        tqdm.check_options(progress_bar_options)
     except (TqdmKeyError, TypeError) as e:
         raise e from ValueError("There's an error in progress_bar_options. Either one of the parameters doesn't exist "
                                 "or it's not properly formatted. See tqdm.tqdm() for details.")
 
     return progress_bar_options
```

### Comparing `mpire-2.8.1/mpire/pool.py` & `mpire-2.9.0/mpire/pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -710,15 +710,15 @@
                                          worker_init_timeout, worker_exit_timeout)
 
         # Chunk the function arguments. Make single arguments when we're not dealing with numpy arrays
         if not numpy_chunking:
             iterator_of_chunked_args = chunk_tasks(iterable_of_args, n_tasks, chunk_size, n_splits)
 
         # Grab original lock in case we have a progress bar and we need to restore it
-        tqdm, _ = get_tqdm(progress_bar_style)
+        tqdm = get_tqdm(progress_bar_style)
         original_tqdm_lock = tqdm.get_lock()
         tqdm_manager_owner = False
 
         imap_iterator = None
         try:
             if self._map_running:
                 self._worker_comms.signal_exception_thrown(MAIN_PROCESS)
```

### Comparing `mpire-2.8.1/mpire/dashboard/static/jquery.min.js` & `mpire-2.9.0/mpire/dashboard/static/jquery.min.js`

 * *Files identical despite different names*

### Comparing `mpire-2.8.1/mpire/dashboard/static/bootstrap.min.css` & `mpire-2.9.0/mpire/dashboard/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `mpire-2.8.1/mpire/dashboard/static/style.css` & `mpire-2.9.0/mpire/dashboard/static/style.css`

 * *Files identical despite different names*

### Comparing `mpire-2.8.1/mpire/dashboard/static/jquery-ui.min.js` & `mpire-2.9.0/mpire/dashboard/static/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `mpire-2.8.1/mpire/dashboard/static/bootstrap.bundle.min.js` & `mpire-2.9.0/mpire/dashboard/static/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `mpire-2.8.1/mpire/dashboard/static/glyphicons.css` & `mpire-2.9.0/mpire/dashboard/static/glyphicons.css`

 * *Files identical despite different names*

### Comparing `mpire-2.8.1/mpire/dashboard/static/fonts/glyphicons-halflings-regular.ttf` & `mpire-2.9.0/mpire/dashboard/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `mpire-2.8.1/mpire/dashboard/static/fonts/glyphicons-halflings-regular.woff` & `mpire-2.9.0/mpire/dashboard/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `mpire-2.8.1/mpire/dashboard/static/fonts/glyphicons-halflings-regular.svg` & `mpire-2.9.0/mpire/dashboard/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `mpire-2.8.1/mpire/dashboard/static/fonts/glyphicons-halflings-regular.eot` & `mpire-2.9.0/mpire/dashboard/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `mpire-2.8.1/mpire/dashboard/static/fonts/glyphicons-halflings-regular.woff2` & `mpire-2.9.0/mpire/dashboard/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `mpire-2.8.1/mpire/dashboard/static/refresh.js` & `mpire-2.9.0/mpire/dashboard/static/refresh.js`

 * *Files identical despite different names*

### Comparing `mpire-2.8.1/mpire/dashboard/dashboard.py` & `mpire-2.9.0/mpire/dashboard/dashboard.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import atexit
-import errno
 import getpass
 import logging
 import socket
 from datetime import datetime
-from multiprocessing import Event, Process, Value
+from multiprocessing import Event, Process
 from pkg_resources import resource_string
 from typing import Dict, Optional, Sequence, Union
 
-from flask import escape, Flask, jsonify, render_template, request
+from flask import Flask, jsonify, render_template, request
+from markupsafe import escape
+from mpire.dashboard.utils import get_two_available_ports
 from werkzeug.serving import make_server
 
 from mpire.signal import DisableKeyboardInterruptSignal, ignore_keyboard_interrupt
 from mpire.dashboard.manager import (DASHBOARD_MANAGER_HOST, DASHBOARD_MANAGER_PORT,
-                                     get_manager_client_dicts, start_manager_server)
+                                     get_manager_client_dicts, shutdown_manager_server, start_manager_server)
 
 logger = logging.getLogger(__name__)
 logger_werkzeug = logging.getLogger('werkzeug')
 logger_werkzeug.setLevel(logging.ERROR)
 app = Flask(__name__)
 _server = None
 _progress_bar_html = resource_string(__name__, 'templates/progress_bar.html').decode('utf-8')
@@ -103,43 +104,55 @@
 
 
 def start_dashboard(port_range: Sequence = range(8080, 8100)) -> Dict[str, Union[int, str]]:
     """
     Starts a new MPIRE dashboard
 
     :param port_range: Port range to try.
-    :return: A dictionary containing the dashboard port number and manager host and port_nr being used
+    :return: A dictionary containing the dashboard port number and manager host and port number being used
     """
     global _DASHBOARD_MANAGER, _DASHBOARD_TQDM_DICT, _DASHBOARD_TQDM_DETAILS_DICT
 
     if not DASHBOARD_STARTED_EVENT.is_set():
+        
+        dashboard_port_nr, manager_port_nr = get_two_available_ports(port_range)
 
         # Prevent signal from propagating to child process
         with DisableKeyboardInterruptSignal():
 
             # Set up manager server
-            _DASHBOARD_MANAGER = start_manager_server(port_range)
+            _DASHBOARD_MANAGER = start_manager_server(manager_port_nr)
 
             # Start flask server
             logging.getLogger('werkzeug').setLevel(logging.WARN)
-            dashboard_port_nr = Value('i', 0, lock=False)
             Process(target=_run, args=(DASHBOARD_STARTED_EVENT, DASHBOARD_MANAGER_HOST.value,
-                                       DASHBOARD_MANAGER_PORT.value, dashboard_port_nr, port_range),
+                                       DASHBOARD_MANAGER_PORT.value, dashboard_port_nr),
                     daemon=True, name='dashboard-process').start()
             DASHBOARD_STARTED_EVENT.wait()
 
             # Return connect information
-            return {'dashboard_port_nr': dashboard_port_nr.value,
+            return {'dashboard_port_nr': dashboard_port_nr,
                     'manager_host': DASHBOARD_MANAGER_HOST.value.decode() or socket.gethostname(),
                     'manager_port_nr': DASHBOARD_MANAGER_PORT.value}
 
     else:
         raise RuntimeError("You already have a running dashboard")
 
 
+def shutdown_dashboard() -> None:
+    """ Shuts down the dashboard """
+    if DASHBOARD_STARTED_EVENT.is_set():
+        global _DASHBOARD_MANAGER, _DASHBOARD_TQDM_DICT, _DASHBOARD_TQDM_DETAILS_DICT
+        shutdown_manager_server(_DASHBOARD_MANAGER)
+        _DASHBOARD_MANAGER = None
+        _DASHBOARD_TQDM_DICT = None
+        _DASHBOARD_TQDM_DETAILS_DICT = None
+        DASHBOARD_STARTED_EVENT.clear()
+        
+
 def connect_to_dashboard(manager_port_nr: int, manager_host: Optional[Union[bytes, str]] = None) -> None:
     """
     Connects to an existing MPIRE dashboard
 
     :param manager_port_nr: Port to use when connecting to a manager
     :param manager_host: Host to use when connecting to a manager. If ``None`` it will use localhost
     """
@@ -161,50 +174,38 @@
     except ConnectionRefusedError:
         raise ConnectionRefusedError("Could not connect to dashboard manager at "
                                      f"{manager_host.decode()}:{manager_port_nr}")
 
     DASHBOARD_STARTED_EVENT.set()
 
 
-def _run(started: Event, manager_host: str, manager_port_nr: int, dashboard_port_nr: Value,
-         port_range: Sequence) -> None:
+def _run(started: Event, manager_host: str, manager_port_nr: int, dashboard_port_nr: int) -> None:
     """
     Starts a dashboard server
 
     :param started: Event that signals the dashboard server has started
     :param manager_host: Dashboard manager host
     :param manager_port_nr: Dashboard manager port number
-    :param dashboard_port_nr: Value object for storing the dashboad port number that is used
-    :param port_range: Port range to try.
+    :param dashboard_port_nr: Dashboard port number
     """
     ignore_keyboard_interrupt()  # For Windows compatibility
 
     # Set dashboard connection details. This is needed when spawn is the default start method
     DASHBOARD_MANAGER_HOST.value = manager_host
     DASHBOARD_MANAGER_PORT.value = manager_port_nr
 
     # Connect to manager from this process
     global _DASHBOARD_TQDM_DICT, _DASHBOARD_TQDM_DETAILS_DICT, _server
     _DASHBOARD_TQDM_DICT, _DASHBOARD_TQDM_DETAILS_DICT, _ = get_manager_client_dicts()
 
-    # Try different ports, until a free one is found
-    for port in port_range:
-        try:
-            _server = make_server('0.0.0.0', port, app)
-            dashboard_port_nr.value = port
-            started.set()
-            logger.info("Server started on 0.0.0.0:%d", port)
-            _server.serve_forever()
-            break
-        except OSError as exc:
-            if exc.errno != errno.EADDRINUSE:
-                raise exc
-
-    if not _server:
-        raise OSError(f"Dashboard server: All ports are in use: {port_range}")
+    # Start server
+    _server = make_server('0.0.0.0', dashboard_port_nr, app)
+    started.set()
+    logger.info(f"Server started on 0.0.0.0:{dashboard_port_nr}")
+    _server.serve_forever()
 
 
 @atexit.register
 def stop() -> None:
     """
     Called when the program exits, will shutdown the server
     """
```

### Comparing `mpire-2.8.1/mpire/dashboard/templates/mpire.html` & `mpire-2.9.0/mpire/dashboard/templates/mpire.html`

 * *Files identical despite different names*

### Comparing `mpire-2.8.1/mpire/dashboard/templates/index.html` & `mpire-2.9.0/mpire/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `mpire-2.8.1/mpire/dashboard/templates/progress_bar.html` & `mpire-2.9.0/mpire/dashboard/templates/progress_bar.html`

 * *Files identical despite different names*

### Comparing `mpire-2.8.1/mpire/dashboard/connection_utils.py` & `mpire-2.9.0/mpire/dashboard/connection_utils.py`

 * *Files identical despite different names*

### Comparing `mpire-2.8.1/mpire/dashboard/manager.py` & `mpire-2.9.0/mpire/dashboard/manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -37,48 +37,44 @@
 def get_dashboard_tqdm_lock() -> Lock:
     """
     :return: Dashboard tqdm lock which should be used in a SyncManager context
     """
     return DASHBOARD_TQDM_LOCK
 
 
-def start_manager_server(port_range: Sequence = range(8080, 8100)) -> SyncManager:
+def start_manager_server(manager_port_nr: int) -> SyncManager:
     """
     Start a SyncManager
 
-    :param port_range: Port range to try. Reverses the list and will then pick the first one available
+    :param manager_port_nr: Port number to use for the manager
     :return: SyncManager
     """
-    for port_nr in reversed(port_range):
-        try:
-            # If a port is already occupied the SyncManager process will spit out EOFError and OSError messages. The
-            # former can be catched, but the latter will still show up. So we first check if a port is available
-            # manually
-            s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-            s.bind(('', port_nr))
-            s.close()
-
-            # Create manager
-            sm = SyncManager(address=("127.0.0.1", port_nr), authkey=b'mpire_dashboard')
-            sm.register('get_dashboard_tqdm_dict', get_dashboard_tqdm_dict)
-            sm.register('get_dashboard_tqdm_details_dict', get_dashboard_tqdm_details_dict)
-            sm.register('get_dashboard_tqdm_lock', get_dashboard_tqdm_lock)
-            sm.start(ignore_keyboard_interrupt)
-
-            # Set host and port number so other processes know where to connect to
-            DASHBOARD_MANAGER_HOST.value = b"127.0.0.1"
-            DASHBOARD_MANAGER_PORT.value = port_nr
-
-            return sm
-
-        except OSError:
-            # Port is occupied, ignore it and try another
-            pass
+    # Create manager
+    sm = SyncManager(address=("127.0.0.1", manager_port_nr), authkey=b'mpire_dashboard')
+    sm.register('get_dashboard_tqdm_dict', get_dashboard_tqdm_dict)
+    sm.register('get_dashboard_tqdm_details_dict', get_dashboard_tqdm_details_dict)
+    sm.register('get_dashboard_tqdm_lock', get_dashboard_tqdm_lock)
+    sm.start(ignore_keyboard_interrupt)
 
-    raise OSError(f"Dashboard Manager Server: All ports are in use: {port_range}")
+    # Set host and port number so other processes know where to connect to
+    DASHBOARD_MANAGER_HOST.value = b"127.0.0.1"
+    DASHBOARD_MANAGER_PORT.value = manager_port_nr
+
+    return sm
+
+
+def shutdown_manager_server(manager: SyncManager) -> None:
+    """
+    Shutdown a SyncManager
+    
+    :param manager: SyncManager to shutdown
+    """
+    manager.shutdown()
+    DASHBOARD_MANAGER_HOST.value = b""
+    DASHBOARD_MANAGER_PORT.value = 0
 
 
 def get_manager_client_dicts() -> Tuple[BaseProxy, BaseProxy, BaseProxy]:
     """
     Connect to a SyncManager and obtain the synchronized tqdm dashboard dicts
 
     :return: Synchronized tqdm dict, tqdm details dict, tqdm lock
```

### Comparing `mpire-2.8.1/mpire/insights.py` & `mpire-2.9.0/mpire/insights.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import ctypes
 import math
 import multiprocessing.context
-import multiprocessing.managers
+import os
 from datetime import datetime
 from functools import partial
 from typing import Dict, Optional, List, Tuple
 
-from mpire.context import RUNNING_WINDOWS
-from mpire.signal import ignore_keyboard_interrupt
-from mpire.utils import format_seconds
+from mpire.utils import PicklableSyncManager, format_seconds
 
 
 class WorkerInsights:
 
     """
     Worker insights class for profiling the worker start up time, waiting time and working time. When worker init and
     exit functions are provided it will time those as well.
@@ -62,33 +60,25 @@
     def reset_insights(self, enable_insights: bool) -> None:
         """
         Resets the insights containers
 
         :param enable_insights: Whether to enable worker insights
         """
         if enable_insights:
-            # When we're on Windows, we don't use a Manager as it's giving authentication errors. The max_task_args
-            # information is therefore not available on Windows systems. This needs to be fixed at some point in time
-            if not RUNNING_WINDOWS:
-                # We need to ignore the KeyboardInterrupt signal for the manager to avoid BrokenPipeErrors
-                self.insights_manager = multiprocessing.managers.SyncManager(ctx=self.ctx)
-                self.insights_manager.start(ignore_keyboard_interrupt)
+            self.insights_manager = PicklableSyncManager(authkey=os.urandom(24))
+            self.insights_manager.start()
             self.insights_manager_lock = self.ctx.Lock()
             self.worker_start_up_time = self.ctx.Array(ctypes.c_double, self.n_jobs, lock=False)
             self.worker_init_time = self.ctx.Array(ctypes.c_double, self.n_jobs, lock=False)
             self.worker_n_completed_tasks = self.ctx.Array(ctypes.c_int, self.n_jobs, lock=False)
             self.worker_waiting_time = self.ctx.Array(ctypes.c_double, self.n_jobs, lock=False)
             self.worker_working_time = self.ctx.Array(ctypes.c_double, self.n_jobs, lock=False)
             self.worker_exit_time = self.ctx.Array(ctypes.c_double, self.n_jobs, lock=False)
             self.max_task_duration = self.ctx.Array(ctypes.c_double, self.n_jobs * 5, lock=False)
-            if RUNNING_WINDOWS:
-                # Doesn't actually do anything, but reduces the amount of if/else statements in other code parts
-                self.max_task_args = [""] * self.n_jobs * 5
-            else:
-                self.max_task_args = self.insights_manager.list([""] * self.n_jobs * 5)
+            self.max_task_args = self.insights_manager.list([""] * self.n_jobs * 5)
         else:
             self.insights_manager = None
             self.insights_manager_lock = None
             self.worker_start_up_time = None
             self.worker_init_time = None
             self.worker_n_completed_tasks = None
             self.worker_waiting_time = None
@@ -144,27 +134,28 @@
             sorted for heapq
         :param force_update: Whether to force the update
         :return: Last updated datetime
         """
         now = datetime.now()
         if self.insights_enabled and (force_update or (now - max_task_duration_last_updated).total_seconds() > 2):
             task_durations, task_args = zip(*max_task_duration_list)
-            self.max_task_duration[worker_id * 5:(worker_id + 1) * 5] = task_durations
+            self.max_task_duration[worker_id * 5 : (worker_id + 1) * 5] = task_durations
             with self.insights_manager_lock:
-                self.max_task_args[worker_id * 5:(worker_id + 1) * 5] = task_args
+                self.max_task_args[worker_id * 5 : (worker_id + 1) * 5] = task_args
             max_task_duration_last_updated = now
 
         return max_task_duration_last_updated
 
     def get_insights(self) -> Dict:
         """
         Creates insights from the raw insight data
 
         :return: dictionary containing worker insights
         """
+
         def argsort(seq):
             """
             argsort, as to not be dependent on numpy, by
             https://stackoverflow.com/questions/3382352/equivalent-of-numpy-argsort-in-basic-python/3382369#3382369
             """
             return sorted(range(len(seq)), key=seq.__getitem__)
 
@@ -184,18 +175,18 @@
 
         # Determine max 5 tasks based on duration, exclude zero values and args that haven't been synced yet (empty str)
         sorted_idx = argsort(self.max_task_duration)[-5:][::-1]
         top_5_max_task_durations, top_5_max_task_args = [], []
         for idx in sorted_idx:
             if self.max_task_duration[idx] == 0:
                 break
-            if self.max_task_args[idx] == "" and not RUNNING_WINDOWS:
+            if self.max_task_args[idx] == "":
                 continue
             top_5_max_task_durations.append(format_seconds_func(self.max_task_duration[idx]))
-            top_5_max_task_args.append("" if RUNNING_WINDOWS else self.max_task_args[idx])
+            top_5_max_task_args.append(self.max_task_args[idx])
 
         # Populate
         total_start_up_time = sum(self.worker_start_up_time)
         total_init_time = sum(self.worker_init_time)
         total_waiting_time = sum(self.worker_waiting_time)
         total_working_time = sum(self.worker_working_time)
         total_exit_time = sum(self.worker_exit_time)
@@ -210,15 +201,15 @@
                         total_init_time=format_seconds_func(total_init_time),
                         total_waiting_time=format_seconds_func(total_waiting_time),
                         total_working_time=format_seconds_func(total_working_time),
                         total_exit_time=format_seconds_func(total_exit_time),
                         top_5_max_task_durations=top_5_max_task_durations,
                         top_5_max_task_args=top_5_max_task_args)
 
-        insights['total_time'] = format_seconds_func(total_time)
+        insights["total_time"] = format_seconds_func(total_time)
 
         # Calculate ratio, mean and standard deviation of different parts of the worker lifespan
         for part, total in (('start_up', total_start_up_time),
                             ('init', total_init_time),
                             ('waiting', total_waiting_time),
                             ('working', total_working_time),
                             ('exit', total_exit_time)):
@@ -265,13 +256,12 @@
                 worker_str.append(f"{part.replace('_', ' ')}: {insights[f'{part}_time'][worker_id]}s")
             insights_str.append(' - '.join(worker_str))
 
         # Add task stats
         insights_str.extend(["",
                              "Top 5 longest tasks",
                              "-------------------"])
-        max_task_duration_args_separator = "" if RUNNING_WINDOWS else " - "
         for task_idx, (duration, args) in enumerate(zip(insights['top_5_max_task_durations'],
                                                         insights['top_5_max_task_args']), start=1):
-            insights_str.append(f"{task_idx}. Time: {duration}{max_task_duration_args_separator}{args}")
+            insights_str.append(f"{task_idx}. Time: {duration} - {args}")
 
         return "\n".join(insights_str)
```

### Comparing `mpire-2.8.1/mpire/comms.py` & `mpire-2.9.0/mpire/comms.py`

 * *Files identical despite different names*

### Comparing `mpire-2.8.1/mpire/worker.py` & `mpire-2.9.0/mpire/worker.py`

 * *Files identical despite different names*

### Comparing `mpire-2.8.1/README.rst` & `mpire-2.9.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 - Intuitive, Pythonic syntax
 - Multiprocessing with ``map``/``map_unordered``/``imap``/``imap_unordered``/``apply``/``apply_async`` functions
 - Easy use of copy-on-write shared objects with a pool of workers (copy-on-write is only available for start method
   ``fork``)
 - Each worker can have its own state and with convenient worker init and exit functionality this state can be easily
   manipulated (e.g., to load a memory-intensive model only once for each worker without the need of sending it through a
   queue)
-- Progress bar support using tqdm_
+- Progress bar support using tqdm_ (``rich`` and notebook widgets are supported)
 - Progress dashboard support
 - Worker insights to provide insight into your multiprocessing efficiency
 - Graceful and user-friendly exception handling
 - Timeouts, including for worker init and exit functions
 - Automatic task chunking for all available map functions to speed up processing of small task queues (including numpy
   arrays)
 - Adjustable maximum number of active tasks to avoid memory problems
```

