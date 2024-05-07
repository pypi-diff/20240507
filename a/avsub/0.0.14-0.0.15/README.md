# Comparing `tmp/avsub-0.0.14.tar.gz` & `tmp/avsub-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avsub-0.0.14.tar", last modified: Mon Apr 29 04:24:07 2024, max compression
+gzip compressed data, was "avsub-0.0.15.tar", last modified: Tue May  7 14:55:17 2024, max compression
```

## Comparing `avsub-0.0.14.tar` & `avsub-0.0.15.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 serhat    (1000) serhat    (1000)        0 2024-04-29 04:24:07.943363 avsub-0.0.14/
--rw-r--r--   0 serhat    (1000) serhat    (1000)    35149 2024-04-29 04:22:03.000000 avsub-0.0.14/LICENSE
--rw-r--r--   0 serhat    (1000) serhat    (1000)      833 2024-04-29 04:24:07.940029 avsub-0.0.14/PKG-INFO
-drwxr-xr-x   0 serhat    (1000) serhat    (1000)        0 2024-04-29 04:24:07.940029 avsub-0.0.14/avsub/
--rw-r--r--   0 serhat    (1000) serhat    (1000)        0 2024-04-29 04:22:03.000000 avsub-0.0.14/avsub/__init__.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)     3776 2024-04-29 04:22:03.000000 avsub-0.0.14/avsub/__main__.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)       79 2024-04-29 04:22:03.000000 avsub-0.0.14/avsub/__version__.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)      437 2024-04-29 04:22:03.000000 avsub-0.0.14/avsub/actions.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)     5785 2024-04-29 04:22:03.000000 avsub-0.0.14/avsub/cli.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)      703 2024-04-29 04:22:03.000000 avsub-0.0.14/avsub/consts.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)     3981 2024-04-29 04:22:03.000000 avsub-0.0.14/avsub/ffmpeg.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)      202 2024-04-29 04:22:03.000000 avsub-0.0.14/avsub/globs.py
--rw-r--r--   0 serhat    (1000) serhat    (1000)     1456 2024-04-29 04:22:03.000000 avsub-0.0.14/avsub/utils.py
-drwxr-xr-x   0 serhat    (1000) serhat    (1000)        0 2024-04-29 04:24:07.940029 avsub-0.0.14/avsub.egg-info/
--rw-r--r--   0 serhat    (1000) serhat    (1000)      833 2024-04-29 04:24:07.000000 avsub-0.0.14/avsub.egg-info/PKG-INFO
--rw-r--r--   0 serhat    (1000) serhat    (1000)      347 2024-04-29 04:24:07.000000 avsub-0.0.14/avsub.egg-info/SOURCES.txt
--rw-r--r--   0 serhat    (1000) serhat    (1000)        1 2024-04-29 04:24:07.000000 avsub-0.0.14/avsub.egg-info/dependency_links.txt
--rw-r--r--   0 serhat    (1000) serhat    (1000)       46 2024-04-29 04:24:07.000000 avsub-0.0.14/avsub.egg-info/entry_points.txt
--rw-r--r--   0 serhat    (1000) serhat    (1000)        1 2024-04-29 04:24:07.000000 avsub-0.0.14/avsub.egg-info/not-zip-safe
--rw-r--r--   0 serhat    (1000) serhat    (1000)        6 2024-04-29 04:24:07.000000 avsub-0.0.14/avsub.egg-info/top_level.txt
--rw-r--r--   0 serhat    (1000) serhat    (1000)     1066 2024-04-29 04:22:03.000000 avsub-0.0.14/pyproject.toml
--rw-r--r--   0 serhat    (1000) serhat    (1000)       38 2024-04-29 04:24:07.943363 avsub-0.0.14/setup.cfg
+drwxr-xr-x   0 serhat    (1000) serhat    (1000)        0 2024-05-07 14:55:17.109498 avsub-0.0.15/
+-rw-r--r--   0 serhat    (1000) serhat    (1000)    35149 2024-05-07 14:55:08.000000 avsub-0.0.15/LICENSE
+-rw-r--r--   0 serhat    (1000) serhat    (1000)      675 2024-05-07 14:55:17.109498 avsub-0.0.15/PKG-INFO
+drwxr-xr-x   0 serhat    (1000) serhat    (1000)        0 2024-05-07 14:55:17.106165 avsub-0.0.15/avsub/
+-rw-r--r--   0 serhat    (1000) serhat    (1000)        0 2024-05-07 14:55:08.000000 avsub-0.0.15/avsub/__init__.py
+-rw-r--r--   0 serhat    (1000) serhat    (1000)     3776 2024-05-07 14:55:08.000000 avsub-0.0.15/avsub/__main__.py
+-rw-r--r--   0 serhat    (1000) serhat    (1000)       79 2024-05-07 14:55:08.000000 avsub-0.0.15/avsub/__version__.py
+-rw-r--r--   0 serhat    (1000) serhat    (1000)      437 2024-05-07 14:55:08.000000 avsub-0.0.15/avsub/actions.py
+-rw-r--r--   0 serhat    (1000) serhat    (1000)     5785 2024-05-07 14:55:08.000000 avsub-0.0.15/avsub/cli.py
+-rw-r--r--   0 serhat    (1000) serhat    (1000)      703 2024-05-07 14:55:08.000000 avsub-0.0.15/avsub/consts.py
+-rw-r--r--   0 serhat    (1000) serhat    (1000)     3981 2024-05-07 14:55:08.000000 avsub-0.0.15/avsub/ffmpeg.py
+-rw-r--r--   0 serhat    (1000) serhat    (1000)      202 2024-05-07 14:55:08.000000 avsub-0.0.15/avsub/globs.py
+-rw-r--r--   0 serhat    (1000) serhat    (1000)     1456 2024-05-07 14:55:08.000000 avsub-0.0.15/avsub/utils.py
+drwxr-xr-x   0 serhat    (1000) serhat    (1000)        0 2024-05-07 14:55:17.109498 avsub-0.0.15/avsub.egg-info/
+-rw-r--r--   0 serhat    (1000) serhat    (1000)      675 2024-05-07 14:55:17.000000 avsub-0.0.15/avsub.egg-info/PKG-INFO
+-rw-r--r--   0 serhat    (1000) serhat    (1000)      347 2024-05-07 14:55:17.000000 avsub-0.0.15/avsub.egg-info/SOURCES.txt
+-rw-r--r--   0 serhat    (1000) serhat    (1000)        1 2024-05-07 14:55:17.000000 avsub-0.0.15/avsub.egg-info/dependency_links.txt
+-rw-r--r--   0 serhat    (1000) serhat    (1000)       46 2024-05-07 14:55:17.000000 avsub-0.0.15/avsub.egg-info/entry_points.txt
+-rw-r--r--   0 serhat    (1000) serhat    (1000)        1 2024-05-07 14:55:16.000000 avsub-0.0.15/avsub.egg-info/not-zip-safe
+-rw-r--r--   0 serhat    (1000) serhat    (1000)        6 2024-05-07 14:55:17.000000 avsub-0.0.15/avsub.egg-info/top_level.txt
+-rw-r--r--   0 serhat    (1000) serhat    (1000)      922 2024-05-07 14:55:08.000000 avsub-0.0.15/pyproject.toml
+-rw-r--r--   0 serhat    (1000) serhat    (1000)       38 2024-05-07 14:55:17.109498 avsub-0.0.15/setup.cfg
```

### Comparing `avsub-0.0.14/LICENSE` & `avsub-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `avsub-0.0.14/avsub/__main__.py` & `avsub-0.0.15/avsub/__main__.py`

 * *Files identical despite different names*

### Comparing `avsub-0.0.14/avsub/cli.py` & `avsub-0.0.15/avsub/cli.py`

 * *Files identical despite different names*

### Comparing `avsub-0.0.14/avsub/consts.py` & `avsub-0.0.15/avsub/consts.py`

 * *Files identical despite different names*

### Comparing `avsub-0.0.14/avsub/ffmpeg.py` & `avsub-0.0.15/avsub/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `avsub-0.0.14/avsub/utils.py` & `avsub-0.0.15/avsub/utils.py`

 * *Files identical despite different names*

### Comparing `avsub-0.0.14/pyproject.toml` & `avsub-0.0.15/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,27 +2,24 @@
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'avsub'
 authors = [{name = 'Serhat Çelik'}]
 description = 'A simplified command-line interface for FFmpeg'
-requires-python = '>=3.9, <3.12'
+requires-python = '~=3.9'
 keywords = ['avsub', 'audio', 'video', 'subtitle', 'ffmpeg']
 license = {text = 'GPLv3'}
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Console',
     'Intended Audience :: End Users/Desktop',
     'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3 :: Only',
-    'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3.10',
-    'Programming Language :: Python :: 3.11',
     'Topic :: Multimedia',
     'Topic :: Multimedia :: Sound/Audio',
     'Topic :: Multimedia :: Video',
 ]
 dynamic = ['version']
 
 [project.scripts]
```

