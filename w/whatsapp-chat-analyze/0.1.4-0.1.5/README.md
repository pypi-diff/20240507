# Comparing `tmp/whatsapp_chat_analyze-0.1.4.tar.gz` & `tmp/whatsapp_chat_analyze-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp_chat_analyze-0.1.4.tar", max compression
+gzip compressed data, was "whatsapp_chat_analyze-0.1.5.tar", max compression
```

## Comparing `whatsapp_chat_analyze-0.1.4.tar` & `whatsapp_chat_analyze-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1682 2024-05-06 04:35:18.706328 whatsapp_chat_analyze-0.1.4/README.md
--rw-r--r--   0        0        0      898 2024-05-07 02:58:37.488764 whatsapp_chat_analyze-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-07 02:58:37.489721 whatsapp_chat_analyze-0.1.4/whatsapp_chat_analyze/__init__.py
--rwxr-xr-x   0        0        0    14106 2024-05-07 02:53:30.217582 whatsapp_chat_analyze-0.1.4/whatsapp_chat_analyze/cli.py
--rw-r--r--   0        0        0     2718 1970-01-01 00:00:00.000000 whatsapp_chat_analyze-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2088 2024-05-07 03:17:09.217312 whatsapp_chat_analyze-0.1.5/README.md
+-rw-r--r--   0        0        0      898 2024-05-07 03:17:15.478013 whatsapp_chat_analyze-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-07 03:17:15.478720 whatsapp_chat_analyze-0.1.5/whatsapp_chat_analyze/__init__.py
+-rwxr-xr-x   0        0        0    14106 2024-05-07 02:53:30.217582 whatsapp_chat_analyze-0.1.5/whatsapp_chat_analyze/cli.py
+-rw-r--r--   0        0        0     3124 1970-01-01 00:00:00.000000 whatsapp_chat_analyze-0.1.5/PKG-INFO
```

### Comparing `whatsapp_chat_analyze-0.1.4/README.md` & `whatsapp_chat_analyze-0.1.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -9,21 +9,30 @@
     - [pipx](#pipx)
     - [pip](#pip)
   - [Usage](#usage)
   - [Develop](#develop)
 
 ## Demo
 
+![](https://github.com/cli/cli/assets/45612704/08026ab5-24c0-4ec1-8afe-903d57654e15)
+
+For more plots and interactity, check out the blog post: https://teddysc.me/blog/whatsapp-chat-analyze .
+
 ## Features
 
+- Simple to install and use, no cloning involved, supports modern Python versions 
 - Extracts chat data from .txt or .zip files
 - Export to csv (`-c`)
+- Pretty interactive charts with plotly and save them to HTML files
+- 6 different plots, see [demo](#demo)
 
 ## Installation
 
+Python>=3.10 required.
+
 ### pipx
 
 This is the recommended installation method.
 
 ```
 $ pipx install whatsapp-chat-analyze
 ```
```

### Comparing `whatsapp_chat_analyze-0.1.4/pyproject.toml` & `whatsapp_chat_analyze-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whatsapp-chat-analyze"
-version = "0.1.4"
+version = "0.1.5"
 description = "Ingest and analyze WhatsApp chat data, and plot beautiful visualizations."
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/tddschn/whatsapp-chat-analyze"
 repository = "https://github.com/tddschn/whatsapp-chat-analyze"
 classifiers = ["Topic :: Utilities"]
```

### Comparing `whatsapp_chat_analyze-0.1.4/whatsapp_chat_analyze/cli.py` & `whatsapp_chat_analyze-0.1.5/whatsapp_chat_analyze/cli.py`

 * *Files identical despite different names*

### Comparing `whatsapp_chat_analyze-0.1.4/PKG-INFO` & `whatsapp_chat_analyze-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-chat-analyze
-Version: 0.1.4
+Version: 0.1.5
 Summary: Ingest and analyze WhatsApp chat data, and plot beautiful visualizations.
 Home-page: https://github.com/tddschn/whatsapp-chat-analyze
 License: MIT
 Keywords: cli,utility,whatsapp,chat,analyze,visualization
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
@@ -33,21 +33,30 @@
     - [pipx](#pipx)
     - [pip](#pip)
   - [Usage](#usage)
   - [Develop](#develop)
 
 ## Demo
 
+![](https://github.com/cli/cli/assets/45612704/08026ab5-24c0-4ec1-8afe-903d57654e15)
+
+For more plots and interactity, check out the blog post: https://teddysc.me/blog/whatsapp-chat-analyze .
+
 ## Features
 
+- Simple to install and use, no cloning involved, supports modern Python versions 
 - Extracts chat data from .txt or .zip files
 - Export to csv (`-c`)
+- Pretty interactive charts with plotly and save them to HTML files
+- 6 different plots, see [demo](#demo)
 
 ## Installation
 
+Python>=3.10 required.
+
 ### pipx
 
 This is the recommended installation method.
 
 ```
 $ pipx install whatsapp-chat-analyze
 ```
```

