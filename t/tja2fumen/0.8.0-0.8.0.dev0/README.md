# Comparing `tmp/tja2fumen-0.8.0.tar.gz` & `tmp/tja2fumen-0.8.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tja2fumen-0.8.0.tar", last modified: Tue Apr 30 02:12:50 2024, max compression
+gzip compressed data, was "tja2fumen-0.8.0.dev0.tar", last modified: Mon May  6 23:40:00 2024, max compression
```

## Comparing `tja2fumen-0.8.0.tar` & `tja2fumen-0.8.0.dev0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 02:12:50.233527 tja2fumen-0.8.0/
--rw-rw-rw-   0        0        0     1085 2024-04-30 02:11:55.000000 tja2fumen-0.8.0/LICENSE.txt
--rw-rw-rw-   0        0        0       37 2024-04-30 02:11:55.000000 tja2fumen-0.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0    15196 2024-04-30 02:12:50.233527 tja2fumen-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0    13103 2024-04-30 02:11:55.000000 tja2fumen-0.8.0/README.md
--rw-rw-rw-   0        0        0     1382 2024-04-30 02:12:46.000000 tja2fumen-0.8.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-30 02:12:50.233527 tja2fumen-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0       98 2024-04-30 02:11:55.000000 tja2fumen-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:12:50.217889 tja2fumen-0.8.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-30 02:12:50.217889 tja2fumen-0.8.0/src/tja2fumen/
--rw-rw-rw-   0        0        0     5856 2024-04-30 02:11:55.000000 tja2fumen-0.8.0/src/tja2fumen/__init__.py
--rw-rw-rw-   0        0        0    16022 2024-04-30 02:11:55.000000 tja2fumen-0.8.0/src/tja2fumen/classes.py
--rw-rw-rw-   0        0        0     3263 2024-04-30 02:11:55.000000 tja2fumen-0.8.0/src/tja2fumen/constants.py
--rw-rw-rw-   0        0        0    27352 2024-04-30 02:11:55.000000 tja2fumen-0.8.0/src/tja2fumen/converters.py
--rw-rw-rw-   0        0        0   307495 2024-04-30 02:11:55.000000 tja2fumen-0.8.0/src/tja2fumen/hp_values.csv
--rw-rw-rw-   0        0        0    27085 2024-04-30 02:11:55.000000 tja2fumen-0.8.0/src/tja2fumen/parsers.py
--rw-rw-rw-   0        0        0     2806 2024-04-30 02:11:55.000000 tja2fumen-0.8.0/src/tja2fumen/writers.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:12:50.217889 tja2fumen-0.8.0/src/tja2fumen.egg-info/
--rw-rw-rw-   0        0        0    15196 2024-04-30 02:12:50.000000 tja2fumen-0.8.0/src/tja2fumen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2024-04-30 02:12:50.000000 tja2fumen-0.8.0/src/tja2fumen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 02:12:50.000000 tja2fumen-0.8.0/src/tja2fumen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-30 02:12:50.000000 tja2fumen-0.8.0/src/tja2fumen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       83 2024-04-30 02:12:50.000000 tja2fumen-0.8.0/src/tja2fumen.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-30 02:12:50.000000 tja2fumen-0.8.0/src/tja2fumen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 23:40:00.547821 tja2fumen-0.8.0.dev0/
+-rw-rw-rw-   0        0        0     1085 2024-05-06 23:39:09.000000 tja2fumen-0.8.0.dev0/LICENSE.txt
+-rw-rw-rw-   0        0        0       37 2024-05-06 23:39:09.000000 tja2fumen-0.8.0.dev0/MANIFEST.in
+-rw-rw-rw-   0        0        0    15201 2024-05-06 23:40:00.547821 tja2fumen-0.8.0.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0    13103 2024-05-06 23:39:09.000000 tja2fumen-0.8.0.dev0/README.md
+-rw-rw-rw-   0        0        0     1387 2024-05-06 23:39:56.000000 tja2fumen-0.8.0.dev0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 23:40:00.547821 tja2fumen-0.8.0.dev0/setup.cfg
+-rw-rw-rw-   0        0        0       98 2024-05-06 23:39:09.000000 tja2fumen-0.8.0.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 23:40:00.532194 tja2fumen-0.8.0.dev0/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 23:40:00.532194 tja2fumen-0.8.0.dev0/src/tja2fumen/
+-rw-rw-rw-   0        0        0     5702 2024-05-06 23:39:09.000000 tja2fumen-0.8.0.dev0/src/tja2fumen/__init__.py
+-rw-rw-rw-   0        0        0    16022 2024-05-06 23:39:09.000000 tja2fumen-0.8.0.dev0/src/tja2fumen/classes.py
+-rw-rw-rw-   0        0        0     3263 2024-05-06 23:39:09.000000 tja2fumen-0.8.0.dev0/src/tja2fumen/constants.py
+-rw-rw-rw-   0        0        0    27352 2024-05-06 23:39:09.000000 tja2fumen-0.8.0.dev0/src/tja2fumen/converters.py
+-rw-rw-rw-   0        0        0   307495 2024-05-06 23:39:09.000000 tja2fumen-0.8.0.dev0/src/tja2fumen/hp_values.csv
+-rw-rw-rw-   0        0        0    27085 2024-05-06 23:39:09.000000 tja2fumen-0.8.0.dev0/src/tja2fumen/parsers.py
+-rw-rw-rw-   0        0        0     2806 2024-05-06 23:39:09.000000 tja2fumen-0.8.0.dev0/src/tja2fumen/writers.py
+drwxrwxrwx   0        0        0        0 2024-05-06 23:40:00.547821 tja2fumen-0.8.0.dev0/src/tja2fumen.egg-info/
+-rw-rw-rw-   0        0        0    15201 2024-05-06 23:40:00.000000 tja2fumen-0.8.0.dev0/src/tja2fumen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2024-05-06 23:40:00.000000 tja2fumen-0.8.0.dev0/src/tja2fumen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 23:40:00.000000 tja2fumen-0.8.0.dev0/src/tja2fumen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-06 23:40:00.000000 tja2fumen-0.8.0.dev0/src/tja2fumen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       83 2024-05-06 23:40:00.000000 tja2fumen-0.8.0.dev0/src/tja2fumen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-06 23:40:00.000000 tja2fumen-0.8.0.dev0/src/tja2fumen.egg-info/top_level.txt
```

### Comparing `tja2fumen-0.8.0/LICENSE.txt` & `tja2fumen-0.8.0.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.8.0/PKG-INFO` & `tja2fumen-0.8.0.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tja2fumen
-Version: 0.8.0
+Version: 0.8.0.dev0
 Summary: Convert TJA chart files into fumen (.bin) chart files
 License: MIT License
         
         Copyright (c) 2023 Vivaria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: tja2fumen Version: 0.8.0 Summary: Convert TJA chart
-files into fumen (.bin) chart files License: MIT License Copyright (c) 2023
-Vivaria Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"), to
-deal in the Software without restriction, including without limitation the
-rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
-sell copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions: The above copyright
-notice and this permission notice shall be included in all copies or
-substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT
-WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
-WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE
-FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
-TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR
-THE USE OR OTHER DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://
-github.com/vivaria/tja2fumen/ Project-URL: Bug Reports, https://github.com/
-vivaria/tja2fumen/issues/ Project-URL: Source, https://github.com/vivaria/
-tja2fumen/ Keywords: taiko,tatsujin,fumen,TJA Requires-Python: >=3.8
+Metadata-Version: 2.1 Name: tja2fumen Version: 0.8.0.dev0 Summary: Convert TJA
+chart files into fumen (.bin) chart files License: MIT License Copyright (c)
+2023 Vivaria Permission is hereby granted, free of charge, to any person
+obtaining a copy of this software and associated documentation files (the
+"Software"), to deal in the Software without restriction, including without
+limitation the rights to use, copy, modify, merge, publish, distribute,
+sublicense, and/or sell copies of the Software, and to permit persons to whom
+the Software is furnished to do so, subject to the following conditions: The
+above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS
+IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
+LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
+AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
+CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
+SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. Project-URL: Homepage,
+https://github.com/vivaria/tja2fumen/ Project-URL: Bug Reports, https://
+github.com/vivaria/tja2fumen/issues/ Project-URL: Source, https://github.com/
+vivaria/tja2fumen/ Keywords: taiko,tatsujin,fumen,TJA Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE.txt Provides-
 Extra: dev Requires-Dist: pytest; extra == "dev" Requires-Dist: build; extra ==
 "dev" Requires-Dist: pyinstaller; extra == "dev" Requires-Dist: twine; extra ==
 "dev" Requires-Dist: toml-cli; extra == "dev" Requires-Dist: flake8; extra ==
 "dev" Requires-Dist: pyproject-flake8; extra == "dev" Requires-Dist: mypy;
 extra == "dev" Requires-Dist: pylint; extra == "dev"  
                       [tja2fumen â TJA chart converter]
```

### Comparing `tja2fumen-0.8.0/README.md` & `tja2fumen-0.8.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.8.0/pyproject.toml` & `tja2fumen-0.8.0.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tja2fumen"
-version = "0.8.0"
+version = "0.8.0.dev0"
 description = "Convert TJA chart files into fumen (.bin) chart files"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["taiko", "tatsujin", "fumen", "TJA"]
 
 [project.urls]  # Optional
```

### Comparing `tja2fumen-0.8.0/src/tja2fumen/__init__.py` & `tja2fumen-0.8.0.dev0/src/tja2fumen/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         raise FileNotFoundError("No such file or directory: " + path_input)
 
     for file in files:
         process_file(file)
 
 
 def parse_files(directory: str) -> Tuple[List[str], List[str]]:
-    """Find all .tja or .bin files within a directory."""
+    """Find all  or .bin files within a directory."""
     tja_files, bin_files = [], []
     for root, _, files in os.walk(directory):
         for file in files:
             if file.endswith(".tja"):
                 tja_files.append(os.path.join(root, file))
             elif file.endswith(".bin"):
                 if file.startswith("song_"):
@@ -89,27 +89,24 @@
 
 
 def process_file(fname: str) -> None:
     """Process a single file path (TJA or BIN)."""
     if fname.endswith(".bin"):
         print(f"Repairing {fname}")
         repair_bin(fname)
-    elif fname.endswith(".tja"):
+    else:
         print(f"Converting {fname}")
         # Parse lines in TJA file
         parsed_tja = parse_tja(fname)
 
         # Convert parsed TJA courses and write each course to `.bin` files
         base_name = os.path.splitext(fname)[0]
         for course_name, course in parsed_tja.courses.items():
             convert_and_write(course, course_name, base_name,
                               single_course=len(parsed_tja.courses) == 1)
-    else:
-        raise ValueError(f"Unrecognized file type: {fname} "
-                         f"(expected .tja or .bin)")
 
 
 def convert_and_write(tja_data: TJACourse,
                       course_name: str,
                       base_name: str,
                       single_course: bool = False) -> None:
     """Process the parsed data for a single TJA course."""
```

### Comparing `tja2fumen-0.8.0/src/tja2fumen/classes.py` & `tja2fumen-0.8.0.dev0/src/tja2fumen/classes.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.8.0/src/tja2fumen/constants.py` & `tja2fumen-0.8.0.dev0/src/tja2fumen/constants.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.8.0/src/tja2fumen/converters.py` & `tja2fumen-0.8.0.dev0/src/tja2fumen/converters.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.8.0/src/tja2fumen/hp_values.csv` & `tja2fumen-0.8.0.dev0/src/tja2fumen/hp_values.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.8.0/src/tja2fumen/parsers.py` & `tja2fumen-0.8.0.dev0/src/tja2fumen/parsers.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.8.0/src/tja2fumen/writers.py` & `tja2fumen-0.8.0.dev0/src/tja2fumen/writers.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.8.0/src/tja2fumen.egg-info/PKG-INFO` & `tja2fumen-0.8.0.dev0/src/tja2fumen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tja2fumen
-Version: 0.8.0
+Version: 0.8.0.dev0
 Summary: Convert TJA chart files into fumen (.bin) chart files
 License: MIT License
         
         Copyright (c) 2023 Vivaria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: tja2fumen Version: 0.8.0 Summary: Convert TJA chart
-files into fumen (.bin) chart files License: MIT License Copyright (c) 2023
-Vivaria Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"), to
-deal in the Software without restriction, including without limitation the
-rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
-sell copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions: The above copyright
-notice and this permission notice shall be included in all copies or
-substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT
-WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
-WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE
-FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
-TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR
-THE USE OR OTHER DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://
-github.com/vivaria/tja2fumen/ Project-URL: Bug Reports, https://github.com/
-vivaria/tja2fumen/issues/ Project-URL: Source, https://github.com/vivaria/
-tja2fumen/ Keywords: taiko,tatsujin,fumen,TJA Requires-Python: >=3.8
+Metadata-Version: 2.1 Name: tja2fumen Version: 0.8.0.dev0 Summary: Convert TJA
+chart files into fumen (.bin) chart files License: MIT License Copyright (c)
+2023 Vivaria Permission is hereby granted, free of charge, to any person
+obtaining a copy of this software and associated documentation files (the
+"Software"), to deal in the Software without restriction, including without
+limitation the rights to use, copy, modify, merge, publish, distribute,
+sublicense, and/or sell copies of the Software, and to permit persons to whom
+the Software is furnished to do so, subject to the following conditions: The
+above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS
+IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
+LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
+AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
+CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
+SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. Project-URL: Homepage,
+https://github.com/vivaria/tja2fumen/ Project-URL: Bug Reports, https://
+github.com/vivaria/tja2fumen/issues/ Project-URL: Source, https://github.com/
+vivaria/tja2fumen/ Keywords: taiko,tatsujin,fumen,TJA Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE.txt Provides-
 Extra: dev Requires-Dist: pytest; extra == "dev" Requires-Dist: build; extra ==
 "dev" Requires-Dist: pyinstaller; extra == "dev" Requires-Dist: twine; extra ==
 "dev" Requires-Dist: toml-cli; extra == "dev" Requires-Dist: flake8; extra ==
 "dev" Requires-Dist: pyproject-flake8; extra == "dev" Requires-Dist: mypy;
 extra == "dev" Requires-Dist: pylint; extra == "dev"  
                       [tja2fumen â TJA chart converter]
```

