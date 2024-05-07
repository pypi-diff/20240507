# Comparing `tmp/mcextract-1.1.0.tar.gz` & `tmp/mcextract-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcextract-1.1.0.tar", last modified: Fri Aug 18 22:10:41 2023, max compression
+gzip compressed data, was "mcextract-1.2.0.tar", last modified: Tue May  7 03:49:32 2024, max compression
```

## Comparing `mcextract-1.1.0.tar` & `mcextract-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-08-18 22:10:41.380380 mcextract-1.1.0/
--rw-rw-rw-   0        0        0     1088 2023-07-04 20:41:34.000000 mcextract-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     3846 2023-08-18 22:10:41.380380 mcextract-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3104 2023-08-18 22:09:42.000000 mcextract-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-18 22:10:41.374383 mcextract-1.1.0/mcextract/
--rw-rw-rw-   0        0        0      105 2023-08-18 20:42:38.000000 mcextract-1.1.0/mcextract/__init__.py
--rw-rw-rw-   0        0        0      123 2023-08-18 20:43:14.000000 mcextract-1.1.0/mcextract/__main__.py
-drwxrwxrwx   0        0        0        0 2023-08-18 22:10:41.379381 mcextract-1.1.0/mcextract/assets/
--rw-rw-rw-   0        0        0     2692 2022-01-31 00:25:37.000000 mcextract-1.1.0/mcextract/assets/icon.ico
--rw-rw-rw-   0        0        0    23792 2023-07-04 20:25:47.000000 mcextract-1.1.0/mcextract/client.py
--rw-rw-rw-   0        0        0    17069 2023-08-18 21:48:22.000000 mcextract-1.1.0/mcextract/server.py
-drwxrwxrwx   0        0        0        0 2023-08-18 22:10:41.379381 mcextract-1.1.0/mcextract.egg-info/
--rw-rw-rw-   0        0        0     3846 2023-08-18 22:10:41.000000 mcextract-1.1.0/mcextract.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-08-18 22:10:41.000000 mcextract-1.1.0/mcextract.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-18 22:10:41.000000 mcextract-1.1.0/mcextract.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-08-18 22:10:41.000000 mcextract-1.1.0/mcextract.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-18 22:10:41.000000 mcextract-1.1.0/mcextract.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-08-18 22:10:41.381380 mcextract-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1289 2023-08-18 20:45:15.000000 mcextract-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:49:32.639329 mcextract-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-07 03:49:24.000000 mcextract-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-07 03:49:32.639329 mcextract-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-07 03:49:24.000000 mcextract-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:49:32.635329 mcextract-1.2.0/mcextract/
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-07 03:49:30.000000 mcextract-1.2.0/mcextract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-07 03:49:24.000000 mcextract-1.2.0/mcextract/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-07 03:49:30.000000 mcextract-1.2.0/mcextract/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:49:32.635329 mcextract-1.2.0/mcextract.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-07 03:49:32.000000 mcextract-1.2.0/mcextract.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-07 03:49:32.000000 mcextract-1.2.0/mcextract.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 03:49:32.000000 mcextract-1.2.0/mcextract.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 03:49:32.000000 mcextract-1.2.0/mcextract.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 03:49:32.000000 mcextract-1.2.0/mcextract.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-07 03:49:32.000000 mcextract-1.2.0/mcextract.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 03:49:32.000000 mcextract-1.2.0/mcextract.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-07 03:49:32.639329 mcextract-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 03:49:24.000000 mcextract-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:49:32.639329 mcextract-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 03:49:24.000000 mcextract-1.2.0/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-07 03:49:30.000000 mcextract-1.2.0/tests/test_extract_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-07 03:49:30.000000 mcextract-1.2.0/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 03:49:30.000000 mcextract-1.2.0/tests/test_generate_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-07 03:49:24.000000 mcextract-1.2.0/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-07 03:49:30.000000 mcextract-1.2.0/tests/test_map_cli.py
```

### Comparing `mcextract-1.1.0/LICENSE` & `mcextract-1.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Legopitstop
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 Legopitstop
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

