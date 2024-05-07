# Comparing `tmp/starlette_compress-0.1.4.tar.gz` & `tmp/starlette_compress-0.1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette_compress-0.1.4.tar", max compression
+gzip compressed data, was "starlette_compress-0.1.5.4.tar", max compression
```

## Comparing `starlette_compress-0.1.4.tar` & `starlette_compress-0.1.5.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1211 2024-05-07 02:03:17.682917 starlette_compress-0.1.4/LICENSE
--rw-r--r--   0        0        0     2619 2024-05-07 02:03:17.682917 starlette_compress-0.1.4/README.md
--rw-r--r--   0        0        0     4691 2024-05-07 02:03:17.682917 starlette_compress-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    14104 2024-05-07 02:03:17.682917 starlette_compress-0.1.4/starlette_compress/__init__.py
--rw-r--r--   0        0        0     4030 1970-01-01 00:00:00.000000 starlette_compress-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-05-07 02:46:52.653614 starlette_compress-0.1.5.4/LICENSE
+-rw-r--r--   0        0        0     2619 2024-05-07 02:46:52.653614 starlette_compress-0.1.5.4/README.md
+-rw-r--r--   0        0        0     4693 2024-05-07 02:46:52.653614 starlette_compress-0.1.5.4/pyproject.toml
+-rw-r--r--   0        0        0    14104 2024-05-07 02:46:52.653614 starlette_compress-0.1.5.4/starlette_compress/__init__.py
+-rw-r--r--   0        0        0     4032 1970-01-01 00:00:00.000000 starlette_compress-0.1.5.4/PKG-INFO
```

### Comparing `starlette_compress-0.1.4/LICENSE` & `starlette_compress-0.1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `starlette_compress-0.1.4/README.md` & `starlette_compress-0.1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `starlette_compress-0.1.4/pyproject.toml` & `starlette_compress-0.1.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ]
 description = "Compression middleware for Starlette - supporting ZStd, Brotli, and GZip"
 keywords = ["starlette", "middleware", "compression", "zstd", "brotli", "gzip", "http"]
 license = "Unlicense"
 name = "starlette-compress"
 readme = "README.md"
 repository = "https://github.com/Zaczero/starlette-compress"
-version = "0.1.4"
+version = "0.1.5.4"
 
 [tool.poetry.dependencies]
 brotli = {version = ">=1", markers = "platform_python_implementation == 'CPython'"}
 brotlicffi = {version = ">=1", markers = "platform_python_implementation != 'CPython'"}
 python = "^3.8"
 starlette = "*"
 zstandard = ">=0.15"
```

### Comparing `starlette_compress-0.1.4/starlette_compress/__init__.py` & `starlette_compress-0.1.5.4/starlette_compress/__init__.py`

 * *Files identical despite different names*

### Comparing `starlette_compress-0.1.4/PKG-INFO` & `starlette_compress-0.1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starlette-compress
-Version: 0.1.4
+Version: 0.1.5.4
 Summary: Compression middleware for Starlette - supporting ZStd, Brotli, and GZip
 Home-page: https://github.com/Zaczero/starlette-compress
 License: Unlicense
 Keywords: starlette,middleware,compression,zstd,brotli,gzip,http
 Author: Kamil Monicz
 Author-email: kamil@monicz.dev
 Requires-Python: >=3.8,<4.0
```

