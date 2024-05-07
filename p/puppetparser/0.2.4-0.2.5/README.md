# Comparing `tmp/puppetparser-0.2.4.tar.gz` & `tmp/puppetparser-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puppetparser-0.2.4.tar", max compression
+gzip compressed data, was "puppetparser-0.2.5.tar", max compression
```

## Comparing `puppetparser-0.2.4.tar` & `puppetparser-0.2.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2024-01-03 13:45:14.417814 puppetparser-0.2.4/LICENSE
--rw-r--r--   0        0        0      804 2024-03-22 17:40:49.304234 puppetparser-0.2.4/README.md
--rw-r--r--   0        0        0       22 2024-01-03 13:45:14.417814 puppetparser-0.2.4/puppetparser/.gitignore
--rw-r--r--   0        0        0        0 2024-01-03 13:45:14.417814 puppetparser-0.2.4/puppetparser/__init__.py
--rw-r--r--   0        0        0       98 2024-03-22 19:57:57.298496 puppetparser-0.2.4/puppetparser/__main__.py
--rw-r--r--   0        0        0    11508 2024-03-23 11:56:14.207085 puppetparser-0.2.4/puppetparser/model.py
--rw-r--r--   0        0        0    64993 2024-03-22 19:57:58.390481 puppetparser-0.2.4/puppetparser/parser.py
--rw-r--r--   0        0        0     1001 2024-03-23 11:55:51.303418 puppetparser-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 puppetparser-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-01-03 13:45:14.417814 puppetparser-0.2.5/LICENSE
+-rw-r--r--   0        0        0      804 2024-03-22 17:40:49.304234 puppetparser-0.2.5/README.md
+-rw-r--r--   0        0        0       22 2024-01-03 13:45:14.417814 puppetparser-0.2.5/puppetparser/.gitignore
+-rw-r--r--   0        0        0        0 2024-01-03 13:45:14.417814 puppetparser-0.2.5/puppetparser/__init__.py
+-rw-r--r--   0        0        0       98 2024-03-22 19:57:57.298496 puppetparser-0.2.5/puppetparser/__main__.py
+-rw-r--r--   0        0        0    11508 2024-03-23 12:11:46.688998 puppetparser-0.2.5/puppetparser/model.py
+-rw-r--r--   0        0        0    64997 2024-05-07 14:12:37.072439 puppetparser-0.2.5/puppetparser/parser.py
+-rw-r--r--   0        0        0     1001 2024-05-07 14:13:39.647548 puppetparser-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 puppetparser-0.2.5/PKG-INFO
```

### Comparing `puppetparser-0.2.4/LICENSE` & `puppetparser-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `puppetparser-0.2.4/README.md` & `puppetparser-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `puppetparser-0.2.4/puppetparser/model.py` & `puppetparser-0.2.5/puppetparser/model.py`

 * *Files identical despite different names*

### Comparing `puppetparser-0.2.4/puppetparser/parser.py` & `puppetparser-0.2.5/puppetparser/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class InvalidPuppetScript(Exception):
     pass
 
 
 def find_column(input: str, pos: int) -> int:
     rfind = input.rfind("\n", 0, pos)
     if rfind == -1:
-        return pos
+        return pos + 1
     line_start = rfind + 1
     return (pos - line_start) + 1
 
 
 def parse(script: str) -> Tuple[List[CodeElement], List[Comment]]:
     comments: List[Comment] = []
```

### Comparing `puppetparser-0.2.4/pyproject.toml` & `puppetparser-0.2.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "puppetparser"
-version = "0.2.4"
+version = "0.2.5"
 description = "A parser from Puppet to an object model"
 authors = ["Nuno Saavedra <nuno.saavedra@tecnico.ulisboa.pt>"]
 license = "GPL-3.0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

### Comparing `puppetparser-0.2.4/PKG-INFO` & `puppetparser-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puppetparser
-Version: 0.2.4
+Version: 0.2.5
 Summary: A parser from Puppet to an object model
 License: GPL-3.0
 Keywords: puppet,parser,object model
 Author: Nuno Saavedra
 Author-email: nuno.saavedra@tecnico.ulisboa.pt
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

