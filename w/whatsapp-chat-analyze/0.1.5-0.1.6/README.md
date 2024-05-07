# Comparing `tmp/whatsapp_chat_analyze-0.1.5.tar.gz` & `tmp/whatsapp_chat_analyze-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp_chat_analyze-0.1.5.tar", max compression
+gzip compressed data, was "whatsapp_chat_analyze-0.1.6.tar", max compression
```

## Comparing `whatsapp_chat_analyze-0.1.5.tar` & `whatsapp_chat_analyze-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2088 2024-05-07 03:17:09.217312 whatsapp_chat_analyze-0.1.5/README.md
--rw-r--r--   0        0        0      898 2024-05-07 03:17:15.478013 whatsapp_chat_analyze-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-07 03:17:15.478720 whatsapp_chat_analyze-0.1.5/whatsapp_chat_analyze/__init__.py
--rwxr-xr-x   0        0        0    14106 2024-05-07 02:53:30.217582 whatsapp_chat_analyze-0.1.5/whatsapp_chat_analyze/cli.py
--rw-r--r--   0        0        0     3124 1970-01-01 00:00:00.000000 whatsapp_chat_analyze-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     2143 2024-05-07 03:25:04.966162 whatsapp_chat_analyze-0.1.6/README.md
+-rw-r--r--   0        0        0      898 2024-05-07 03:25:08.855885 whatsapp_chat_analyze-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-07 03:25:08.856319 whatsapp_chat_analyze-0.1.6/whatsapp_chat_analyze/__init__.py
+-rwxr-xr-x   0        0        0    14106 2024-05-07 02:53:30.217582 whatsapp_chat_analyze-0.1.6/whatsapp_chat_analyze/cli.py
+-rw-r--r--   0        0        0     3179 1970-01-01 00:00:00.000000 whatsapp_chat_analyze-0.1.6/PKG-INFO
```

### Comparing `whatsapp_chat_analyze-0.1.5/README.md` & `whatsapp_chat_analyze-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 ## Features
 
 - Simple to install and use, no cloning involved, supports modern Python versions 
 - Extracts chat data from .txt or .zip files
 - Export to csv (`-c`)
 - Pretty interactive charts with plotly and save them to HTML files
 - 6 different plots, see [demo](#demo)
+- Anonymize sender names to `A`, `B`, `C`, etc. (`-a`)
 
 ## Installation
 
 Python>=3.10 required.
 
 ### pipx
```

### Comparing `whatsapp_chat_analyze-0.1.5/pyproject.toml` & `whatsapp_chat_analyze-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whatsapp-chat-analyze"
-version = "0.1.5"
+version = "0.1.6"
 description = "Ingest and analyze WhatsApp chat data, and plot beautiful visualizations."
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/tddschn/whatsapp-chat-analyze"
 repository = "https://github.com/tddschn/whatsapp-chat-analyze"
 classifiers = ["Topic :: Utilities"]
```

### Comparing `whatsapp_chat_analyze-0.1.5/whatsapp_chat_analyze/cli.py` & `whatsapp_chat_analyze-0.1.6/whatsapp_chat_analyze/cli.py`

 * *Files identical despite different names*

### Comparing `whatsapp_chat_analyze-0.1.5/PKG-INFO` & `whatsapp_chat_analyze-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-chat-analyze
-Version: 0.1.5
+Version: 0.1.6
 Summary: Ingest and analyze WhatsApp chat data, and plot beautiful visualizations.
 Home-page: https://github.com/tddschn/whatsapp-chat-analyze
 License: MIT
 Keywords: cli,utility,whatsapp,chat,analyze,visualization
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
@@ -44,14 +44,15 @@
 ## Features
 
 - Simple to install and use, no cloning involved, supports modern Python versions 
 - Extracts chat data from .txt or .zip files
 - Export to csv (`-c`)
 - Pretty interactive charts with plotly and save them to HTML files
 - 6 different plots, see [demo](#demo)
+- Anonymize sender names to `A`, `B`, `C`, etc. (`-a`)
 
 ## Installation
 
 Python>=3.10 required.
 
 ### pipx
```

