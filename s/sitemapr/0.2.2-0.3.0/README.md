# Comparing `tmp/sitemapr-0.2.2.tar.gz` & `tmp/sitemapr-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitemapr-0.2.2.tar", max compression
+gzip compressed data, was "sitemapr-0.3.0.tar", max compression
```

## Comparing `sitemapr-0.2.2.tar` & `sitemapr-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2024-05-06 05:15:34.752604 sitemapr-0.2.2/LICENSE
--rw-r--r--   0        0        0     2060 2024-05-06 05:15:34.752604 sitemapr-0.2.2/README.md
--rw-r--r--   0        0        0     1065 2024-05-06 05:15:34.752604 sitemapr-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      126 2024-05-06 05:15:34.752604 sitemapr-0.2.2/sitemapr/__init__.py
--rw-r--r--   0        0        0     4610 2024-05-06 05:15:34.752604 sitemapr-0.2.2/sitemapr/core.py
--rw-r--r--   0        0        0      741 2024-05-06 05:15:34.752604 sitemapr-0.2.2/sitemapr/models.py
--rw-r--r--   0        0        0     2693 1970-01-01 00:00:00.000000 sitemapr-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-07 14:45:45.791539 sitemapr-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2274 2024-05-07 14:45:45.791539 sitemapr-0.3.0/README.md
+-rw-r--r--   0        0        0     1065 2024-05-07 14:45:45.791539 sitemapr-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      126 2024-05-07 14:45:45.791539 sitemapr-0.3.0/sitemapr/__init__.py
+-rw-r--r--   0        0        0     5140 2024-05-07 14:45:45.791539 sitemapr-0.3.0/sitemapr/core.py
+-rw-r--r--   0        0        0      934 2024-05-07 14:45:45.791539 sitemapr-0.3.0/sitemapr/models.py
+-rw-r--r--   0        0        0     2907 1970-01-01 00:00:00.000000 sitemapr-0.3.0/PKG-INFO
```

### Comparing `sitemapr-0.2.2/LICENSE` & `sitemapr-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sitemapr-0.2.2/README.md` & `sitemapr-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -37,21 +37,24 @@
 pages = [
     Page(
         path="",
         query_params=[
             Param(name="page", values=["home", "about", "contact"]),
             Param(name="sort", values=["asc", "desc"]),
         ],
+        priority="1.0",
     ),
     Page(
         path="/blog",
         query_params=[
             Param(name="page", values=["1", "2", "3"]),
             Param(name="sort", values=["asc", "desc"]),
         ],
+        # For lastmod, priority, and changefreq field, you can use callback function for more precise control
+        lastmod=lambda loc, path_params, query_params: "2024-05-07T00:00:00+00"
     ),
     Page(
         path="/blog/{id}",
         path_params=[Param(name="id", values=["1", "2", "3"])],
     ),
 ]
```

### Comparing `sitemapr-0.2.2/pyproject.toml` & `sitemapr-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sitemapr"
-version = "0.2.2"
+version = "0.3.0"
 description = "sitemapr is a library that generates sitemaps for SPA websites with declaritve configuration in Python."
 authors = ["sjquant <seonujang92@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `sitemapr-0.2.2/sitemapr/core.py` & `sitemapr-0.3.0/sitemapr/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -98,25 +98,44 @@
         path_param_combinations: list[dict[str, str]] = self._get_param_combinations(
             page.path_params
         )
         for query_params, path_params in product(
             query_param_combinations, path_param_combinations
         ):
             path = page.path.format(**path_params)
-            query_string = urlencode(query_params).replace('&', '&amp;')
+            query_string = urlencode(query_params).replace("&", "&amp;")
             loc = (
                 f"{self._base_url}{path}?{query_string}"
                 if query_string
                 else f"{self._base_url}{path}"
             )
+
+            lastmod = (
+                page.lastmod(loc, path_params, query_params)
+                if callable(page.lastmod)
+                else page.lastmod
+            )
+
+            changefreq = (
+                page.changefreq(loc, path_params, query_params)
+                if callable(page.changefreq)
+                else page.changefreq
+            )
+
+            priority = (
+                page.priority(loc, path_params, query_params)
+                if callable(page.priority)
+                else page.priority
+            )
+
             yield SiteMapUrl(
                 loc=loc,
-                lastmod=page.lastmod,
-                changefreq=page.changefreq,
-                priority=page.priority,
+                lastmod=lastmod,
+                changefreq=changefreq,
+                priority=priority,
             )
 
     def _get_param_combinations(
         self, params: list[Param] | None
     ) -> list[dict[str, str]]:
         if not params:
             return [{}]
```

### Comparing `sitemapr-0.2.2/PKG-INFO` & `sitemapr-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitemapr
-Version: 0.2.2
+Version: 0.3.0
 Summary: sitemapr is a library that generates sitemaps for SPA websites with declaritve configuration in Python.
 License: MIT
 Author: sjquant
 Author-email: seonujang92@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -54,21 +54,24 @@
 pages = [
     Page(
         path="",
         query_params=[
             Param(name="page", values=["home", "about", "contact"]),
             Param(name="sort", values=["asc", "desc"]),
         ],
+        priority="1.0",
     ),
     Page(
         path="/blog",
         query_params=[
             Param(name="page", values=["1", "2", "3"]),
             Param(name="sort", values=["asc", "desc"]),
         ],
+        # For lastmod, priority, and changefreq field, you can use callback function for more precise control
+        lastmod=lambda loc, path_params, query_params: "2024-05-07T00:00:00+00"
     ),
     Page(
         path="/blog/{id}",
         path_params=[Param(name="id", values=["1", "2", "3"])],
     ),
 ]
```

