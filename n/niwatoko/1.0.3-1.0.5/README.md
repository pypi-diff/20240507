# Comparing `tmp/niwatoko-1.0.3.tar.gz` & `tmp/niwatoko-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niwatoko-1.0.3.tar", last modified: Tue May  7 08:15:44 2024, max compression
+gzip compressed data, was "niwatoko-1.0.5.tar", last modified: Tue May  7 08:22:37 2024, max compression
```

## Comparing `niwatoko-1.0.3.tar` & `niwatoko-1.0.5.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:15:44.027844 niwatoko-1.0.3/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    11356 2024-05-07 05:52:57.000000 niwatoko-1.0.3/LICENSE
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16804 2024-05-07 08:15:44.027658 niwatoko-1.0.3/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    15918 2024-05-07 02:46:41.000000 niwatoko-1.0.3/README.md
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:15:44.025236 niwatoko-1.0.3/niwatoko/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 05:52:23.000000 niwatoko-1.0.3/niwatoko/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2096 2024-05-07 06:53:37.000000 niwatoko-1.0.3/niwatoko/cli.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:15:44.024427 niwatoko-1.0.3/niwatoko/foundation_model/
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:15:44.024462 niwatoko-1.0.3/niwatoko/foundation_model/interpretation/
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:15:44.026388 niwatoko-1.0.3/niwatoko/foundation_model/interpretation/llm/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1075 2024-05-07 06:49:11.000000 niwatoko-1.0.3/niwatoko/foundation_model/interpretation/llm/claude.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1149 2024-05-07 06:53:25.000000 niwatoko-1.0.3/niwatoko/foundation_model/interpretation/llm/gpt.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:15:44.026049 niwatoko-1.0.3/niwatoko.egg-info/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16804 2024-05-07 08:15:43.000000 niwatoko-1.0.3/niwatoko.egg-info/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      457 2024-05-07 08:15:43.000000 niwatoko-1.0.3/niwatoko.egg-info/SOURCES.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-07 08:15:43.000000 niwatoko-1.0.3/niwatoko.egg-info/dependency_links.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-07 08:15:43.000000 niwatoko-1.0.3/niwatoko.egg-info/entry_points.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       34 2024-05-07 08:15:43.000000 niwatoko-1.0.3/niwatoko.egg-info/requires.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       15 2024-05-07 08:15:43.000000 niwatoko-1.0.3/niwatoko.egg-info/top_level.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-07 08:15:44.027883 niwatoko-1.0.3/setup.cfg
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1593 2024-05-07 08:15:39.000000 niwatoko-1.0.3/setup.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:15:44.027082 niwatoko-1.0.3/tests/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-07 02:46:41.000000 niwatoko-1.0.3/tests/__init__.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:15:44.027343 niwatoko-1.0.3/tests/test_docs/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-07 02:46:41.000000 niwatoko-1.0.3/tests/test_docs/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-07 02:46:41.000000 niwatoko-1.0.3/tests/test_interpreter.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-07 02:46:41.000000 niwatoko-1.0.3/tests/test_parser.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:22:37.548078 niwatoko-1.0.5/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    11356 2024-05-07 05:52:57.000000 niwatoko-1.0.5/LICENSE
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16804 2024-05-07 08:22:37.547931 niwatoko-1.0.5/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    15918 2024-05-07 02:46:41.000000 niwatoko-1.0.5/README.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:22:37.545476 niwatoko-1.0.5/niwatoko/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 05:52:23.000000 niwatoko-1.0.5/niwatoko/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2096 2024-05-07 06:53:37.000000 niwatoko-1.0.5/niwatoko/cli.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:22:37.544632 niwatoko-1.0.5/niwatoko/foundation_model/
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:22:37.544668 niwatoko-1.0.5/niwatoko/foundation_model/interpretation/
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:22:37.546606 niwatoko-1.0.5/niwatoko/foundation_model/interpretation/llm/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1075 2024-05-07 06:49:11.000000 niwatoko-1.0.5/niwatoko/foundation_model/interpretation/llm/claude.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1149 2024-05-07 06:53:25.000000 niwatoko-1.0.5/niwatoko/foundation_model/interpretation/llm/gpt.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:22:37.546832 niwatoko-1.0.5/niwatoko/grammar/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      481 2024-05-07 05:52:23.000000 niwatoko-1.0.5/niwatoko/grammar/system.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:22:37.546271 niwatoko-1.0.5/niwatoko.egg-info/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16804 2024-05-07 08:22:37.000000 niwatoko-1.0.5/niwatoko.egg-info/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      484 2024-05-07 08:22:37.000000 niwatoko-1.0.5/niwatoko.egg-info/SOURCES.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-07 08:22:37.000000 niwatoko-1.0.5/niwatoko.egg-info/dependency_links.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-07 08:22:37.000000 niwatoko-1.0.5/niwatoko.egg-info/entry_points.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       34 2024-05-07 08:22:37.000000 niwatoko-1.0.5/niwatoko.egg-info/requires.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       15 2024-05-07 08:22:37.000000 niwatoko-1.0.5/niwatoko.egg-info/top_level.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-07 08:22:37.548114 niwatoko-1.0.5/setup.cfg
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1628 2024-05-07 08:21:50.000000 niwatoko-1.0.5/setup.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:22:37.547410 niwatoko-1.0.5/tests/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-07 02:46:41.000000 niwatoko-1.0.5/tests/__init__.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:22:37.547705 niwatoko-1.0.5/tests/test_docs/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-07 02:46:41.000000 niwatoko-1.0.5/tests/test_docs/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-07 02:46:41.000000 niwatoko-1.0.5/tests/test_interpreter.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-07 02:46:41.000000 niwatoko-1.0.5/tests/test_parser.py
```

### Comparing `niwatoko-1.0.3/LICENSE` & `niwatoko-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.3/PKG-INFO` & `niwatoko-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.0.3
+Version: 1.0.5
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
```

### Comparing `niwatoko-1.0.3/README.md` & `niwatoko-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.3/niwatoko/cli.py` & `niwatoko-1.0.5/niwatoko/cli.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.3/niwatoko/foundation_model/interpretation/llm/claude.py` & `niwatoko-1.0.5/niwatoko/foundation_model/interpretation/llm/claude.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.3/niwatoko/foundation_model/interpretation/llm/gpt.py` & `niwatoko-1.0.5/niwatoko/foundation_model/interpretation/llm/gpt.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.3/niwatoko.egg-info/PKG-INFO` & `niwatoko-1.0.5/niwatoko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.0.3
+Version: 1.0.5
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
```

### Comparing `niwatoko-1.0.3/setup.py` & `niwatoko-1.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # niwatoko - 自然言語プログラミング言語のPythonパッケージのsetup.pyファイルです。
 # このファイルはパッケージのインストールや配布に必要な情報を含んでいます。
 
 from setuptools import setup, find_packages
 
 setup(
     name='niwatoko',
-    version='1.0.3',
+    version='1.0.5',
     description='自然言語でプログラミングを行うことができる新しいプログラミング言語',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='dai-motoki',
     author_email='dai.motoki1123@gmail.com',
     url='https://niwatoko2.vercel.app/',
     packages=find_packages(),
@@ -36,10 +36,11 @@
     python_requires='>=3.7',
     entry_points={
         'console_scripts': [
             'niwatoko=niwatoko.cli:main',
         ],
     },
     package_data={
-        'niwatoko': ['foundation_model/interpretation/llm/*'],
+        'niwatoko': ['foundation_model/interpretation/llm/*', 
+                     'grammar/*'],
     },
 )
```

### Comparing `niwatoko-1.0.3/tests/__init__.py` & `niwatoko-1.0.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.3/tests/test_docs/__init__.py` & `niwatoko-1.0.5/tests/test_docs/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.3/tests/test_interpreter.py` & `niwatoko-1.0.5/tests/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.3/tests/test_parser.py` & `niwatoko-1.0.5/tests/test_parser.py`

 * *Files identical despite different names*

