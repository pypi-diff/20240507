# Comparing `tmp/mypy-boto3-budgets-1.34.0.tar.gz` & `tmp/mypy_boto3_budgets-1.34.100.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-budgets-1.34.0.tar", last modified: Wed Dec 13 21:22:04 2023, max compression
+gzip compressed data, was "mypy_boto3_budgets-1.34.100.tar", last modified: Tue May  7 19:46:54 2024, max compression
```

## Comparing `mypy-boto3-budgets-1.34.0.tar` & `mypy_boto3_budgets-1.34.100.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:04.767142 mypy-boto3-budgets-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:06:20.000000 mypy-boto3-budgets-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14100 2023-12-13 21:22:04.767142 mypy-boto3-budgets-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12567 2023-12-13 21:06:20.000000 mypy-boto3-budgets-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:04.767142 mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2023-12-13 21:06:20.000000 mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2023-12-13 21:06:20.000000 mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 21:06:20.000000 mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21963 2023-12-13 21:06:21.000000 mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21959 2023-12-13 21:06:20.000000 mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11205 2023-12-13 21:06:21.000000 mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11203 2023-12-13 21:06:21.000000 mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11056 2023-12-13 21:06:21.000000 mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11046 2023-12-13 21:06:21.000000 mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:06:20.000000 mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    27111 2023-12-13 21:06:21.000000 mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27110 2023-12-13 21:06:21.000000 mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:06:20.000000 mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:04.767142 mypy-boto3-budgets-1.34.0/mypy_boto3_budgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14100 2023-12-13 21:22:04.000000 mypy-boto3-budgets-1.34.0/mypy_boto3_budgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      680 2023-12-13 21:22:04.000000 mypy-boto3-budgets-1.34.0/mypy_boto3_budgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:04.000000 mypy-boto3-budgets-1.34.0/mypy_boto3_budgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:04.000000 mypy-boto3-budgets-1.34.0/mypy_boto3_budgets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:22:04.000000 mypy-boto3-budgets-1.34.0/mypy_boto3_budgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-13 21:22:04.000000 mypy-boto3-budgets-1.34.0/mypy_boto3_budgets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:22:04.767142 mypy-boto3-budgets-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2023-12-13 21:06:20.000000 mypy-boto3-budgets-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:46:54.967059 mypy_boto3_budgets-1.34.100/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-07 19:46:40.000000 mypy_boto3_budgets-1.34.100/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14126 2024-05-07 19:46:54.963059 mypy_boto3_budgets-1.34.100/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12569 2024-05-07 19:46:40.000000 mypy_boto3_budgets-1.34.100/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:46:54.963059 mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-07 19:46:40.000000 mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-07 19:46:40.000000 mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-07 19:46:40.000000 mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23720 2024-05-07 19:46:40.000000 mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23717 2024-05-07 19:46:40.000000 mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11385 2024-05-07 19:46:40.000000 mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11385 2024-05-07 19:46:40.000000 mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11001 2024-05-07 19:46:40.000000 mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10992 2024-05-07 19:46:40.000000 mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:46:40.000000 mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    28879 2024-05-07 19:46:41.000000 mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28879 2024-05-07 19:46:40.000000 mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-07 19:46:40.000000 mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:46:54.963059 mypy_boto3_budgets-1.34.100/mypy_boto3_budgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14126 2024-05-07 19:46:54.000000 mypy_boto3_budgets-1.34.100/mypy_boto3_budgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-07 19:46:54.000000 mypy_boto3_budgets-1.34.100/mypy_boto3_budgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:46:54.000000 mypy_boto3_budgets-1.34.100/mypy_boto3_budgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:46:54.000000 mypy_boto3_budgets-1.34.100/mypy_boto3_budgets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-07 19:46:54.000000 mypy_boto3_budgets-1.34.100/mypy_boto3_budgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 19:46:54.000000 mypy_boto3_budgets-1.34.100/mypy_boto3_budgets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 19:46:54.967059 mypy_boto3_budgets-1.34.100/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-07 19:46:40.000000 mypy_boto3_budgets-1.34.100/setup.py
```

### Comparing `mypy-boto3-budgets-1.34.0/LICENSE` & `mypy_boto3_budgets-1.34.100/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-budgets-1.34.0/PKG-INFO` & `mypy_boto3_budgets-1.34.100/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-budgets
-Version: 1.34.0
-Summary: Type annotations for boto3.Budgets 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.100
+Summary: Type annotations for boto3.Budgets 1.34.100 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-budgets"></a>
 
 # mypy-boto3-budgets
 
 [![PyPI - mypy-boto3-budgets](https://img.shields.io/pypi/v/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-budgets)](https://pepy.tech/project/mypy-boto3-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Budgets 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
+[boto3.Budgets 1.34.100](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-budgets docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-budgets-1.34.0/README.md` & `mypy_boto3_budgets-1.34.100/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-budgets)](https://pepy.tech/project/mypy-boto3-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Budgets 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
+[boto3.Budgets 1.34.100](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-budgets docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/__init__.py` & `mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     DescribeBudgetsPaginator,
     DescribeNotificationsForBudgetPaginator,
     DescribeSubscribersForNotificationPaginator,
 )
 
 Client = BudgetsClient
 
-
 __all__ = (
     "BudgetsClient",
     "Client",
     "DescribeBudgetActionHistoriesPaginator",
     "DescribeBudgetActionsForAccountPaginator",
     "DescribeBudgetActionsForBudgetPaginator",
     "DescribeBudgetNotificationsForAccountPaginator",
```

### Comparing `mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/__init__.pyi` & `mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/__main__.py` & `mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Budgets 1.34.0\nVersion:         1.34.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.Budgets 1.34.100\n"
+        "Version:         1.34.100\n"
+        "Builder version: 7.24.0\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.0")
+    print("1.34.100")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/client.py` & `mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,42 +28,43 @@
     DescribeBudgetPerformanceHistoryPaginator,
     DescribeBudgetsPaginator,
     DescribeNotificationsForBudgetPaginator,
     DescribeSubscribersForNotificationPaginator,
 )
 from .type_defs import (
     ActionThresholdTypeDef,
-    BudgetTypeDef,
+    BudgetUnionTypeDef,
     CreateBudgetActionResponseTypeDef,
-    DefinitionTypeDef,
+    DefinitionUnionTypeDef,
     DeleteBudgetActionResponseTypeDef,
     DescribeBudgetActionHistoriesResponseTypeDef,
     DescribeBudgetActionResponseTypeDef,
     DescribeBudgetActionsForAccountResponseTypeDef,
     DescribeBudgetActionsForBudgetResponseTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
     DescribeBudgetResponseTypeDef,
     DescribeBudgetsResponseTypeDef,
     DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
     ExecuteBudgetActionResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     NotificationTypeDef,
     NotificationWithSubscribersTypeDef,
+    ResourceTagTypeDef,
     SubscriberTypeDef,
-    TimePeriodTypeDef,
+    TimePeriodUnionTypeDef,
     UpdateBudgetActionResponseTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("BudgetsClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -78,14 +79,15 @@
     DuplicateRecordException: Type[BotocoreClientError]
     ExpiredNextTokenException: Type[BotocoreClientError]
     InternalErrorException: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     ResourceLockedException: Type[BotocoreClientError]
+    ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
 
 
 class BudgetsClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/)
@@ -118,16 +120,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#close)
         """
 
     def create_budget(
         self,
         *,
         AccountId: str,
-        Budget: BudgetTypeDef,
-        NotificationsWithSubscribers: Sequence[NotificationWithSubscribersTypeDef] = ...
+        Budget: BudgetUnionTypeDef,
+        NotificationsWithSubscribers: Sequence[NotificationWithSubscribersTypeDef] = ...,
+        ResourceTags: Sequence[ResourceTagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a budget and, if included, notifications and subscribers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_budget)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#create_budget)
         """
@@ -136,48 +139,49 @@
         self,
         *,
         AccountId: str,
         BudgetName: str,
         NotificationType: NotificationTypeType,
         ActionType: ActionTypeType,
         ActionThreshold: ActionThresholdTypeDef,
-        Definition: DefinitionTypeDef,
+        Definition: DefinitionUnionTypeDef,
         ExecutionRoleArn: str,
         ApprovalModel: ApprovalModelType,
-        Subscribers: Sequence[SubscriberTypeDef]
+        Subscribers: Sequence[SubscriberTypeDef],
+        ResourceTags: Sequence[ResourceTagTypeDef] = ...,
     ) -> CreateBudgetActionResponseTypeDef:
         """
         Creates a budget action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_budget_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#create_budget_action)
         """
 
     def create_notification(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
-        Subscribers: Sequence[SubscriberTypeDef]
+        Subscribers: Sequence[SubscriberTypeDef],
     ) -> Dict[str, Any]:
         """
         Creates a notification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_notification)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#create_notification)
         """
 
     def create_subscriber(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
-        Subscriber: SubscriberTypeDef
+        Subscriber: SubscriberTypeDef,
     ) -> Dict[str, Any]:
         """
         Creates a subscriber.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_subscriber)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#create_subscriber)
         """
@@ -212,15 +216,15 @@
 
     def delete_subscriber(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
-        Subscriber: SubscriberTypeDef
+        Subscriber: SubscriberTypeDef,
     ) -> Dict[str, Any]:
         """
         Deletes a subscriber.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.delete_subscriber)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#delete_subscriber)
         """
@@ -245,17 +249,17 @@
 
     def describe_budget_action_histories(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
-        TimePeriod: TimePeriodTypeDef = ...,
+        TimePeriod: TimePeriodUnionTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeBudgetActionHistoriesResponseTypeDef:
         """
         Describes a budget action history detail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_action_histories)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#describe_budget_action_histories)
         """
@@ -291,17 +295,17 @@
         """
 
     def describe_budget_performance_history(
         self,
         *,
         AccountId: str,
         BudgetName: str,
-        TimePeriod: TimePeriodTypeDef = ...,
+        TimePeriod: TimePeriodUnionTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeBudgetPerformanceHistoryResponseTypeDef:
         """
         Describes the history for `DAILY`, `MONTHLY`, and `QUARTERLY` budgets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_performance_history)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#describe_budget_performance_history)
         """
@@ -329,15 +333,15 @@
     def describe_subscribers_for_notification(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeSubscribersForNotificationResponseTypeDef:
         """
         Lists the subscribers that are associated with a notification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_subscribers_for_notification)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#describe_subscribers_for_notification)
         """
@@ -362,15 +366,41 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#generate_presigned_url)
         """
 
-    def update_budget(self, *, AccountId: str, NewBudget: BudgetTypeDef) -> Dict[str, Any]:
+    def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResponseTypeDef:
+        """
+        Lists tags associated with a budget or budget action resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.list_tags_for_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#list_tags_for_resource)
+        """
+
+    def tag_resource(
+        self, *, ResourceARN: str, ResourceTags: Sequence[ResourceTagTypeDef]
+    ) -> Dict[str, Any]:
+        """
+        Creates tags for a budget or budget action resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.tag_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#tag_resource)
+        """
+
+    def untag_resource(self, *, ResourceARN: str, ResourceTagKeys: Sequence[str]) -> Dict[str, Any]:
+        """
+        Deletes tags associated with a budget or budget action resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.untag_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#untag_resource)
+        """
+
+    def update_budget(self, *, AccountId: str, NewBudget: BudgetUnionTypeDef) -> Dict[str, Any]:
         """
         Updates a budget.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_budget)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#update_budget)
         """
 
@@ -378,33 +408,33 @@
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
         NotificationType: NotificationTypeType = ...,
         ActionThreshold: ActionThresholdTypeDef = ...,
-        Definition: DefinitionTypeDef = ...,
+        Definition: DefinitionUnionTypeDef = ...,
         ExecutionRoleArn: str = ...,
         ApprovalModel: ApprovalModelType = ...,
-        Subscribers: Sequence[SubscriberTypeDef] = ...
+        Subscribers: Sequence[SubscriberTypeDef] = ...,
     ) -> UpdateBudgetActionResponseTypeDef:
         """
         Updates a budget action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_budget_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#update_budget_action)
         """
 
     def update_notification(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         OldNotification: NotificationTypeDef,
-        NewNotification: NotificationTypeDef
+        NewNotification: NotificationTypeDef,
     ) -> Dict[str, Any]:
         """
         Updates a notification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_notification)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#update_notification)
         """
@@ -412,15 +442,15 @@
     def update_subscriber(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
         OldSubscriber: SubscriberTypeDef,
-        NewSubscriber: SubscriberTypeDef
+        NewSubscriber: SubscriberTypeDef,
     ) -> Dict[str, Any]:
         """
         Updates a subscriber.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_subscriber)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#update_subscriber)
         """
```

### Comparing `mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/client.pyi` & `mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/client.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -28,33 +28,35 @@
     DescribeBudgetPerformanceHistoryPaginator,
     DescribeBudgetsPaginator,
     DescribeNotificationsForBudgetPaginator,
     DescribeSubscribersForNotificationPaginator,
 )
 from .type_defs import (
     ActionThresholdTypeDef,
-    BudgetTypeDef,
+    BudgetUnionTypeDef,
     CreateBudgetActionResponseTypeDef,
-    DefinitionTypeDef,
+    DefinitionUnionTypeDef,
     DeleteBudgetActionResponseTypeDef,
     DescribeBudgetActionHistoriesResponseTypeDef,
     DescribeBudgetActionResponseTypeDef,
     DescribeBudgetActionsForAccountResponseTypeDef,
     DescribeBudgetActionsForBudgetResponseTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
     DescribeBudgetResponseTypeDef,
     DescribeBudgetsResponseTypeDef,
     DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
     ExecuteBudgetActionResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     NotificationTypeDef,
     NotificationWithSubscribersTypeDef,
+    ResourceTagTypeDef,
     SubscriberTypeDef,
-    TimePeriodTypeDef,
+    TimePeriodUnionTypeDef,
     UpdateBudgetActionResponseTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -75,14 +77,15 @@
     DuplicateRecordException: Type[BotocoreClientError]
     ExpiredNextTokenException: Type[BotocoreClientError]
     InternalErrorException: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     ResourceLockedException: Type[BotocoreClientError]
+    ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
 
 class BudgetsClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/)
     """
@@ -114,16 +117,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#close)
         """
 
     def create_budget(
         self,
         *,
         AccountId: str,
-        Budget: BudgetTypeDef,
-        NotificationsWithSubscribers: Sequence[NotificationWithSubscribersTypeDef] = ...
+        Budget: BudgetUnionTypeDef,
+        NotificationsWithSubscribers: Sequence[NotificationWithSubscribersTypeDef] = ...,
+        ResourceTags: Sequence[ResourceTagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a budget and, if included, notifications and subscribers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_budget)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#create_budget)
         """
@@ -132,48 +136,49 @@
         self,
         *,
         AccountId: str,
         BudgetName: str,
         NotificationType: NotificationTypeType,
         ActionType: ActionTypeType,
         ActionThreshold: ActionThresholdTypeDef,
-        Definition: DefinitionTypeDef,
+        Definition: DefinitionUnionTypeDef,
         ExecutionRoleArn: str,
         ApprovalModel: ApprovalModelType,
-        Subscribers: Sequence[SubscriberTypeDef]
+        Subscribers: Sequence[SubscriberTypeDef],
+        ResourceTags: Sequence[ResourceTagTypeDef] = ...,
     ) -> CreateBudgetActionResponseTypeDef:
         """
         Creates a budget action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_budget_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#create_budget_action)
         """
 
     def create_notification(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
-        Subscribers: Sequence[SubscriberTypeDef]
+        Subscribers: Sequence[SubscriberTypeDef],
     ) -> Dict[str, Any]:
         """
         Creates a notification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_notification)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#create_notification)
         """
 
     def create_subscriber(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
-        Subscriber: SubscriberTypeDef
+        Subscriber: SubscriberTypeDef,
     ) -> Dict[str, Any]:
         """
         Creates a subscriber.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_subscriber)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#create_subscriber)
         """
@@ -208,15 +213,15 @@
 
     def delete_subscriber(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
-        Subscriber: SubscriberTypeDef
+        Subscriber: SubscriberTypeDef,
     ) -> Dict[str, Any]:
         """
         Deletes a subscriber.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.delete_subscriber)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#delete_subscriber)
         """
@@ -241,17 +246,17 @@
 
     def describe_budget_action_histories(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
-        TimePeriod: TimePeriodTypeDef = ...,
+        TimePeriod: TimePeriodUnionTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeBudgetActionHistoriesResponseTypeDef:
         """
         Describes a budget action history detail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_action_histories)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#describe_budget_action_histories)
         """
@@ -287,17 +292,17 @@
         """
 
     def describe_budget_performance_history(
         self,
         *,
         AccountId: str,
         BudgetName: str,
-        TimePeriod: TimePeriodTypeDef = ...,
+        TimePeriod: TimePeriodUnionTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeBudgetPerformanceHistoryResponseTypeDef:
         """
         Describes the history for `DAILY`, `MONTHLY`, and `QUARTERLY` budgets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_performance_history)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#describe_budget_performance_history)
         """
@@ -325,15 +330,15 @@
     def describe_subscribers_for_notification(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeSubscribersForNotificationResponseTypeDef:
         """
         Lists the subscribers that are associated with a notification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_subscribers_for_notification)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#describe_subscribers_for_notification)
         """
@@ -358,15 +363,41 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#generate_presigned_url)
         """
 
-    def update_budget(self, *, AccountId: str, NewBudget: BudgetTypeDef) -> Dict[str, Any]:
+    def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResponseTypeDef:
+        """
+        Lists tags associated with a budget or budget action resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.list_tags_for_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#list_tags_for_resource)
+        """
+
+    def tag_resource(
+        self, *, ResourceARN: str, ResourceTags: Sequence[ResourceTagTypeDef]
+    ) -> Dict[str, Any]:
+        """
+        Creates tags for a budget or budget action resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.tag_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#tag_resource)
+        """
+
+    def untag_resource(self, *, ResourceARN: str, ResourceTagKeys: Sequence[str]) -> Dict[str, Any]:
+        """
+        Deletes tags associated with a budget or budget action resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.untag_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#untag_resource)
+        """
+
+    def update_budget(self, *, AccountId: str, NewBudget: BudgetUnionTypeDef) -> Dict[str, Any]:
         """
         Updates a budget.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_budget)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#update_budget)
         """
 
@@ -374,33 +405,33 @@
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
         NotificationType: NotificationTypeType = ...,
         ActionThreshold: ActionThresholdTypeDef = ...,
-        Definition: DefinitionTypeDef = ...,
+        Definition: DefinitionUnionTypeDef = ...,
         ExecutionRoleArn: str = ...,
         ApprovalModel: ApprovalModelType = ...,
-        Subscribers: Sequence[SubscriberTypeDef] = ...
+        Subscribers: Sequence[SubscriberTypeDef] = ...,
     ) -> UpdateBudgetActionResponseTypeDef:
         """
         Updates a budget action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_budget_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#update_budget_action)
         """
 
     def update_notification(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         OldNotification: NotificationTypeDef,
-        NewNotification: NotificationTypeDef
+        NewNotification: NotificationTypeDef,
     ) -> Dict[str, Any]:
         """
         Updates a notification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_notification)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#update_notification)
         """
@@ -408,15 +439,15 @@
     def update_subscriber(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
         OldSubscriber: SubscriberTypeDef,
-        NewSubscriber: SubscriberTypeDef
+        NewSubscriber: SubscriberTypeDef,
     ) -> Dict[str, Any]:
         """
         Updates a subscriber.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_subscriber)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#update_subscriber)
         """
```

### Comparing `mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/literals.py` & `mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ActionStatusType",
     "ActionSubTypeType",
     "ActionTypeType",
     "ApprovalModelType",
     "AutoAdjustTypeType",
     "BudgetTypeType",
@@ -45,15 +44,14 @@
     "TimeUnitType",
     "BudgetsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 ActionStatusType = Literal[
     "EXECUTION_FAILURE",
     "EXECUTION_IN_PROGRESS",
     "EXECUTION_SUCCESS",
     "PENDING",
     "RESET_FAILURE",
     "RESET_IN_PROGRESS",
@@ -119,14 +117,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -137,14 +136,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -162,14 +162,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -182,24 +183,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
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
@@ -260,15 +263,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -340,17 +342,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -395,14 +399,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -440,19 +445,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/literals.pyi` & `mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -135,14 +136,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -160,14 +162,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -180,24 +183,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
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
@@ -258,15 +263,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -338,17 +342,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -393,14 +399,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -438,19 +445,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/paginator.py` & `mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -35,176 +35,166 @@
 """
 
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    DescribeBudgetActionHistoriesResponsePaginatorTypeDef,
-    DescribeBudgetActionsForAccountResponsePaginatorTypeDef,
-    DescribeBudgetActionsForBudgetResponsePaginatorTypeDef,
+    DescribeBudgetActionHistoriesResponseTypeDef,
+    DescribeBudgetActionsForAccountResponseTypeDef,
+    DescribeBudgetActionsForBudgetResponseTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
-    DescribeBudgetsResponsePaginatorTypeDef,
+    DescribeBudgetsResponseTypeDef,
     DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
     NotificationTypeDef,
     PaginatorConfigTypeDef,
-    TimePeriodTypeDef,
+    TimePeriodUnionTypeDef,
 )
 
 __all__ = (
     "DescribeBudgetActionHistoriesPaginator",
     "DescribeBudgetActionsForAccountPaginator",
     "DescribeBudgetActionsForBudgetPaginator",
     "DescribeBudgetNotificationsForAccountPaginator",
     "DescribeBudgetPerformanceHistoryPaginator",
     "DescribeBudgetsPaginator",
     "DescribeNotificationsForBudgetPaginator",
     "DescribeSubscribersForNotificationPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribeBudgetActionHistoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionHistories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionhistoriespaginator)
     """
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
-        TimePeriod: TimePeriodTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[DescribeBudgetActionHistoriesResponsePaginatorTypeDef]:
+        TimePeriod: TimePeriodUnionTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[DescribeBudgetActionHistoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionHistories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionhistoriespaginator)
         """
 
-
 class DescribeBudgetActionsForAccountPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForAccount)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionsforaccountpaginator)
     """
 
     def paginate(
         self, *, AccountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[DescribeBudgetActionsForAccountResponsePaginatorTypeDef]:
+    ) -> _PageIterator[DescribeBudgetActionsForAccountResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForAccount.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionsforaccountpaginator)
         """
 
-
 class DescribeBudgetActionsForBudgetPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForBudget)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionsforbudgetpaginator)
     """
 
     def paginate(
         self, *, AccountId: str, BudgetName: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[DescribeBudgetActionsForBudgetResponsePaginatorTypeDef]:
+    ) -> _PageIterator[DescribeBudgetActionsForBudgetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForBudget.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionsforbudgetpaginator)
         """
 
-
 class DescribeBudgetNotificationsForAccountPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetNotificationsForAccount)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetnotificationsforaccountpaginator)
     """
 
     def paginate(
         self, *, AccountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeBudgetNotificationsForAccountResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetNotificationsForAccount.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetnotificationsforaccountpaginator)
         """
 
-
 class DescribeBudgetPerformanceHistoryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetPerformanceHistory)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetperformancehistorypaginator)
     """
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
-        TimePeriod: TimePeriodTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        TimePeriod: TimePeriodUnionTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeBudgetPerformanceHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetPerformanceHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetperformancehistorypaginator)
         """
 
-
 class DescribeBudgetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetspaginator)
     """
 
     def paginate(
         self, *, AccountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[DescribeBudgetsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[DescribeBudgetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetspaginator)
         """
 
-
 class DescribeNotificationsForBudgetPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeNotificationsForBudget)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describenotificationsforbudgetpaginator)
     """
 
     def paginate(
         self, *, AccountId: str, BudgetName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeNotificationsForBudgetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeNotificationsForBudget.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describenotificationsforbudgetpaginator)
         """
 
-
 class DescribeSubscribersForNotificationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeSubscribersForNotification)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describesubscribersfornotificationpaginator)
     """
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeSubscribersForNotificationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeSubscribersForNotification.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describesubscribersfornotificationpaginator)
         """
```

### Comparing `mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/paginator.pyi` & `mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,25 +35,25 @@
 """
 
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    DescribeBudgetActionHistoriesResponsePaginatorTypeDef,
-    DescribeBudgetActionsForAccountResponsePaginatorTypeDef,
-    DescribeBudgetActionsForBudgetResponsePaginatorTypeDef,
+    DescribeBudgetActionHistoriesResponseTypeDef,
+    DescribeBudgetActionsForAccountResponseTypeDef,
+    DescribeBudgetActionsForBudgetResponseTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
-    DescribeBudgetsResponsePaginatorTypeDef,
+    DescribeBudgetsResponseTypeDef,
     DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
     NotificationTypeDef,
     PaginatorConfigTypeDef,
-    TimePeriodTypeDef,
+    TimePeriodUnionTypeDef,
 )
 
 __all__ = (
     "DescribeBudgetActionHistoriesPaginator",
     "DescribeBudgetActionsForAccountPaginator",
     "DescribeBudgetActionsForBudgetPaginator",
     "DescribeBudgetNotificationsForAccountPaginator",
@@ -61,140 +61,149 @@
     "DescribeBudgetsPaginator",
     "DescribeNotificationsForBudgetPaginator",
     "DescribeSubscribersForNotificationPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeBudgetActionHistoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionHistories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionhistoriespaginator)
     """
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
-        TimePeriod: TimePeriodTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[DescribeBudgetActionHistoriesResponsePaginatorTypeDef]:
+        TimePeriod: TimePeriodUnionTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[DescribeBudgetActionHistoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionHistories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionhistoriespaginator)
         """
 
+
 class DescribeBudgetActionsForAccountPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForAccount)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionsforaccountpaginator)
     """
 
     def paginate(
         self, *, AccountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[DescribeBudgetActionsForAccountResponsePaginatorTypeDef]:
+    ) -> _PageIterator[DescribeBudgetActionsForAccountResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForAccount.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionsforaccountpaginator)
         """
 
+
 class DescribeBudgetActionsForBudgetPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForBudget)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionsforbudgetpaginator)
     """
 
     def paginate(
         self, *, AccountId: str, BudgetName: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[DescribeBudgetActionsForBudgetResponsePaginatorTypeDef]:
+    ) -> _PageIterator[DescribeBudgetActionsForBudgetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionsForBudget.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionsforbudgetpaginator)
         """
 
+
 class DescribeBudgetNotificationsForAccountPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetNotificationsForAccount)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetnotificationsforaccountpaginator)
     """
 
     def paginate(
         self, *, AccountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeBudgetNotificationsForAccountResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetNotificationsForAccount.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetnotificationsforaccountpaginator)
         """
 
+
 class DescribeBudgetPerformanceHistoryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetPerformanceHistory)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetperformancehistorypaginator)
     """
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
-        TimePeriod: TimePeriodTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        TimePeriod: TimePeriodUnionTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeBudgetPerformanceHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetPerformanceHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetperformancehistorypaginator)
         """
 
+
 class DescribeBudgetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetspaginator)
     """
 
     def paginate(
         self, *, AccountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[DescribeBudgetsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[DescribeBudgetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetspaginator)
         """
 
+
 class DescribeNotificationsForBudgetPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeNotificationsForBudget)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describenotificationsforbudgetpaginator)
     """
 
     def paginate(
         self, *, AccountId: str, BudgetName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeNotificationsForBudgetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeNotificationsForBudget.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describenotificationsforbudgetpaginator)
         """
 
+
 class DescribeSubscribersForNotificationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeSubscribersForNotification)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describesubscribersfornotificationpaginator)
     """
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeSubscribersForNotificationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeSubscribersForNotification.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describesubscribersfornotificationpaginator)
         """
```

### Comparing `mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/type_defs.py` & `mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/type_defs.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,97 +38,105 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActionThresholdTypeDef",
     "SubscriberTypeDef",
     "HistoricalOptionsTypeDef",
     "TimestampTypeDef",
-    "NotificationTypeDef",
     "CostTypesTypeDef",
     "SpendTypeDef",
+    "TimePeriodExtraOutputTypeDef",
+    "NotificationTypeDef",
+    "TimePeriodOutputTypeDef",
+    "ResourceTagTypeDef",
     "ResponseMetadataTypeDef",
-    "IamActionDefinitionPaginatorTypeDef",
-    "ScpActionDefinitionPaginatorTypeDef",
-    "SsmActionDefinitionPaginatorTypeDef",
+    "IamActionDefinitionExtraOutputTypeDef",
+    "ScpActionDefinitionExtraOutputTypeDef",
+    "SsmActionDefinitionExtraOutputTypeDef",
+    "IamActionDefinitionOutputTypeDef",
+    "ScpActionDefinitionOutputTypeDef",
+    "SsmActionDefinitionOutputTypeDef",
     "IamActionDefinitionTypeDef",
     "ScpActionDefinitionTypeDef",
     "SsmActionDefinitionTypeDef",
     "DeleteBudgetActionRequestRequestTypeDef",
     "DeleteBudgetRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeBudgetActionRequestRequestTypeDef",
     "DescribeBudgetActionsForAccountRequestRequestTypeDef",
     "DescribeBudgetActionsForBudgetRequestRequestTypeDef",
     "DescribeBudgetNotificationsForAccountRequestRequestTypeDef",
     "DescribeBudgetRequestRequestTypeDef",
     "DescribeBudgetsRequestRequestTypeDef",
     "DescribeNotificationsForBudgetRequestRequestTypeDef",
     "ExecuteBudgetActionRequestRequestTypeDef",
-    "AutoAdjustDataPaginatorTypeDef",
+    "ListTagsForResourceRequestRequestTypeDef",
+    "UntagResourceRequestRequestTypeDef",
+    "AutoAdjustDataExtraOutputTypeDef",
+    "AutoAdjustDataOutputTypeDef",
     "AutoAdjustDataTypeDef",
     "TimePeriodTypeDef",
+    "CalculatedSpendTypeDef",
     "BudgetNotificationsForAccountTypeDef",
     "CreateNotificationRequestRequestTypeDef",
     "CreateSubscriberRequestRequestTypeDef",
     "DeleteNotificationRequestRequestTypeDef",
     "DeleteSubscriberRequestRequestTypeDef",
     "DescribeSubscribersForNotificationRequestRequestTypeDef",
     "NotificationWithSubscribersTypeDef",
     "UpdateNotificationRequestRequestTypeDef",
     "UpdateSubscriberRequestRequestTypeDef",
-    "CalculatedSpendTypeDef",
+    "BudgetedAndActualAmountsTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateBudgetActionResponseTypeDef",
     "DescribeNotificationsForBudgetResponseTypeDef",
     "DescribeSubscribersForNotificationResponseTypeDef",
     "ExecuteBudgetActionResponseTypeDef",
-    "DefinitionPaginatorTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "DefinitionExtraOutputTypeDef",
+    "DefinitionOutputTypeDef",
     "DefinitionTypeDef",
     "DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
     "DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
     "DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
     "DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
     "DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
     "DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
-    "BudgetedAndActualAmountsTypeDef",
     "DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
     "DescribeBudgetActionHistoriesRequestRequestTypeDef",
     "DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
     "DescribeBudgetPerformanceHistoryRequestRequestTypeDef",
-    "DescribeBudgetNotificationsForAccountResponseTypeDef",
-    "BudgetPaginatorTypeDef",
+    "TimePeriodUnionTypeDef",
+    "BudgetExtraOutputTypeDef",
+    "BudgetOutputTypeDef",
     "BudgetTypeDef",
-    "ActionPaginatorTypeDef",
+    "DescribeBudgetNotificationsForAccountResponseTypeDef",
+    "BudgetPerformanceHistoryTypeDef",
     "ActionTypeDef",
     "CreateBudgetActionRequestRequestTypeDef",
+    "DefinitionUnionTypeDef",
     "UpdateBudgetActionRequestRequestTypeDef",
-    "BudgetPerformanceHistoryTypeDef",
-    "DescribeBudgetsResponsePaginatorTypeDef",
-    "CreateBudgetRequestRequestTypeDef",
-    "DescribeBudgetResponseTypeDef",
     "DescribeBudgetsResponseTypeDef",
+    "DescribeBudgetResponseTypeDef",
+    "BudgetUnionTypeDef",
+    "CreateBudgetRequestRequestTypeDef",
     "UpdateBudgetRequestRequestTypeDef",
-    "ActionHistoryDetailsPaginatorTypeDef",
-    "DescribeBudgetActionsForAccountResponsePaginatorTypeDef",
-    "DescribeBudgetActionsForBudgetResponsePaginatorTypeDef",
+    "DescribeBudgetPerformanceHistoryResponseTypeDef",
     "ActionHistoryDetailsTypeDef",
     "DeleteBudgetActionResponseTypeDef",
     "DescribeBudgetActionResponseTypeDef",
     "DescribeBudgetActionsForAccountResponseTypeDef",
     "DescribeBudgetActionsForBudgetResponseTypeDef",
     "UpdateBudgetActionResponseTypeDef",
-    "DescribeBudgetPerformanceHistoryResponseTypeDef",
-    "ActionHistoryPaginatorTypeDef",
     "ActionHistoryTypeDef",
-    "DescribeBudgetActionHistoriesResponsePaginatorTypeDef",
     "DescribeBudgetActionHistoriesResponseTypeDef",
 )
 
 ActionThresholdTypeDef = TypedDict(
     "ActionThresholdTypeDef",
     {
         "ActionThresholdValue": float,
@@ -146,24 +154,14 @@
     "HistoricalOptionsTypeDef",
     {
         "BudgetAdjustmentPeriod": int,
         "LookBackAvailablePeriods": NotRequired[int],
     },
 )
 TimestampTypeDef = Union[datetime, str]
-NotificationTypeDef = TypedDict(
-    "NotificationTypeDef",
-    {
-        "NotificationType": NotificationTypeType,
-        "ComparisonOperator": ComparisonOperatorType,
-        "Threshold": float,
-        "ThresholdType": NotRequired[ThresholdTypeType],
-        "NotificationState": NotRequired[NotificationStateType],
-    },
-)
 CostTypesTypeDef = TypedDict(
     "CostTypesTypeDef",
     {
         "IncludeTax": NotRequired[bool],
         "IncludeSubscription": NotRequired[bool],
         "UseBlended": NotRequired[bool],
         "IncludeRefund": NotRequired[bool],
@@ -179,42 +177,97 @@
 SpendTypeDef = TypedDict(
     "SpendTypeDef",
     {
         "Amount": str,
         "Unit": str,
     },
 )
+TimePeriodExtraOutputTypeDef = TypedDict(
+    "TimePeriodExtraOutputTypeDef",
+    {
+        "Start": NotRequired[datetime],
+        "End": NotRequired[datetime],
+    },
+)
+NotificationTypeDef = TypedDict(
+    "NotificationTypeDef",
+    {
+        "NotificationType": NotificationTypeType,
+        "ComparisonOperator": ComparisonOperatorType,
+        "Threshold": float,
+        "ThresholdType": NotRequired[ThresholdTypeType],
+        "NotificationState": NotRequired[NotificationStateType],
+    },
+)
+TimePeriodOutputTypeDef = TypedDict(
+    "TimePeriodOutputTypeDef",
+    {
+        "Start": NotRequired[datetime],
+        "End": NotRequired[datetime],
+    },
+)
+ResourceTagTypeDef = TypedDict(
+    "ResourceTagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
-IamActionDefinitionPaginatorTypeDef = TypedDict(
-    "IamActionDefinitionPaginatorTypeDef",
+IamActionDefinitionExtraOutputTypeDef = TypedDict(
+    "IamActionDefinitionExtraOutputTypeDef",
     {
         "PolicyArn": str,
         "Roles": NotRequired[List[str]],
         "Groups": NotRequired[List[str]],
         "Users": NotRequired[List[str]],
     },
 )
-ScpActionDefinitionPaginatorTypeDef = TypedDict(
-    "ScpActionDefinitionPaginatorTypeDef",
+ScpActionDefinitionExtraOutputTypeDef = TypedDict(
+    "ScpActionDefinitionExtraOutputTypeDef",
     {
         "PolicyId": str,
         "TargetIds": List[str],
     },
 )
-SsmActionDefinitionPaginatorTypeDef = TypedDict(
-    "SsmActionDefinitionPaginatorTypeDef",
+SsmActionDefinitionExtraOutputTypeDef = TypedDict(
+    "SsmActionDefinitionExtraOutputTypeDef",
+    {
+        "ActionSubType": ActionSubTypeType,
+        "Region": str,
+        "InstanceIds": List[str],
+    },
+)
+IamActionDefinitionOutputTypeDef = TypedDict(
+    "IamActionDefinitionOutputTypeDef",
+    {
+        "PolicyArn": str,
+        "Roles": NotRequired[List[str]],
+        "Groups": NotRequired[List[str]],
+        "Users": NotRequired[List[str]],
+    },
+)
+ScpActionDefinitionOutputTypeDef = TypedDict(
+    "ScpActionDefinitionOutputTypeDef",
+    {
+        "PolicyId": str,
+        "TargetIds": List[str],
+    },
+)
+SsmActionDefinitionOutputTypeDef = TypedDict(
+    "SsmActionDefinitionOutputTypeDef",
     {
         "ActionSubType": ActionSubTypeType,
         "Region": str,
         "InstanceIds": List[str],
     },
 )
 IamActionDefinitionTypeDef = TypedDict(
@@ -326,16 +379,37 @@
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
         "ExecutionType": ExecutionTypeType,
     },
 )
-AutoAdjustDataPaginatorTypeDef = TypedDict(
-    "AutoAdjustDataPaginatorTypeDef",
+ListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "ListTagsForResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "ResourceTagKeys": Sequence[str],
+    },
+)
+AutoAdjustDataExtraOutputTypeDef = TypedDict(
+    "AutoAdjustDataExtraOutputTypeDef",
+    {
+        "AutoAdjustType": AutoAdjustTypeType,
+        "HistoricalOptions": NotRequired[HistoricalOptionsTypeDef],
+        "LastAutoAdjustTime": NotRequired[datetime],
+    },
+)
+AutoAdjustDataOutputTypeDef = TypedDict(
+    "AutoAdjustDataOutputTypeDef",
     {
         "AutoAdjustType": AutoAdjustTypeType,
         "HistoricalOptions": NotRequired[HistoricalOptionsTypeDef],
         "LastAutoAdjustTime": NotRequired[datetime],
     },
 )
 AutoAdjustDataTypeDef = TypedDict(
@@ -349,14 +423,21 @@
 TimePeriodTypeDef = TypedDict(
     "TimePeriodTypeDef",
     {
         "Start": NotRequired[TimestampTypeDef],
         "End": NotRequired[TimestampTypeDef],
     },
 )
+CalculatedSpendTypeDef = TypedDict(
+    "CalculatedSpendTypeDef",
+    {
+        "ActualSpend": SpendTypeDef,
+        "ForecastedSpend": NotRequired[SpendTypeDef],
+    },
+)
 BudgetNotificationsForAccountTypeDef = TypedDict(
     "BudgetNotificationsForAccountTypeDef",
     {
         "Notifications": NotRequired[List[NotificationTypeDef]],
         "BudgetName": NotRequired[str],
     },
 )
@@ -427,19 +508,27 @@
         "AccountId": str,
         "BudgetName": str,
         "Notification": NotificationTypeDef,
         "OldSubscriber": SubscriberTypeDef,
         "NewSubscriber": SubscriberTypeDef,
     },
 )
-CalculatedSpendTypeDef = TypedDict(
-    "CalculatedSpendTypeDef",
+BudgetedAndActualAmountsTypeDef = TypedDict(
+    "BudgetedAndActualAmountsTypeDef",
     {
-        "ActualSpend": SpendTypeDef,
-        "ForecastedSpend": NotRequired[SpendTypeDef],
+        "BudgetedAmount": NotRequired[SpendTypeDef],
+        "ActualAmount": NotRequired[SpendTypeDef],
+        "TimePeriod": NotRequired[TimePeriodOutputTypeDef],
+    },
+)
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "ResourceTags": Sequence[ResourceTagTypeDef],
     },
 )
 CreateBudgetActionResponseTypeDef = TypedDict(
     "CreateBudgetActionResponseTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
@@ -447,42 +536,57 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeNotificationsForBudgetResponseTypeDef = TypedDict(
     "DescribeNotificationsForBudgetResponseTypeDef",
     {
         "Notifications": List[NotificationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeSubscribersForNotificationResponseTypeDef = TypedDict(
     "DescribeSubscribersForNotificationResponseTypeDef",
     {
         "Subscribers": List[SubscriberTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ExecuteBudgetActionResponseTypeDef = TypedDict(
     "ExecuteBudgetActionResponseTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
         "ExecutionType": ExecutionTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-DefinitionPaginatorTypeDef = TypedDict(
-    "DefinitionPaginatorTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "IamActionDefinition": NotRequired[IamActionDefinitionPaginatorTypeDef],
-        "ScpActionDefinition": NotRequired[ScpActionDefinitionPaginatorTypeDef],
-        "SsmActionDefinition": NotRequired[SsmActionDefinitionPaginatorTypeDef],
+        "ResourceTags": List[ResourceTagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DefinitionExtraOutputTypeDef = TypedDict(
+    "DefinitionExtraOutputTypeDef",
+    {
+        "IamActionDefinition": NotRequired[IamActionDefinitionExtraOutputTypeDef],
+        "ScpActionDefinition": NotRequired[ScpActionDefinitionExtraOutputTypeDef],
+        "SsmActionDefinition": NotRequired[SsmActionDefinitionExtraOutputTypeDef],
+    },
+)
+DefinitionOutputTypeDef = TypedDict(
+    "DefinitionOutputTypeDef",
+    {
+        "IamActionDefinition": NotRequired[IamActionDefinitionOutputTypeDef],
+        "ScpActionDefinition": NotRequired[ScpActionDefinitionOutputTypeDef],
+        "SsmActionDefinition": NotRequired[SsmActionDefinitionOutputTypeDef],
     },
 )
 DefinitionTypeDef = TypedDict(
     "DefinitionTypeDef",
     {
         "IamActionDefinition": NotRequired[IamActionDefinitionTypeDef],
         "ScpActionDefinition": NotRequired[ScpActionDefinitionTypeDef],
@@ -531,22 +635,14 @@
     {
         "AccountId": str,
         "BudgetName": str,
         "Notification": NotificationTypeDef,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
-BudgetedAndActualAmountsTypeDef = TypedDict(
-    "BudgetedAndActualAmountsTypeDef",
-    {
-        "BudgetedAmount": NotRequired[SpendTypeDef],
-        "ActualAmount": NotRequired[SpendTypeDef],
-        "TimePeriod": NotRequired[TimePeriodTypeDef],
-    },
-)
 DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef = TypedDict(
     "DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
         "TimePeriod": NotRequired[TimePeriodTypeDef],
@@ -579,36 +675,45 @@
         "AccountId": str,
         "BudgetName": str,
         "TimePeriod": NotRequired[TimePeriodTypeDef],
         "MaxResults": NotRequired[int],
         "NextToken": NotRequired[str],
     },
 )
-DescribeBudgetNotificationsForAccountResponseTypeDef = TypedDict(
-    "DescribeBudgetNotificationsForAccountResponseTypeDef",
+TimePeriodUnionTypeDef = Union[TimePeriodTypeDef, TimePeriodExtraOutputTypeDef]
+BudgetExtraOutputTypeDef = TypedDict(
+    "BudgetExtraOutputTypeDef",
     {
-        "BudgetNotificationsForAccount": List[BudgetNotificationsForAccountTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "BudgetName": str,
+        "TimeUnit": TimeUnitType,
+        "BudgetType": BudgetTypeType,
+        "BudgetLimit": NotRequired[SpendTypeDef],
+        "PlannedBudgetLimits": NotRequired[Dict[str, SpendTypeDef]],
+        "CostFilters": NotRequired[Dict[str, List[str]]],
+        "CostTypes": NotRequired[CostTypesTypeDef],
+        "TimePeriod": NotRequired[TimePeriodExtraOutputTypeDef],
+        "CalculatedSpend": NotRequired[CalculatedSpendTypeDef],
+        "LastUpdatedTime": NotRequired[datetime],
+        "AutoAdjustData": NotRequired[AutoAdjustDataExtraOutputTypeDef],
     },
 )
-BudgetPaginatorTypeDef = TypedDict(
-    "BudgetPaginatorTypeDef",
+BudgetOutputTypeDef = TypedDict(
+    "BudgetOutputTypeDef",
     {
         "BudgetName": str,
         "TimeUnit": TimeUnitType,
         "BudgetType": BudgetTypeType,
         "BudgetLimit": NotRequired[SpendTypeDef],
         "PlannedBudgetLimits": NotRequired[Dict[str, SpendTypeDef]],
         "CostFilters": NotRequired[Dict[str, List[str]]],
         "CostTypes": NotRequired[CostTypesTypeDef],
-        "TimePeriod": NotRequired[TimePeriodTypeDef],
+        "TimePeriod": NotRequired[TimePeriodOutputTypeDef],
         "CalculatedSpend": NotRequired[CalculatedSpendTypeDef],
         "LastUpdatedTime": NotRequired[datetime],
-        "AutoAdjustData": NotRequired[AutoAdjustDataPaginatorTypeDef],
+        "AutoAdjustData": NotRequired[AutoAdjustDataOutputTypeDef],
     },
 )
 BudgetTypeDef = TypedDict(
     "BudgetTypeDef",
     {
         "BudgetName": str,
         "TimeUnit": TimeUnitType,
@@ -619,38 +724,42 @@
         "CostTypes": NotRequired[CostTypesTypeDef],
         "TimePeriod": NotRequired[TimePeriodTypeDef],
         "CalculatedSpend": NotRequired[CalculatedSpendTypeDef],
         "LastUpdatedTime": NotRequired[TimestampTypeDef],
         "AutoAdjustData": NotRequired[AutoAdjustDataTypeDef],
     },
 )
-ActionPaginatorTypeDef = TypedDict(
-    "ActionPaginatorTypeDef",
+DescribeBudgetNotificationsForAccountResponseTypeDef = TypedDict(
+    "DescribeBudgetNotificationsForAccountResponseTypeDef",
     {
-        "ActionId": str,
-        "BudgetName": str,
-        "NotificationType": NotificationTypeType,
-        "ActionType": ActionTypeType,
-        "ActionThreshold": ActionThresholdTypeDef,
-        "Definition": DefinitionPaginatorTypeDef,
-        "ExecutionRoleArn": str,
-        "ApprovalModel": ApprovalModelType,
-        "Status": ActionStatusType,
-        "Subscribers": List[SubscriberTypeDef],
+        "BudgetNotificationsForAccount": List[BudgetNotificationsForAccountTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+BudgetPerformanceHistoryTypeDef = TypedDict(
+    "BudgetPerformanceHistoryTypeDef",
+    {
+        "BudgetName": NotRequired[str],
+        "BudgetType": NotRequired[BudgetTypeType],
+        "CostFilters": NotRequired[Dict[str, List[str]]],
+        "CostTypes": NotRequired[CostTypesTypeDef],
+        "TimeUnit": NotRequired[TimeUnitType],
+        "BudgetedAndActualAmountsList": NotRequired[List[BudgetedAndActualAmountsTypeDef]],
     },
 )
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "ActionId": str,
         "BudgetName": str,
         "NotificationType": NotificationTypeType,
         "ActionType": ActionTypeType,
         "ActionThreshold": ActionThresholdTypeDef,
-        "Definition": DefinitionTypeDef,
+        "Definition": DefinitionOutputTypeDef,
         "ExecutionRoleArn": str,
         "ApprovalModel": ApprovalModelType,
         "Status": ActionStatusType,
         "Subscribers": List[SubscriberTypeDef],
     },
 )
 CreateBudgetActionRequestRequestTypeDef = TypedDict(
@@ -661,100 +770,70 @@
         "NotificationType": NotificationTypeType,
         "ActionType": ActionTypeType,
         "ActionThreshold": ActionThresholdTypeDef,
         "Definition": DefinitionTypeDef,
         "ExecutionRoleArn": str,
         "ApprovalModel": ApprovalModelType,
         "Subscribers": Sequence[SubscriberTypeDef],
+        "ResourceTags": NotRequired[Sequence[ResourceTagTypeDef]],
     },
 )
+DefinitionUnionTypeDef = Union[DefinitionTypeDef, DefinitionExtraOutputTypeDef]
 UpdateBudgetActionRequestRequestTypeDef = TypedDict(
     "UpdateBudgetActionRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
         "NotificationType": NotRequired[NotificationTypeType],
         "ActionThreshold": NotRequired[ActionThresholdTypeDef],
         "Definition": NotRequired[DefinitionTypeDef],
         "ExecutionRoleArn": NotRequired[str],
         "ApprovalModel": NotRequired[ApprovalModelType],
         "Subscribers": NotRequired[Sequence[SubscriberTypeDef]],
     },
 )
-BudgetPerformanceHistoryTypeDef = TypedDict(
-    "BudgetPerformanceHistoryTypeDef",
+DescribeBudgetsResponseTypeDef = TypedDict(
+    "DescribeBudgetsResponseTypeDef",
     {
-        "BudgetName": NotRequired[str],
-        "BudgetType": NotRequired[BudgetTypeType],
-        "CostFilters": NotRequired[Dict[str, List[str]]],
-        "CostTypes": NotRequired[CostTypesTypeDef],
-        "TimeUnit": NotRequired[TimeUnitType],
-        "BudgetedAndActualAmountsList": NotRequired[List[BudgetedAndActualAmountsTypeDef]],
+        "Budgets": List[BudgetExtraOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-DescribeBudgetsResponsePaginatorTypeDef = TypedDict(
-    "DescribeBudgetsResponsePaginatorTypeDef",
+DescribeBudgetResponseTypeDef = TypedDict(
+    "DescribeBudgetResponseTypeDef",
     {
-        "Budgets": List[BudgetPaginatorTypeDef],
-        "NextToken": str,
+        "Budget": BudgetOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+BudgetUnionTypeDef = Union[BudgetTypeDef, BudgetExtraOutputTypeDef]
 CreateBudgetRequestRequestTypeDef = TypedDict(
     "CreateBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "Budget": BudgetTypeDef,
         "NotificationsWithSubscribers": NotRequired[Sequence[NotificationWithSubscribersTypeDef]],
-    },
-)
-DescribeBudgetResponseTypeDef = TypedDict(
-    "DescribeBudgetResponseTypeDef",
-    {
-        "Budget": BudgetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeBudgetsResponseTypeDef = TypedDict(
-    "DescribeBudgetsResponseTypeDef",
-    {
-        "Budgets": List[BudgetTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceTags": NotRequired[Sequence[ResourceTagTypeDef]],
     },
 )
 UpdateBudgetRequestRequestTypeDef = TypedDict(
     "UpdateBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "NewBudget": BudgetTypeDef,
     },
 )
-ActionHistoryDetailsPaginatorTypeDef = TypedDict(
-    "ActionHistoryDetailsPaginatorTypeDef",
-    {
-        "Message": str,
-        "Action": ActionPaginatorTypeDef,
-    },
-)
-DescribeBudgetActionsForAccountResponsePaginatorTypeDef = TypedDict(
-    "DescribeBudgetActionsForAccountResponsePaginatorTypeDef",
-    {
-        "Actions": List[ActionPaginatorTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeBudgetActionsForBudgetResponsePaginatorTypeDef = TypedDict(
-    "DescribeBudgetActionsForBudgetResponsePaginatorTypeDef",
+DescribeBudgetPerformanceHistoryResponseTypeDef = TypedDict(
+    "DescribeBudgetPerformanceHistoryResponseTypeDef",
     {
-        "Actions": List[ActionPaginatorTypeDef],
-        "NextToken": str,
+        "BudgetPerformanceHistory": BudgetPerformanceHistoryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ActionHistoryDetailsTypeDef = TypedDict(
     "ActionHistoryDetailsTypeDef",
     {
         "Message": str,
         "Action": ActionTypeDef,
@@ -778,71 +857,46 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeBudgetActionsForAccountResponseTypeDef = TypedDict(
     "DescribeBudgetActionsForAccountResponseTypeDef",
     {
         "Actions": List[ActionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeBudgetActionsForBudgetResponseTypeDef = TypedDict(
     "DescribeBudgetActionsForBudgetResponseTypeDef",
     {
         "Actions": List[ActionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateBudgetActionResponseTypeDef = TypedDict(
     "UpdateBudgetActionResponseTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "OldAction": ActionTypeDef,
         "NewAction": ActionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-DescribeBudgetPerformanceHistoryResponseTypeDef = TypedDict(
-    "DescribeBudgetPerformanceHistoryResponseTypeDef",
-    {
-        "BudgetPerformanceHistory": BudgetPerformanceHistoryTypeDef,
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-ActionHistoryPaginatorTypeDef = TypedDict(
-    "ActionHistoryPaginatorTypeDef",
-    {
-        "Timestamp": datetime,
-        "Status": ActionStatusType,
-        "EventType": EventTypeType,
-        "ActionHistoryDetails": ActionHistoryDetailsPaginatorTypeDef,
-    },
-)
 ActionHistoryTypeDef = TypedDict(
     "ActionHistoryTypeDef",
     {
         "Timestamp": datetime,
         "Status": ActionStatusType,
         "EventType": EventTypeType,
         "ActionHistoryDetails": ActionHistoryDetailsTypeDef,
     },
 )
-DescribeBudgetActionHistoriesResponsePaginatorTypeDef = TypedDict(
-    "DescribeBudgetActionHistoriesResponsePaginatorTypeDef",
-    {
-        "ActionHistories": List[ActionHistoryPaginatorTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 DescribeBudgetActionHistoriesResponseTypeDef = TypedDict(
     "DescribeBudgetActionHistoriesResponseTypeDef",
     {
         "ActionHistories": List[ActionHistoryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
```

### Comparing `mypy-boto3-budgets-1.34.0/mypy_boto3_budgets/type_defs.pyi` & `mypy_boto3_budgets-1.34.100/mypy_boto3_budgets/type_defs.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -43,91 +43,100 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "ActionThresholdTypeDef",
     "SubscriberTypeDef",
     "HistoricalOptionsTypeDef",
     "TimestampTypeDef",
-    "NotificationTypeDef",
     "CostTypesTypeDef",
     "SpendTypeDef",
+    "TimePeriodExtraOutputTypeDef",
+    "NotificationTypeDef",
+    "TimePeriodOutputTypeDef",
+    "ResourceTagTypeDef",
     "ResponseMetadataTypeDef",
-    "IamActionDefinitionPaginatorTypeDef",
-    "ScpActionDefinitionPaginatorTypeDef",
-    "SsmActionDefinitionPaginatorTypeDef",
+    "IamActionDefinitionExtraOutputTypeDef",
+    "ScpActionDefinitionExtraOutputTypeDef",
+    "SsmActionDefinitionExtraOutputTypeDef",
+    "IamActionDefinitionOutputTypeDef",
+    "ScpActionDefinitionOutputTypeDef",
+    "SsmActionDefinitionOutputTypeDef",
     "IamActionDefinitionTypeDef",
     "ScpActionDefinitionTypeDef",
     "SsmActionDefinitionTypeDef",
     "DeleteBudgetActionRequestRequestTypeDef",
     "DeleteBudgetRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeBudgetActionRequestRequestTypeDef",
     "DescribeBudgetActionsForAccountRequestRequestTypeDef",
     "DescribeBudgetActionsForBudgetRequestRequestTypeDef",
     "DescribeBudgetNotificationsForAccountRequestRequestTypeDef",
     "DescribeBudgetRequestRequestTypeDef",
     "DescribeBudgetsRequestRequestTypeDef",
     "DescribeNotificationsForBudgetRequestRequestTypeDef",
     "ExecuteBudgetActionRequestRequestTypeDef",
-    "AutoAdjustDataPaginatorTypeDef",
+    "ListTagsForResourceRequestRequestTypeDef",
+    "UntagResourceRequestRequestTypeDef",
+    "AutoAdjustDataExtraOutputTypeDef",
+    "AutoAdjustDataOutputTypeDef",
     "AutoAdjustDataTypeDef",
     "TimePeriodTypeDef",
+    "CalculatedSpendTypeDef",
     "BudgetNotificationsForAccountTypeDef",
     "CreateNotificationRequestRequestTypeDef",
     "CreateSubscriberRequestRequestTypeDef",
     "DeleteNotificationRequestRequestTypeDef",
     "DeleteSubscriberRequestRequestTypeDef",
     "DescribeSubscribersForNotificationRequestRequestTypeDef",
     "NotificationWithSubscribersTypeDef",
     "UpdateNotificationRequestRequestTypeDef",
     "UpdateSubscriberRequestRequestTypeDef",
-    "CalculatedSpendTypeDef",
+    "BudgetedAndActualAmountsTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateBudgetActionResponseTypeDef",
     "DescribeNotificationsForBudgetResponseTypeDef",
     "DescribeSubscribersForNotificationResponseTypeDef",
     "ExecuteBudgetActionResponseTypeDef",
-    "DefinitionPaginatorTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "DefinitionExtraOutputTypeDef",
+    "DefinitionOutputTypeDef",
     "DefinitionTypeDef",
     "DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
     "DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
     "DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
     "DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
     "DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
     "DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
-    "BudgetedAndActualAmountsTypeDef",
     "DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
     "DescribeBudgetActionHistoriesRequestRequestTypeDef",
     "DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
     "DescribeBudgetPerformanceHistoryRequestRequestTypeDef",
-    "DescribeBudgetNotificationsForAccountResponseTypeDef",
-    "BudgetPaginatorTypeDef",
+    "TimePeriodUnionTypeDef",
+    "BudgetExtraOutputTypeDef",
+    "BudgetOutputTypeDef",
     "BudgetTypeDef",
-    "ActionPaginatorTypeDef",
+    "DescribeBudgetNotificationsForAccountResponseTypeDef",
+    "BudgetPerformanceHistoryTypeDef",
     "ActionTypeDef",
     "CreateBudgetActionRequestRequestTypeDef",
+    "DefinitionUnionTypeDef",
     "UpdateBudgetActionRequestRequestTypeDef",
-    "BudgetPerformanceHistoryTypeDef",
-    "DescribeBudgetsResponsePaginatorTypeDef",
-    "CreateBudgetRequestRequestTypeDef",
-    "DescribeBudgetResponseTypeDef",
     "DescribeBudgetsResponseTypeDef",
+    "DescribeBudgetResponseTypeDef",
+    "BudgetUnionTypeDef",
+    "CreateBudgetRequestRequestTypeDef",
     "UpdateBudgetRequestRequestTypeDef",
-    "ActionHistoryDetailsPaginatorTypeDef",
-    "DescribeBudgetActionsForAccountResponsePaginatorTypeDef",
-    "DescribeBudgetActionsForBudgetResponsePaginatorTypeDef",
+    "DescribeBudgetPerformanceHistoryResponseTypeDef",
     "ActionHistoryDetailsTypeDef",
     "DeleteBudgetActionResponseTypeDef",
     "DescribeBudgetActionResponseTypeDef",
     "DescribeBudgetActionsForAccountResponseTypeDef",
     "DescribeBudgetActionsForBudgetResponseTypeDef",
     "UpdateBudgetActionResponseTypeDef",
-    "DescribeBudgetPerformanceHistoryResponseTypeDef",
-    "ActionHistoryPaginatorTypeDef",
     "ActionHistoryTypeDef",
-    "DescribeBudgetActionHistoriesResponsePaginatorTypeDef",
     "DescribeBudgetActionHistoriesResponseTypeDef",
 )
 
 ActionThresholdTypeDef = TypedDict(
     "ActionThresholdTypeDef",
     {
         "ActionThresholdValue": float,
@@ -145,24 +154,14 @@
     "HistoricalOptionsTypeDef",
     {
         "BudgetAdjustmentPeriod": int,
         "LookBackAvailablePeriods": NotRequired[int],
     },
 )
 TimestampTypeDef = Union[datetime, str]
-NotificationTypeDef = TypedDict(
-    "NotificationTypeDef",
-    {
-        "NotificationType": NotificationTypeType,
-        "ComparisonOperator": ComparisonOperatorType,
-        "Threshold": float,
-        "ThresholdType": NotRequired[ThresholdTypeType],
-        "NotificationState": NotRequired[NotificationStateType],
-    },
-)
 CostTypesTypeDef = TypedDict(
     "CostTypesTypeDef",
     {
         "IncludeTax": NotRequired[bool],
         "IncludeSubscription": NotRequired[bool],
         "UseBlended": NotRequired[bool],
         "IncludeRefund": NotRequired[bool],
@@ -178,42 +177,97 @@
 SpendTypeDef = TypedDict(
     "SpendTypeDef",
     {
         "Amount": str,
         "Unit": str,
     },
 )
+TimePeriodExtraOutputTypeDef = TypedDict(
+    "TimePeriodExtraOutputTypeDef",
+    {
+        "Start": NotRequired[datetime],
+        "End": NotRequired[datetime],
+    },
+)
+NotificationTypeDef = TypedDict(
+    "NotificationTypeDef",
+    {
+        "NotificationType": NotificationTypeType,
+        "ComparisonOperator": ComparisonOperatorType,
+        "Threshold": float,
+        "ThresholdType": NotRequired[ThresholdTypeType],
+        "NotificationState": NotRequired[NotificationStateType],
+    },
+)
+TimePeriodOutputTypeDef = TypedDict(
+    "TimePeriodOutputTypeDef",
+    {
+        "Start": NotRequired[datetime],
+        "End": NotRequired[datetime],
+    },
+)
+ResourceTagTypeDef = TypedDict(
+    "ResourceTagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
-IamActionDefinitionPaginatorTypeDef = TypedDict(
-    "IamActionDefinitionPaginatorTypeDef",
+IamActionDefinitionExtraOutputTypeDef = TypedDict(
+    "IamActionDefinitionExtraOutputTypeDef",
     {
         "PolicyArn": str,
         "Roles": NotRequired[List[str]],
         "Groups": NotRequired[List[str]],
         "Users": NotRequired[List[str]],
     },
 )
-ScpActionDefinitionPaginatorTypeDef = TypedDict(
-    "ScpActionDefinitionPaginatorTypeDef",
+ScpActionDefinitionExtraOutputTypeDef = TypedDict(
+    "ScpActionDefinitionExtraOutputTypeDef",
     {
         "PolicyId": str,
         "TargetIds": List[str],
     },
 )
-SsmActionDefinitionPaginatorTypeDef = TypedDict(
-    "SsmActionDefinitionPaginatorTypeDef",
+SsmActionDefinitionExtraOutputTypeDef = TypedDict(
+    "SsmActionDefinitionExtraOutputTypeDef",
+    {
+        "ActionSubType": ActionSubTypeType,
+        "Region": str,
+        "InstanceIds": List[str],
+    },
+)
+IamActionDefinitionOutputTypeDef = TypedDict(
+    "IamActionDefinitionOutputTypeDef",
+    {
+        "PolicyArn": str,
+        "Roles": NotRequired[List[str]],
+        "Groups": NotRequired[List[str]],
+        "Users": NotRequired[List[str]],
+    },
+)
+ScpActionDefinitionOutputTypeDef = TypedDict(
+    "ScpActionDefinitionOutputTypeDef",
+    {
+        "PolicyId": str,
+        "TargetIds": List[str],
+    },
+)
+SsmActionDefinitionOutputTypeDef = TypedDict(
+    "SsmActionDefinitionOutputTypeDef",
     {
         "ActionSubType": ActionSubTypeType,
         "Region": str,
         "InstanceIds": List[str],
     },
 )
 IamActionDefinitionTypeDef = TypedDict(
@@ -325,16 +379,37 @@
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
         "ExecutionType": ExecutionTypeType,
     },
 )
-AutoAdjustDataPaginatorTypeDef = TypedDict(
-    "AutoAdjustDataPaginatorTypeDef",
+ListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "ListTagsForResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "ResourceTagKeys": Sequence[str],
+    },
+)
+AutoAdjustDataExtraOutputTypeDef = TypedDict(
+    "AutoAdjustDataExtraOutputTypeDef",
+    {
+        "AutoAdjustType": AutoAdjustTypeType,
+        "HistoricalOptions": NotRequired[HistoricalOptionsTypeDef],
+        "LastAutoAdjustTime": NotRequired[datetime],
+    },
+)
+AutoAdjustDataOutputTypeDef = TypedDict(
+    "AutoAdjustDataOutputTypeDef",
     {
         "AutoAdjustType": AutoAdjustTypeType,
         "HistoricalOptions": NotRequired[HistoricalOptionsTypeDef],
         "LastAutoAdjustTime": NotRequired[datetime],
     },
 )
 AutoAdjustDataTypeDef = TypedDict(
@@ -348,14 +423,21 @@
 TimePeriodTypeDef = TypedDict(
     "TimePeriodTypeDef",
     {
         "Start": NotRequired[TimestampTypeDef],
         "End": NotRequired[TimestampTypeDef],
     },
 )
+CalculatedSpendTypeDef = TypedDict(
+    "CalculatedSpendTypeDef",
+    {
+        "ActualSpend": SpendTypeDef,
+        "ForecastedSpend": NotRequired[SpendTypeDef],
+    },
+)
 BudgetNotificationsForAccountTypeDef = TypedDict(
     "BudgetNotificationsForAccountTypeDef",
     {
         "Notifications": NotRequired[List[NotificationTypeDef]],
         "BudgetName": NotRequired[str],
     },
 )
@@ -426,19 +508,27 @@
         "AccountId": str,
         "BudgetName": str,
         "Notification": NotificationTypeDef,
         "OldSubscriber": SubscriberTypeDef,
         "NewSubscriber": SubscriberTypeDef,
     },
 )
-CalculatedSpendTypeDef = TypedDict(
-    "CalculatedSpendTypeDef",
+BudgetedAndActualAmountsTypeDef = TypedDict(
+    "BudgetedAndActualAmountsTypeDef",
     {
-        "ActualSpend": SpendTypeDef,
-        "ForecastedSpend": NotRequired[SpendTypeDef],
+        "BudgetedAmount": NotRequired[SpendTypeDef],
+        "ActualAmount": NotRequired[SpendTypeDef],
+        "TimePeriod": NotRequired[TimePeriodOutputTypeDef],
+    },
+)
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "ResourceTags": Sequence[ResourceTagTypeDef],
     },
 )
 CreateBudgetActionResponseTypeDef = TypedDict(
     "CreateBudgetActionResponseTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
@@ -446,42 +536,57 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeNotificationsForBudgetResponseTypeDef = TypedDict(
     "DescribeNotificationsForBudgetResponseTypeDef",
     {
         "Notifications": List[NotificationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeSubscribersForNotificationResponseTypeDef = TypedDict(
     "DescribeSubscribersForNotificationResponseTypeDef",
     {
         "Subscribers": List[SubscriberTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ExecuteBudgetActionResponseTypeDef = TypedDict(
     "ExecuteBudgetActionResponseTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
         "ExecutionType": ExecutionTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-DefinitionPaginatorTypeDef = TypedDict(
-    "DefinitionPaginatorTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceTags": List[ResourceTagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DefinitionExtraOutputTypeDef = TypedDict(
+    "DefinitionExtraOutputTypeDef",
     {
-        "IamActionDefinition": NotRequired[IamActionDefinitionPaginatorTypeDef],
-        "ScpActionDefinition": NotRequired[ScpActionDefinitionPaginatorTypeDef],
-        "SsmActionDefinition": NotRequired[SsmActionDefinitionPaginatorTypeDef],
+        "IamActionDefinition": NotRequired[IamActionDefinitionExtraOutputTypeDef],
+        "ScpActionDefinition": NotRequired[ScpActionDefinitionExtraOutputTypeDef],
+        "SsmActionDefinition": NotRequired[SsmActionDefinitionExtraOutputTypeDef],
+    },
+)
+DefinitionOutputTypeDef = TypedDict(
+    "DefinitionOutputTypeDef",
+    {
+        "IamActionDefinition": NotRequired[IamActionDefinitionOutputTypeDef],
+        "ScpActionDefinition": NotRequired[ScpActionDefinitionOutputTypeDef],
+        "SsmActionDefinition": NotRequired[SsmActionDefinitionOutputTypeDef],
     },
 )
 DefinitionTypeDef = TypedDict(
     "DefinitionTypeDef",
     {
         "IamActionDefinition": NotRequired[IamActionDefinitionTypeDef],
         "ScpActionDefinition": NotRequired[ScpActionDefinitionTypeDef],
@@ -530,22 +635,14 @@
     {
         "AccountId": str,
         "BudgetName": str,
         "Notification": NotificationTypeDef,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
-BudgetedAndActualAmountsTypeDef = TypedDict(
-    "BudgetedAndActualAmountsTypeDef",
-    {
-        "BudgetedAmount": NotRequired[SpendTypeDef],
-        "ActualAmount": NotRequired[SpendTypeDef],
-        "TimePeriod": NotRequired[TimePeriodTypeDef],
-    },
-)
 DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef = TypedDict(
     "DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
         "TimePeriod": NotRequired[TimePeriodTypeDef],
@@ -578,36 +675,45 @@
         "AccountId": str,
         "BudgetName": str,
         "TimePeriod": NotRequired[TimePeriodTypeDef],
         "MaxResults": NotRequired[int],
         "NextToken": NotRequired[str],
     },
 )
-DescribeBudgetNotificationsForAccountResponseTypeDef = TypedDict(
-    "DescribeBudgetNotificationsForAccountResponseTypeDef",
+TimePeriodUnionTypeDef = Union[TimePeriodTypeDef, TimePeriodExtraOutputTypeDef]
+BudgetExtraOutputTypeDef = TypedDict(
+    "BudgetExtraOutputTypeDef",
     {
-        "BudgetNotificationsForAccount": List[BudgetNotificationsForAccountTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "BudgetName": str,
+        "TimeUnit": TimeUnitType,
+        "BudgetType": BudgetTypeType,
+        "BudgetLimit": NotRequired[SpendTypeDef],
+        "PlannedBudgetLimits": NotRequired[Dict[str, SpendTypeDef]],
+        "CostFilters": NotRequired[Dict[str, List[str]]],
+        "CostTypes": NotRequired[CostTypesTypeDef],
+        "TimePeriod": NotRequired[TimePeriodExtraOutputTypeDef],
+        "CalculatedSpend": NotRequired[CalculatedSpendTypeDef],
+        "LastUpdatedTime": NotRequired[datetime],
+        "AutoAdjustData": NotRequired[AutoAdjustDataExtraOutputTypeDef],
     },
 )
-BudgetPaginatorTypeDef = TypedDict(
-    "BudgetPaginatorTypeDef",
+BudgetOutputTypeDef = TypedDict(
+    "BudgetOutputTypeDef",
     {
         "BudgetName": str,
         "TimeUnit": TimeUnitType,
         "BudgetType": BudgetTypeType,
         "BudgetLimit": NotRequired[SpendTypeDef],
         "PlannedBudgetLimits": NotRequired[Dict[str, SpendTypeDef]],
         "CostFilters": NotRequired[Dict[str, List[str]]],
         "CostTypes": NotRequired[CostTypesTypeDef],
-        "TimePeriod": NotRequired[TimePeriodTypeDef],
+        "TimePeriod": NotRequired[TimePeriodOutputTypeDef],
         "CalculatedSpend": NotRequired[CalculatedSpendTypeDef],
         "LastUpdatedTime": NotRequired[datetime],
-        "AutoAdjustData": NotRequired[AutoAdjustDataPaginatorTypeDef],
+        "AutoAdjustData": NotRequired[AutoAdjustDataOutputTypeDef],
     },
 )
 BudgetTypeDef = TypedDict(
     "BudgetTypeDef",
     {
         "BudgetName": str,
         "TimeUnit": TimeUnitType,
@@ -618,38 +724,42 @@
         "CostTypes": NotRequired[CostTypesTypeDef],
         "TimePeriod": NotRequired[TimePeriodTypeDef],
         "CalculatedSpend": NotRequired[CalculatedSpendTypeDef],
         "LastUpdatedTime": NotRequired[TimestampTypeDef],
         "AutoAdjustData": NotRequired[AutoAdjustDataTypeDef],
     },
 )
-ActionPaginatorTypeDef = TypedDict(
-    "ActionPaginatorTypeDef",
+DescribeBudgetNotificationsForAccountResponseTypeDef = TypedDict(
+    "DescribeBudgetNotificationsForAccountResponseTypeDef",
     {
-        "ActionId": str,
-        "BudgetName": str,
-        "NotificationType": NotificationTypeType,
-        "ActionType": ActionTypeType,
-        "ActionThreshold": ActionThresholdTypeDef,
-        "Definition": DefinitionPaginatorTypeDef,
-        "ExecutionRoleArn": str,
-        "ApprovalModel": ApprovalModelType,
-        "Status": ActionStatusType,
-        "Subscribers": List[SubscriberTypeDef],
+        "BudgetNotificationsForAccount": List[BudgetNotificationsForAccountTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+BudgetPerformanceHistoryTypeDef = TypedDict(
+    "BudgetPerformanceHistoryTypeDef",
+    {
+        "BudgetName": NotRequired[str],
+        "BudgetType": NotRequired[BudgetTypeType],
+        "CostFilters": NotRequired[Dict[str, List[str]]],
+        "CostTypes": NotRequired[CostTypesTypeDef],
+        "TimeUnit": NotRequired[TimeUnitType],
+        "BudgetedAndActualAmountsList": NotRequired[List[BudgetedAndActualAmountsTypeDef]],
     },
 )
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "ActionId": str,
         "BudgetName": str,
         "NotificationType": NotificationTypeType,
         "ActionType": ActionTypeType,
         "ActionThreshold": ActionThresholdTypeDef,
-        "Definition": DefinitionTypeDef,
+        "Definition": DefinitionOutputTypeDef,
         "ExecutionRoleArn": str,
         "ApprovalModel": ApprovalModelType,
         "Status": ActionStatusType,
         "Subscribers": List[SubscriberTypeDef],
     },
 )
 CreateBudgetActionRequestRequestTypeDef = TypedDict(
@@ -660,100 +770,70 @@
         "NotificationType": NotificationTypeType,
         "ActionType": ActionTypeType,
         "ActionThreshold": ActionThresholdTypeDef,
         "Definition": DefinitionTypeDef,
         "ExecutionRoleArn": str,
         "ApprovalModel": ApprovalModelType,
         "Subscribers": Sequence[SubscriberTypeDef],
+        "ResourceTags": NotRequired[Sequence[ResourceTagTypeDef]],
     },
 )
+DefinitionUnionTypeDef = Union[DefinitionTypeDef, DefinitionExtraOutputTypeDef]
 UpdateBudgetActionRequestRequestTypeDef = TypedDict(
     "UpdateBudgetActionRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
         "NotificationType": NotRequired[NotificationTypeType],
         "ActionThreshold": NotRequired[ActionThresholdTypeDef],
         "Definition": NotRequired[DefinitionTypeDef],
         "ExecutionRoleArn": NotRequired[str],
         "ApprovalModel": NotRequired[ApprovalModelType],
         "Subscribers": NotRequired[Sequence[SubscriberTypeDef]],
     },
 )
-BudgetPerformanceHistoryTypeDef = TypedDict(
-    "BudgetPerformanceHistoryTypeDef",
+DescribeBudgetsResponseTypeDef = TypedDict(
+    "DescribeBudgetsResponseTypeDef",
     {
-        "BudgetName": NotRequired[str],
-        "BudgetType": NotRequired[BudgetTypeType],
-        "CostFilters": NotRequired[Dict[str, List[str]]],
-        "CostTypes": NotRequired[CostTypesTypeDef],
-        "TimeUnit": NotRequired[TimeUnitType],
-        "BudgetedAndActualAmountsList": NotRequired[List[BudgetedAndActualAmountsTypeDef]],
+        "Budgets": List[BudgetExtraOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-DescribeBudgetsResponsePaginatorTypeDef = TypedDict(
-    "DescribeBudgetsResponsePaginatorTypeDef",
+DescribeBudgetResponseTypeDef = TypedDict(
+    "DescribeBudgetResponseTypeDef",
     {
-        "Budgets": List[BudgetPaginatorTypeDef],
-        "NextToken": str,
+        "Budget": BudgetOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+BudgetUnionTypeDef = Union[BudgetTypeDef, BudgetExtraOutputTypeDef]
 CreateBudgetRequestRequestTypeDef = TypedDict(
     "CreateBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "Budget": BudgetTypeDef,
         "NotificationsWithSubscribers": NotRequired[Sequence[NotificationWithSubscribersTypeDef]],
-    },
-)
-DescribeBudgetResponseTypeDef = TypedDict(
-    "DescribeBudgetResponseTypeDef",
-    {
-        "Budget": BudgetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeBudgetsResponseTypeDef = TypedDict(
-    "DescribeBudgetsResponseTypeDef",
-    {
-        "Budgets": List[BudgetTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceTags": NotRequired[Sequence[ResourceTagTypeDef]],
     },
 )
 UpdateBudgetRequestRequestTypeDef = TypedDict(
     "UpdateBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "NewBudget": BudgetTypeDef,
     },
 )
-ActionHistoryDetailsPaginatorTypeDef = TypedDict(
-    "ActionHistoryDetailsPaginatorTypeDef",
-    {
-        "Message": str,
-        "Action": ActionPaginatorTypeDef,
-    },
-)
-DescribeBudgetActionsForAccountResponsePaginatorTypeDef = TypedDict(
-    "DescribeBudgetActionsForAccountResponsePaginatorTypeDef",
-    {
-        "Actions": List[ActionPaginatorTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeBudgetActionsForBudgetResponsePaginatorTypeDef = TypedDict(
-    "DescribeBudgetActionsForBudgetResponsePaginatorTypeDef",
+DescribeBudgetPerformanceHistoryResponseTypeDef = TypedDict(
+    "DescribeBudgetPerformanceHistoryResponseTypeDef",
     {
-        "Actions": List[ActionPaginatorTypeDef],
-        "NextToken": str,
+        "BudgetPerformanceHistory": BudgetPerformanceHistoryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ActionHistoryDetailsTypeDef = TypedDict(
     "ActionHistoryDetailsTypeDef",
     {
         "Message": str,
         "Action": ActionTypeDef,
@@ -777,71 +857,46 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeBudgetActionsForAccountResponseTypeDef = TypedDict(
     "DescribeBudgetActionsForAccountResponseTypeDef",
     {
         "Actions": List[ActionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeBudgetActionsForBudgetResponseTypeDef = TypedDict(
     "DescribeBudgetActionsForBudgetResponseTypeDef",
     {
         "Actions": List[ActionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateBudgetActionResponseTypeDef = TypedDict(
     "UpdateBudgetActionResponseTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "OldAction": ActionTypeDef,
         "NewAction": ActionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-DescribeBudgetPerformanceHistoryResponseTypeDef = TypedDict(
-    "DescribeBudgetPerformanceHistoryResponseTypeDef",
-    {
-        "BudgetPerformanceHistory": BudgetPerformanceHistoryTypeDef,
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-ActionHistoryPaginatorTypeDef = TypedDict(
-    "ActionHistoryPaginatorTypeDef",
-    {
-        "Timestamp": datetime,
-        "Status": ActionStatusType,
-        "EventType": EventTypeType,
-        "ActionHistoryDetails": ActionHistoryDetailsPaginatorTypeDef,
-    },
-)
 ActionHistoryTypeDef = TypedDict(
     "ActionHistoryTypeDef",
     {
         "Timestamp": datetime,
         "Status": ActionStatusType,
         "EventType": EventTypeType,
         "ActionHistoryDetails": ActionHistoryDetailsTypeDef,
     },
 )
-DescribeBudgetActionHistoriesResponsePaginatorTypeDef = TypedDict(
-    "DescribeBudgetActionHistoriesResponsePaginatorTypeDef",
-    {
-        "ActionHistories": List[ActionHistoryPaginatorTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 DescribeBudgetActionHistoriesResponseTypeDef = TypedDict(
     "DescribeBudgetActionHistoriesResponseTypeDef",
     {
         "ActionHistories": List[ActionHistoryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
```

### Comparing `mypy-boto3-budgets-1.34.0/mypy_boto3_budgets.egg-info/PKG-INFO` & `mypy_boto3_budgets-1.34.100/mypy_boto3_budgets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-budgets
-Version: 1.34.0
-Summary: Type annotations for boto3.Budgets 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.100
+Summary: Type annotations for boto3.Budgets 1.34.100 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-budgets"></a>
 
 # mypy-boto3-budgets
 
 [![PyPI - mypy-boto3-budgets](https://img.shields.io/pypi/v/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-budgets)](https://pepy.tech/project/mypy-boto3-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Budgets 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
+[boto3.Budgets 1.34.100](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-budgets docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-budgets-1.34.0/mypy_boto3_budgets.egg-info/SOURCES.txt` & `mypy_boto3_budgets-1.34.100/mypy_boto3_budgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.34.0/setup.py` & `mypy_boto3_budgets-1.34.100/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,47 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-budgets",
-    version="1.34.0",
+    version="1.34.100",
     packages=["mypy_boto3_budgets"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.Budgets 1.34.0 service generated with mypy-boto3-builder 7.21.0"
-    ),
+    description="Type annotations for boto3.Budgets 1.34.100 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="boto3 budgets type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_budgets": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

