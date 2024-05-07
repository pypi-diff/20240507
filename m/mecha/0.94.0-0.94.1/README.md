# Comparing `tmp/mecha-0.94.0.tar.gz` & `tmp/mecha-0.94.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecha-0.94.0.tar", max compression
+gzip compressed data, was "mecha-0.94.1.tar", max compression
```

## Comparing `mecha-0.94.0.tar` & `mecha-0.94.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1073 2024-04-28 23:54:56.629248 mecha-0.94.0/LICENSE
--rw-r--r--   0        0        0     8612 2024-04-28 23:54:56.629248 mecha-0.94.0/README.md
--rw-r--r--   0        0        0      344 2024-04-28 23:55:42.117950 mecha-0.94.0/mecha/__init__.py
--rw-r--r--   0        0        0       35 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/__main__.py
--rw-r--r--   0        0        0    22660 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/api.py
--rw-r--r--   0        0        0    36695 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/ast.py
--rw-r--r--   0        0        0     3057 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/cli.py
--rw-r--r--   0        0        0      719 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/commands.py
--rw-r--r--   0        0        0     6147 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/config.py
--rw-r--r--   0        0        0        0 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/__init__.py
--rw-r--r--   0        0        0     1840 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/annotate_diagnostics.py
--rw-r--r--   0        0        0    12498 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/bake_macros.py
--rw-r--r--   0        0        0      177 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/clear_diagnostics.py
--rw-r--r--   0        0        0     1096 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/debug_ast.py
--rw-r--r--   0        0        0     5840 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/embed.py
--rw-r--r--   0        0        0     2932 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/implicit_execute.py
--rw-r--r--   0        0        0     2592 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/inline_function_tag.py
--rw-r--r--   0        0        0     6358 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/json_files.py
--rw-r--r--   0        0        0     2561 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/lint_basic.py
--rw-r--r--   0        0        0     2678 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/messages.py
--rw-r--r--   0        0        0     6188 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/nested_location.py
--rw-r--r--   0        0        0    12727 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/nested_resources.py
--rw-r--r--   0        0        0     9514 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/nested_yaml.py
--rw-r--r--   0        0        0    15453 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/nesting.py
--rw-r--r--   0        0        0     1050 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/raw.py
--rw-r--r--   0        0        0     2468 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/relative_location.py
--rw-r--r--   0        0        0     2234 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/source_map.py
--rw-r--r--   0        0        0    11944 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/statistics.py
--rw-r--r--   0        0        0       21 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/validation/__init__.py
--rw-r--r--   0        0        0    38232 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/validation/mcdoc.py
--rw-r--r--   0        0        0     6205 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/database.py
--rw-r--r--   0        0        0     5964 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/diagnostic.py
--rw-r--r--   0        0        0    13332 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/dispatch.py
--rw-r--r--   0        0        0      106 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/error.py
--rw-r--r--   0        0        0    72796 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/parse.py
--rw-r--r--   0        0        0      205 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/plugin.py
--rw-r--r--   0        0        0     1181 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/preprocess.py
--rw-r--r--   0        0        0     1214 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/prototype.py
--rw-r--r--   0        0        0        0 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/py.typed
--rw-r--r--   0        0        0   257142 2024-04-28 23:54:56.641248 mecha-0.94.0/mecha/resources/1_16.json
--rw-r--r--   0        0        0   266016 2024-04-28 23:54:56.641248 mecha-0.94.0/mecha/resources/1_17.json
--rw-r--r--   0        0        0   265402 2024-04-28 23:54:56.641248 mecha-0.94.0/mecha/resources/1_18.json
--rw-r--r--   0        0        0   393608 2024-04-28 23:54:56.641248 mecha-0.94.0/mecha/resources/1_19.json
--rw-r--r--   0        0        0   396856 2024-04-28 23:54:56.641248 mecha-0.94.0/mecha/resources/1_20.json
--rw-r--r--   0        0        0        0 2024-04-28 23:54:56.641248 mecha-0.94.0/mecha/resources/__init__.py
--rw-r--r--   0        0        0      369 2024-04-28 23:54:56.641248 mecha-0.94.0/mecha/resources/inline_function_tag.json
--rw-r--r--   0        0        0     7984 2024-04-28 23:54:56.641248 mecha-0.94.0/mecha/resources/nesting.json
--rw-r--r--   0        0        0      526 2024-04-28 23:54:56.641248 mecha-0.94.0/mecha/resources/patches.json
--rw-r--r--   0        0        0    12620 2024-04-28 23:54:56.641248 mecha-0.94.0/mecha/serialize.py
--rw-r--r--   0        0        0     3440 2024-04-28 23:54:56.641248 mecha-0.94.0/mecha/spec.py
--rw-r--r--   0        0        0     6393 2024-04-28 23:54:56.641248 mecha-0.94.0/mecha/utils.py
--rw-r--r--   0        0        0     1293 2024-04-28 23:55:42.141951 mecha-0.94.0/pyproject.toml
--rw-r--r--   0        0        0     9352 1970-01-01 00:00:00.000000 mecha-0.94.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-07 17:47:27.871167 mecha-0.94.1/LICENSE
+-rw-r--r--   0        0        0     8612 2024-05-07 17:47:27.871167 mecha-0.94.1/README.md
+-rw-r--r--   0        0        0      344 2024-05-07 17:48:13.823292 mecha-0.94.1/mecha/__init__.py
+-rw-r--r--   0        0        0       35 2024-05-07 17:47:27.879167 mecha-0.94.1/mecha/__main__.py
+-rw-r--r--   0        0        0    22660 2024-05-07 17:47:27.879167 mecha-0.94.1/mecha/api.py
+-rw-r--r--   0        0        0    36695 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/ast.py
+-rw-r--r--   0        0        0     3057 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/cli.py
+-rw-r--r--   0        0        0      719 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/commands.py
+-rw-r--r--   0        0        0     6147 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/config.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/contrib/__init__.py
+-rw-r--r--   0        0        0     1840 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/contrib/annotate_diagnostics.py
+-rw-r--r--   0        0        0    12498 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/contrib/bake_macros.py
+-rw-r--r--   0        0        0      177 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/contrib/clear_diagnostics.py
+-rw-r--r--   0        0        0     1096 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/contrib/debug_ast.py
+-rw-r--r--   0        0        0     5840 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/contrib/embed.py
+-rw-r--r--   0        0        0     2932 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/contrib/implicit_execute.py
+-rw-r--r--   0        0        0     2592 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/contrib/inline_function_tag.py
+-rw-r--r--   0        0        0     6358 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/contrib/json_files.py
+-rw-r--r--   0        0        0     2561 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/contrib/lint_basic.py
+-rw-r--r--   0        0        0     2678 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/contrib/messages.py
+-rw-r--r--   0        0        0     6188 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/contrib/nested_location.py
+-rw-r--r--   0        0        0    12727 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/contrib/nested_resources.py
+-rw-r--r--   0        0        0     9514 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/contrib/nested_yaml.py
+-rw-r--r--   0        0        0    15453 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/contrib/nesting.py
+-rw-r--r--   0        0        0     1050 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/contrib/raw.py
+-rw-r--r--   0        0        0     2468 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/contrib/relative_location.py
+-rw-r--r--   0        0        0     2234 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/contrib/source_map.py
+-rw-r--r--   0        0        0    11944 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/contrib/statistics.py
+-rw-r--r--   0        0        0       21 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/contrib/validation/__init__.py
+-rw-r--r--   0        0        0    38232 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/contrib/validation/mcdoc.py
+-rw-r--r--   0        0        0     6205 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/database.py
+-rw-r--r--   0        0        0     5964 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/diagnostic.py
+-rw-r--r--   0        0        0    13332 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/dispatch.py
+-rw-r--r--   0        0        0      106 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/error.py
+-rw-r--r--   0        0        0    72796 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/parse.py
+-rw-r--r--   0        0        0      205 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/plugin.py
+-rw-r--r--   0        0        0     1181 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/preprocess.py
+-rw-r--r--   0        0        0     1214 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/prototype.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/py.typed
+-rw-r--r--   0        0        0   257142 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/resources/1_16.json
+-rw-r--r--   0        0        0   266016 2024-05-07 17:47:27.883167 mecha-0.94.1/mecha/resources/1_17.json
+-rw-r--r--   0        0        0   265402 2024-05-07 17:47:27.887167 mecha-0.94.1/mecha/resources/1_18.json
+-rw-r--r--   0        0        0   393608 2024-05-07 17:47:27.887167 mecha-0.94.1/mecha/resources/1_19.json
+-rw-r--r--   0        0        0   396856 2024-05-07 17:47:27.887167 mecha-0.94.1/mecha/resources/1_20.json
+-rw-r--r--   0        0        0        0 2024-05-07 17:47:27.887167 mecha-0.94.1/mecha/resources/__init__.py
+-rw-r--r--   0        0        0      369 2024-05-07 17:47:27.887167 mecha-0.94.1/mecha/resources/inline_function_tag.json
+-rw-r--r--   0        0        0     7984 2024-05-07 17:47:27.887167 mecha-0.94.1/mecha/resources/nesting.json
+-rw-r--r--   0        0        0      526 2024-05-07 17:47:27.887167 mecha-0.94.1/mecha/resources/patches.json
+-rw-r--r--   0        0        0    12620 2024-05-07 17:47:27.887167 mecha-0.94.1/mecha/serialize.py
+-rw-r--r--   0        0        0     3440 2024-05-07 17:47:27.887167 mecha-0.94.1/mecha/spec.py
+-rw-r--r--   0        0        0     6492 2024-05-07 17:47:27.887167 mecha-0.94.1/mecha/utils.py
+-rw-r--r--   0        0        0     1293 2024-05-07 17:48:13.847292 mecha-0.94.1/pyproject.toml
+-rw-r--r--   0        0        0     9352 1970-01-01 00:00:00.000000 mecha-0.94.1/PKG-INFO
```

### Comparing `mecha-0.94.0/LICENSE` & `mecha-0.94.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/README.md` & `mecha-0.94.1/README.md`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/api.py` & `mecha-0.94.1/mecha/api.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/ast.py` & `mecha-0.94.1/mecha/ast.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/cli.py` & `mecha-0.94.1/mecha/cli.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/commands.py` & `mecha-0.94.1/mecha/commands.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/config.py` & `mecha-0.94.1/mecha/config.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/contrib/annotate_diagnostics.py` & `mecha-0.94.1/mecha/contrib/annotate_diagnostics.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/contrib/bake_macros.py` & `mecha-0.94.1/mecha/contrib/bake_macros.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/contrib/debug_ast.py` & `mecha-0.94.1/mecha/contrib/debug_ast.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/contrib/embed.py` & `mecha-0.94.1/mecha/contrib/embed.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/contrib/implicit_execute.py` & `mecha-0.94.1/mecha/contrib/implicit_execute.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/contrib/inline_function_tag.py` & `mecha-0.94.1/mecha/contrib/inline_function_tag.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/contrib/json_files.py` & `mecha-0.94.1/mecha/contrib/json_files.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/contrib/lint_basic.py` & `mecha-0.94.1/mecha/contrib/lint_basic.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/contrib/messages.py` & `mecha-0.94.1/mecha/contrib/messages.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/contrib/nested_location.py` & `mecha-0.94.1/mecha/contrib/nested_location.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/contrib/nested_resources.py` & `mecha-0.94.1/mecha/contrib/nested_resources.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/contrib/nested_yaml.py` & `mecha-0.94.1/mecha/contrib/nested_yaml.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/contrib/nesting.py` & `mecha-0.94.1/mecha/contrib/nesting.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/contrib/raw.py` & `mecha-0.94.1/mecha/contrib/raw.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/contrib/relative_location.py` & `mecha-0.94.1/mecha/contrib/relative_location.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/contrib/source_map.py` & `mecha-0.94.1/mecha/contrib/source_map.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/contrib/statistics.py` & `mecha-0.94.1/mecha/contrib/statistics.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/contrib/validation/mcdoc.py` & `mecha-0.94.1/mecha/contrib/validation/mcdoc.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/database.py` & `mecha-0.94.1/mecha/database.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/diagnostic.py` & `mecha-0.94.1/mecha/diagnostic.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/dispatch.py` & `mecha-0.94.1/mecha/dispatch.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/parse.py` & `mecha-0.94.1/mecha/parse.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/preprocess.py` & `mecha-0.94.1/mecha/preprocess.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/prototype.py` & `mecha-0.94.1/mecha/prototype.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/resources/1_16.json` & `mecha-0.94.1/mecha/resources/1_16.json`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/resources/1_17.json` & `mecha-0.94.1/mecha/resources/1_17.json`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/resources/1_18.json` & `mecha-0.94.1/mecha/resources/1_18.json`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/resources/1_19.json` & `mecha-0.94.1/mecha/resources/1_19.json`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/resources/1_20.json` & `mecha-0.94.1/mecha/resources/1_20.json`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/resources/nesting.json` & `mecha-0.94.1/mecha/resources/nesting.json`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/resources/patches.json` & `mecha-0.94.1/mecha/resources/patches.json`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/serialize.py` & `mecha-0.94.1/mecha/serialize.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/spec.py` & `mecha-0.94.1/mecha/spec.py`

 * *Files identical despite different names*

### Comparing `mecha-0.94.0/mecha/utils.py` & `mecha-0.94.1/mecha/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,16 +40,17 @@
     """Helper for converting numbers to string and keeping their original type."""
     return float(string) if "." in string or "e" in string else int(string)
 
 
 def number_to_string(number: Union[int, float]) -> str:
     """Helper for converting numbers to string and removing scientific notation."""
     value = str(number)
-    if "e" in value:
-        value = f"{number:.20f}".rstrip("0")
+    if (index := value.find("e")) != -1:
+        exponent = int(value[index + 1 :])
+        value = f"{number:.{max(index - 1 - (value[1] == '.') - exponent, 1)}f}"
     return value
 
 
 class InvalidEscapeSequence(MechaError):
     """Raised when a QuotedStringHandler encounters an invalid escape sequence."""
 
     characters: str
```

### Comparing `mecha-0.94.0/pyproject.toml` & `mecha-0.94.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mecha"
-version = "0.94.0"
+version = "0.94.1"
 description = "A powerful Minecraft command library"
 authors = ["Valentin Berlier <berlier.v@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/mcbeet/mecha"
 repository = "https://github.com/mcbeet/mecha"
 documentation = "https://github.com/mcbeet/mecha"
```

### Comparing `mecha-0.94.0/PKG-INFO` & `mecha-0.94.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecha
-Version: 0.94.0
+Version: 0.94.1
 Summary: A powerful Minecraft command library
 Home-page: https://github.com/mcbeet/mecha
 License: MIT
 Keywords: beet,minecraft,datapack,minecraft-commands,mcfunction
 Author: Valentin Berlier
 Author-email: berlier.v@gmail.com
 Requires-Python: >=3.10,<4.0
```

