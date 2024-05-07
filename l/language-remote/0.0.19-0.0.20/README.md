# Comparing `tmp/language_remote-0.0.19.tar.gz` & `tmp/language_remote-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "language_remote-0.0.19.tar", last modified: Tue May  7 13:07:48 2024, max compression
+gzip compressed data, was "language_remote-0.0.20.tar", last modified: Tue May  7 20:37:21 2024, max compression
```

## Comparing `language_remote-0.0.19.tar` & `language_remote-0.0.20.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:07:48.148207 language_remote-0.0.19/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-07 13:07:48.144207 language_remote-0.0.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-07 13:07:29.000000 language_remote-0.0.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:07:48.144207 language_remote-0.0.19/language_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:07:48.144207 language_remote-0.0.19/language_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:07:29.000000 language_remote-0.0.19/language_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-07 13:07:29.000000 language_remote-0.0.19/language_remote/src/lang_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-07 13:07:29.000000 language_remote-0.0.19/language_remote/src/language_code_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:07:48.144207 language_remote-0.0.19/language_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-07 13:07:48.000000 language_remote-0.0.19/language_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-07 13:07:48.000000 language_remote-0.0.19/language_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:07:48.000000 language_remote-0.0.19/language_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 13:07:48.000000 language_remote-0.0.19/language_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 13:07:48.000000 language_remote-0.0.19/language_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-07 13:07:29.000000 language_remote-0.0.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 13:07:48.148207 language_remote-0.0.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-07 13:07:29.000000 language_remote-0.0.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:37:21.405856 language_remote-0.0.20/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-07 20:37:21.405856 language_remote-0.0.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-07 20:37:02.000000 language_remote-0.0.20/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:37:21.405856 language_remote-0.0.20/language_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:37:21.405856 language_remote-0.0.20/language_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:37:02.000000 language_remote-0.0.20/language_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-07 20:37:02.000000 language_remote-0.0.20/language_remote/src/lang_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-07 20:37:02.000000 language_remote-0.0.20/language_remote/src/language_code_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:37:21.405856 language_remote-0.0.20/language_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-07 20:37:21.000000 language_remote-0.0.20/language_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-07 20:37:21.000000 language_remote-0.0.20/language_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:37:21.000000 language_remote-0.0.20/language_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 20:37:21.000000 language_remote-0.0.20/language_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 20:37:21.000000 language_remote-0.0.20/language_remote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-07 20:37:02.000000 language_remote-0.0.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 20:37:21.405856 language_remote-0.0.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-07 20:37:02.000000 language_remote-0.0.20/setup.py
```

### Comparing `language_remote-0.0.19/README.md` & `language_remote-0.0.20/README.md`

 * *Files identical despite different names*

### Comparing `language_remote-0.0.19/language_remote/src/lang_code.py` & `language_remote-0.0.20/language_remote/src/lang_code.py`

 * *Files identical despite different names*

### Comparing `language_remote-0.0.19/language_remote/src/language_code_constants.py` & `language_remote-0.0.20/language_remote/src/language_code_constants.py`

 * *Files identical despite different names*

### Comparing `language_remote-0.0.19/setup.py` & `language_remote-0.0.20/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "language-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/language-remote
-    version='0.0.19',
+    version='0.0.20',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Language Remote",
```

