# Comparing `tmp/got-cli-0.1.1.tar.gz` & `tmp/got-cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "got-cli-0.1.1.tar", last modified: Sun May  5 17:39:30 2024, max compression
+gzip compressed data, was "got-cli-0.1.2.tar", last modified: Tue May  7 12:54:27 2024, max compression
```

## Comparing `got-cli-0.1.1.tar` & `got-cli-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 guialves   (501) staff       (20)        0 2024-05-05 17:39:30.147258 got-cli-0.1.1/
--rw-r--r--   0 guialves   (501) staff       (20)     1067 2024-05-05 17:06:50.000000 got-cli-0.1.1/LICENSE
--rw-r--r--   0 guialves   (501) staff       (20)      323 2024-05-05 17:39:30.147129 got-cli-0.1.1/PKG-INFO
--rw-r--r--   0 guialves   (501) staff       (20)     2268 2024-05-05 16:57:38.000000 got-cli-0.1.1/README.md
-drwxr-xr-x   0 guialves   (501) staff       (20)        0 2024-05-05 17:39:30.145048 got-cli-0.1.1/got/
--rw-r--r--   0 guialves   (501) staff       (20)        0 2024-05-04 17:10:40.000000 got-cli-0.1.1/got/__init__.py
-drwxr-xr-x   0 guialves   (501) staff       (20)        0 2024-05-05 17:39:30.145997 got-cli-0.1.1/got/ai/
--rw-r--r--   0 guialves   (501) staff       (20)     1767 2024-05-05 17:29:12.000000 got-cli-0.1.1/got/ai/__init__.py
--rw-r--r--   0 guialves   (501) staff       (20)     1299 2024-05-05 16:11:02.000000 got-cli-0.1.1/got/ai/chatgpt.py
--rw-r--r--   0 guialves   (501) staff       (20)      483 2024-05-05 17:32:08.000000 got-cli-0.1.1/got/ai/factory.py
--rw-r--r--   0 guialves   (501) staff       (20)     1386 2024-05-05 16:11:25.000000 got-cli-0.1.1/got/ai/groq.py
--rw-r--r--   0 guialves   (501) staff       (20)     3012 2024-05-05 16:31:23.000000 got-cli-0.1.1/got/cli.py
--rw-r--r--   0 guialves   (501) staff       (20)     2096 2024-05-05 17:34:49.000000 got-cli-0.1.1/got/commit.py
--rw-r--r--   0 guialves   (501) staff       (20)     2699 2024-05-05 16:09:24.000000 got-cli-0.1.1/got/git.py
--rw-r--r--   0 guialves   (501) staff       (20)    11881 2024-05-05 16:39:33.000000 got-cli-0.1.1/got/printer.py
-drwxr-xr-x   0 guialves   (501) staff       (20)        0 2024-05-05 17:39:30.146952 got-cli-0.1.1/got_cli.egg-info/
--rw-r--r--   0 guialves   (501) staff       (20)      323 2024-05-05 17:39:30.000000 got-cli-0.1.1/got_cli.egg-info/PKG-INFO
--rw-r--r--   0 guialves   (501) staff       (20)      351 2024-05-05 17:39:30.000000 got-cli-0.1.1/got_cli.egg-info/SOURCES.txt
--rw-r--r--   0 guialves   (501) staff       (20)        1 2024-05-05 17:39:30.000000 got-cli-0.1.1/got_cli.egg-info/dependency_links.txt
--rw-r--r--   0 guialves   (501) staff       (20)       37 2024-05-05 17:39:30.000000 got-cli-0.1.1/got_cli.egg-info/entry_points.txt
--rw-r--r--   0 guialves   (501) staff       (20)       77 2024-05-05 17:39:30.000000 got-cli-0.1.1/got_cli.egg-info/requires.txt
--rw-r--r--   0 guialves   (501) staff       (20)        4 2024-05-05 17:39:30.000000 got-cli-0.1.1/got_cli.egg-info/top_level.txt
--rw-r--r--   0 guialves   (501) staff       (20)       38 2024-05-05 17:39:30.147390 got-cli-0.1.1/setup.cfg
--rw-r--r--   0 guialves   (501) staff       (20)      685 2024-05-05 17:39:29.000000 got-cli-0.1.1/setup.py
+drwxr-xr-x   0 guialves   (501) staff       (20)        0 2024-05-07 12:54:27.478499 got-cli-0.1.2/
+-rw-r--r--   0 guialves   (501) staff       (20)     1067 2024-05-05 17:06:50.000000 got-cli-0.1.2/LICENSE
+-rw-r--r--   0 guialves   (501) staff       (20)      323 2024-05-07 12:54:27.478269 got-cli-0.1.2/PKG-INFO
+-rw-r--r--   0 guialves   (501) staff       (20)     2275 2024-05-07 12:53:56.000000 got-cli-0.1.2/README.md
+drwxr-xr-x   0 guialves   (501) staff       (20)        0 2024-05-07 12:54:27.473600 got-cli-0.1.2/got/
+-rw-r--r--   0 guialves   (501) staff       (20)        0 2024-05-04 17:10:40.000000 got-cli-0.1.2/got/__init__.py
+drwxr-xr-x   0 guialves   (501) staff       (20)        0 2024-05-07 12:54:27.475929 got-cli-0.1.2/got/ai/
+-rw-r--r--   0 guialves   (501) staff       (20)     1767 2024-05-05 17:29:12.000000 got-cli-0.1.2/got/ai/__init__.py
+-rw-r--r--   0 guialves   (501) staff       (20)     1299 2024-05-05 16:11:02.000000 got-cli-0.1.2/got/ai/chatgpt.py
+-rw-r--r--   0 guialves   (501) staff       (20)      483 2024-05-05 17:32:08.000000 got-cli-0.1.2/got/ai/factory.py
+-rw-r--r--   0 guialves   (501) staff       (20)     1386 2024-05-05 16:11:25.000000 got-cli-0.1.2/got/ai/groq.py
+-rw-r--r--   0 guialves   (501) staff       (20)     3019 2024-05-07 12:54:05.000000 got-cli-0.1.2/got/cli.py
+-rw-r--r--   0 guialves   (501) staff       (20)     2096 2024-05-05 17:34:49.000000 got-cli-0.1.2/got/commit.py
+-rw-r--r--   0 guialves   (501) staff       (20)     2699 2024-05-05 16:09:24.000000 got-cli-0.1.2/got/git.py
+-rw-r--r--   0 guialves   (501) staff       (20)    11881 2024-05-05 16:39:33.000000 got-cli-0.1.2/got/printer.py
+drwxr-xr-x   0 guialves   (501) staff       (20)        0 2024-05-07 12:54:27.477973 got-cli-0.1.2/got_cli.egg-info/
+-rw-r--r--   0 guialves   (501) staff       (20)      323 2024-05-07 12:54:27.000000 got-cli-0.1.2/got_cli.egg-info/PKG-INFO
+-rw-r--r--   0 guialves   (501) staff       (20)      351 2024-05-07 12:54:27.000000 got-cli-0.1.2/got_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 guialves   (501) staff       (20)        1 2024-05-07 12:54:27.000000 got-cli-0.1.2/got_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 guialves   (501) staff       (20)       37 2024-05-07 12:54:27.000000 got-cli-0.1.2/got_cli.egg-info/entry_points.txt
+-rw-r--r--   0 guialves   (501) staff       (20)       77 2024-05-07 12:54:27.000000 got-cli-0.1.2/got_cli.egg-info/requires.txt
+-rw-r--r--   0 guialves   (501) staff       (20)        4 2024-05-07 12:54:27.000000 got-cli-0.1.2/got_cli.egg-info/top_level.txt
+-rw-r--r--   0 guialves   (501) staff       (20)       38 2024-05-07 12:54:27.478578 got-cli-0.1.2/setup.cfg
+-rw-r--r--   0 guialves   (501) staff       (20)      685 2024-05-07 12:54:27.000000 got-cli-0.1.2/setup.py
```

### Comparing `got-cli-0.1.1/LICENSE` & `got-cli-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `got-cli-0.1.1/README.md` & `got-cli-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 got commit -a -p
 ```
 
 Options:
 
 - `-a`: Add all changes to stage before committing.
 - `-p`: Push changes to the remote repository after committing.
-- `-m`: Specify the language model to use for generating commit messages (Default: gpt-4-turbo).
+- `-m`: Specify the language model to use for generating commit messages (Default: mixtral-8x7b-32768).
 - `-t`: Specify maximum amount of tokens to be used by the model (Default: 4096).
 
   Available models: `gpt-3.5-turbo, gpt-4-turbo, gemma-7b-it, llama2-70b-4096, llama3-70b-8192, llama3-8b-8192, mixtral-8x7b-32768`
 
 ### Modifying Prompts
 
 To modify the prompts and examples used by the cli:
```

### Comparing `got-cli-0.1.1/got/ai/__init__.py` & `got-cli-0.1.2/got/ai/__init__.py`

 * *Files identical despite different names*

### Comparing `got-cli-0.1.1/got/ai/chatgpt.py` & `got-cli-0.1.2/got/ai/chatgpt.py`

 * *Files identical despite different names*

### Comparing `got-cli-0.1.1/got/ai/groq.py` & `got-cli-0.1.2/got/ai/groq.py`

 * *Files identical despite different names*

### Comparing `got-cli-0.1.1/got/cli.py` & `got-cli-0.1.2/got/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 OPENAI_MODELS = ["gpt-3.5-turbo", "gpt-4-turbo"]
 GROQ_MODELS = ["gemma-7b-it", "llama2-70b-4096", "llama3-70b-8192", "llama3-8b-8192", "mixtral-8x7b-32768"]
 
 
 @got.command()
 @click.option("-a", is_flag=True, help="Also add to stage before committing", default=False)
 @click.option("-p", is_flag=True, help="Also push to remote after commiting", default=False)
-@click.option("-m", help="LLM model", type=click.Choice([*OPENAI_MODELS, *GROQ_MODELS]), default="gpt-4-turbo")
+@click.option("-m", help="LLM model", type=click.Choice([*OPENAI_MODELS, *GROQ_MODELS]), default="mixtral-8x7b-32768")
 @click.option("-t", help="Max tokens to be used by the model", default=4096)
 def commit(a, p, m, t):
     term = Terminal()
     print(term.enter_fullscreen)
     print(term.clear)
     
     git = Git()
```

### Comparing `got-cli-0.1.1/got/commit.py` & `got-cli-0.1.2/got/commit.py`

 * *Files identical despite different names*

### Comparing `got-cli-0.1.1/got/git.py` & `got-cli-0.1.2/got/git.py`

 * *Files identical despite different names*

### Comparing `got-cli-0.1.1/got/printer.py` & `got-cli-0.1.2/got/printer.py`

 * *Files identical despite different names*

### Comparing `got-cli-0.1.1/setup.py` & `got-cli-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 #
 setup(
     name="got-cli",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     license="MIT",
     install_requires=[
         "openai==1.25.1",
         "groq==0.5.0",
         "click==8.1.3",
         "python-dotenv==1.0.1",
```

