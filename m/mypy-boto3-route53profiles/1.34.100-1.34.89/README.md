# Comparing `tmp/mypy_boto3_route53profiles-1.34.100.tar.gz` & `tmp/mypy_boto3_route53profiles-1.34.89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_route53profiles-1.34.100.tar", last modified: Tue May  7 19:46:55 2024, max compression
+gzip compressed data, was "mypy_boto3_route53profiles-1.34.89.tar", last modified: Mon Apr 22 19:19:12 2024, max compression
```

## Comparing `mypy_boto3_route53profiles-1.34.100.tar` & `mypy_boto3_route53profiles-1.34.89.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:46:55.655063 mypy_boto3_route53profiles-1.34.100/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-07 19:46:43.000000 mypy_boto3_route53profiles-1.34.100/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-05-07 19:46:55.655063 mypy_boto3_route53profiles-1.34.100/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-05-07 19:46:43.000000 mypy_boto3_route53profiles-1.34.100/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:46:55.655063 mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-07 19:46:43.000000 mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-07 19:46:43.000000 mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-07 19:46:43.000000 mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14893 2024-05-07 19:46:43.000000 mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14890 2024-05-07 19:46:43.000000 mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-05-07 19:46:44.000000 mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-05-07 19:46:44.000000 mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-07 19:46:43.000000 mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-07 19:46:43.000000 mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:46:43.000000 mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12005 2024-05-07 19:46:44.000000 mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12005 2024-05-07 19:46:44.000000 mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-07 19:46:43.000000 mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:46:55.655063 mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-05-07 19:46:55.000000 mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-07 19:46:55.000000 mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:46:55.000000 mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:46:55.000000 mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-07 19:46:55.000000 mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 19:46:55.000000 mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 19:46:55.655063 mypy_boto3_route53profiles-1.34.100/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-07 19:46:43.000000 mypy_boto3_route53profiles-1.34.100/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:12.995682 mypy_boto3_route53profiles-1.34.89/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-22 19:18:37.000000 mypy_boto3_route53profiles-1.34.89/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13533 2024-04-22 19:19:12.995682 mypy_boto3_route53profiles-1.34.89/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11946 2024-04-22 19:18:37.000000 mypy_boto3_route53profiles-1.34.89/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:12.991682 mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-22 19:18:37.000000 mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-22 19:18:37.000000 mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-22 19:18:37.000000 mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14893 2024-04-22 19:18:37.000000 mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14890 2024-04-22 19:18:37.000000 mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-04-22 19:18:37.000000 mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-04-22 19:18:37.000000 mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-22 19:18:37.000000 mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-22 19:18:37.000000 mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:18:37.000000 mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11966 2024-04-22 19:18:37.000000 mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11966 2024-04-22 19:18:37.000000 mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 19:18:37.000000 mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:12.995682 mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13533 2024-04-22 19:19:12.000000 mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-22 19:19:12.000000 mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:19:12.000000 mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:19:12.000000 mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-22 19:19:12.000000 mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-22 19:19:12.000000 mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 19:19:12.995682 mypy_boto3_route53profiles-1.34.89/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-22 19:18:37.000000 mypy_boto3_route53profiles-1.34.89/setup.py
```

### Comparing `mypy_boto3_route53profiles-1.34.100/LICENSE` & `mypy_boto3_route53profiles-1.34.89/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_route53profiles-1.34.100/PKG-INFO` & `mypy_boto3_route53profiles-1.34.89/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53profiles
-Version: 1.34.100
-Summary: Type annotations for boto3.Route53Profiles 1.34.100 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.89
+Summary: Type annotations for boto3.Route53Profiles 1.34.89 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53profiles/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53profiles)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53profiles/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53profiles)](https://pepy.tech/project/mypy-boto3-route53profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Profiles 1.34.100](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53profiles.html#Route53Profiles)
+[boto3.Route53Profiles 1.34.89](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53profiles.html#Route53Profiles)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-route53profiles docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53profiles/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_route53profiles-1.34.100/README.md` & `mypy_boto3_route53profiles-1.34.89/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53profiles)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53profiles/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53profiles)](https://pepy.tech/project/mypy-boto3-route53profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Profiles 1.34.100](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53profiles.html#Route53Profiles)
+[boto3.Route53Profiles 1.34.89](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53profiles.html#Route53Profiles)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-route53profiles docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53profiles/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/__init__.py` & `mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/__init__.pyi` & `mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/__main__.py` & `mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Route53Profiles 1.34.100\n"
-        "Version:         1.34.100\n"
-        "Builder version: 7.24.0\n"
+        "Type annotations for boto3.Route53Profiles 1.34.89\n"
+        "Version:         1.34.89\n"
+        "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53profiles//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53profiles.html#Route53Profiles\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.100")
+    print("1.34.89")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/client.py` & `mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/client.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/client.pyi` & `mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/literals.py` & `mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/literals.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/literals.pyi` & `mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/paginator.py` & `mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/paginator.pyi` & `mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/type_defs.py` & `mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,17 +286,17 @@
         "ProfileAssociation": ProfileAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListProfileAssociationsResponseTypeDef = TypedDict(
     "ListProfileAssociationsResponseTypeDef",
     {
+        "NextToken": str,
         "ProfileAssociations": List[ProfileAssociationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -322,17 +322,17 @@
         "ProfileResourceAssociation": ProfileResourceAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListProfileResourceAssociationsResponseTypeDef = TypedDict(
     "ListProfileResourceAssociationsResponseTypeDef",
     {
+        "NextToken": str,
         "ProfileResourceAssociations": List[ProfileResourceAssociationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 UpdateProfileResourceAssociationResponseTypeDef = TypedDict(
     "UpdateProfileResourceAssociationResponseTypeDef",
     {
         "ProfileResourceAssociation": ProfileResourceAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -380,12 +380,12 @@
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListProfilesResponseTypeDef = TypedDict(
     "ListProfilesResponseTypeDef",
     {
+        "NextToken": str,
         "ProfileSummaries": List[ProfileSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
```

### Comparing `mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles/type_defs.pyi` & `mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -286,17 +286,17 @@
         "ProfileAssociation": ProfileAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListProfileAssociationsResponseTypeDef = TypedDict(
     "ListProfileAssociationsResponseTypeDef",
     {
+        "NextToken": str,
         "ProfileAssociations": List[ProfileAssociationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -322,17 +322,17 @@
         "ProfileResourceAssociation": ProfileResourceAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListProfileResourceAssociationsResponseTypeDef = TypedDict(
     "ListProfileResourceAssociationsResponseTypeDef",
     {
+        "NextToken": str,
         "ProfileResourceAssociations": List[ProfileResourceAssociationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 UpdateProfileResourceAssociationResponseTypeDef = TypedDict(
     "UpdateProfileResourceAssociationResponseTypeDef",
     {
         "ProfileResourceAssociation": ProfileResourceAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -380,12 +380,12 @@
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListProfilesResponseTypeDef = TypedDict(
     "ListProfilesResponseTypeDef",
     {
+        "NextToken": str,
         "ProfileSummaries": List[ProfileSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
```

### Comparing `mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles.egg-info/PKG-INFO` & `mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53profiles
-Version: 1.34.100
-Summary: Type annotations for boto3.Route53Profiles 1.34.100 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.89
+Summary: Type annotations for boto3.Route53Profiles 1.34.89 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53profiles/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53profiles)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53profiles/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53profiles)](https://pepy.tech/project/mypy-boto3-route53profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Profiles 1.34.100](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53profiles.html#Route53Profiles)
+[boto3.Route53Profiles 1.34.89](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53profiles.html#Route53Profiles)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-route53profiles docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53profiles/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_route53profiles-1.34.100/mypy_boto3_route53profiles.egg-info/SOURCES.txt` & `mypy_boto3_route53profiles-1.34.89/mypy_boto3_route53profiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_route53profiles-1.34.100/setup.py` & `mypy_boto3_route53profiles-1.34.89/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-route53profiles",
-    version="1.34.100",
+    version="1.34.89",
     packages=["mypy_boto3_route53profiles"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.Route53Profiles 1.34.100 service generated with mypy-boto3-builder 7.24.0",
+    description="Type annotations for boto3.Route53Profiles 1.34.89 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

