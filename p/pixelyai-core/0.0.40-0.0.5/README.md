# Comparing `tmp/pixelyai_core-0.0.40.tar.gz` & `tmp/pixelyai_core-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixelyai_core-0.0.40.tar", last modified: Tue May  7 09:36:49 2024, max compression
+gzip compressed data, was "pixelyai_core-0.0.5.tar", last modified: Sat Jan  6 09:35:10 2024, max compression
```

## Comparing `pixelyai_core-0.0.40.tar` & `pixelyai_core-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,37 @@
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-05-07 09:36:49.296673 pixelyai_core-0.0.40/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1506 2024-05-05 12:37:22.000000 pixelyai_core-0.0.40/LICENSE
--rw-r--r--   0 erfan     (1000) erfan     (1000)     6265 2024-05-07 09:36:49.292674 pixelyai_core-0.0.40/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     4817 2024-05-05 12:37:22.000000 pixelyai_core-0.0.40/README.md
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1535 2024-05-07 09:32:41.000000 pixelyai_core-0.0.40/pyproject.toml
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2024-05-07 09:36:49.296673 pixelyai_core-0.0.40/setup.cfg
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-05-07 09:36:49.292674 pixelyai_core-0.0.40/src/
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-05-07 09:36:49.292674 pixelyai_core-0.0.40/src/pixelyai_core/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      273 2024-05-07 09:32:41.000000 pixelyai_core-0.0.40/src/pixelyai_core/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2815 2024-05-05 14:10:14.000000 pixelyai_core-0.0.40/src/pixelyai_core/client.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-05-07 09:36:49.292674 pixelyai_core-0.0.40/src/pixelyai_core/engine_websocket/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2024-05-05 12:37:22.000000 pixelyai_core-0.0.40/src/pixelyai_core/engine_websocket/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      105 2024-05-05 12:37:22.000000 pixelyai_core-0.0.40/src/pixelyai_core/engine_websocket/client.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1124 2024-05-05 12:37:22.000000 pixelyai_core-0.0.40/src/pixelyai_core/engine_websocket/serve.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-05-07 09:36:49.292674 pixelyai_core-0.0.40/src/pixelyai_core/prompt_templates/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      153 2024-05-05 12:37:22.000000 pixelyai_core-0.0.40/src/pixelyai_core/prompt_templates/__init__.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-05-07 09:36:49.292674 pixelyai_core-0.0.40/src/pixelyai_core/prompt_templates/chat/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       42 2024-05-05 12:37:22.000000 pixelyai_core-0.0.40/src/pixelyai_core/prompt_templates/chat/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      625 2024-05-05 12:37:22.000000 pixelyai_core-0.0.40/src/pixelyai_core/prompt_templates/chat/agnet.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      884 2024-05-07 09:31:52.000000 pixelyai_core-0.0.40/src/pixelyai_core/prompt_templates/chat/prompt.jinja2
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-05-07 09:36:49.292674 pixelyai_core-0.0.40/src/pixelyai_core/prompt_templates/retrival_argumented_generation/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       40 2024-05-05 12:37:22.000000 pixelyai_core-0.0.40/src/pixelyai_core/prompt_templates/retrival_argumented_generation/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      689 2024-05-05 12:37:22.000000 pixelyai_core-0.0.40/src/pixelyai_core/prompt_templates/retrival_argumented_generation/agent.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1129 2024-05-07 09:31:52.000000 pixelyai_core-0.0.40/src/pixelyai_core/prompt_templates/retrival_argumented_generation/prompt.jinja2
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-05-07 09:36:49.292674 pixelyai_core-0.0.40/src/pixelyai_core/serving/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       56 2024-05-05 12:37:22.000000 pixelyai_core-0.0.40/src/pixelyai_core/serving/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3530 2024-05-05 12:37:22.000000 pixelyai_core-0.0.40/src/pixelyai_core/serving/engine_module.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-05-07 09:36:49.292674 pixelyai_core-0.0.40/src/pixelyai_core.egg-info/
--rw-r--r--   0 erfan     (1000) erfan     (1000)     6265 2024-05-07 09:36:49.000000 pixelyai_core-0.0.40/src/pixelyai_core.egg-info/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      946 2024-05-07 09:36:49.000000 pixelyai_core-0.0.40/src/pixelyai_core.egg-info/SOURCES.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2024-05-07 09:36:49.000000 pixelyai_core-0.0.40/src/pixelyai_core.egg-info/dependency_links.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      262 2024-05-07 09:36:49.000000 pixelyai_core-0.0.40/src/pixelyai_core.egg-info/requires.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       14 2024-05-07 09:36:49.000000 pixelyai_core-0.0.40/src/pixelyai_core.egg-info/top_level.txt
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-01-06 09:35:10.399007 pixelyai_core-0.0.5/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1506 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/LICENSE
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3081 2024-01-06 09:35:10.399007 pixelyai_core-0.0.5/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2198 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/README.md
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      616 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/pyproject.toml
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2024-01-06 09:35:10.399007 pixelyai_core-0.0.5/setup.cfg
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1547 2024-01-06 09:35:07.000000 pixelyai_core-0.0.5/setup.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-01-06 09:35:10.395007 pixelyai_core-0.0.5/src/
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-01-06 09:35:10.395007 pixelyai_core-0.0.5/src/python/
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-01-06 09:35:10.395007 pixelyai_core-0.0.5/src/python/pixelyai_core/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       46 2024-01-06 09:35:07.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-01-06 09:35:10.395007 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      536 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-01-06 09:35:10.395007 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/ggml_serve/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       45 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/ggml_serve/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     6245 2024-01-06 09:34:43.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/ggml_serve/_serve_module.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-01-06 09:35:10.399007 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/ggml_serve/inference/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       33 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/ggml_serve/inference/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1904 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/ggml_serve/inference/_setting.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     8653 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/ggml_serve/inference/inference.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-01-06 09:35:10.399007 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/jax_serve/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       44 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/jax_serve/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3030 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/jax_serve/_serve_module.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-01-06 09:35:10.399007 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/torch_serve/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       46 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/torch_serve/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1766 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/torch_serve/_serve_module.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-01-06 09:35:10.399007 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/user_interface/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       56 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/user_interface/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5419 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/user_interface/_gradio_user_interface.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4362 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/user_interface/_utils.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    25323 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/utils.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-01-06 09:35:10.395007 pixelyai_core-0.0.5/src/python/pixelyai_core.egg-info/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3081 2024-01-06 09:35:10.000000 pixelyai_core-0.0.5/src/python/pixelyai_core.egg-info/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1146 2024-01-06 09:35:10.000000 pixelyai_core-0.0.5/src/python/pixelyai_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2024-01-06 09:35:10.000000 pixelyai_core-0.0.5/src/python/pixelyai_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      241 2024-01-06 09:35:10.000000 pixelyai_core-0.0.5/src/python/pixelyai_core.egg-info/requires.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       14 2024-01-06 09:35:10.000000 pixelyai_core-0.0.5/src/python/pixelyai_core.egg-info/top_level.txt
```

### Comparing `pixelyai_core-0.0.40/LICENSE` & `pixelyai_core-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pixelyai_core-0.0.40/pyproject.toml` & `pixelyai_core-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,45 @@
-[project]
+from setuptools import setup, find_packages
 
-name = "pixelyai-core"
-version = "0.0.40"
-
-authors = [
-    { name = "Erfan Zare Chavoshi", email = "Erfanzare810@gmail.com" }
-]
-requires-python = ">=3.8"
-
-readme = "README.md"
-
-dependencies = [
-    "typing~=3.7.4.3",
-    "ipython~=8.17.2",
-    "tqdm~=4.64.1",
-    "pydantic==2.5.3",
-    "setuptools~=68.1.2",
-    "gradio~=4.18.0",
-    "numpy~=1.26.2",
-    "uvicorn~=0.23.2",
-    "fastapi==0.110.1",
-    "pydantic-core==2.14.6",
-    "requests~=2.31.0",
-    "transformers>=4.36.1",
-    "huggingface-hub>=0.20.1",
-    "absl-py==2.0.0",
-    "Jinja2~=3.1.2",
-    "agentx"
-]
-
-classifiers = [
-    "Development Status :: 3 - Alpha",
-    "Intended Audience :: Developers",
-    "Topic :: Scientific/Engineering :: Artificial Intelligence",
-    "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
-]
-description = "PixelyAI Serve Engine"
-
-[project.urls]
-
-Homepage = "https://github.com/erfanzar/PixelyAI"
-Issues = "https://github.com/erfanzar/PixelyAI/issues"
-Documentation = "https://erfanzar.github.io/PixelyAI"
-
-[build-system]
-
-requires = ["setuptools>=42", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[tool.setuptools]
-packages = ["pixelyai_core"]
-package-dir = { "" = "src" }
-
-[tool.setuptools.package-data]
-"pixelyai_core" = ["**/*.jinja2", "**/*.py"]
+setup(
+    name="pixelyai_core",
+    version="0.0.5",
+    author="Erfan Zare Chavoshi",
+    author_email="erfanzare82@eyahoo.com",
+    description="Serve Utilises of PixelyAI",
+    url="https://github.com/erfanzar/PixelyAI",
+    packages=find_packages("src/python"),
+    long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
+    classifiers=[
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "Topic :: Scientific/Engineering :: Artificial Intelligence",
+        "License :: OSI Approved :: Apache Software License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+    ],
+    keywords="machine learning, deep learning, pytorch, jax, flax, ggml, c++",
+    install_requires=[
+        "typing~=3.7.4.3",
+        "ipython~=8.17.2",
+        "tqdm~=4.64.1",
+        "pydantic==2.5.3",
+        "setuptools~=68.1.2",
+        "gradio~=4.12.0",
+        "numpy~=1.26.2",
+        "uvicorn~=0.23.2",
+        "fastapi~=0.104.1",
+        "pydantic-core==2.14.6",
+        "requests~=2.31.0",
+        "transformers~=4.36.1",
+        "huggingface-hub==0.20.1",
+        "absl-py==2.0.0",
+    ],
+    python_requires=">=3.8",
+    package_dir={"": "src/python"},
+    password="PixelyAICore"
+)
```

