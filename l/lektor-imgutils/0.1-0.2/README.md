# Comparing `tmp/lektor-imgutils-0.1.tar.gz` & `tmp/lektor_imgutils-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lektor-imgutils-0.1.tar", last modified: Wed Jul  5 21:48:20 2023, max compression
+gzip compressed data, was "lektor_imgutils-0.2.tar", last modified: Tue May  7 17:35:55 2024, max compression
```

## Comparing `lektor-imgutils-0.1.tar` & `lektor_imgutils-0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-05 21:48:20.884284 lektor-imgutils-0.1/
--rw-------   0 uyar      (1000) uyar      (1000)      179 2023-07-05 21:25:49.000000 lektor-imgutils-0.1/.gitignore
--rw-------   0 uyar      (1000) uyar      (1000)      169 2023-07-05 21:32:45.000000 lektor-imgutils-0.1/CHANGES.rst
--rw-------   0 uyar      (1000) uyar      (1000)     1491 2023-07-05 19:51:35.000000 lektor-imgutils-0.1/LICENSE.txt
--rw-------   0 uyar      (1000) uyar      (1000)     3644 2023-07-05 21:48:20.884284 lektor-imgutils-0.1/PKG-INFO
--rw-------   0 uyar      (1000) uyar      (1000)      838 2023-07-05 21:44:37.000000 lektor-imgutils-0.1/README.rst
-drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-05 21:48:20.884284 lektor-imgutils-0.1/lektor_imgutils/
--rw-------   0 uyar      (1000) uyar      (1000)     3141 2023-07-05 21:12:21.000000 lektor-imgutils-0.1/lektor_imgutils/__init__.py
-drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-05 21:48:20.884284 lektor-imgutils-0.1/lektor_imgutils.egg-info/
--rw-------   0 uyar      (1000) uyar      (1000)     3644 2023-07-05 21:48:20.000000 lektor-imgutils-0.1/lektor_imgutils.egg-info/PKG-INFO
--rw-------   0 uyar      (1000) uyar      (1000)      362 2023-07-05 21:48:20.000000 lektor-imgutils-0.1/lektor_imgutils.egg-info/SOURCES.txt
--rw-------   0 uyar      (1000) uyar      (1000)        1 2023-07-05 21:48:20.000000 lektor-imgutils-0.1/lektor_imgutils.egg-info/dependency_links.txt
--rw-------   0 uyar      (1000) uyar      (1000)       59 2023-07-05 21:48:20.000000 lektor-imgutils-0.1/lektor_imgutils.egg-info/entry_points.txt
--rw-------   0 uyar      (1000) uyar      (1000)       89 2023-07-05 21:48:20.000000 lektor-imgutils-0.1/lektor_imgutils.egg-info/requires.txt
--rw-------   0 uyar      (1000) uyar      (1000)       16 2023-07-05 21:48:20.000000 lektor-imgutils-0.1/lektor_imgutils.egg-info/top_level.txt
--rw-------   0 uyar      (1000) uyar      (1000)     1880 2023-07-05 20:03:31.000000 lektor-imgutils-0.1/pyproject.toml
--rw-------   0 uyar      (1000) uyar      (1000)     1110 2023-07-05 20:03:43.000000 lektor-imgutils-0.1/requirements-dev.txt
--rw-------   0 uyar      (1000) uyar      (1000)      105 2023-07-05 20:03:43.000000 lektor-imgutils-0.1/requirements.txt
--rw-------   0 uyar      (1000) uyar      (1000)       38 2023-07-05 21:48:20.884284 lektor-imgutils-0.1/setup.cfg
+drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2024-05-07 17:35:55.632842 lektor_imgutils-0.2/
+-rw-r--r--   0 uyar      (1000) uyar      (1000)      179 2023-07-05 21:25:49.000000 lektor_imgutils-0.2/.gitignore
+-rw-r--r--   0 uyar      (1000) uyar      (1000)      294 2024-05-07 17:25:03.000000 lektor_imgutils-0.2/CHANGES.rst
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     1496 2024-02-21 14:36:17.000000 lektor_imgutils-0.2/LICENSE.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     3967 2024-05-07 17:35:55.632842 lektor_imgutils-0.2/PKG-INFO
+-rw-r--r--   0 uyar      (1000) uyar      (1000)      753 2024-05-07 17:25:03.000000 lektor_imgutils-0.2/README.rst
+drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2024-05-07 17:35:55.632842 lektor_imgutils-0.2/lektor_imgutils.egg-info/
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     3967 2024-05-07 17:35:55.000000 lektor_imgutils-0.2/lektor_imgutils.egg-info/PKG-INFO
+-rw-r--r--   0 uyar      (1000) uyar      (1000)      376 2024-05-07 17:35:55.000000 lektor_imgutils-0.2/lektor_imgutils.egg-info/SOURCES.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)        1 2024-05-07 17:35:55.000000 lektor_imgutils-0.2/lektor_imgutils.egg-info/dependency_links.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)       59 2024-05-07 17:35:55.000000 lektor_imgutils-0.2/lektor_imgutils.egg-info/entry_points.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)      163 2024-05-07 17:35:55.000000 lektor_imgutils-0.2/lektor_imgutils.egg-info/requires.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)       16 2024-05-07 17:35:55.000000 lektor_imgutils-0.2/lektor_imgutils.egg-info/top_level.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     3903 2024-05-07 17:31:47.000000 lektor_imgutils-0.2/lektor_imgutils.py
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     2326 2024-05-07 17:29:08.000000 lektor_imgutils-0.2/pyproject.toml
+-rw-r--r--   0 uyar      (1000) uyar      (1000)      892 2024-05-07 17:33:17.000000 lektor_imgutils-0.2/requirements-dev.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)      535 2024-05-07 17:33:17.000000 lektor_imgutils-0.2/requirements.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)       38 2024-05-07 17:35:55.632842 lektor_imgutils-0.2/setup.cfg
+drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2024-05-07 17:35:55.632842 lektor_imgutils-0.2/tests/
+-rw-r--r--   0 uyar      (1000) uyar      (1000)      193 2024-05-07 17:31:23.000000 lektor_imgutils-0.2/tests/test_imgutils.py
```

### Comparing `lektor-imgutils-0.1/LICENSE.txt` & `lektor_imgutils-0.2/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2023 H. Turgut Uyar <uyar@tekir.org>
+Copyright 2023-2024 H. Turgut Uyar <uyar@tekir.org>
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice,
    this list of conditions and the following disclaimer.
```

### Comparing `lektor-imgutils-0.1/PKG-INFO` & `lektor_imgutils-0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lektor-imgutils
-Version: 0.1
+Version: 0.2
 Summary: Image handling utilities for Lektor.
 Author-email: "H. Turgut Uyar" <uyar@tekir.org>
-License: Copyright 2023 H. Turgut Uyar <uyar@tekir.org>
+License: Copyright 2023-2024 H. Turgut Uyar <uyar@tekir.org>
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice,
            this list of conditions and the following disclaimer.
         
@@ -28,34 +28,47 @@
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: repository, https://github.com/uyar/lektor-imgutils
 Keywords: lektor,plugin,image,responsive,srcset,picture
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Framework :: Lektor
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet
-Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
-Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+Requires-Dist: lektor
+Requires-Dist: lxml
+Requires-Dist: cssselect
+Requires-Dist: pillow
+Requires-Dist: typedload
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
 Provides-Extra: style
+Requires-Dist: ruff; extra == "style"
+Provides-Extra: types
+Requires-Dist: mypy; extra == "types"
+Requires-Dist: lxml-stubs; extra == "types"
 Provides-Extra: dev
-License-File: LICENSE.txt
+Requires-Dist: lektor-imgutils[style,tests,types]; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: tox; extra == "dev"
 
 lektor-imgutils
 ===============
 
 lektor-imgutils is a plugin for the `Lektor <https://www.getlektor.com>`_
 static site generator
 that manipulates image files and image-related markup
@@ -63,26 +76,22 @@
 
 To use the plugin, add it to your project::
 
   lektor plugin add lektor-imgutils
 
 The plugin can be configured using the ``configs/imgutils.ini`` file.
 Each section specifies a rule that will be applied to selected images.
-Each section must have a "selector" key which is a CSS selector
-to select the image elements.
-The section names are insignificant.
+The section key is a CSS selector key which is used to select the image elements.
 
 Examples
 --------
 
 Set missing width and height attributes to all images::
 
-  [default]
-  selector = img
-  size = yes
+  [img]
+  size = intrinsic
 
 Set lazy loading and async decoding on all images in the ".content" part::
 
-  [content]
-  selector = .content img
+  [.content img]
   loading = lazy
   decoding = async
```

### Comparing `lektor-imgutils-0.1/README.rst` & `lektor_imgutils-0.2/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -8,26 +8,22 @@
 
 To use the plugin, add it to your project::
 
   lektor plugin add lektor-imgutils
 
 The plugin can be configured using the ``configs/imgutils.ini`` file.
 Each section specifies a rule that will be applied to selected images.
-Each section must have a "selector" key which is a CSS selector
-to select the image elements.
-The section names are insignificant.
+The section key is a CSS selector key which is used to select the image elements.
 
 Examples
 --------
 
 Set missing width and height attributes to all images::
 
-  [default]
-  selector = img
-  size = yes
+  [img]
+  size = intrinsic
 
 Set lazy loading and async decoding on all images in the ".content" part::
 
-  [content]
-  selector = .content img
+  [.content img]
   loading = lazy
   decoding = async
```

### Comparing `lektor-imgutils-0.1/lektor_imgutils.egg-info/PKG-INFO` & `lektor_imgutils-0.2/lektor_imgutils.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lektor-imgutils
-Version: 0.1
+Version: 0.2
 Summary: Image handling utilities for Lektor.
 Author-email: "H. Turgut Uyar" <uyar@tekir.org>
-License: Copyright 2023 H. Turgut Uyar <uyar@tekir.org>
+License: Copyright 2023-2024 H. Turgut Uyar <uyar@tekir.org>
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice,
            this list of conditions and the following disclaimer.
         
@@ -28,34 +28,47 @@
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: repository, https://github.com/uyar/lektor-imgutils
 Keywords: lektor,plugin,image,responsive,srcset,picture
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Framework :: Lektor
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet
-Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
-Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+Requires-Dist: lektor
+Requires-Dist: lxml
+Requires-Dist: cssselect
+Requires-Dist: pillow
+Requires-Dist: typedload
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
 Provides-Extra: style
+Requires-Dist: ruff; extra == "style"
+Provides-Extra: types
+Requires-Dist: mypy; extra == "types"
+Requires-Dist: lxml-stubs; extra == "types"
 Provides-Extra: dev
-License-File: LICENSE.txt
+Requires-Dist: lektor-imgutils[style,tests,types]; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: tox; extra == "dev"
 
 lektor-imgutils
 ===============
 
 lektor-imgutils is a plugin for the `Lektor <https://www.getlektor.com>`_
 static site generator
 that manipulates image files and image-related markup
@@ -63,26 +76,22 @@
 
 To use the plugin, add it to your project::
 
   lektor plugin add lektor-imgutils
 
 The plugin can be configured using the ``configs/imgutils.ini`` file.
 Each section specifies a rule that will be applied to selected images.
-Each section must have a "selector" key which is a CSS selector
-to select the image elements.
-The section names are insignificant.
+The section key is a CSS selector key which is used to select the image elements.
 
 Examples
 --------
 
 Set missing width and height attributes to all images::
 
-  [default]
-  selector = img
-  size = yes
+  [img]
+  size = intrinsic
 
 Set lazy loading and async decoding on all images in the ".content" part::
 
-  [content]
-  selector = .content img
+  [.content img]
   loading = lazy
   decoding = async
```

