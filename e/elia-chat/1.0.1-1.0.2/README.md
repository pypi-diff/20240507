# Comparing `tmp/elia_chat-1.0.1.tar.gz` & `tmp/elia_chat-1.0.2.tar.gz`

## Comparing `elia_chat-1.0.1.tar` & `elia_chat-1.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 elia_chat-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 elia_chat-1.0.1/.python-version
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 elia_chat-1.0.1/requirements-dev.lock
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 elia_chat-1.0.1/requirements.lock
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 elia_chat-1.0.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/__init__.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/__main__.py
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/app.py
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/chats_manager.py
--rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/config.py
--rw-r--r--   0        0        0     8500 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/elia.scss
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/launch_args.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/locations.py
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/models.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/runtime_config.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/time_display.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/database/__init__.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/database/converters.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/database/database.py
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/database/import_chatgpt.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/database/models.py
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/screens/chat_details.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/screens/chat_screen.py
--rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/screens/help_screen.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/screens/home_screen.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/widgets/agent_is_typing.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/widgets/app_header.py
--rw-r--r--   0        0        0    10418 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/widgets/chat.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/widgets/chat_header.py
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/widgets/chat_list.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/widgets/chat_options.py
--rw-r--r--   0        0        0     5470 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/widgets/chatbox.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/widgets/prompt_input.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 elia_chat-1.0.1/elia_chat/widgets/token_analysis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 elia_chat-1.0.1/.gitignore
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 elia_chat-1.0.1/README.md
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 elia_chat-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 elia_chat-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 elia_chat-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 elia_chat-1.0.2/.python-version
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 elia_chat-1.0.2/requirements-dev.lock
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 elia_chat-1.0.2/requirements.lock
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 elia_chat-1.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/__init__.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/__main__.py
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/app.py
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/chats_manager.py
+-rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/config.py
+-rw-r--r--   0        0        0     8500 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/elia.scss
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/launch_args.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/locations.py
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/models.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/runtime_config.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/time_display.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/database/__init__.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/database/converters.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/database/database.py
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/database/import_chatgpt.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/database/models.py
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/screens/chat_details.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/screens/chat_screen.py
+-rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/screens/help_screen.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/screens/home_screen.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/widgets/agent_is_typing.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/widgets/app_header.py
+-rw-r--r--   0        0        0    10418 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/widgets/chat.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/widgets/chat_header.py
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/widgets/chat_list.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/widgets/chat_options.py
+-rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/widgets/chatbox.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/widgets/prompt_input.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 elia_chat-1.0.2/elia_chat/widgets/token_analysis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 elia_chat-1.0.2/.gitignore
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 elia_chat-1.0.2/README.md
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 elia_chat-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 elia_chat-1.0.2/PKG-INFO
```

### Comparing `elia_chat-1.0.1/.pre-commit-config.yaml` & `elia_chat-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/requirements-dev.lock` & `elia_chat-1.0.2/requirements-dev.lock`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 frozenlist==1.4.1
     # via aiohttp
     # via aiosignal
 fsspec==2024.3.1
     # via huggingface-hub
 greenlet==3.0.3
     # via elia-chat
-    # via sqlalchemy
 h11==0.14.0
     # via httpcore
 httpcore==1.0.2
     # via httpx
 httpx==0.26.0
     # via openai
 huggingface-hub==0.22.2
```

### Comparing `elia_chat-1.0.1/requirements.lock` & `elia_chat-1.0.2/requirements.lock`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 frozenlist==1.4.1
     # via aiohttp
     # via aiosignal
 fsspec==2024.3.1
     # via huggingface-hub
 greenlet==3.0.3
     # via elia-chat
-    # via sqlalchemy
 h11==0.14.0
     # via httpcore
 httpcore==1.0.2
     # via httpx
 httpx==0.26.0
     # via openai
 huggingface-hub==0.22.2
```

### Comparing `elia_chat-1.0.1/elia_chat/__main__.py` & `elia_chat-1.0.2/elia_chat/__main__.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/elia_chat/app.py` & `elia_chat-1.0.2/elia_chat/app.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/elia_chat/chats_manager.py` & `elia_chat-1.0.2/elia_chat/chats_manager.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/elia_chat/config.py` & `elia_chat-1.0.2/elia_chat/config.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/elia_chat/elia.scss` & `elia_chat-1.0.2/elia_chat/elia.scss`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/elia_chat/locations.py` & `elia_chat-1.0.2/elia_chat/locations.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/elia_chat/models.py` & `elia_chat-1.0.2/elia_chat/models.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/elia_chat/time_display.py` & `elia_chat-1.0.2/elia_chat/time_display.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/elia_chat/database/converters.py` & `elia_chat-1.0.2/elia_chat/database/converters.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/elia_chat/database/database.py` & `elia_chat-1.0.2/elia_chat/database/database.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/elia_chat/database/import_chatgpt.py` & `elia_chat-1.0.2/elia_chat/database/import_chatgpt.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/elia_chat/database/models.py` & `elia_chat-1.0.2/elia_chat/database/models.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/elia_chat/screens/chat_details.py` & `elia_chat-1.0.2/elia_chat/screens/chat_details.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/elia_chat/screens/chat_screen.py` & `elia_chat-1.0.2/elia_chat/screens/chat_screen.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/elia_chat/screens/help_screen.py` & `elia_chat-1.0.2/elia_chat/screens/help_screen.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/elia_chat/screens/home_screen.py` & `elia_chat-1.0.2/elia_chat/screens/home_screen.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/elia_chat/widgets/app_header.py` & `elia_chat-1.0.2/elia_chat/widgets/app_header.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/elia_chat/widgets/chat.py` & `elia_chat-1.0.2/elia_chat/widgets/chat.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/elia_chat/widgets/chat_header.py` & `elia_chat-1.0.2/elia_chat/widgets/chat_header.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/elia_chat/widgets/chat_list.py` & `elia_chat-1.0.2/elia_chat/widgets/chat_list.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/elia_chat/widgets/chat_options.py` & `elia_chat-1.0.2/elia_chat/widgets/chat_options.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/elia_chat/widgets/chatbox.py` & `elia_chat-1.0.2/elia_chat/widgets/chatbox.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from rich.console import RenderableType
 from rich.markdown import Markdown
+from rich.syntax import Syntax
 from textual.binding import Binding
 from textual.css.query import NoMatches
 from textual.geometry import Size
 from textual.reactive import reactive
 from textual.widget import Widget
 from textual.widgets import TextArea
 
@@ -125,26 +126,31 @@
             else:
                 child.focus()
 
     @property
     def markdown(self) -> Markdown:
         """Return the content as a Rich Markdown object."""
         content = self.message.message.get("content")
-        if isinstance(content, str):
-            content = content.replace("<", "\\<")
-            content = content.replace(">", "\\>")
-        else:
+        if not isinstance(content, str):
             content = ""
         return Markdown(content)
 
     def render(self) -> RenderableType:
         if self.selection_mode:
             # When in selection mode, this widget has a TextArea child,
             # so we do not need to render anything.
             return ""
+
+        message = self.message.message
+        if message["role"] == "user":
+            content = message["content"] or ""
+            if isinstance(content, str):
+                return Syntax(content, lexer="markdown", background_color="#121212")
+            else:
+                return ""
         return self.markdown
 
     def get_content_width(self, container: Size, viewport: Size) -> int:
         # Naive approach. Can sometimes look strange, but works well enough.
         content = self.message.message.get("content")
         if isinstance(content, str):
             content_width = min(len(content), container.width)
```

### Comparing `elia_chat-1.0.1/elia_chat/widgets/prompt_input.py` & `elia_chat-1.0.2/elia_chat/widgets/prompt_input.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/elia_chat/widgets/token_analysis.py` & `elia_chat-1.0.2/elia_chat/widgets/token_analysis.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/.gitignore` & `elia_chat-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.1/README.md` & `elia_chat-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -81,9 +81,9 @@
 ```bash
 elia reset
 ```
 
 ### Uninstalling
 
 ```bash
-pipx uninstall elia
+pipx uninstall elia-chat
 ```
```

### Comparing `elia_chat-1.0.1/pyproject.toml` & `elia_chat-1.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "elia_chat"
-version = "1.0.1"
+version = "1.0.2"
 description = "A powerful terminal user interface for interacting with large language models."
 authors = [
     { name = "Darren Burns", email = "darrenb900@gmail.com" }
 ]
 dependencies = [
     "textual[syntax]==0.58.1",
     "sqlmodel>=0.0.9",
```

### Comparing `elia_chat-1.0.1/PKG-INFO` & `elia_chat-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: elia_chat
-Version: 1.0.1
+Version: 1.0.2
 Summary: A powerful terminal user interface for interacting with large language models.
 Author-email: Darren Burns <darrenb900@gmail.com>
 Requires-Python: >=3.11
 Requires-Dist: aiosqlite>=0.20.0
 Requires-Dist: click-default-group>=1.2.4
 Requires-Dist: click>=8.1.6
 Requires-Dist: greenlet>=3.0.3
@@ -99,9 +99,9 @@
 ```bash
 elia reset
 ```
 
 ### Uninstalling
 
 ```bash
-pipx uninstall elia
+pipx uninstall elia-chat
 ```
```

