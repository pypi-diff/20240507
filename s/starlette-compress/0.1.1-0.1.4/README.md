# Comparing `tmp/starlette_compress-0.1.1.tar.gz` & `tmp/starlette_compress-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette_compress-0.1.1.tar", max compression
+gzip compressed data, was "starlette_compress-0.1.4.tar", max compression
```

## Comparing `starlette_compress-0.1.1.tar` & `starlette_compress-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1211 2024-05-06 22:59:25.637314 starlette_compress-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2024-05-06 22:45:06.504407 starlette_compress-0.1.1/README.md
--rw-r--r--   0        0        0     4713 2024-05-07 00:08:30.835914 starlette_compress-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    14138 2024-05-07 00:07:33.799530 starlette_compress-0.1.1/starlette_compress/__init__.py
--rw-r--r--   0        0        0     1411 1970-01-01 00:00:00.000000 starlette_compress-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-05-07 02:03:17.682917 starlette_compress-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2619 2024-05-07 02:03:17.682917 starlette_compress-0.1.4/README.md
+-rw-r--r--   0        0        0     4691 2024-05-07 02:03:17.682917 starlette_compress-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    14104 2024-05-07 02:03:17.682917 starlette_compress-0.1.4/starlette_compress/__init__.py
+-rw-r--r--   0        0        0     4030 1970-01-01 00:00:00.000000 starlette_compress-0.1.4/PKG-INFO
```

### Comparing `starlette_compress-0.1.1/LICENSE` & `starlette_compress-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `starlette_compress-0.1.1/pyproject.toml` & `starlette_compress-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,29 +18,28 @@
 ]
 description = "Compression middleware for Starlette - supporting ZStd, Brotli, and GZip"
 keywords = ["starlette", "middleware", "compression", "zstd", "brotli", "gzip", "http"]
 license = "Unlicense"
 name = "starlette-compress"
 readme = "README.md"
 repository = "https://github.com/Zaczero/starlette-compress"
-version = "0.1.1"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 brotli = {version = ">=1", markers = "platform_python_implementation == 'CPython'"}
 brotlicffi = {version = ">=1", markers = "platform_python_implementation != 'CPython'"}
 python = "^3.8"
 starlette = "*"
 zstandard = ">=0.15"
 
 [tool.poetry.group.test.dependencies]
 httpx = "<1"
 mypy = "^1.0.0"
 pytest = "^8.0.0"
 pytest-cov = "^5.0.0"
-pytest-watcher = "<1"
 trio = "<1"
 uvloop = "<1"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
```

### Comparing `starlette_compress-0.1.1/starlette_compress/__init__.py` & `starlette_compress-0.1.4/starlette_compress/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,39 +389,39 @@
     'text/vnd.rim.location.xloc',
     'text/vtt',
     'text/x-component',
     'text/x-cross-domain-policy',
 }
 
 
-def register_compress_content_type(content_type: str) -> None:
+def add_compress_type(content_type: str) -> None:
     """
-    Register a new content type to be compressed.
+    Add a new content-type to be compressed.
     """
     _compress_content_types.add(content_type)
 
 
-def deregister_compress_content_type(content_type: str) -> None:
+def remove_compress_type(content_type: str) -> None:
     """
-    Deregister a content type from being compressed.
+    Remove a content-type from being compressed.
     """
     _compress_content_types.discard(content_type)
 
 
 def _is_start_message_satisfied(message: Message) -> bool:
     """
     Check if response should be compressed based on the start message.
     """
     headers = Headers(raw=message['headers'])
 
     # must not already be compressed
     if 'Content-Encoding' in headers:
         return False
 
-    # content type header must be present
+    # content-type header must be present
     content_type = headers.get('Content-Type')
     if not content_type:
         return False
 
-    # must be a compressible content type
+    # must be a compressible content-type
     basic_content_type = content_type.partition(';')[0].strip()
     return basic_content_type in _compress_content_types
```

