# Comparing `tmp/niwatoko-1.0.7.tar.gz` & `tmp/niwatoko-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niwatoko-1.0.7.tar", last modified: Tue May  7 08:39:30 2024, max compression
+gzip compressed data, was "niwatoko-1.0.8.tar", last modified: Tue May  7 08:53:51 2024, max compression
```

## Comparing `niwatoko-1.0.7.tar` & `niwatoko-1.0.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:39:30.417841 niwatoko-1.0.7/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    11356 2024-05-07 05:52:57.000000 niwatoko-1.0.7/LICENSE
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16804 2024-05-07 08:39:30.417687 niwatoko-1.0.7/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    15918 2024-05-07 02:46:41.000000 niwatoko-1.0.7/README.md
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:39:30.413168 niwatoko-1.0.7/niwatoko/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 05:52:23.000000 niwatoko-1.0.7/niwatoko/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2494 2024-05-07 08:36:30.000000 niwatoko-1.0.7/niwatoko/cli.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:39:30.412274 niwatoko-1.0.7/niwatoko/foundation_model/
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:39:30.412312 niwatoko-1.0.7/niwatoko/foundation_model/interpretation/
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:39:30.414483 niwatoko-1.0.7/niwatoko/foundation_model/interpretation/llm/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1075 2024-05-07 06:49:11.000000 niwatoko-1.0.7/niwatoko/foundation_model/interpretation/llm/claude.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1309 2024-05-07 08:37:07.000000 niwatoko-1.0.7/niwatoko/foundation_model/interpretation/llm/gpt.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:39:30.414711 niwatoko-1.0.7/niwatoko/grammar/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      481 2024-05-07 05:52:23.000000 niwatoko-1.0.7/niwatoko/grammar/system.md
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:39:30.414061 niwatoko-1.0.7/niwatoko.egg-info/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16804 2024-05-07 08:39:30.000000 niwatoko-1.0.7/niwatoko.egg-info/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      769 2024-05-07 08:39:30.000000 niwatoko-1.0.7/niwatoko.egg-info/SOURCES.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-07 08:39:30.000000 niwatoko-1.0.7/niwatoko.egg-info/dependency_links.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-07 08:39:30.000000 niwatoko-1.0.7/niwatoko.egg-info/entry_points.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       34 2024-05-07 08:39:30.000000 niwatoko-1.0.7/niwatoko.egg-info/requires.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       15 2024-05-07 08:39:30.000000 niwatoko-1.0.7/niwatoko.egg-info/top_level.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-07 08:39:30.417875 niwatoko-1.0.7/setup.cfg
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1697 2024-05-07 08:38:01.000000 niwatoko-1.0.7/setup.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:39:30.415390 niwatoko-1.0.7/tests/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-07 02:46:41.000000 niwatoko-1.0.7/tests/__init__.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:39:30.417355 niwatoko-1.0.7/tests/test_docs/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-07 02:46:41.000000 niwatoko-1.0.7/tests/test_docs/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2609 2024-05-07 05:48:44.000000 niwatoko-1.0.7/tests/test_docs/test_doc1.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2853 2024-05-07 05:48:44.000000 niwatoko-1.0.7/tests/test_docs/test_doc2.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2625 2024-05-07 05:48:44.000000 niwatoko-1.0.7/tests/test_docs/test_doc3.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1678 2024-05-07 06:18:12.000000 niwatoko-1.0.7/tests/test_docs/test_gen_github_issue.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1950 2024-05-07 07:00:44.000000 niwatoko-1.0.7/tests/test_docs/test_gen_grimoire.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1909 2024-05-07 06:33:47.000000 niwatoko-1.0.7/tests/test_docs/test_gen_grimoire2.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1850 2024-05-07 07:04:51.000000 niwatoko-1.0.7/tests/test_docs/test_gen_grimoire_en.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5307 2024-05-07 05:52:23.000000 niwatoko-1.0.7/tests/test_docs/test_gen_zoltraak_pypi.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-07 02:46:41.000000 niwatoko-1.0.7/tests/test_interpreter.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-07 02:46:41.000000 niwatoko-1.0.7/tests/test_parser.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:53:51.777636 niwatoko-1.0.8/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    11356 2024-05-07 05:52:57.000000 niwatoko-1.0.8/LICENSE
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16804 2024-05-07 08:53:51.777469 niwatoko-1.0.8/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    15918 2024-05-07 02:46:41.000000 niwatoko-1.0.8/README.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:53:51.771800 niwatoko-1.0.8/niwatoko/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 05:52:23.000000 niwatoko-1.0.8/niwatoko/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2798 2024-05-07 08:52:52.000000 niwatoko-1.0.8/niwatoko/cli.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:53:51.770954 niwatoko-1.0.8/niwatoko/foundation_model/
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:53:51.770992 niwatoko-1.0.8/niwatoko/foundation_model/interpretation/
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:53:51.773020 niwatoko-1.0.8/niwatoko/foundation_model/interpretation/llm/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1075 2024-05-07 06:49:11.000000 niwatoko-1.0.8/niwatoko/foundation_model/interpretation/llm/claude.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1309 2024-05-07 08:37:07.000000 niwatoko-1.0.8/niwatoko/foundation_model/interpretation/llm/gpt.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:53:51.773222 niwatoko-1.0.8/niwatoko/grammar/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      481 2024-05-07 05:52:23.000000 niwatoko-1.0.8/niwatoko/grammar/system.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:53:51.772682 niwatoko-1.0.8/niwatoko.egg-info/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16804 2024-05-07 08:53:51.000000 niwatoko-1.0.8/niwatoko.egg-info/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      769 2024-05-07 08:53:51.000000 niwatoko-1.0.8/niwatoko.egg-info/SOURCES.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-07 08:53:51.000000 niwatoko-1.0.8/niwatoko.egg-info/dependency_links.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-07 08:53:51.000000 niwatoko-1.0.8/niwatoko.egg-info/entry_points.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       34 2024-05-07 08:53:51.000000 niwatoko-1.0.8/niwatoko.egg-info/requires.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       15 2024-05-07 08:53:51.000000 niwatoko-1.0.8/niwatoko.egg-info/top_level.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-07 08:53:51.777671 niwatoko-1.0.8/setup.cfg
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1697 2024-05-07 08:53:18.000000 niwatoko-1.0.8/setup.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:53:51.773879 niwatoko-1.0.8/tests/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-07 02:46:41.000000 niwatoko-1.0.8/tests/__init__.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:53:51.777128 niwatoko-1.0.8/tests/test_docs/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-07 02:46:41.000000 niwatoko-1.0.8/tests/test_docs/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2609 2024-05-07 05:48:44.000000 niwatoko-1.0.8/tests/test_docs/test_doc1.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2853 2024-05-07 05:48:44.000000 niwatoko-1.0.8/tests/test_docs/test_doc2.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2625 2024-05-07 05:48:44.000000 niwatoko-1.0.8/tests/test_docs/test_doc3.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1678 2024-05-07 06:18:12.000000 niwatoko-1.0.8/tests/test_docs/test_gen_github_issue.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1950 2024-05-07 07:00:44.000000 niwatoko-1.0.8/tests/test_docs/test_gen_grimoire.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1909 2024-05-07 06:33:47.000000 niwatoko-1.0.8/tests/test_docs/test_gen_grimoire2.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1850 2024-05-07 07:04:51.000000 niwatoko-1.0.8/tests/test_docs/test_gen_grimoire_en.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5307 2024-05-07 05:52:23.000000 niwatoko-1.0.8/tests/test_docs/test_gen_zoltraak_pypi.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-07 02:46:41.000000 niwatoko-1.0.8/tests/test_interpreter.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-07 02:46:41.000000 niwatoko-1.0.8/tests/test_parser.py
```

### Comparing `niwatoko-1.0.7/LICENSE` & `niwatoko-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.7/PKG-INFO` & `niwatoko-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.0.7
+Version: 1.0.8
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
```

### Comparing `niwatoko-1.0.7/README.md` & `niwatoko-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.7/niwatoko/cli.py` & `niwatoko-1.0.8/niwatoko/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 from niwatoko.foundation_model.interpretation.llm.gpt import generate_response as gpt_generate_response
 
 @click.command()
 @click.argument('file_path', type=click.Path(exists=True), required=False)
 @click.option('-m', '--model', type=click.Choice(['openai', 'claude']), default='openai', help='使用するモデルを選択します。')
 @click.option('-o', '--output', type=click.Path(), help='生成されたコードの出力先ファイルを指定します。')
 @click.option('-v', '--version', is_flag=True, help='バージョン情報を表示します。')
+
+
 def main(file_path, model, output, version):
     """
     自然言語のソースコードを読み込んで実行するコマンドラインインターフェース。
 
     Args:
         file_path (str): 自然言語のソースコードが書かれたファイルのパス。
         model (str): 使用するモデル（OpenAIまたはClaude）。
         output (str): 生成されたコードの出力先ファイルのパス。
         version (bool): バージョン情報を表示するかどうか。
     """
     if version:
         print(f"niwatoko バージョン: {get_version()}")
         return
-
     if not file_path:
         print("ファイルパスが指定されていません。")
         return
 
     with open(file_path, 'r') as file:
         natural_language_code = file.read()
 
@@ -56,8 +57,20 @@
     # print(generated_code)
 
     if output:
         with open(output, 'w') as file:
             file.write(generated_code)
             print(f"生成されたコードを {output} に書き出しました。")
 
-    # exec(generated_code)
+def get_version():
+    import re
+
+    with open('setup.py', 'r') as file:
+        content = file.read()
+
+    match = re.search(r'version=[\'\"](.+?)[\'\"]', content)
+    if match:
+        version = match.group(1)
+    else:
+        raise ValueError("バージョン情報が見つかりませんでした。")
+
+    return version
```

### Comparing `niwatoko-1.0.7/niwatoko/foundation_model/interpretation/llm/claude.py` & `niwatoko-1.0.8/niwatoko/foundation_model/interpretation/llm/claude.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.7/niwatoko/foundation_model/interpretation/llm/gpt.py` & `niwatoko-1.0.8/niwatoko/foundation_model/interpretation/llm/gpt.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.7/niwatoko.egg-info/PKG-INFO` & `niwatoko-1.0.8/niwatoko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.0.7
+Version: 1.0.8
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
```

### Comparing `niwatoko-1.0.7/niwatoko.egg-info/SOURCES.txt` & `niwatoko-1.0.8/niwatoko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.7/setup.py` & `niwatoko-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # niwatoko - 自然言語プログラミング言語のPythonパッケージのsetup.pyファイルです。
 # このファイルはパッケージのインストールや配布に必要な情報を含んでいます。
 
 from setuptools import setup, find_packages
 
 setup(
     name='niwatoko',
-    version='1.0.7',
+    version='1.0.8',
     description='自然言語でプログラミングを行うことができる新しいプログラミング言語',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='dai-motoki',
     author_email='dai.motoki1123@gmail.com',
     url='https://niwatoko2.vercel.app/',
     packages=find_packages(),
```

### Comparing `niwatoko-1.0.7/tests/__init__.py` & `niwatoko-1.0.8/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.7/tests/test_docs/__init__.py` & `niwatoko-1.0.8/tests/test_docs/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.7/tests/test_docs/test_doc1.md` & `niwatoko-1.0.8/tests/test_docs/test_doc1.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.7/tests/test_docs/test_doc2.md` & `niwatoko-1.0.8/tests/test_docs/test_doc2.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.7/tests/test_docs/test_doc3.md` & `niwatoko-1.0.8/tests/test_docs/test_doc3.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.7/tests/test_docs/test_gen_github_issue.md` & `niwatoko-1.0.8/tests/test_docs/test_gen_github_issue.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.7/tests/test_docs/test_gen_grimoire.md` & `niwatoko-1.0.8/tests/test_docs/test_gen_grimoire.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.7/tests/test_docs/test_gen_grimoire2.md` & `niwatoko-1.0.8/tests/test_docs/test_gen_grimoire2.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.7/tests/test_docs/test_gen_grimoire_en.md` & `niwatoko-1.0.8/tests/test_docs/test_gen_grimoire_en.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.7/tests/test_docs/test_gen_zoltraak_pypi.md` & `niwatoko-1.0.8/tests/test_docs/test_gen_zoltraak_pypi.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.7/tests/test_interpreter.py` & `niwatoko-1.0.8/tests/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.7/tests/test_parser.py` & `niwatoko-1.0.8/tests/test_parser.py`

 * *Files identical despite different names*
