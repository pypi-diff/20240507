# Comparing `tmp/niwatoko-1.0.0.tar.gz` & `tmp/niwatoko-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niwatoko-1.0.0.tar", last modified: Tue May  7 02:24:03 2024, max compression
+gzip compressed data, was "niwatoko-1.0.1.tar", last modified: Tue May  7 02:25:58 2024, max compression
```

## Comparing `niwatoko-1.0.0.tar` & `niwatoko-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 02:24:03.174944 niwatoko-1.0.0/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2807 2024-05-06 13:47:27.000000 niwatoko-1.0.0/LICENSE
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16702 2024-05-07 02:24:03.174758 niwatoko-1.0.0/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    15918 2024-05-07 01:32:03.000000 niwatoko-1.0.0/README.md
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 02:24:03.173603 niwatoko-1.0.0/niwatoko.egg-info/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16702 2024-05-07 02:24:03.000000 niwatoko-1.0.0/niwatoko.egg-info/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      313 2024-05-07 02:24:03.000000 niwatoko-1.0.0/niwatoko.egg-info/SOURCES.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-07 02:24:03.000000 niwatoko-1.0.0/niwatoko.egg-info/dependency_links.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-07 02:24:03.000000 niwatoko-1.0.0/niwatoko.egg-info/entry_points.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       17 2024-05-07 02:24:03.000000 niwatoko-1.0.0/niwatoko.egg-info/requires.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        6 2024-05-07 02:24:03.000000 niwatoko-1.0.0/niwatoko.egg-info/top_level.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-07 02:24:03.174976 niwatoko-1.0.0/setup.cfg
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1364 2024-05-07 02:23:53.000000 niwatoko-1.0.0/setup.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 02:24:03.174177 niwatoko-1.0.0/tests/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-06 13:44:44.000000 niwatoko-1.0.0/tests/__init__.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 02:24:03.174427 niwatoko-1.0.0/tests/test_docs/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-06 13:45:38.000000 niwatoko-1.0.0/tests/test_docs/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-06 13:44:55.000000 niwatoko-1.0.0/tests/test_interpreter.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-06 13:44:49.000000 niwatoko-1.0.0/tests/test_parser.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 02:25:58.820341 niwatoko-1.0.1/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2807 2024-05-06 13:47:27.000000 niwatoko-1.0.1/LICENSE
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16804 2024-05-07 02:25:58.819781 niwatoko-1.0.1/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    15918 2024-05-07 01:32:03.000000 niwatoko-1.0.1/README.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 02:25:58.816838 niwatoko-1.0.1/niwatoko.egg-info/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16804 2024-05-07 02:25:58.000000 niwatoko-1.0.1/niwatoko.egg-info/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      313 2024-05-07 02:25:58.000000 niwatoko-1.0.1/niwatoko.egg-info/SOURCES.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-07 02:25:58.000000 niwatoko-1.0.1/niwatoko.egg-info/dependency_links.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-07 02:25:58.000000 niwatoko-1.0.1/niwatoko.egg-info/entry_points.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       17 2024-05-07 02:25:58.000000 niwatoko-1.0.1/niwatoko.egg-info/requires.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        6 2024-05-07 02:25:58.000000 niwatoko-1.0.1/niwatoko.egg-info/top_level.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-07 02:25:58.820476 niwatoko-1.0.1/setup.cfg
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1464 2024-05-07 02:25:54.000000 niwatoko-1.0.1/setup.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 02:25:58.817526 niwatoko-1.0.1/tests/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-06 13:44:44.000000 niwatoko-1.0.1/tests/__init__.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 02:25:58.817813 niwatoko-1.0.1/tests/test_docs/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-06 13:45:38.000000 niwatoko-1.0.1/tests/test_docs/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-06 13:44:55.000000 niwatoko-1.0.1/tests/test_interpreter.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-06 13:44:49.000000 niwatoko-1.0.1/tests/test_parser.py
```

### Comparing `niwatoko-1.0.0/LICENSE` & `niwatoko-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.0/PKG-INFO` & `niwatoko-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.0.0
+Version: 1.0.1
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 要件定義書: niwatoko - 自然言語プログラミング言語のPythonパッケージ
```

### Comparing `niwatoko-1.0.0/README.md` & `niwatoko-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.0/niwatoko.egg-info/PKG-INFO` & `niwatoko-1.0.1/niwatoko.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.0.0
+Version: 1.0.1
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 要件定義書: niwatoko - 自然言語プログラミング言語のPythonパッケージ
```

### Comparing `niwatoko-1.0.0/setup.py` & `niwatoko-1.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # niwatoko - 自然言語プログラミング言語のPythonパッケージのsetup.pyファイルです。
 # このファイルはパッケージのインストールや配布に必要な情報を含んでいます。
 
 from setuptools import setup, find_packages
 
 setup(
     name='niwatoko',
-    version='1.0.0',
+    version='1.0.1',
     description='自然言語でプログラミングを行うことができる新しいプログラミング言語',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='dai-motoki',
     author_email='dai.motoki1123@gmail.com',
     url='https://niwatoko2.vercel.app/',
     packages=find_packages(),
@@ -22,14 +22,16 @@
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Natural Language :: Japanese',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.7',
     entry_points={
         'console_scripts': [
             'niwatoko=niwatoko.cli:main',
```

### Comparing `niwatoko-1.0.0/tests/__init__.py` & `niwatoko-1.0.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.0/tests/test_docs/__init__.py` & `niwatoko-1.0.1/tests/test_docs/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.0/tests/test_interpreter.py` & `niwatoko-1.0.1/tests/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.0/tests/test_parser.py` & `niwatoko-1.0.1/tests/test_parser.py`

 * *Files identical despite different names*

