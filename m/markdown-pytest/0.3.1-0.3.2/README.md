# Comparing `tmp/markdown_pytest-0.3.1.tar.gz` & `tmp/markdown_pytest-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_pytest-0.3.1.tar", max compression
+gzip compressed data, was "markdown_pytest-0.3.2.tar", max compression
```

## Comparing `markdown_pytest-0.3.1.tar` & `markdown_pytest-0.3.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2024-04-09 22:23:16.117985 markdown_pytest-0.3.1/LICENSE
--rw-r--r--   0        0        0     5019 2024-04-09 22:23:16.118066 markdown_pytest-0.3.1/README.md
--rw-r--r--   0        0        0     5967 2024-04-09 22:23:16.118140 markdown_pytest-0.3.1/markdown_pytest.py
--rw-r--r--   0        0        0     1761 2024-04-09 22:27:16.514970 markdown_pytest-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6668 1970-01-01 00:00:00.000000 markdown_pytest-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-09 22:23:16.117985 markdown_pytest-0.3.2/LICENSE
+-rw-r--r--   0        0        0     5260 2024-05-07 14:04:24.499985 markdown_pytest-0.3.2/README.md
+-rw-r--r--   0        0        0     6965 2024-05-07 14:04:24.500659 markdown_pytest-0.3.2/markdown_pytest.py
+-rw-r--r--   0        0        0     1761 2024-05-07 14:06:53.007531 markdown_pytest-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6909 1970-01-01 00:00:00.000000 markdown_pytest-0.3.2/PKG-INFO
```

### Comparing `markdown_pytest-0.3.1/LICENSE` & `markdown_pytest-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_pytest-0.3.1/README.md` & `markdown_pytest-0.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,28 @@
 
 The `name` key is required, and blocks that do not contain it will be ignored.
 
 Some Markdown parsers support two or three dashes around comments, this module 
 supports both variants. The `case` parameter is optional and might be used for
 subtests, see "Code split" section.
 
+Additionally, a code block can be put inside the comment block to hide some 
+initialization from the readers.
+
+````markdown
+<!-- name: test_name
+```python
+init_some_variable = 123
+```
+-->
+```python
+assert init_some_variable == 123
+```
+````
+
 Common parsing rules
 --------------------
 
 This module uses its own, very simple Markdown parser, which only supports code 
 block parsing. In general, the parsing behavior of a file follows the following 
 rules:
```

### Comparing `markdown_pytest-0.3.1/markdown_pytest.py` & `markdown_pytest-0.3.2/markdown_pytest.py`

 * *Files 15% similar despite different names*

```diff
@@ -68,27 +68,55 @@
         try:
             return self.next()
         except IndexError:
             raise StopIteration
 
 
 def parse_arguments(line_iterator: LinesIterator) -> Dict[str, str]:
+
+    outside_comment = inside_comment = False
+    index = line_iterator.index
+    # Checking if the code block is outside of the comment block
     for lineno, line in line_iterator.reverse_iterator(1):
         if not line.strip():
             continue
-        if not line.strip().endswith(COMMENT_BRACKETS[1]):
-            return {}
+        if line.strip().endswith(COMMENT_BRACKETS[1]):
+            outside_comment = True
         break
 
+    # Checking if the code block is inside of the comment block
+    if not outside_comment:
+        for lineno, line in line_iterator:
+            if not line.strip():
+                continue
+            if line.strip().endswith(COMMENT_BRACKETS[0]):
+                return {}
+            elif line.strip().endswith(COMMENT_BRACKETS[1]):
+                inside_comment = True
+                line_iterator.seek_relative(1)
+                break
+
+    if not outside_comment and not inside_comment:
+        return {}
+
     lines = []
-    for lineno, line in line_iterator.reverse_iterator(1):
+    reverse_iterator = line_iterator.reverse_iterator(1)
+    for lineno, line in reverse_iterator:
+        if line.strip().startswith("```"):
+            for _, line in reverse_iterator:
+                if line.strip().startswith("```"):
+                    break
+            continue
         lines.append(line)
         if line.strip().startswith(COMMENT_BRACKETS[0]):
             break
 
+    # Restore the iterator (due to inside comment forward iterations)
+    line_iterator.index = index
+
     if not lines:
         return {}
 
     lines = lines[::-1]
     result = {}
     args = "".join(
         "".join(lines).strip()[
```

### Comparing `markdown_pytest-0.3.1/pyproject.toml` & `markdown_pytest-0.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "markdown-pytest"
-version = "0.3.1"
+version = "0.3.2"
 license = "Apache-2.0"
 description = "Pytest plugin for runs tests directly from Markdown files"
 authors = ["Dmitry Orlov <me@mosquito.su>"]
 readme = "README.md"
 keywords=["pytest", "markdown", "documentation"]
 homepage = "https://github.com/mosquito/markdown-pytest"
 classifiers = [
```

### Comparing `markdown_pytest-0.3.1/PKG-INFO` & `markdown_pytest-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown-pytest
-Version: 0.3.1
+Version: 0.3.2
 Summary: Pytest plugin for runs tests directly from Markdown files
 Home-page: https://github.com/mosquito/markdown-pytest
 License: Apache-2.0
 Keywords: pytest,markdown,documentation
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
 Requires-Python: >=3.8,<4.0
@@ -100,14 +100,28 @@
 
 The `name` key is required, and blocks that do not contain it will be ignored.
 
 Some Markdown parsers support two or three dashes around comments, this module 
 supports both variants. The `case` parameter is optional and might be used for
 subtests, see "Code split" section.
 
+Additionally, a code block can be put inside the comment block to hide some 
+initialization from the readers.
+
+````markdown
+<!-- name: test_name
+```python
+init_some_variable = 123
+```
+-->
+```python
+assert init_some_variable == 123
+```
+````
+
 Common parsing rules
 --------------------
 
 This module uses its own, very simple Markdown parser, which only supports code 
 block parsing. In general, the parsing behavior of a file follows the following 
 rules:
```

