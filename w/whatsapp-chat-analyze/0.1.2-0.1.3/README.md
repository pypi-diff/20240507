# Comparing `tmp/whatsapp_chat_analyze-0.1.2.tar.gz` & `tmp/whatsapp_chat_analyze-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp_chat_analyze-0.1.2.tar", max compression
+gzip compressed data, was "whatsapp_chat_analyze-0.1.3.tar", max compression
```

## Comparing `whatsapp_chat_analyze-0.1.2.tar` & `whatsapp_chat_analyze-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1682 2024-05-06 04:35:18.706328 whatsapp_chat_analyze-0.1.2/README.md
--rw-r--r--   0        0        0      898 2024-05-06 04:36:39.949573 whatsapp_chat_analyze-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-06 04:36:39.950136 whatsapp_chat_analyze-0.1.2/whatsapp_chat_analyze/__init__.py
--rwxr-xr-x   0        0        0    10780 2024-05-06 04:36:33.023041 whatsapp_chat_analyze-0.1.2/whatsapp_chat_analyze/cli.py
--rw-r--r--   0        0        0     2718 1970-01-01 00:00:00.000000 whatsapp_chat_analyze-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1682 2024-05-06 04:35:18.706328 whatsapp_chat_analyze-0.1.3/README.md
+-rw-r--r--   0        0        0      898 2024-05-06 14:52:24.856626 whatsapp_chat_analyze-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-06 14:52:24.859608 whatsapp_chat_analyze-0.1.3/whatsapp_chat_analyze/__init__.py
+-rwxr-xr-x   0        0        0    10916 2024-05-06 14:52:05.397668 whatsapp_chat_analyze-0.1.3/whatsapp_chat_analyze/cli.py
+-rw-r--r--   0        0        0     2718 1970-01-01 00:00:00.000000 whatsapp_chat_analyze-0.1.3/PKG-INFO
```

### Comparing `whatsapp_chat_analyze-0.1.2/README.md` & `whatsapp_chat_analyze-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `whatsapp_chat_analyze-0.1.2/pyproject.toml` & `whatsapp_chat_analyze-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whatsapp-chat-analyze"
-version = "0.1.2"
+version = "0.1.3"
 description = "Ingest and analyze WhatsApp chat data, and plot beautiful visualizations."
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/tddschn/whatsapp-chat-analyze"
 repository = "https://github.com/tddschn/whatsapp-chat-analyze"
 classifiers = ["Topic :: Utilities"]
```

### Comparing `whatsapp_chat_analyze-0.1.2/whatsapp_chat_analyze/cli.py` & `whatsapp_chat_analyze-0.1.3/whatsapp_chat_analyze/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,21 @@
     parser.add_argument(
         "-a",
         "--anonymize",
         help="Anonymize the chat by replacing author names with generic names",
         action="store_true",
     )
 
+    parser.add_argument(
+        "-V",
+        "--version",
+        action="version",
+        version=f"%(prog)s {__version__}",
+    )
+
     return parser.parse_args()
 
 
 def parse_chat(chat_file):
     import re
 
     DATE_TIME = re.compile(
```

### Comparing `whatsapp_chat_analyze-0.1.2/PKG-INFO` & `whatsapp_chat_analyze-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-chat-analyze
-Version: 0.1.2
+Version: 0.1.3
 Summary: Ingest and analyze WhatsApp chat data, and plot beautiful visualizations.
 Home-page: https://github.com/tddschn/whatsapp-chat-analyze
 License: MIT
 Keywords: cli,utility,whatsapp,chat,analyze,visualization
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
```

