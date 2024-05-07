# Comparing `tmp/niwatoko-1.0.5.tar.gz` & `tmp/niwatoko-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niwatoko-1.0.5.tar", last modified: Tue May  7 08:22:37 2024, max compression
+gzip compressed data, was "niwatoko-1.0.6.tar", last modified: Tue May  7 08:24:42 2024, max compression
```

## Comparing `niwatoko-1.0.5.tar` & `niwatoko-1.0.6.tar`

### file list

```diff
@@ -1,29 +1,37 @@
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:22:37.548078 niwatoko-1.0.5/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    11356 2024-05-07 05:52:57.000000 niwatoko-1.0.5/LICENSE
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16804 2024-05-07 08:22:37.547931 niwatoko-1.0.5/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    15918 2024-05-07 02:46:41.000000 niwatoko-1.0.5/README.md
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:22:37.545476 niwatoko-1.0.5/niwatoko/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 05:52:23.000000 niwatoko-1.0.5/niwatoko/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2096 2024-05-07 06:53:37.000000 niwatoko-1.0.5/niwatoko/cli.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:22:37.544632 niwatoko-1.0.5/niwatoko/foundation_model/
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:22:37.544668 niwatoko-1.0.5/niwatoko/foundation_model/interpretation/
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:22:37.546606 niwatoko-1.0.5/niwatoko/foundation_model/interpretation/llm/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1075 2024-05-07 06:49:11.000000 niwatoko-1.0.5/niwatoko/foundation_model/interpretation/llm/claude.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1149 2024-05-07 06:53:25.000000 niwatoko-1.0.5/niwatoko/foundation_model/interpretation/llm/gpt.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:22:37.546832 niwatoko-1.0.5/niwatoko/grammar/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      481 2024-05-07 05:52:23.000000 niwatoko-1.0.5/niwatoko/grammar/system.md
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:22:37.546271 niwatoko-1.0.5/niwatoko.egg-info/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16804 2024-05-07 08:22:37.000000 niwatoko-1.0.5/niwatoko.egg-info/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      484 2024-05-07 08:22:37.000000 niwatoko-1.0.5/niwatoko.egg-info/SOURCES.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-07 08:22:37.000000 niwatoko-1.0.5/niwatoko.egg-info/dependency_links.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-07 08:22:37.000000 niwatoko-1.0.5/niwatoko.egg-info/entry_points.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       34 2024-05-07 08:22:37.000000 niwatoko-1.0.5/niwatoko.egg-info/requires.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       15 2024-05-07 08:22:37.000000 niwatoko-1.0.5/niwatoko.egg-info/top_level.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-07 08:22:37.548114 niwatoko-1.0.5/setup.cfg
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1628 2024-05-07 08:21:50.000000 niwatoko-1.0.5/setup.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:22:37.547410 niwatoko-1.0.5/tests/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-07 02:46:41.000000 niwatoko-1.0.5/tests/__init__.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:22:37.547705 niwatoko-1.0.5/tests/test_docs/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-07 02:46:41.000000 niwatoko-1.0.5/tests/test_docs/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-07 02:46:41.000000 niwatoko-1.0.5/tests/test_interpreter.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-07 02:46:41.000000 niwatoko-1.0.5/tests/test_parser.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:24:42.575955 niwatoko-1.0.6/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    11356 2024-05-07 05:52:57.000000 niwatoko-1.0.6/LICENSE
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16804 2024-05-07 08:24:42.575749 niwatoko-1.0.6/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    15918 2024-05-07 02:46:41.000000 niwatoko-1.0.6/README.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:24:42.570517 niwatoko-1.0.6/niwatoko/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 05:52:23.000000 niwatoko-1.0.6/niwatoko/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2096 2024-05-07 06:53:37.000000 niwatoko-1.0.6/niwatoko/cli.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:24:42.569608 niwatoko-1.0.6/niwatoko/foundation_model/
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:24:42.569647 niwatoko-1.0.6/niwatoko/foundation_model/interpretation/
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:24:42.571880 niwatoko-1.0.6/niwatoko/foundation_model/interpretation/llm/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1075 2024-05-07 06:49:11.000000 niwatoko-1.0.6/niwatoko/foundation_model/interpretation/llm/claude.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1149 2024-05-07 06:53:25.000000 niwatoko-1.0.6/niwatoko/foundation_model/interpretation/llm/gpt.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:24:42.572139 niwatoko-1.0.6/niwatoko/grammar/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      481 2024-05-07 05:52:23.000000 niwatoko-1.0.6/niwatoko/grammar/system.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:24:42.571368 niwatoko-1.0.6/niwatoko.egg-info/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16804 2024-05-07 08:24:42.000000 niwatoko-1.0.6/niwatoko.egg-info/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      769 2024-05-07 08:24:42.000000 niwatoko-1.0.6/niwatoko.egg-info/SOURCES.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-07 08:24:42.000000 niwatoko-1.0.6/niwatoko.egg-info/dependency_links.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-07 08:24:42.000000 niwatoko-1.0.6/niwatoko.egg-info/entry_points.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       34 2024-05-07 08:24:42.000000 niwatoko-1.0.6/niwatoko.egg-info/requires.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       15 2024-05-07 08:24:42.000000 niwatoko-1.0.6/niwatoko.egg-info/top_level.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-07 08:24:42.576006 niwatoko-1.0.6/setup.cfg
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1697 2024-05-07 08:24:25.000000 niwatoko-1.0.6/setup.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:24:42.572942 niwatoko-1.0.6/tests/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-07 02:46:41.000000 niwatoko-1.0.6/tests/__init__.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:24:42.575248 niwatoko-1.0.6/tests/test_docs/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-07 02:46:41.000000 niwatoko-1.0.6/tests/test_docs/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2609 2024-05-07 05:48:44.000000 niwatoko-1.0.6/tests/test_docs/test_doc1.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2853 2024-05-07 05:48:44.000000 niwatoko-1.0.6/tests/test_docs/test_doc2.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2625 2024-05-07 05:48:44.000000 niwatoko-1.0.6/tests/test_docs/test_doc3.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1678 2024-05-07 06:18:12.000000 niwatoko-1.0.6/tests/test_docs/test_gen_github_issue.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1950 2024-05-07 07:00:44.000000 niwatoko-1.0.6/tests/test_docs/test_gen_grimoire.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1909 2024-05-07 06:33:47.000000 niwatoko-1.0.6/tests/test_docs/test_gen_grimoire2.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1850 2024-05-07 07:04:51.000000 niwatoko-1.0.6/tests/test_docs/test_gen_grimoire_en.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5307 2024-05-07 05:52:23.000000 niwatoko-1.0.6/tests/test_docs/test_gen_zoltraak_pypi.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-07 02:46:41.000000 niwatoko-1.0.6/tests/test_interpreter.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-07 02:46:41.000000 niwatoko-1.0.6/tests/test_parser.py
```

### Comparing `niwatoko-1.0.5/LICENSE` & `niwatoko-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.5/PKG-INFO` & `niwatoko-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.0.5
+Version: 1.0.6
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
```

### Comparing `niwatoko-1.0.5/README.md` & `niwatoko-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.5/niwatoko/cli.py` & `niwatoko-1.0.6/niwatoko/cli.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.5/niwatoko/foundation_model/interpretation/llm/claude.py` & `niwatoko-1.0.6/niwatoko/foundation_model/interpretation/llm/claude.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.5/niwatoko/foundation_model/interpretation/llm/gpt.py` & `niwatoko-1.0.6/niwatoko/foundation_model/interpretation/llm/gpt.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.5/niwatoko.egg-info/PKG-INFO` & `niwatoko-1.0.6/niwatoko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.0.5
+Version: 1.0.6
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
```

### Comparing `niwatoko-1.0.5/setup.py` & `niwatoko-1.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # niwatoko - 自然言語プログラミング言語のPythonパッケージのsetup.pyファイルです。
 # このファイルはパッケージのインストールや配布に必要な情報を含んでいます。
 
 from setuptools import setup, find_packages
 
 setup(
     name='niwatoko',
-    version='1.0.5',
+    version='1.0.6',
     description='自然言語でプログラミングを行うことができる新しいプログラミング言語',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='dai-motoki',
     author_email='dai.motoki1123@gmail.com',
     url='https://niwatoko2.vercel.app/',
     packages=find_packages(),
@@ -36,11 +36,12 @@
     python_requires='>=3.7',
     entry_points={
         'console_scripts': [
             'niwatoko=niwatoko.cli:main',
         ],
     },
     package_data={
+        '': ['*.txt', '*.md', '*.json', '*.csv', '*.yaml', '*.yml'],
         'niwatoko': ['foundation_model/interpretation/llm/*', 
                      'grammar/*'],
     },
 )
```

### Comparing `niwatoko-1.0.5/tests/__init__.py` & `niwatoko-1.0.6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.5/tests/test_docs/__init__.py` & `niwatoko-1.0.6/tests/test_docs/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.5/tests/test_interpreter.py` & `niwatoko-1.0.6/tests/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.5/tests/test_parser.py` & `niwatoko-1.0.6/tests/test_parser.py`

 * *Files identical despite different names*

