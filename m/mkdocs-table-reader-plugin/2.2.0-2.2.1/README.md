# Comparing `tmp/mkdocs_table_reader_plugin-2.2.0.tar.gz` & `tmp/mkdocs_table_reader_plugin-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_table_reader_plugin-2.2.0.tar", last modified: Sat May  4 08:11:31 2024, max compression
+gzip compressed data, was "mkdocs_table_reader_plugin-2.2.1.tar", last modified: Tue May  7 09:20:57 2024, max compression
```

## Comparing `mkdocs_table_reader_plugin-2.2.0.tar` & `mkdocs_table_reader_plugin-2.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:11:31.830786 mkdocs_table_reader_plugin-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-04 08:11:31.830786 mkdocs_table_reader_plugin-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:11:31.830786 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin/safe_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:11:31.830786 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-04 08:11:31.000000 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-04 08:11:31.000000 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 08:11:31.000000 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-04 08:11:31.000000 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-04 08:11:31.000000 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-04 08:11:31.000000 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 08:11:31.830786 mkdocs_table_reader_plugin-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:11:31.830786 mkdocs_table_reader_plugin-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10979 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/tests/test_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/tests/test_markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/tests/test_safe_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:57.381267 mkdocs_table_reader_plugin-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-07 09:20:57.381267 mkdocs_table_reader_plugin-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:57.381267 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin/safe_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:57.381267 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-07 09:20:57.000000 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-07 09:20:57.000000 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:20:57.000000 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-07 09:20:57.000000 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-07 09:20:57.000000 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 09:20:57.000000 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 09:20:57.381267 mkdocs_table_reader_plugin-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:57.381267 mkdocs_table_reader_plugin-2.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10979 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/tests/test_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/tests/test_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/tests/test_safe_eval.py
```

### Comparing `mkdocs_table_reader_plugin-2.2.0/LICENSE` & `mkdocs_table_reader_plugin-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_table_reader_plugin-2.2.0/PKG-INFO` & `mkdocs_table_reader_plugin-2.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-reader-plugin
-Version: 2.2.0
+Version: 2.2.1
 Summary: MkDocs plugin to directly insert tables from files into markdown.
 Home-page: https://github.com/timvink/mkdocs-table-reader-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs plugin
 Classifier: Operating System :: OS Independent
@@ -53,20 +53,20 @@
   - table-reader
 ```
 
 > If you have no `plugins` entry in your config file yet, you'll likely also want to add the `search` plugin. MkDocs enables it by default if there is no `plugins` entry set.
 
 ## Usage
 
-In your markdown documents you can now use:
+In your markdown files you can now use:
 
 ```html
 {{ read_csv('path_to_table.csv') }}
 ```
 
 Where the path is relative to the location of your project's `mkdocs.yml` file (although you can [change that](https://timvink.github.io/mkdocs-table-reader-plugin/options) to be relative to your `docs/` directory).
 
-- There are [readers](https://timvink.github.io/mkdocs-table-reader-plugin/readers/) for `.csv`, `.fwf`, `.json`, `.xlsx`, `.yaml` and `.tsv`. There is also the `read_raw()` reader that will allow you to insert tables (or other content) already in markdown format.
+- There are [readers](https://timvink.github.io/mkdocs-table-reader-plugin/readers/) for `.csv`, `.fwf`, `.json`, `.xlsx`, `.yaml` and `.tsv` files. There is also the `read_raw()` reader that will allow you to insert tables (or other content) already in markdown format.
 
 ## Documentation and how-to guides
 
 See [timvink.github.io/mkdocs-table-reader-plugin/](https://timvink.github.io/mkdocs-table-reader-plugin/)
```

### Comparing `mkdocs_table_reader_plugin-2.2.0/README.md` & `mkdocs_table_reader_plugin-2.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -28,20 +28,20 @@
   - table-reader
 ```
 
 > If you have no `plugins` entry in your config file yet, you'll likely also want to add the `search` plugin. MkDocs enables it by default if there is no `plugins` entry set.
 
 ## Usage
 
-In your markdown documents you can now use:
+In your markdown files you can now use:
 
 ```html
 {{ read_csv('path_to_table.csv') }}
 ```
 
 Where the path is relative to the location of your project's `mkdocs.yml` file (although you can [change that](https://timvink.github.io/mkdocs-table-reader-plugin/options) to be relative to your `docs/` directory).
 
-- There are [readers](https://timvink.github.io/mkdocs-table-reader-plugin/readers/) for `.csv`, `.fwf`, `.json`, `.xlsx`, `.yaml` and `.tsv`. There is also the `read_raw()` reader that will allow you to insert tables (or other content) already in markdown format.
+- There are [readers](https://timvink.github.io/mkdocs-table-reader-plugin/readers/) for `.csv`, `.fwf`, `.json`, `.xlsx`, `.yaml` and `.tsv` files. There is also the `read_raw()` reader that will allow you to insert tables (or other content) already in markdown format.
 
 ## Documentation and how-to guides
 
 See [timvink.github.io/mkdocs-table-reader-plugin/](https://timvink.github.io/mkdocs-table-reader-plugin/)
```

### Comparing `mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin/markdown.py` & `mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin/markdown.py`

 * *Files identical despite different names*

### Comparing `mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin/plugin.py` & `mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin/readers.py` & `mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin/readers.py`

 * *Files identical despite different names*

### Comparing `mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin/safe_eval.py` & `mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin/safe_eval.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,27 +70,32 @@
     """
     # below generated by copilot, validated by unit tests
     segments = []
     current_segment = ''
     in_quotes = False
     quote_char = ''
     bracket_count = 0
+    tuple_count = 0
     
     for char in input_str:
         if char in "\"'" and not in_quotes:
             in_quotes = True
             quote_char = char
         elif char == quote_char and in_quotes:
             in_quotes = False
             quote_char = ''
         elif char == '[':
             bracket_count += 1
         elif char == ']':
             bracket_count -= 1
-        elif char == ',' and not in_quotes and bracket_count == 0:
+        elif char == '(':
+            tuple_count += 1
+        elif char == ')':
+            tuple_count -= 1
+        elif char == ',' and not in_quotes and bracket_count == 0 and tuple_count == 0:
             segments.append(current_segment.strip())
             current_segment = ''
             continue
         
         current_segment += char
     
     segments.append(current_segment.strip())  # Add the last segment
```

### Comparing `mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin/utils.py` & `mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin/utils.py`

 * *Files identical despite different names*

### Comparing `mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin.egg-info/PKG-INFO` & `mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-reader-plugin
-Version: 2.2.0
+Version: 2.2.1
 Summary: MkDocs plugin to directly insert tables from files into markdown.
 Home-page: https://github.com/timvink/mkdocs-table-reader-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs plugin
 Classifier: Operating System :: OS Independent
@@ -53,20 +53,20 @@
   - table-reader
 ```
 
 > If you have no `plugins` entry in your config file yet, you'll likely also want to add the `search` plugin. MkDocs enables it by default if there is no `plugins` entry set.
 
 ## Usage
 
-In your markdown documents you can now use:
+In your markdown files you can now use:
 
 ```html
 {{ read_csv('path_to_table.csv') }}
 ```
 
 Where the path is relative to the location of your project's `mkdocs.yml` file (although you can [change that](https://timvink.github.io/mkdocs-table-reader-plugin/options) to be relative to your `docs/` directory).
 
-- There are [readers](https://timvink.github.io/mkdocs-table-reader-plugin/readers/) for `.csv`, `.fwf`, `.json`, `.xlsx`, `.yaml` and `.tsv`. There is also the `read_raw()` reader that will allow you to insert tables (or other content) already in markdown format.
+- There are [readers](https://timvink.github.io/mkdocs-table-reader-plugin/readers/) for `.csv`, `.fwf`, `.json`, `.xlsx`, `.yaml` and `.tsv` files. There is also the `read_raw()` reader that will allow you to insert tables (or other content) already in markdown format.
 
 ## Documentation and how-to guides
 
 See [timvink.github.io/mkdocs-table-reader-plugin/](https://timvink.github.io/mkdocs-table-reader-plugin/)
```

### Comparing `mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin.egg-info/SOURCES.txt` & `mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs_table_reader_plugin-2.2.0/setup.py` & `mkdocs_table_reader_plugin-2.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mkdocs-table-reader-plugin",
-    version="2.2.0",
+    version="2.2.1",
     description="MkDocs plugin to directly insert tables from files into markdown.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="mkdocs plugin",
     url="https://github.com/timvink/mkdocs-table-reader-plugin",
     author="Tim Vink",
     author_email="vinktim@gmail.com",
```

### Comparing `mkdocs_table_reader_plugin-2.2.0/tests/test_build.py` & `mkdocs_table_reader_plugin-2.2.1/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `mkdocs_table_reader_plugin-2.2.0/tests/test_kwargs.py` & `mkdocs_table_reader_plugin-2.2.1/tests/test_kwargs.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 
 
 def test_parse_argkwarg():
 
     assert parse_argkwarg("sep=';'") == ([], {'sep': ';'})
     assert parse_argkwarg('"file.csv", usecols=["A", "B"]') == (['file.csv'], {'usecols': ['A', 'B']})
     assert parse_argkwarg('"file.csv", usecols=[\'A\',\'B\']') == (['file.csv'], {'usecols': ['A', 'B']})
-    assert parse_argkwarg("'assets/tables/table_with_carriage_return.csv', sep = ','") == (['assets/tables/table_with_carriage_return.csv'], {'sep': ','})
+    assert parse_argkwarg("'assets/tables/table_with_carriage_return.csv', sep = ','") == (['assets/tables/table_with_carriage_return.csv'], {'sep': ','})
+    assert parse_argkwarg("'includes/statistics.csv', keep_default_na=False, colalign=('center','center','center','center','center','center','center')") == (['includes/statistics.csv'], {'keep_default_na': False, 'colalign': ('center','center','center','center','center','center','center')})
```

### Comparing `mkdocs_table_reader_plugin-2.2.0/tests/test_markdown.py` & `mkdocs_table_reader_plugin-2.2.1/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `mkdocs_table_reader_plugin-2.2.0/tests/test_safe_eval.py` & `mkdocs_table_reader_plugin-2.2.1/tests/test_safe_eval.py`

 * *Files identical despite different names*

