# Comparing `tmp/mypy-boto3-b2bi-1.34.74.tar.gz` & `tmp/mypy-boto3-b2bi-1.34.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-b2bi-1.34.74.tar", last modified: Fri Mar 29 19:18:22 2024, max compression
+gzip compressed data, was "mypy-boto3-b2bi-1.34.78.tar", last modified: Thu Apr  4 19:33:16 2024, max compression
```

## Comparing `mypy-boto3-b2bi-1.34.74.tar` & `mypy-boto3-b2bi-1.34.78.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:18:22.680138 mypy-boto3-b2bi-1.34.74/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-29 19:17:39.000000 mypy-boto3-b2bi-1.34.74/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12885 2024-03-29 19:18:22.676138 mypy-boto3-b2bi-1.34.74/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-03-29 19:17:39.000000 mypy-boto3-b2bi-1.34.74/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:18:22.676138 mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-29 19:17:39.000000 mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-29 19:17:39.000000 mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-29 19:17:39.000000 mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20999 2024-03-29 19:17:40.000000 mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20996 2024-03-29 19:17:39.000000 mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-03-29 19:17:40.000000 mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-03-29 19:17:40.000000 mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-03-29 19:17:40.000000 mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-03-29 19:17:40.000000 mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 19:17:39.000000 mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    20226 2024-03-29 19:17:40.000000 mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    20226 2024-03-29 19:17:40.000000 mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-29 19:17:39.000000 mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:18:22.676138 mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12885 2024-03-29 19:18:22.000000 mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-29 19:18:22.000000 mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 19:18:22.000000 mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 19:18:22.000000 mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-29 19:18:22.000000 mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-29 19:18:22.000000 mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 19:18:22.680138 mypy-boto3-b2bi-1.34.74/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-03-29 19:17:39.000000 mypy-boto3-b2bi-1.34.74/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:16.168019 mypy-boto3-b2bi-1.34.78/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-04 19:32:15.000000 mypy-boto3-b2bi-1.34.78/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12885 2024-04-04 19:33:16.168019 mypy-boto3-b2bi-1.34.78/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-04 19:32:15.000000 mypy-boto3-b2bi-1.34.78/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:16.164019 mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-04 19:32:15.000000 mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-04 19:32:15.000000 mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-04 19:32:15.000000 mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20999 2024-04-04 19:32:16.000000 mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20996 2024-04-04 19:32:16.000000 mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-04-04 19:32:16.000000 mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-04-04 19:32:16.000000 mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-04 19:32:16.000000 mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-04-04 19:32:16.000000 mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:32:15.000000 mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    20226 2024-04-04 19:32:16.000000 mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20226 2024-04-04 19:32:16.000000 mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 19:32:15.000000 mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:16.168019 mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12885 2024-04-04 19:33:16.000000 mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-04 19:33:16.000000 mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:33:16.000000 mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:33:16.000000 mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-04 19:33:16.000000 mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 19:33:16.000000 mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 19:33:16.168019 mypy-boto3-b2bi-1.34.78/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-04 19:32:15.000000 mypy-boto3-b2bi-1.34.78/setup.py
```

### Comparing `mypy-boto3-b2bi-1.34.74/LICENSE` & `mypy-boto3-b2bi-1.34.78/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-b2bi-1.34.74/PKG-INFO` & `mypy-boto3-b2bi-1.34.78/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-b2bi
-Version: 1.34.74
-Summary: Type annotations for boto3.B2BI 1.34.74 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.78
+Summary: Type annotations for boto3.B2BI 1.34.78 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_b2bi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-b2bi.svg?color=blue)](https://pypi.org/project/mypy-boto3-b2bi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_b2bi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-b2bi)](https://pepy.tech/project/mypy-boto3-b2bi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.B2BI 1.34.74](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI)
+[boto3.B2BI 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-b2bi-1.34.74/README.md` & `mypy-boto3-b2bi-1.34.78/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-b2bi.svg?color=blue)](https://pypi.org/project/mypy-boto3-b2bi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_b2bi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-b2bi)](https://pepy.tech/project/mypy-boto3-b2bi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.B2BI 1.34.74](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI)
+[boto3.B2BI 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/__init__.py` & `mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/__init__.pyi` & `mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/__main__.py` & `mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.B2BI 1.34.74\n"
-        "Version:         1.34.74\n"
+        "Type annotations for boto3.B2BI 1.34.78\n"
+        "Version:         1.34.78\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_b2bi//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.74")
+    print("1.34.78")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/client.py` & `mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/client.pyi` & `mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/literals.py` & `mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/literals.py`

 * *Files 21% similar despite different names*

```diff
@@ -55,36 +55,58 @@
     "X12_214",
     "X12_215",
     "X12_259",
     "X12_260",
     "X12_266",
     "X12_269",
     "X12_270",
+    "X12_270_X279",
     "X12_271",
+    "X12_271_X279",
     "X12_274",
     "X12_275",
+    "X12_275_X210",
+    "X12_275_X211",
     "X12_276",
+    "X12_276_X212",
     "X12_277",
+    "X12_277_X212",
+    "X12_277_X214",
+    "X12_277_X364",
     "X12_278",
+    "X12_278_X217",
     "X12_310",
     "X12_315",
     "X12_322",
     "X12_404",
     "X12_410",
     "X12_417",
     "X12_421",
     "X12_426",
     "X12_810",
     "X12_820",
+    "X12_820_X218",
+    "X12_820_X306",
     "X12_824",
+    "X12_824_X186",
     "X12_830",
     "X12_832",
     "X12_834",
+    "X12_834_X220",
+    "X12_834_X307",
+    "X12_834_X318",
     "X12_835",
+    "X12_835_X221",
     "X12_837",
+    "X12_837_X222",
+    "X12_837_X223",
+    "X12_837_X224",
+    "X12_837_X291",
+    "X12_837_X292",
+    "X12_837_X298",
     "X12_844",
     "X12_846",
     "X12_849",
     "X12_850",
     "X12_852",
     "X12_855",
     "X12_856",
@@ -95,16 +117,17 @@
     "X12_869",
     "X12_870",
     "X12_940",
     "X12_945",
     "X12_990",
     "X12_997",
     "X12_999",
+    "X12_999_X231",
 ]
-X12VersionType = Literal["VERSION_4010", "VERSION_4030", "VERSION_5010"]
+X12VersionType = Literal["VERSION_4010", "VERSION_4030", "VERSION_5010", "VERSION_5010_HIPAA"]
 B2BIServiceName = Literal["b2bi"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -200,14 +223,15 @@
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
```

### Comparing `mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/literals.pyi` & `mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/literals.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -55,36 +55,58 @@
     "X12_214",
     "X12_215",
     "X12_259",
     "X12_260",
     "X12_266",
     "X12_269",
     "X12_270",
+    "X12_270_X279",
     "X12_271",
+    "X12_271_X279",
     "X12_274",
     "X12_275",
+    "X12_275_X210",
+    "X12_275_X211",
     "X12_276",
+    "X12_276_X212",
     "X12_277",
+    "X12_277_X212",
+    "X12_277_X214",
+    "X12_277_X364",
     "X12_278",
+    "X12_278_X217",
     "X12_310",
     "X12_315",
     "X12_322",
     "X12_404",
     "X12_410",
     "X12_417",
     "X12_421",
     "X12_426",
     "X12_810",
     "X12_820",
+    "X12_820_X218",
+    "X12_820_X306",
     "X12_824",
+    "X12_824_X186",
     "X12_830",
     "X12_832",
     "X12_834",
+    "X12_834_X220",
+    "X12_834_X307",
+    "X12_834_X318",
     "X12_835",
+    "X12_835_X221",
     "X12_837",
+    "X12_837_X222",
+    "X12_837_X223",
+    "X12_837_X224",
+    "X12_837_X291",
+    "X12_837_X292",
+    "X12_837_X298",
     "X12_844",
     "X12_846",
     "X12_849",
     "X12_850",
     "X12_852",
     "X12_855",
     "X12_856",
@@ -95,16 +117,17 @@
     "X12_869",
     "X12_870",
     "X12_940",
     "X12_945",
     "X12_990",
     "X12_997",
     "X12_999",
+    "X12_999_X231",
 ]
-X12VersionType = Literal["VERSION_4010", "VERSION_4030", "VERSION_5010"]
+X12VersionType = Literal["VERSION_4010", "VERSION_4030", "VERSION_5010", "VERSION_5010_HIPAA"]
 B2BIServiceName = Literal["b2bi"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -200,14 +223,15 @@
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
```

### Comparing `mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/paginator.py` & `mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/paginator.pyi` & `mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/type_defs.py` & `mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi/type_defs.pyi` & `mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi.egg-info/PKG-INFO` & `mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-b2bi
-Version: 1.34.74
-Summary: Type annotations for boto3.B2BI 1.34.74 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.78
+Summary: Type annotations for boto3.B2BI 1.34.78 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_b2bi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-b2bi.svg?color=blue)](https://pypi.org/project/mypy-boto3-b2bi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_b2bi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-b2bi)](https://pepy.tech/project/mypy-boto3-b2bi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.B2BI 1.34.74](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI)
+[boto3.B2BI 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-b2bi-1.34.74/mypy_boto3_b2bi.egg-info/SOURCES.txt` & `mypy-boto3-b2bi-1.34.78/mypy_boto3_b2bi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-b2bi-1.34.74/setup.py` & `mypy-boto3-b2bi-1.34.78/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-b2bi",
-    version="1.34.74",
+    version="1.34.78",
     packages=["mypy_boto3_b2bi"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.B2BI 1.34.74 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.B2BI 1.34.78 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

