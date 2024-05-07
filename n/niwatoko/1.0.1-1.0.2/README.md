# Comparing `tmp/niwatoko-1.0.1.tar.gz` & `tmp/niwatoko-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niwatoko-1.0.1.tar", last modified: Tue May  7 02:25:58 2024, max compression
+gzip compressed data, was "niwatoko-1.0.2.tar", last modified: Tue May  7 08:06:26 2024, max compression
```

## Comparing `niwatoko-1.0.1.tar` & `niwatoko-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 02:25:58.820341 niwatoko-1.0.1/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2807 2024-05-06 13:47:27.000000 niwatoko-1.0.1/LICENSE
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16804 2024-05-07 02:25:58.819781 niwatoko-1.0.1/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    15918 2024-05-07 01:32:03.000000 niwatoko-1.0.1/README.md
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 02:25:58.816838 niwatoko-1.0.1/niwatoko.egg-info/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16804 2024-05-07 02:25:58.000000 niwatoko-1.0.1/niwatoko.egg-info/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      313 2024-05-07 02:25:58.000000 niwatoko-1.0.1/niwatoko.egg-info/SOURCES.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-07 02:25:58.000000 niwatoko-1.0.1/niwatoko.egg-info/dependency_links.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-07 02:25:58.000000 niwatoko-1.0.1/niwatoko.egg-info/entry_points.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       17 2024-05-07 02:25:58.000000 niwatoko-1.0.1/niwatoko.egg-info/requires.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        6 2024-05-07 02:25:58.000000 niwatoko-1.0.1/niwatoko.egg-info/top_level.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-07 02:25:58.820476 niwatoko-1.0.1/setup.cfg
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1464 2024-05-07 02:25:54.000000 niwatoko-1.0.1/setup.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 02:25:58.817526 niwatoko-1.0.1/tests/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-06 13:44:44.000000 niwatoko-1.0.1/tests/__init__.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 02:25:58.817813 niwatoko-1.0.1/tests/test_docs/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-06 13:45:38.000000 niwatoko-1.0.1/tests/test_docs/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-06 13:44:55.000000 niwatoko-1.0.1/tests/test_interpreter.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-06 13:44:49.000000 niwatoko-1.0.1/tests/test_parser.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:06:26.782523 niwatoko-1.0.2/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    11356 2024-05-07 05:52:57.000000 niwatoko-1.0.2/LICENSE
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16804 2024-05-07 08:06:26.782327 niwatoko-1.0.2/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    15918 2024-05-07 02:46:41.000000 niwatoko-1.0.2/README.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:06:26.780626 niwatoko-1.0.2/niwatoko/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 05:52:23.000000 niwatoko-1.0.2/niwatoko/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2096 2024-05-07 06:53:37.000000 niwatoko-1.0.2/niwatoko/cli.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:06:26.781336 niwatoko-1.0.2/niwatoko.egg-info/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16804 2024-05-07 08:06:26.000000 niwatoko-1.0.2/niwatoko.egg-info/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      350 2024-05-07 08:06:26.000000 niwatoko-1.0.2/niwatoko.egg-info/SOURCES.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-07 08:06:26.000000 niwatoko-1.0.2/niwatoko.egg-info/dependency_links.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-07 08:06:26.000000 niwatoko-1.0.2/niwatoko.egg-info/entry_points.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       34 2024-05-07 08:06:26.000000 niwatoko-1.0.2/niwatoko.egg-info/requires.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       15 2024-05-07 08:06:26.000000 niwatoko-1.0.2/niwatoko.egg-info/top_level.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-07 08:06:26.782556 niwatoko-1.0.2/setup.cfg
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1574 2024-05-07 08:00:13.000000 niwatoko-1.0.2/setup.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:06:26.781896 niwatoko-1.0.2/tests/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-07 02:46:41.000000 niwatoko-1.0.2/tests/__init__.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-07 08:06:26.782093 niwatoko-1.0.2/tests/test_docs/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-07 02:46:41.000000 niwatoko-1.0.2/tests/test_docs/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-07 02:46:41.000000 niwatoko-1.0.2/tests/test_interpreter.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-07 02:46:41.000000 niwatoko-1.0.2/tests/test_parser.py
```

### Comparing `niwatoko-1.0.1/LICENSE` & `niwatoko-1.0.2/tests/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-# 要件定義書の内容は非常に包括的で、niwatoko - 自然言語プログラミング言語のPythonパッケージの開発に関する詳細な仕様が記載されています。主な内容は以下の通りです:
+# 理解しました。この要件定義書に基づいて、niwatoko - 自然言語プログラミング言語のPythonパッケージを開発していくことが可能です。特に以下の点に注意して開発を進めていく必要があります:
 # 
-# 1. **目的**: niwatoko は自然言語でプログラミングを行うことができる新しいプログラミング言語で、このプロジェクトの目的は、niwatoko のPythonパッケージを開発し、ユーザーが自然言語を使ってプログラムを記述し、実行できるようにすることです。
+# 1. パッケージの基本構造: 提案された`niwatoko/`ディレクトリ構造を基に、各モジュールの役割と相互関係を明確にしていきます。
 # 
-# 2. **パッケージの基本構造**: niwatoko パッケージの基本的な構造が示されており、メインディレクトリ、テストコード、ドキュメント、設定ファイルなどが含まれています。
+# 2. setup.pyの作成: パッケージのメタデータ、依存ライブラリ、ライセンス情報などを適切に設定します。
 # 
-# 3. **setup.pyの書き方**: パッケージのメタデータと依存関係を定義するための`setup.py`ファイルの例が示されています。
+# 3. __init__.py の活用: パッケージの公開APIを明確にし、ユーザーが使いやすいインターフェースを提供します。
 # 
-# 4. **__init__.pyの役割**: パッケージの初期化処理を行う`__init__.py`ファイルの役割が説明されています。
+# 4. README.mdの充実: パッケージの概要、インストール方法、使用例、ライセンス情報、貢献方法などを詳細に記述します。
 # 
-# 5. **README.mdの書き方**: パッケージの概要、インストール方法、使用方法、ライセンス情報、貢献方法、サポート方法などを記載するためのREADMEファイルの構成が示されています。
+# 5. LICENSEファイルの選定: 適切なオープンソースライセンスを選択し、ライセンス条件を遵守します。
 # 
-# 6. **LICENSEファイル**: パッケージのライセンスを明記するための方法が説明されています。
+# 6. バージョン管理: セマンティックバージョニングに従ってバージョンを管理し、API互換性を保ちます。
 # 
-# 7. **パッケージのバージョン管理**: セマンティックバージョニングに基づいたバージョン管理の方法が示されています。
+# 7. テストの実装: 提案された構成に従ってテストコードを作成し、コードの品質と機能を保証します。
 # 
-# 8. **テストの書き方**: テストファイルの命名規則、テストクラスの定義方法、テストメソッドの命名規則、テストの実装方法などが説明されています。
+# 8. ドキュメントの作成: Sphinxを使用してモジュール、関数、クラスのドキュメントを生成し、ユーザーが理解しやすい情報を提供します。
 # 
-# 9. **ドキュメントの作成方法**: Sphinxを使用したドキュメントの作成方法が示されています。
+# 9. Docker化とCI/CD: Dockerを使ってアプリケーションをパッケージ化し、GitHub Actionsでテスト、ビルド、デプロイを自動化します。
 # 
-# 10. **Docker化とCI/CDの設定**: Dockerを使ってアプリケーションをコンテナ化し、GitHub Actionsを使ってCI/CDパイプラインを設定する方法が説明されています。
+# 10. WebアプリケーションのUI: StreamlitやGradioを使って、ユーザーが自然言語でプログラミングできるWebアプリケーションを構築します。
 # 
-# 11. **WebアプリケーションのUI設定**: StreamlitやGradioを使ってWebアプリケーションのUIを設定する方法が示されています。
-# 
-# 全体として、niwatoko パッケージの開発に必要な要件が非常に詳細に定義されており、パッケージの構造、ドキュメンテーション、テスト、デプロイメント、UI設定など、開発に必要な様々な側面が網羅されています。この要件定義書に沿って開発を進めれば、高品質で拡張性のあるniwatoko パッケージを実現できると思われます。
+# これらの要件に沿って、niwatoko パッケージの開発を進めていくことで、自然言語でプログラミングできる新しい言語を実現できるでしょう。
```

### Comparing `niwatoko-1.0.1/PKG-INFO` & `niwatoko-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.0.1
+Version: 1.0.2
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
```

### Comparing `niwatoko-1.0.1/README.md` & `niwatoko-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.1/niwatoko.egg-info/PKG-INFO` & `niwatoko-1.0.2/niwatoko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.0.1
+Version: 1.0.2
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
```

### Comparing `niwatoko-1.0.1/setup.py` & `niwatoko-1.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # niwatoko - 自然言語プログラミング言語のPythonパッケージのsetup.pyファイルです。
 # このファイルはパッケージのインストールや配布に必要な情報を含んでいます。
 
 from setuptools import setup, find_packages
 
 setup(
     name='niwatoko',
-    version='1.0.1',
+    version='1.0.2',
     description='自然言語でプログラミングを行うことができる新しいプログラミング言語',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='dai-motoki',
     author_email='dai.motoki1123@gmail.com',
     url='https://niwatoko2.vercel.app/',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'streamlit',
-        'gradio'
+        'gradio',
+        'openai',
+        'anthropic',
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Natural Language :: Japanese',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
@@ -33,8 +35,11 @@
     ],
     python_requires='>=3.7',
     entry_points={
         'console_scripts': [
             'niwatoko=niwatoko.cli:main',
         ],
     },
+    package_data={
+        'niwatoko': ['foundation_model/*'],
+    },
 )
```

### Comparing `niwatoko-1.0.1/tests/__init__.py` & `niwatoko-1.0.2/tests/test_interpreter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,57 @@
-# 理解しました。この要件定義書に基づいて、niwatoko - 自然言語プログラミング言語のPythonパッケージを開発していくことが可能です。特に以下の点に注意して開発を進めていく必要があります:
+# はい、要件定義書に基づいて、interpreterモジュールのテストを作成しましょう。tests/test_interpreter.pyファイルに以下のようなテストを書いていきます。
 # 
-# 1. パッケージの基本構造: 提案された`niwatoko/`ディレクトリ構造を基に、各モジュールの役割と相互関係を明確にしていきます。
+import unittest
+from niwatoko.interpreter import interpret
+from niwatoko.parser import parse
+
+class TestInterpreter(unittest.TestCase):
+    def test_simple_addition(self):
+        program = "Add 2 and 3."
+        ast = parse(program)
+        result = interpret(ast)
+        self.assertEqual(result, 5)
+
+    def test_variable_assignment(self):
+        program = """
+        Set x to 10.
+        Set y to 20.
+        Add x and y.
+        """
+        ast = parse(program)
+        result = interpret(ast)
+        self.assertEqual(result, 30)
+
+    def test_function_definition(self):
+        program = """
+        Define a function that takes two numbers and returns their sum.
+        Call the function with 4 and 6.
+        """
+        ast = parse(program)
+        result = interpret(ast)
+        self.assertEqual(result, 10)
+
+    def test_error_handling(self):
+        program = "Multiply 2 and 3."
+        ast = parse(program)
+        with self.assertRaises(NotImplementedError):
+            interpret(ast)
+
+if __name__ == '__main__':
+    unittest.main()
+# 
+# このテストケースでは、以下のことをチェックしています:
+# 
+# 1. 2つの数の加算
+# 2. 変数の割り当てと加算
+# 3. 関数の定義と呼び出し
+# 4. サポートされていない操作に対するエラー処理
+# 
+# これらのテストを実行することで、interpreterモジュールの基本的な機能が正しく動作することを確認できます。
 # 
-# 2. setup.pyの作成: パッケージのメタデータ、依存ライブラリ、ライセンス情報などを適切に設定します。
+# テストを実行するには、以下のコマンドを使用します:
 # 
-# 3. __init__.py の活用: パッケージの公開APIを明確にし、ユーザーが使いやすいインターフェースを提供します。
+# python -m unittest tests.test_interpreter
 # 
-# 4. README.mdの充実: パッケージの概要、インストール方法、使用例、ライセンス情報、貢献方法などを詳細に記述します。
+# テストが成功すれば、interpreterモジュールの実装が要件を満たしていることを示しています。テストが失敗した場合は、interpreterモジュールの実装を修正する必要があります。
 # 
-# 5. LICENSEファイルの選定: 適切なオープンソースライセンスを選択し、ライセンス条件を遵守します。
-# 
-# 6. バージョン管理: セマンティックバージョニングに従ってバージョンを管理し、API互換性を保ちます。
-# 
-# 7. テストの実装: 提案された構成に従ってテストコードを作成し、コードの品質と機能を保証します。
-# 
-# 8. ドキュメントの作成: Sphinxを使用してモジュール、関数、クラスのドキュメントを生成し、ユーザーが理解しやすい情報を提供します。
-# 
-# 9. Docker化とCI/CD: Dockerを使ってアプリケーションをパッケージ化し、GitHub Actionsでテスト、ビルド、デプロイを自動化します。
-# 
-# 10. WebアプリケーションのUI: StreamlitやGradioを使って、ユーザーが自然言語でプログラミングできるWebアプリケーションを構築します。
-# 
-# これらの要件に沿って、niwatoko パッケージの開発を進めていくことで、自然言語でプログラミングできる新しい言語を実現できるでしょう。
+# このようにして、要件定義書に基づいて段階的にテストを追加していくことで、パッケージの品質を高めていくことができます。
```

### Comparing `niwatoko-1.0.1/tests/test_docs/__init__.py` & `niwatoko-1.0.2/tests/test_docs/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.0.1/tests/test_interpreter.py` & `niwatoko-1.0.2/tests/test_parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,61 @@
-# はい、要件定義書に基づいて、interpreterモジュールのテストを作成しましょう。tests/test_interpreter.pyファイルに以下のようなテストを書いていきます。
+# はい、ここでは `parser.py` モジュールのテストを書く方法について説明します。
+# 
+# `tests/test_parser.py` ファイルを作成し、以下のようなテストコードを書きます:
 # 
 import unittest
-from niwatoko.interpreter import interpret
 from niwatoko.parser import parse
 
-class TestInterpreter(unittest.TestCase):
-    def test_simple_addition(self):
-        program = "Add 2 and 3."
-        ast = parse(program)
-        result = interpret(ast)
-        self.assertEqual(result, 5)
-
-    def test_variable_assignment(self):
+class TestParser(unittest.TestCase):
+    def test_simple_program(self):
         program = """
-        Set x to 10.
-        Set y to 20.
-        Add x and y.
+        Create a function that takes two numbers as input and returns their sum.
         """
         ast = parse(program)
-        result = interpret(ast)
-        self.assertEqual(result, 30)
+        self.assertIsNotNone(ast)
+        self.assertEqual(len(ast.body), 1)
+        self.assertEqual(ast.body[0].name, "create_function")
+        self.assertEqual(len(ast.body[0].arguments), 2)
+        self.assertEqual(ast.body[0].return_type, "sum")
 
-    def test_function_definition(self):
+    def test_invalid_program(self):
         program = """
-        Define a function that takes two numbers and returns their sum.
-        Call the function with 4 and 6.
+        This is not a valid program.
         """
-        ast = parse(program)
-        result = interpret(ast)
-        self.assertEqual(result, 10)
+        with self.assertRaises(ValueError):
+            parse(program)
 
-    def test_error_handling(self):
-        program = "Multiply 2 and 3."
+    def test_program_with_multiple_statements(self):
+        program = """
+        Create a function that takes two numbers as input and returns their sum.
+        Create a function that takes two strings as input and returns their concatenation.
+        """
         ast = parse(program)
-        with self.assertRaises(NotImplementedError):
-            interpret(ast)
+        self.assertIsNotNone(ast)
+        self.assertEqual(len(ast.body), 2)
+        self.assertEqual(ast.body[0].name, "create_function")
+        self.assertEqual(ast.body[1].name, "create_function")
 
 if __name__ == '__main__':
     unittest.main()
 # 
 # このテストケースでは、以下のことをチェックしています:
 # 
-# 1. 2つの数の加算
-# 2. 変数の割り当てと加算
-# 3. 関数の定義と呼び出し
-# 4. サポートされていない操作に対するエラー処理
-# 
-# これらのテストを実行することで、interpreterモジュールの基本的な機能が正しく動作することを確認できます。
+# 1. 簡単な自然言語プログラムを正しくパースできること
+# 2. 無効な自然言語プログラムを渡した場合に、適切な例外が発生すること
+# 3. 複数の文からなる自然言語プログラムを正しくパースできること
 # 
 # テストを実行するには、以下のコマンドを使用します:
 # 
-# python -m unittest tests.test_interpreter
+# python -m unittest tests.test_parser
+# 
+# これにより、`tests/test_parser.py` ファイルのテストが実行されます。
+# 
+# テストの実装に際しては、以下のようなポイントに注意しましょう:
 # 
-# テストが成功すれば、interpreterモジュールの実装が要件を満たしていることを示しています。テストが失敗した場合は、interpreterモジュールの実装を修正する必要があります。
+# - 各テストケースでは、1つの機能や動作を検証するようにする
+# - 期待する結果と実際の結果を明確に比較する
+# - 例外処理のテストも忘れずに行う
+# - テストの命名規則は `test_` で始まるようにする
+# - テストの実行は自動化し、継続的に行う
 # 
-# このようにして、要件定義書に基づいて段階的にテストを追加していくことで、パッケージの品質を高めていくことができます。
+# これらの方法でparserモジュールのテストを書いていきます。テストの作成と並行して、実際の実装も進めていきましょう。
```

