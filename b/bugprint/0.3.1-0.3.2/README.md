# Comparing `tmp/bugprint-0.3.1.tar.gz` & `tmp/bugprint-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bugprint-0.3.1.tar", last modified: Tue May  7 01:24:52 2024, max compression
+gzip compressed data, was "bugprint-0.3.2.tar", last modified: Tue May  7 01:56:09 2024, max compression
```

## Comparing `bugprint-0.3.1.tar` & `bugprint-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 erikluu    (501) staff       (20)        0 2024-05-07 01:24:52.112466 bugprint-0.3.1/
--rw-r--r--   0 erikluu    (501) staff       (20)     1074 2024-05-07 01:12:25.000000 bugprint-0.3.1/LICENSE
--rw-r--r--   0 erikluu    (501) staff       (20)      431 2024-05-07 01:24:52.112256 bugprint-0.3.1/PKG-INFO
--rw-r--r--   0 erikluu    (501) staff       (20)      355 2024-05-07 01:13:48.000000 bugprint-0.3.1/README.md
-drwxr-xr-x   0 erikluu    (501) staff       (20)        0 2024-05-07 01:24:52.111072 bugprint-0.3.1/bugprint/
--rw-r--r--   0 erikluu    (501) staff       (20)       22 2024-05-07 01:22:47.000000 bugprint-0.3.1/bugprint/__init__.py
--rw-r--r--   0 erikluu    (501) staff       (20)      295 2024-05-07 00:38:51.000000 bugprint-0.3.1/bugprint/funcs.py
-drwxr-xr-x   0 erikluu    (501) staff       (20)        0 2024-05-07 01:24:52.112024 bugprint-0.3.1/bugprint.egg-info/
--rw-r--r--   0 erikluu    (501) staff       (20)      431 2024-05-07 01:24:52.000000 bugprint-0.3.1/bugprint.egg-info/PKG-INFO
--rw-r--r--   0 erikluu    (501) staff       (20)      193 2024-05-07 01:24:52.000000 bugprint-0.3.1/bugprint.egg-info/SOURCES.txt
--rw-r--r--   0 erikluu    (501) staff       (20)        1 2024-05-07 01:24:52.000000 bugprint-0.3.1/bugprint.egg-info/dependency_links.txt
--rw-r--r--   0 erikluu    (501) staff       (20)        9 2024-05-07 01:24:52.000000 bugprint-0.3.1/bugprint.egg-info/top_level.txt
--rw-r--r--   0 erikluu    (501) staff       (20)       38 2024-05-07 01:24:52.112509 bugprint-0.3.1/setup.cfg
--rw-r--r--   0 erikluu    (501) staff       (20)      820 2024-05-07 01:24:45.000000 bugprint-0.3.1/setup.py
+drwxr-xr-x   0 erikluu    (501) staff       (20)        0 2024-05-07 01:56:09.072355 bugprint-0.3.2/
+-rw-r--r--   0 erikluu    (501) staff       (20)     1074 2024-05-07 01:12:25.000000 bugprint-0.3.2/LICENSE
+-rw-r--r--   0 erikluu    (501) staff       (20)     1021 2024-05-07 01:56:09.071898 bugprint-0.3.2/PKG-INFO
+-rw-r--r--   0 erikluu    (501) staff       (20)      501 2024-05-07 01:29:28.000000 bugprint-0.3.2/README.md
+drwxr-xr-x   0 erikluu    (501) staff       (20)        0 2024-05-07 01:56:09.070444 bugprint-0.3.2/bugprint/
+-rw-r--r--   0 erikluu    (501) staff       (20)       32 2024-05-07 01:51:02.000000 bugprint-0.3.2/bugprint/__init__.py
+-rw-r--r--   0 erikluu    (501) staff       (20)      467 2024-05-07 01:54:13.000000 bugprint-0.3.2/bugprint/funcs.py
+drwxr-xr-x   0 erikluu    (501) staff       (20)        0 2024-05-07 01:56:09.071571 bugprint-0.3.2/bugprint.egg-info/
+-rw-r--r--   0 erikluu    (501) staff       (20)     1021 2024-05-07 01:56:09.000000 bugprint-0.3.2/bugprint.egg-info/PKG-INFO
+-rw-r--r--   0 erikluu    (501) staff       (20)      193 2024-05-07 01:56:09.000000 bugprint-0.3.2/bugprint.egg-info/SOURCES.txt
+-rw-r--r--   0 erikluu    (501) staff       (20)        1 2024-05-07 01:56:09.000000 bugprint-0.3.2/bugprint.egg-info/dependency_links.txt
+-rw-r--r--   0 erikluu    (501) staff       (20)        9 2024-05-07 01:56:09.000000 bugprint-0.3.2/bugprint.egg-info/top_level.txt
+-rw-r--r--   0 erikluu    (501) staff       (20)       38 2024-05-07 01:56:09.072417 bugprint-0.3.2/setup.cfg
+-rw-r--r--   0 erikluu    (501) staff       (20)      957 2024-05-07 01:56:08.000000 bugprint-0.3.2/setup.py
```

### Comparing `bugprint-0.3.1/LICENSE` & `bugprint-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bugprint-0.3.1/setup.py` & `bugprint-0.3.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,26 +3,29 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.3.1'
+VERSION = '0.3.2'
 DESCRIPTION = 'Debug printing made easy.'
 
 # Setting up
 setup(
     name="bugprint",
     version=VERSION,
     author="Erik Luu",
     author_email="eeluu19@gmail.com",
     description=DESCRIPTION,
+    long_description_content_type="text/markdown",
+    long_description=long_description,
     packages=find_packages(),
     install_requires=[''],
+    url="https://github.com/erikluu/bugprint",
     license="MIT",
     keywords=['python', 'debug', 'print'],
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

