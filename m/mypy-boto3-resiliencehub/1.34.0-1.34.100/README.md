# Comparing `tmp/mypy-boto3-resiliencehub-1.34.0.tar.gz` & `tmp/mypy_boto3_resiliencehub-1.34.100.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-resiliencehub-1.34.0.tar", last modified: Wed Dec 13 21:23:38 2023, max compression
+gzip compressed data, was "mypy_boto3_resiliencehub-1.34.100.tar", last modified: Tue May  7 19:46:55 2024, max compression
```

## Comparing `mypy-boto3-resiliencehub-1.34.0.tar` & `mypy_boto3_resiliencehub-1.34.100.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:38.671338 mypy-boto3-resiliencehub-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:18:09.000000 mypy-boto3-resiliencehub-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12350 2023-12-13 21:23:38.671338 mypy-boto3-resiliencehub-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10793 2023-12-13 21:18:09.000000 mypy-boto3-resiliencehub-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:38.671338 mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2023-12-13 21:18:09.000000 mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2023-12-13 21:18:09.000000 mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      929 2023-12-13 21:18:09.000000 mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41761 2023-12-13 21:18:12.000000 mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    41758 2023-12-13 21:18:10.000000 mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12372 2023-12-13 21:18:13.000000 mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12370 2023-12-13 21:18:13.000000 mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:18:09.000000 mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    53342 2023-12-13 21:18:14.000000 mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    53341 2023-12-13 21:18:13.000000 mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:18:09.000000 mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:38.671338 mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12350 2023-12-13 21:23:38.000000 mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      717 2023-12-13 21:23:38.000000 mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:38.000000 mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:38.000000 mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:23:38.000000 mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-13 21:23:38.000000 mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:23:38.671338 mypy-boto3-resiliencehub-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2023-12-13 21:18:09.000000 mypy-boto3-resiliencehub-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:46:55.307061 mypy_boto3_resiliencehub-1.34.100/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-07 19:46:42.000000 mypy_boto3_resiliencehub-1.34.100/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13109 2024-05-07 19:46:55.307061 mypy_boto3_resiliencehub-1.34.100/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-05-07 19:46:42.000000 mypy_boto3_resiliencehub-1.34.100/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:46:55.303061 mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-07 19:46:42.000000 mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-07 19:46:42.000000 mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-07 19:46:42.000000 mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43178 2024-05-07 19:46:42.000000 mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43175 2024-05-07 19:46:42.000000 mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12844 2024-05-07 19:46:42.000000 mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12844 2024-05-07 19:46:42.000000 mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-07 19:46:42.000000 mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-07 19:46:42.000000 mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:46:42.000000 mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    55901 2024-05-07 19:46:43.000000 mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55901 2024-05-07 19:46:43.000000 mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-07 19:46:42.000000 mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:46:55.303061 mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13109 2024-05-07 19:46:55.000000 mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-07 19:46:55.000000 mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:46:55.000000 mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:46:55.000000 mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-07 19:46:55.000000 mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 19:46:55.000000 mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 19:46:55.307061 mypy_boto3_resiliencehub-1.34.100/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-07 19:46:42.000000 mypy_boto3_resiliencehub-1.34.100/setup.py
```

### Comparing `mypy-boto3-resiliencehub-1.34.0/LICENSE` & `mypy_boto3_resiliencehub-1.34.100/LICENSE`

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

### Comparing `mypy-boto3-resiliencehub-1.34.0/PKG-INFO` & `mypy_boto3_resiliencehub-1.34.100/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resiliencehub
-Version: 1.34.0
-Summary: Type annotations for boto3.ResilienceHub 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.100
+Summary: Type annotations for boto3.ResilienceHub 1.34.100 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/
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
 
 <a id="mypy-boto3-resiliencehub"></a>
 
 # mypy-boto3-resiliencehub
 
 [![PyPI - mypy-boto3-resiliencehub](https://img.shields.io/pypi/v/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resiliencehub)](https://pepy.tech/project/mypy-boto3-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResilienceHub 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[boto3.ResilienceHub 1.34.100](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
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
 [mypy-boto3-resiliencehub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,14 +73,15 @@
     - [Emacs](#emacs)
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
+    - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
     - [Type definitions](#type-definitions)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
@@ -268,14 +269,36 @@
 from mypy_boto3_resiliencehub import ResilienceHubClient
 
 client: ResilienceHubClient = Session().client("resiliencehub")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
+<a id="paginators-annotations"></a>
+
+### Paginators annotations
+
+`mypy_boto3_resiliencehub.paginator` module contains type annotations for all
+paginators.
+
+```python
+from boto3.session import Session
+
+from mypy_boto3_resiliencehub import ResilienceHubClient
+from mypy_boto3_resiliencehub.paginator import ListAppAssessmentResourceDriftsPaginator
+
+client: ResilienceHubClient = Session().client("resiliencehub")
+
+# Explicit type annotations are optional here
+# Types should be correctly discovered by mypy and IDEs
+list_app_assessment_resource_drifts_paginator: ListAppAssessmentResourceDriftsPaginator = (
+    client.get_paginator("list_app_assessment_resource_drifts")
+)
+```
+
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_resiliencehub.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
```

### Comparing `mypy-boto3-resiliencehub-1.34.0/README.md` & `mypy_boto3_resiliencehub-1.34.100/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resiliencehub)](https://pepy.tech/project/mypy-boto3-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResilienceHub 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[boto3.ResilienceHub 1.34.100](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
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
 [mypy-boto3-resiliencehub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -40,14 +40,15 @@
     - [Emacs](#emacs)
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
+    - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
     - [Type definitions](#type-definitions)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
@@ -235,14 +236,36 @@
 from mypy_boto3_resiliencehub import ResilienceHubClient
 
 client: ResilienceHubClient = Session().client("resiliencehub")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
+<a id="paginators-annotations"></a>
+
+### Paginators annotations
+
+`mypy_boto3_resiliencehub.paginator` module contains type annotations for all
+paginators.
+
+```python
+from boto3.session import Session
+
+from mypy_boto3_resiliencehub import ResilienceHubClient
+from mypy_boto3_resiliencehub.paginator import ListAppAssessmentResourceDriftsPaginator
+
+client: ResilienceHubClient = Session().client("resiliencehub")
+
+# Explicit type annotations are optional here
+# Types should be correctly discovered by mypy and IDEs
+list_app_assessment_resource_drifts_paginator: ListAppAssessmentResourceDriftsPaginator = (
+    client.get_paginator("list_app_assessment_resource_drifts")
+)
+```
+
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_resiliencehub.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
```

### Comparing `mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub/client.py` & `mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     from mypy_boto3_resiliencehub.client import ResilienceHubClient
 
     session = Session()
     client: ResilienceHubClient = session.client("resiliencehub")
     ```
 """
 
+import sys
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AppAssessmentScheduleTypeType,
     AssessmentInvokerType,
@@ -27,14 +28,15 @@
     DisruptionTypeType,
     RecommendationTemplateStatusType,
     RenderRecommendationTypeType,
     ResiliencyPolicyTierType,
     ResourceImportStrategyTypeType,
     TemplateFormatType,
 )
+from .paginator import ListAppAssessmentResourceDriftsPaginator
 from .type_defs import (
     AddDraftAppVersionResourceMappingsResponseTypeDef,
     BatchUpdateRecommendationStatusResponseTypeDef,
     CreateAppResponseTypeDef,
     CreateAppVersionAppComponentResponseTypeDef,
     CreateAppVersionResourceResponseTypeDef,
     CreateRecommendationTemplateResponseTypeDef,
@@ -52,20 +54,21 @@
     DescribeAppVersionResourceResponseTypeDef,
     DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
     DescribeAppVersionResponseTypeDef,
     DescribeAppVersionTemplateResponseTypeDef,
     DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
     DescribeResiliencyPolicyResponseTypeDef,
     EksSourceClusterNamespaceTypeDef,
-    EksSourceTypeDef,
+    EksSourceUnionTypeDef,
     EventSubscriptionTypeDef,
     FailurePolicyTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListAppAssessmentComplianceDriftsResponseTypeDef,
+    ListAppAssessmentResourceDriftsResponseTypeDef,
     ListAppAssessmentsResponseTypeDef,
     ListAppComponentCompliancesResponseTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     ListAppInputSourcesResponseTypeDef,
     ListAppsResponseTypeDef,
     ListAppVersionAppComponentsResponseTypeDef,
     ListAppVersionResourceMappingsResponseTypeDef,
@@ -75,15 +78,15 @@
     ListResiliencyPoliciesResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
     ListSuggestedResiliencyPoliciesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTestRecommendationsResponseTypeDef,
     ListUnsupportedAppVersionResourcesResponseTypeDef,
     LogicalResourceIdTypeDef,
-    PermissionModelTypeDef,
+    PermissionModelUnionTypeDef,
     PublishAppVersionResponseTypeDef,
     PutDraftAppVersionTemplateResponseTypeDef,
     RemoveDraftAppVersionResourceMappingsResponseTypeDef,
     ResolveAppVersionResourcesResponseTypeDef,
     ResourceMappingTypeDef,
     StartAppAssessmentResponseTypeDef,
     TerraformSourceTypeDef,
@@ -92,14 +95,19 @@
     UpdateAppVersionAppComponentResponseTypeDef,
     UpdateAppVersionResourceResponseTypeDef,
     UpdateAppVersionResponseTypeDef,
     UpdateRecommendationStatusRequestEntryTypeDef,
     UpdateResiliencyPolicyResponseTypeDef,
 )
 
+if sys.version_info >= (3, 12):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
 __all__ = ("ResilienceHubClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -145,15 +153,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#add_draft_app_version_resource_mappings)
         """
 
     def batch_update_recommendation_status(
         self,
         *,
         appArn: str,
-        requestEntries: Sequence[UpdateRecommendationStatusRequestEntryTypeDef]
+        requestEntries: Sequence[UpdateRecommendationStatusRequestEntryTypeDef],
     ) -> BatchUpdateRecommendationStatusResponseTypeDef:
         """
         Enables you to include or exclude one or more operational recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.batch_update_recommendation_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#batch_update_recommendation_status)
         """
@@ -178,17 +186,17 @@
         self,
         *,
         name: str,
         assessmentSchedule: AppAssessmentScheduleTypeType = ...,
         clientToken: str = ...,
         description: str = ...,
         eventSubscriptions: Sequence[EventSubscriptionTypeDef] = ...,
-        permissionModel: PermissionModelTypeDef = ...,
+        permissionModel: PermissionModelUnionTypeDef = ...,
         policyArn: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAppResponseTypeDef:
         """
         Creates an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#create_app)
         """
@@ -197,15 +205,15 @@
         self,
         *,
         appArn: str,
         name: str,
         type: str,
         additionalInfo: Mapping[str, Sequence[str]] = ...,
         clientToken: str = ...,
-        id: str = ...
+        id: str = ...,
     ) -> CreateAppVersionAppComponentResponseTypeDef:
         """
         Creates a new Application Component in the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app_version_app_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#create_app_version_app_component)
         """
@@ -218,15 +226,15 @@
         logicalResourceId: LogicalResourceIdTypeDef,
         physicalResourceId: str,
         resourceType: str,
         additionalInfo: Mapping[str, Sequence[str]] = ...,
         awsAccountId: str = ...,
         awsRegion: str = ...,
         clientToken: str = ...,
-        resourceName: str = ...
+        resourceName: str = ...,
     ) -> CreateAppVersionResourceResponseTypeDef:
         """
         Adds a resource to the Resilience Hub application and assigns it to the
         specified Application
         Components.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app_version_resource)
@@ -239,15 +247,15 @@
         assessmentArn: str,
         name: str,
         bucketName: str = ...,
         clientToken: str = ...,
         format: TemplateFormatType = ...,
         recommendationIds: Sequence[str] = ...,
         recommendationTypes: Sequence[RenderRecommendationTypeType] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateRecommendationTemplateResponseTypeDef:
         """
         Creates a new recommendation template for the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_recommendation_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#create_recommendation_template)
         """
@@ -257,15 +265,15 @@
         *,
         policy: Mapping[DisruptionTypeType, FailurePolicyTypeDef],
         policyName: str,
         tier: ResiliencyPolicyTierType,
         clientToken: str = ...,
         dataLocationConstraint: DataLocationConstraintType = ...,
         policyDescription: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateResiliencyPolicyResponseTypeDef:
         """
         Creates a resiliency policy for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_resiliency_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#create_resiliency_policy)
         """
@@ -293,15 +301,15 @@
     def delete_app_input_source(
         self,
         *,
         appArn: str,
         clientToken: str = ...,
         eksSourceClusterNamespace: EksSourceClusterNamespaceTypeDef = ...,
         sourceArn: str = ...,
-        terraformSource: TerraformSourceTypeDef = ...
+        terraformSource: TerraformSourceTypeDef = ...,
     ) -> DeleteAppInputSourceResponseTypeDef:
         """
         Deletes the input source and all of its imported resources from the Resilience
         Hub
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_app_input_source)
@@ -323,15 +331,15 @@
         *,
         appArn: str,
         awsAccountId: str = ...,
         awsRegion: str = ...,
         clientToken: str = ...,
         logicalResourceId: LogicalResourceIdTypeDef = ...,
         physicalResourceId: str = ...,
-        resourceName: str = ...
+        resourceName: str = ...,
     ) -> DeleteAppVersionResourceResponseTypeDef:
         """
         Deletes a resource from the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_app_version_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#delete_app_version_resource)
         """
@@ -399,15 +407,15 @@
         *,
         appArn: str,
         appVersion: str,
         awsAccountId: str = ...,
         awsRegion: str = ...,
         logicalResourceId: LogicalResourceIdTypeDef = ...,
         physicalResourceId: str = ...,
-        resourceName: str = ...
+        resourceName: str = ...,
     ) -> DescribeAppVersionResourceResponseTypeDef:
         """
         Describes a resource of the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_app_version_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#describe_app_version_resource)
         """
@@ -468,18 +476,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#generate_presigned_url)
         """
 
     def import_resources_to_draft_app_version(
         self,
         *,
         appArn: str,
-        eksSources: Sequence[EksSourceTypeDef] = ...,
+        eksSources: Sequence[EksSourceUnionTypeDef] = ...,
         importStrategy: ResourceImportStrategyTypeType = ...,
         sourceArns: Sequence[str] = ...,
-        terraformSources: Sequence[TerraformSourceTypeDef] = ...
+        terraformSources: Sequence[TerraformSourceTypeDef] = ...,
     ) -> ImportResourcesToDraftAppVersionResponseTypeDef:
         """
         Imports resources to Resilience Hub application draft version from different
         input
         sources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.import_resources_to_draft_app_version)
@@ -502,25 +510,36 @@
         """
         List of compliance drifts that were detected while running an assessment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_assessment_compliance_drifts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_assessment_compliance_drifts)
         """
 
+    def list_app_assessment_resource_drifts(
+        self, *, assessmentArn: str, maxResults: int = ..., nextToken: str = ...
+    ) -> ListAppAssessmentResourceDriftsResponseTypeDef:
+        """
+        Indicates the list of resource drifts that were detected while running an
+        assessment.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_assessment_resource_drifts)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_assessment_resource_drifts)
+        """
+
     def list_app_assessments(
         self,
         *,
         appArn: str = ...,
         assessmentName: str = ...,
         assessmentStatus: Sequence[AssessmentStatusType] = ...,
         complianceStatus: ComplianceStatusType = ...,
         invoker: AssessmentInvokerType = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        reverseOrder: bool = ...
+        reverseOrder: bool = ...,
     ) -> ListAppAssessmentsResponseTypeDef:
         """
         Lists the assessments for an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_assessments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_assessments)
         """
@@ -578,15 +597,15 @@
     def list_app_version_resources(
         self,
         *,
         appArn: str,
         appVersion: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        resolutionId: str = ...
+        resolutionId: str = ...,
     ) -> ListAppVersionResourcesResponseTypeDef:
         """
         Lists all the resources in an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_version_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_version_resources)
         """
@@ -594,15 +613,15 @@
     def list_app_versions(
         self,
         *,
         appArn: str,
         endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        startTime: TimestampTypeDef = ...
+        startTime: TimestampTypeDef = ...,
     ) -> ListAppVersionsResponseTypeDef:
         """
         Lists the different versions for the Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_versions)
         """
@@ -612,33 +631,33 @@
         *,
         appArn: str = ...,
         fromLastAssessmentTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         name: str = ...,
         nextToken: str = ...,
         reverseOrder: bool = ...,
-        toLastAssessmentTime: TimestampTypeDef = ...
+        toLastAssessmentTime: TimestampTypeDef = ...,
     ) -> ListAppsResponseTypeDef:
         """
         Lists your Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_apps)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_apps)
         """
 
     def list_recommendation_templates(
         self,
         *,
-        assessmentArn: str,
+        assessmentArn: str = ...,
         maxResults: int = ...,
         name: str = ...,
         nextToken: str = ...,
         recommendationTemplateArn: str = ...,
         reverseOrder: bool = ...,
-        status: Sequence[RecommendationTemplateStatusType] = ...
+        status: Sequence[RecommendationTemplateStatusType] = ...,
     ) -> ListRecommendationTemplatesResponseTypeDef:
         """
         Lists the recommendation templates for the Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_recommendation_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_recommendation_templates)
         """
@@ -696,15 +715,15 @@
     def list_unsupported_app_version_resources(
         self,
         *,
         appArn: str,
         appVersion: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        resolutionId: str = ...
+        resolutionId: str = ...,
     ) -> ListUnsupportedAppVersionResourcesResponseTypeDef:
         """
         Lists the resources that are not currently supported in Resilience Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_unsupported_app_version_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_unsupported_app_version_resources)
         """
@@ -735,15 +754,15 @@
         *,
         appArn: str,
         appRegistryAppNames: Sequence[str] = ...,
         eksSourceNames: Sequence[str] = ...,
         logicalStackNames: Sequence[str] = ...,
         resourceGroupNames: Sequence[str] = ...,
         resourceNames: Sequence[str] = ...,
-        terraformSourceNames: Sequence[str] = ...
+        terraformSourceNames: Sequence[str] = ...,
     ) -> RemoveDraftAppVersionResourceMappingsResponseTypeDef:
         """
         Removes resource mappings from a draft application version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.remove_draft_app_version_resource_mappings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#remove_draft_app_version_resource_mappings)
         """
@@ -761,15 +780,15 @@
     def start_app_assessment(
         self,
         *,
         appArn: str,
         appVersion: str,
         assessmentName: str,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> StartAppAssessmentResponseTypeDef:
         """
         Creates a new application assessment for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.start_app_assessment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#start_app_assessment)
         """
@@ -794,16 +813,16 @@
         self,
         *,
         appArn: str,
         assessmentSchedule: AppAssessmentScheduleTypeType = ...,
         clearResiliencyPolicyArn: bool = ...,
         description: str = ...,
         eventSubscriptions: Sequence[EventSubscriptionTypeDef] = ...,
-        permissionModel: PermissionModelTypeDef = ...,
-        policyArn: str = ...
+        permissionModel: PermissionModelUnionTypeDef = ...,
+        policyArn: str = ...,
     ) -> UpdateAppResponseTypeDef:
         """
         Updates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#update_app)
         """
@@ -821,15 +840,15 @@
     def update_app_version_app_component(
         self,
         *,
         appArn: str,
         id: str,
         additionalInfo: Mapping[str, Sequence[str]] = ...,
         name: str = ...,
-        type: str = ...
+        type: str = ...,
     ) -> UpdateAppVersionAppComponentResponseTypeDef:
         """
         Updates an existing Application Component in the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app_version_app_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#update_app_version_app_component)
         """
@@ -842,15 +861,15 @@
         appComponents: Sequence[str] = ...,
         awsAccountId: str = ...,
         awsRegion: str = ...,
         excluded: bool = ...,
         logicalResourceId: LogicalResourceIdTypeDef = ...,
         physicalResourceId: str = ...,
         resourceName: str = ...,
-        resourceType: str = ...
+        resourceType: str = ...,
     ) -> UpdateAppVersionResourceResponseTypeDef:
         """
         Updates the resource details in the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app_version_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#update_app_version_resource)
         """
@@ -859,15 +878,23 @@
         self,
         *,
         policyArn: str,
         dataLocationConstraint: DataLocationConstraintType = ...,
         policy: Mapping[DisruptionTypeType, FailurePolicyTypeDef] = ...,
         policyDescription: str = ...,
         policyName: str = ...,
-        tier: ResiliencyPolicyTierType = ...
+        tier: ResiliencyPolicyTierType = ...,
     ) -> UpdateResiliencyPolicyResponseTypeDef:
         """
         Updates a resiliency policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_resiliency_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#update_resiliency_policy)
         """
+
+    def get_paginator(
+        self, operation_name: Literal["list_app_assessment_resource_drifts"]
+    ) -> ListAppAssessmentResourceDriftsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#get_paginator)
+        """
```

### Comparing `mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub/client.pyi` & `mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     from mypy_boto3_resiliencehub.client import ResilienceHubClient
 
     session = Session()
     client: ResilienceHubClient = session.client("resiliencehub")
     ```
 """
 
+import sys
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AppAssessmentScheduleTypeType,
     AssessmentInvokerType,
@@ -27,14 +28,15 @@
     DisruptionTypeType,
     RecommendationTemplateStatusType,
     RenderRecommendationTypeType,
     ResiliencyPolicyTierType,
     ResourceImportStrategyTypeType,
     TemplateFormatType,
 )
+from .paginator import ListAppAssessmentResourceDriftsPaginator
 from .type_defs import (
     AddDraftAppVersionResourceMappingsResponseTypeDef,
     BatchUpdateRecommendationStatusResponseTypeDef,
     CreateAppResponseTypeDef,
     CreateAppVersionAppComponentResponseTypeDef,
     CreateAppVersionResourceResponseTypeDef,
     CreateRecommendationTemplateResponseTypeDef,
@@ -52,20 +54,21 @@
     DescribeAppVersionResourceResponseTypeDef,
     DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
     DescribeAppVersionResponseTypeDef,
     DescribeAppVersionTemplateResponseTypeDef,
     DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
     DescribeResiliencyPolicyResponseTypeDef,
     EksSourceClusterNamespaceTypeDef,
-    EksSourceTypeDef,
+    EksSourceUnionTypeDef,
     EventSubscriptionTypeDef,
     FailurePolicyTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListAppAssessmentComplianceDriftsResponseTypeDef,
+    ListAppAssessmentResourceDriftsResponseTypeDef,
     ListAppAssessmentsResponseTypeDef,
     ListAppComponentCompliancesResponseTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     ListAppInputSourcesResponseTypeDef,
     ListAppsResponseTypeDef,
     ListAppVersionAppComponentsResponseTypeDef,
     ListAppVersionResourceMappingsResponseTypeDef,
@@ -75,15 +78,15 @@
     ListResiliencyPoliciesResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
     ListSuggestedResiliencyPoliciesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTestRecommendationsResponseTypeDef,
     ListUnsupportedAppVersionResourcesResponseTypeDef,
     LogicalResourceIdTypeDef,
-    PermissionModelTypeDef,
+    PermissionModelUnionTypeDef,
     PublishAppVersionResponseTypeDef,
     PutDraftAppVersionTemplateResponseTypeDef,
     RemoveDraftAppVersionResourceMappingsResponseTypeDef,
     ResolveAppVersionResourcesResponseTypeDef,
     ResourceMappingTypeDef,
     StartAppAssessmentResponseTypeDef,
     TerraformSourceTypeDef,
@@ -92,14 +95,19 @@
     UpdateAppVersionAppComponentResponseTypeDef,
     UpdateAppVersionResourceResponseTypeDef,
     UpdateAppVersionResponseTypeDef,
     UpdateRecommendationStatusRequestEntryTypeDef,
     UpdateResiliencyPolicyResponseTypeDef,
 )
 
+if sys.version_info >= (3, 12):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
 __all__ = ("ResilienceHubClient",)
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
@@ -142,15 +150,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#add_draft_app_version_resource_mappings)
         """
 
     def batch_update_recommendation_status(
         self,
         *,
         appArn: str,
-        requestEntries: Sequence[UpdateRecommendationStatusRequestEntryTypeDef]
+        requestEntries: Sequence[UpdateRecommendationStatusRequestEntryTypeDef],
     ) -> BatchUpdateRecommendationStatusResponseTypeDef:
         """
         Enables you to include or exclude one or more operational recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.batch_update_recommendation_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#batch_update_recommendation_status)
         """
@@ -175,17 +183,17 @@
         self,
         *,
         name: str,
         assessmentSchedule: AppAssessmentScheduleTypeType = ...,
         clientToken: str = ...,
         description: str = ...,
         eventSubscriptions: Sequence[EventSubscriptionTypeDef] = ...,
-        permissionModel: PermissionModelTypeDef = ...,
+        permissionModel: PermissionModelUnionTypeDef = ...,
         policyArn: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAppResponseTypeDef:
         """
         Creates an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#create_app)
         """
@@ -194,15 +202,15 @@
         self,
         *,
         appArn: str,
         name: str,
         type: str,
         additionalInfo: Mapping[str, Sequence[str]] = ...,
         clientToken: str = ...,
-        id: str = ...
+        id: str = ...,
     ) -> CreateAppVersionAppComponentResponseTypeDef:
         """
         Creates a new Application Component in the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app_version_app_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#create_app_version_app_component)
         """
@@ -215,15 +223,15 @@
         logicalResourceId: LogicalResourceIdTypeDef,
         physicalResourceId: str,
         resourceType: str,
         additionalInfo: Mapping[str, Sequence[str]] = ...,
         awsAccountId: str = ...,
         awsRegion: str = ...,
         clientToken: str = ...,
-        resourceName: str = ...
+        resourceName: str = ...,
     ) -> CreateAppVersionResourceResponseTypeDef:
         """
         Adds a resource to the Resilience Hub application and assigns it to the
         specified Application
         Components.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app_version_resource)
@@ -236,15 +244,15 @@
         assessmentArn: str,
         name: str,
         bucketName: str = ...,
         clientToken: str = ...,
         format: TemplateFormatType = ...,
         recommendationIds: Sequence[str] = ...,
         recommendationTypes: Sequence[RenderRecommendationTypeType] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateRecommendationTemplateResponseTypeDef:
         """
         Creates a new recommendation template for the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_recommendation_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#create_recommendation_template)
         """
@@ -254,15 +262,15 @@
         *,
         policy: Mapping[DisruptionTypeType, FailurePolicyTypeDef],
         policyName: str,
         tier: ResiliencyPolicyTierType,
         clientToken: str = ...,
         dataLocationConstraint: DataLocationConstraintType = ...,
         policyDescription: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateResiliencyPolicyResponseTypeDef:
         """
         Creates a resiliency policy for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_resiliency_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#create_resiliency_policy)
         """
@@ -290,15 +298,15 @@
     def delete_app_input_source(
         self,
         *,
         appArn: str,
         clientToken: str = ...,
         eksSourceClusterNamespace: EksSourceClusterNamespaceTypeDef = ...,
         sourceArn: str = ...,
-        terraformSource: TerraformSourceTypeDef = ...
+        terraformSource: TerraformSourceTypeDef = ...,
     ) -> DeleteAppInputSourceResponseTypeDef:
         """
         Deletes the input source and all of its imported resources from the Resilience
         Hub
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_app_input_source)
@@ -320,15 +328,15 @@
         *,
         appArn: str,
         awsAccountId: str = ...,
         awsRegion: str = ...,
         clientToken: str = ...,
         logicalResourceId: LogicalResourceIdTypeDef = ...,
         physicalResourceId: str = ...,
-        resourceName: str = ...
+        resourceName: str = ...,
     ) -> DeleteAppVersionResourceResponseTypeDef:
         """
         Deletes a resource from the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_app_version_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#delete_app_version_resource)
         """
@@ -396,15 +404,15 @@
         *,
         appArn: str,
         appVersion: str,
         awsAccountId: str = ...,
         awsRegion: str = ...,
         logicalResourceId: LogicalResourceIdTypeDef = ...,
         physicalResourceId: str = ...,
-        resourceName: str = ...
+        resourceName: str = ...,
     ) -> DescribeAppVersionResourceResponseTypeDef:
         """
         Describes a resource of the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_app_version_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#describe_app_version_resource)
         """
@@ -465,18 +473,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#generate_presigned_url)
         """
 
     def import_resources_to_draft_app_version(
         self,
         *,
         appArn: str,
-        eksSources: Sequence[EksSourceTypeDef] = ...,
+        eksSources: Sequence[EksSourceUnionTypeDef] = ...,
         importStrategy: ResourceImportStrategyTypeType = ...,
         sourceArns: Sequence[str] = ...,
-        terraformSources: Sequence[TerraformSourceTypeDef] = ...
+        terraformSources: Sequence[TerraformSourceTypeDef] = ...,
     ) -> ImportResourcesToDraftAppVersionResponseTypeDef:
         """
         Imports resources to Resilience Hub application draft version from different
         input
         sources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.import_resources_to_draft_app_version)
@@ -499,25 +507,36 @@
         """
         List of compliance drifts that were detected while running an assessment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_assessment_compliance_drifts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_assessment_compliance_drifts)
         """
 
+    def list_app_assessment_resource_drifts(
+        self, *, assessmentArn: str, maxResults: int = ..., nextToken: str = ...
+    ) -> ListAppAssessmentResourceDriftsResponseTypeDef:
+        """
+        Indicates the list of resource drifts that were detected while running an
+        assessment.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_assessment_resource_drifts)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_assessment_resource_drifts)
+        """
+
     def list_app_assessments(
         self,
         *,
         appArn: str = ...,
         assessmentName: str = ...,
         assessmentStatus: Sequence[AssessmentStatusType] = ...,
         complianceStatus: ComplianceStatusType = ...,
         invoker: AssessmentInvokerType = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        reverseOrder: bool = ...
+        reverseOrder: bool = ...,
     ) -> ListAppAssessmentsResponseTypeDef:
         """
         Lists the assessments for an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_assessments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_assessments)
         """
@@ -575,15 +594,15 @@
     def list_app_version_resources(
         self,
         *,
         appArn: str,
         appVersion: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        resolutionId: str = ...
+        resolutionId: str = ...,
     ) -> ListAppVersionResourcesResponseTypeDef:
         """
         Lists all the resources in an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_version_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_version_resources)
         """
@@ -591,15 +610,15 @@
     def list_app_versions(
         self,
         *,
         appArn: str,
         endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        startTime: TimestampTypeDef = ...
+        startTime: TimestampTypeDef = ...,
     ) -> ListAppVersionsResponseTypeDef:
         """
         Lists the different versions for the Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_versions)
         """
@@ -609,33 +628,33 @@
         *,
         appArn: str = ...,
         fromLastAssessmentTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         name: str = ...,
         nextToken: str = ...,
         reverseOrder: bool = ...,
-        toLastAssessmentTime: TimestampTypeDef = ...
+        toLastAssessmentTime: TimestampTypeDef = ...,
     ) -> ListAppsResponseTypeDef:
         """
         Lists your Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_apps)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_apps)
         """
 
     def list_recommendation_templates(
         self,
         *,
-        assessmentArn: str,
+        assessmentArn: str = ...,
         maxResults: int = ...,
         name: str = ...,
         nextToken: str = ...,
         recommendationTemplateArn: str = ...,
         reverseOrder: bool = ...,
-        status: Sequence[RecommendationTemplateStatusType] = ...
+        status: Sequence[RecommendationTemplateStatusType] = ...,
     ) -> ListRecommendationTemplatesResponseTypeDef:
         """
         Lists the recommendation templates for the Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_recommendation_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_recommendation_templates)
         """
@@ -693,15 +712,15 @@
     def list_unsupported_app_version_resources(
         self,
         *,
         appArn: str,
         appVersion: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        resolutionId: str = ...
+        resolutionId: str = ...,
     ) -> ListUnsupportedAppVersionResourcesResponseTypeDef:
         """
         Lists the resources that are not currently supported in Resilience Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_unsupported_app_version_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_unsupported_app_version_resources)
         """
@@ -732,15 +751,15 @@
         *,
         appArn: str,
         appRegistryAppNames: Sequence[str] = ...,
         eksSourceNames: Sequence[str] = ...,
         logicalStackNames: Sequence[str] = ...,
         resourceGroupNames: Sequence[str] = ...,
         resourceNames: Sequence[str] = ...,
-        terraformSourceNames: Sequence[str] = ...
+        terraformSourceNames: Sequence[str] = ...,
     ) -> RemoveDraftAppVersionResourceMappingsResponseTypeDef:
         """
         Removes resource mappings from a draft application version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.remove_draft_app_version_resource_mappings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#remove_draft_app_version_resource_mappings)
         """
@@ -758,15 +777,15 @@
     def start_app_assessment(
         self,
         *,
         appArn: str,
         appVersion: str,
         assessmentName: str,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> StartAppAssessmentResponseTypeDef:
         """
         Creates a new application assessment for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.start_app_assessment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#start_app_assessment)
         """
@@ -791,16 +810,16 @@
         self,
         *,
         appArn: str,
         assessmentSchedule: AppAssessmentScheduleTypeType = ...,
         clearResiliencyPolicyArn: bool = ...,
         description: str = ...,
         eventSubscriptions: Sequence[EventSubscriptionTypeDef] = ...,
-        permissionModel: PermissionModelTypeDef = ...,
-        policyArn: str = ...
+        permissionModel: PermissionModelUnionTypeDef = ...,
+        policyArn: str = ...,
     ) -> UpdateAppResponseTypeDef:
         """
         Updates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#update_app)
         """
@@ -818,15 +837,15 @@
     def update_app_version_app_component(
         self,
         *,
         appArn: str,
         id: str,
         additionalInfo: Mapping[str, Sequence[str]] = ...,
         name: str = ...,
-        type: str = ...
+        type: str = ...,
     ) -> UpdateAppVersionAppComponentResponseTypeDef:
         """
         Updates an existing Application Component in the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app_version_app_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#update_app_version_app_component)
         """
@@ -839,15 +858,15 @@
         appComponents: Sequence[str] = ...,
         awsAccountId: str = ...,
         awsRegion: str = ...,
         excluded: bool = ...,
         logicalResourceId: LogicalResourceIdTypeDef = ...,
         physicalResourceId: str = ...,
         resourceName: str = ...,
-        resourceType: str = ...
+        resourceType: str = ...,
     ) -> UpdateAppVersionResourceResponseTypeDef:
         """
         Updates the resource details in the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app_version_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#update_app_version_resource)
         """
@@ -856,15 +875,23 @@
         self,
         *,
         policyArn: str,
         dataLocationConstraint: DataLocationConstraintType = ...,
         policy: Mapping[DisruptionTypeType, FailurePolicyTypeDef] = ...,
         policyDescription: str = ...,
         policyName: str = ...,
-        tier: ResiliencyPolicyTierType = ...
+        tier: ResiliencyPolicyTierType = ...,
     ) -> UpdateResiliencyPolicyResponseTypeDef:
         """
         Updates a resiliency policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_resiliency_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#update_resiliency_policy)
         """
+
+    def get_paginator(
+        self, operation_name: Literal["list_app_assessment_resource_drifts"]
+    ) -> ListAppAssessmentResourceDriftsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#get_paginator)
+        """
```

### Comparing `mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub/literals.py` & `mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AlarmTypeType",
     "AppAssessmentScheduleTypeType",
     "AppComplianceStatusTypeType",
     "AppDriftStatusTypeType",
     "AppStatusTypeType",
     "AssessmentInvokerType",
@@ -36,14 +35,15 @@
     "DisruptionTypeType",
     "DriftStatusType",
     "DriftTypeType",
     "EstimatedCostTierType",
     "EventTypeType",
     "ExcludeRecommendationReasonType",
     "HaArchitectureType",
+    "ListAppAssessmentResourceDriftsPaginatorName",
     "PermissionModelTypeType",
     "PhysicalIdentifierTypeType",
     "RecommendationComplianceStatusType",
     "RecommendationStatusType",
     "RecommendationTemplateStatusType",
     "RenderRecommendationTypeType",
     "ResiliencyPolicyTierType",
@@ -56,18 +56,18 @@
     "SopServiceTypeType",
     "TemplateFormatType",
     "TestRiskType",
     "TestTypeType",
     "ResilienceHubServiceName",
     "ServiceName",
     "ResourceServiceName",
+    "PaginatorName",
     "RegionName",
 )
 
-
 AlarmTypeType = Literal["Canary", "Composite", "Event", "Logs", "Metric"]
 AppAssessmentScheduleTypeType = Literal["Daily", "Disabled"]
 AppComplianceStatusTypeType = Literal[
     "ChangesDetected", "NotAssessed", "PolicyBreached", "PolicyMet"
 ]
 AppDriftStatusTypeType = Literal["Detected", "NotChecked", "NotDetected"]
 AppStatusTypeType = Literal["Active", "Deleting"]
@@ -80,26 +80,27 @@
     "BestRegionRecovery",
     "LeastChange",
     "LeastCost",
     "LeastErrors",
 ]
 CostFrequencyType = Literal["Daily", "Hourly", "Monthly", "Yearly"]
 DataLocationConstraintType = Literal["AnyLocation", "SameContinent", "SameCountry"]
-DifferenceTypeType = Literal["NotEqual"]
+DifferenceTypeType = Literal["Added", "NotEqual", "Removed"]
 DisruptionTypeType = Literal["AZ", "Hardware", "Region", "Software"]
 DriftStatusType = Literal["Detected", "NotChecked", "NotDetected"]
-DriftTypeType = Literal["ApplicationCompliance"]
+DriftTypeType = Literal["AppComponentResiliencyComplianceStatus", "ApplicationCompliance"]
 EstimatedCostTierType = Literal["L1", "L2", "L3", "L4"]
 EventTypeType = Literal["DriftDetected", "ScheduledAssessmentFailure"]
 ExcludeRecommendationReasonType = Literal[
     "AlreadyImplemented", "ComplexityOfImplementation", "NotRelevant"
 ]
 HaArchitectureType = Literal[
     "BackupAndRestore", "MultiSite", "NoRecoveryPlan", "PilotLight", "WarmStandby"
 ]
+ListAppAssessmentResourceDriftsPaginatorName = Literal["list_app_assessment_resource_drifts"]
 PermissionModelTypeType = Literal["LegacyIAMUser", "RoleBased"]
 PhysicalIdentifierTypeType = Literal["Arn", "Native"]
 RecommendationComplianceStatusType = Literal[
     "BreachedCanMeet", "BreachedUnattainable", "MetCanImprove"
 ]
 RecommendationStatusType = Literal["Excluded", "Implemented", "Inactive", "NotImplemented"]
 RecommendationTemplateStatusType = Literal["Failed", "InProgress", "Pending", "Success"]
@@ -142,14 +143,15 @@
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
@@ -160,14 +162,15 @@
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
@@ -185,14 +188,15 @@
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
@@ -205,24 +209,26 @@
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
@@ -283,15 +289,14 @@
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
@@ -363,17 +368,19 @@
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
@@ -418,14 +425,15 @@
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
@@ -463,19 +471,21 @@
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
@@ -504,14 +514,15 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
+PaginatorName = Literal["list_app_assessment_resource_drifts"]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
```

### Comparing `mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub/literals.pyi` & `mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     "DisruptionTypeType",
     "DriftStatusType",
     "DriftTypeType",
     "EstimatedCostTierType",
     "EventTypeType",
     "ExcludeRecommendationReasonType",
     "HaArchitectureType",
+    "ListAppAssessmentResourceDriftsPaginatorName",
     "PermissionModelTypeType",
     "PhysicalIdentifierTypeType",
     "RecommendationComplianceStatusType",
     "RecommendationStatusType",
     "RecommendationTemplateStatusType",
     "RenderRecommendationTypeType",
     "ResiliencyPolicyTierType",
@@ -55,14 +56,15 @@
     "SopServiceTypeType",
     "TemplateFormatType",
     "TestRiskType",
     "TestTypeType",
     "ResilienceHubServiceName",
     "ServiceName",
     "ResourceServiceName",
+    "PaginatorName",
     "RegionName",
 )
 
 AlarmTypeType = Literal["Canary", "Composite", "Event", "Logs", "Metric"]
 AppAssessmentScheduleTypeType = Literal["Daily", "Disabled"]
 AppComplianceStatusTypeType = Literal[
     "ChangesDetected", "NotAssessed", "PolicyBreached", "PolicyMet"
@@ -78,26 +80,27 @@
     "BestRegionRecovery",
     "LeastChange",
     "LeastCost",
     "LeastErrors",
 ]
 CostFrequencyType = Literal["Daily", "Hourly", "Monthly", "Yearly"]
 DataLocationConstraintType = Literal["AnyLocation", "SameContinent", "SameCountry"]
-DifferenceTypeType = Literal["NotEqual"]
+DifferenceTypeType = Literal["Added", "NotEqual", "Removed"]
 DisruptionTypeType = Literal["AZ", "Hardware", "Region", "Software"]
 DriftStatusType = Literal["Detected", "NotChecked", "NotDetected"]
-DriftTypeType = Literal["ApplicationCompliance"]
+DriftTypeType = Literal["AppComponentResiliencyComplianceStatus", "ApplicationCompliance"]
 EstimatedCostTierType = Literal["L1", "L2", "L3", "L4"]
 EventTypeType = Literal["DriftDetected", "ScheduledAssessmentFailure"]
 ExcludeRecommendationReasonType = Literal[
     "AlreadyImplemented", "ComplexityOfImplementation", "NotRelevant"
 ]
 HaArchitectureType = Literal[
     "BackupAndRestore", "MultiSite", "NoRecoveryPlan", "PilotLight", "WarmStandby"
 ]
+ListAppAssessmentResourceDriftsPaginatorName = Literal["list_app_assessment_resource_drifts"]
 PermissionModelTypeType = Literal["LegacyIAMUser", "RoleBased"]
 PhysicalIdentifierTypeType = Literal["Arn", "Native"]
 RecommendationComplianceStatusType = Literal[
     "BreachedCanMeet", "BreachedUnattainable", "MetCanImprove"
 ]
 RecommendationStatusType = Literal["Excluded", "Implemented", "Inactive", "NotImplemented"]
 RecommendationTemplateStatusType = Literal["Failed", "InProgress", "Pending", "Success"]
@@ -140,14 +143,15 @@
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
@@ -158,14 +162,15 @@
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
@@ -183,14 +188,15 @@
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
@@ -203,24 +209,26 @@
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
@@ -281,15 +289,14 @@
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
@@ -361,17 +368,19 @@
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
@@ -416,14 +425,15 @@
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
@@ -461,19 +471,21 @@
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
@@ -502,14 +514,15 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
+PaginatorName = Literal["list_app_assessment_resource_drifts"]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
```

### Comparing `mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub/type_defs.py` & `mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,18 @@
     AppStatusTypeType,
     AssessmentInvokerType,
     AssessmentStatusType,
     ComplianceStatusType,
     ConfigRecommendationOptimizationTypeType,
     CostFrequencyType,
     DataLocationConstraintType,
+    DifferenceTypeType,
     DisruptionTypeType,
     DriftStatusType,
+    DriftTypeType,
     EstimatedCostTierType,
     EventTypeType,
     ExcludeRecommendationReasonType,
     HaArchitectureType,
     PermissionModelTypeType,
     PhysicalIdentifierTypeType,
     RecommendationComplianceStatusType,
@@ -61,30 +63,30 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ResponseMetadataTypeDef",
     "RecommendationItemTypeDef",
     "CostTypeDef",
     "DisruptionComplianceTypeDef",
     "AppComponentTypeDef",
     "EksSourceClusterNamespaceTypeDef",
     "TerraformSourceTypeDef",
     "AppSummaryTypeDef",
     "EventSubscriptionTypeDef",
-    "PermissionModelTypeDef",
+    "PermissionModelOutputTypeDef",
     "AppVersionSummaryTypeDef",
     "BatchUpdateRecommendationStatusFailedEntryTypeDef",
     "UpdateRecommendationStatusItemTypeDef",
     "RecommendationDisruptionComplianceTypeDef",
+    "PermissionModelTypeDef",
     "CreateAppVersionAppComponentRequestRequestTypeDef",
     "LogicalResourceIdTypeDef",
     "CreateRecommendationTemplateRequestRequestTypeDef",
     "FailurePolicyTypeDef",
     "DeleteAppAssessmentRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteAppVersionAppComponentRequestRequestTypeDef",
@@ -94,17 +96,20 @@
     "DescribeAppRequestRequestTypeDef",
     "DescribeAppVersionAppComponentRequestRequestTypeDef",
     "DescribeAppVersionRequestRequestTypeDef",
     "DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef",
     "DescribeAppVersionTemplateRequestRequestTypeDef",
     "DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef",
     "DescribeResiliencyPolicyRequestRequestTypeDef",
+    "EksSourceOutputTypeDef",
     "EksSourceTypeDef",
     "ListAlarmRecommendationsRequestRequestTypeDef",
     "ListAppAssessmentComplianceDriftsRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ListAppAssessmentResourceDriftsRequestRequestTypeDef",
     "ListAppAssessmentsRequestRequestTypeDef",
     "ListAppComponentCompliancesRequestRequestTypeDef",
     "ListAppComponentRecommendationsRequestRequestTypeDef",
     "ListAppInputSourcesRequestRequestTypeDef",
     "ListAppVersionAppComponentsRequestRequestTypeDef",
     "ListAppVersionResourceMappingsRequestRequestTypeDef",
     "ListAppVersionResourcesRequestRequestTypeDef",
@@ -153,29 +158,32 @@
     "DescribeAppVersionAppComponentResponseTypeDef",
     "ListAppVersionAppComponentsResponseTypeDef",
     "UpdateAppVersionAppComponentResponseTypeDef",
     "AppInputSourceTypeDef",
     "DeleteAppInputSourceRequestRequestTypeDef",
     "ListAppsResponseTypeDef",
     "AppTypeDef",
-    "CreateAppRequestRequestTypeDef",
-    "UpdateAppRequestRequestTypeDef",
     "ListAppVersionsResponseTypeDef",
     "BatchUpdateRecommendationStatusSuccessfulEntryTypeDef",
     "UpdateRecommendationStatusRequestEntryTypeDef",
     "ConfigRecommendationTypeDef",
+    "CreateAppRequestRequestTypeDef",
+    "PermissionModelUnionTypeDef",
+    "UpdateAppRequestRequestTypeDef",
     "CreateAppVersionResourceRequestRequestTypeDef",
     "DeleteAppVersionResourceRequestRequestTypeDef",
     "DescribeAppVersionResourceRequestRequestTypeDef",
+    "ResourceIdentifierTypeDef",
     "UpdateAppVersionResourceRequestRequestTypeDef",
     "CreateResiliencyPolicyRequestRequestTypeDef",
     "ResiliencyPolicyTypeDef",
     "UpdateResiliencyPolicyRequestRequestTypeDef",
-    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
     "ImportResourcesToDraftAppVersionResponseTypeDef",
+    "EksSourceUnionTypeDef",
+    "ListAppAssessmentResourceDriftsRequestListAppAssessmentResourceDriftsPaginateTypeDef",
     "ListAppVersionsRequestRequestTypeDef",
     "ListAppsRequestRequestTypeDef",
     "PhysicalResourceTypeDef",
     "ResourceMappingTypeDef",
     "UnsupportedResourceTypeDef",
     "RecommendationTemplateTypeDef",
     "ResiliencyScoreTypeDef",
@@ -189,46 +197,49 @@
     "ListAppInputSourcesResponseTypeDef",
     "CreateAppResponseTypeDef",
     "DescribeAppResponseTypeDef",
     "UpdateAppResponseTypeDef",
     "BatchUpdateRecommendationStatusResponseTypeDef",
     "BatchUpdateRecommendationStatusRequestRequestTypeDef",
     "ComponentRecommendationTypeDef",
+    "ResourceDriftTypeDef",
     "CreateResiliencyPolicyResponseTypeDef",
     "DescribeResiliencyPolicyResponseTypeDef",
     "ListResiliencyPoliciesResponseTypeDef",
     "ListSuggestedResiliencyPoliciesResponseTypeDef",
     "UpdateResiliencyPolicyResponseTypeDef",
+    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
     "CreateAppVersionResourceResponseTypeDef",
     "DeleteAppVersionResourceResponseTypeDef",
     "DescribeAppVersionResourceResponseTypeDef",
     "ListAppVersionResourcesResponseTypeDef",
     "UpdateAppVersionResourceResponseTypeDef",
     "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
     "AddDraftAppVersionResourceMappingsResponseTypeDef",
     "ListAppVersionResourceMappingsResponseTypeDef",
     "ListUnsupportedAppVersionResourcesResponseTypeDef",
     "CreateRecommendationTemplateResponseTypeDef",
     "ListRecommendationTemplatesResponseTypeDef",
     "AppComponentComplianceTypeDef",
     "AppAssessmentTypeDef",
     "ListAppComponentRecommendationsResponseTypeDef",
+    "ListAppAssessmentResourceDriftsResponseTypeDef",
     "ListAppComponentCompliancesResponseTypeDef",
     "DescribeAppAssessmentResponseTypeDef",
     "StartAppAssessmentResponseTypeDef",
 )
 
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
 RecommendationItemTypeDef = TypedDict(
     "RecommendationItemTypeDef",
     {
         "alreadyImplemented": NotRequired[bool],
         "excludeReason": NotRequired[ExcludeRecommendationReasonType],
@@ -304,19 +315,19 @@
     "EventSubscriptionTypeDef",
     {
         "eventType": EventTypeType,
         "name": str,
         "snsTopicArn": NotRequired[str],
     },
 )
-PermissionModelTypeDef = TypedDict(
-    "PermissionModelTypeDef",
+PermissionModelOutputTypeDef = TypedDict(
+    "PermissionModelOutputTypeDef",
     {
         "type": PermissionModelTypeType,
-        "crossAccountRoleArns": NotRequired[Sequence[str]],
+        "crossAccountRoleArns": NotRequired[List[str]],
         "invokerRoleName": NotRequired[str],
     },
 )
 AppVersionSummaryTypeDef = TypedDict(
     "AppVersionSummaryTypeDef",
     {
         "appVersion": str,
@@ -346,14 +357,22 @@
         "expectedComplianceStatus": ComplianceStatusType,
         "expectedRpoDescription": NotRequired[str],
         "expectedRpoInSecs": NotRequired[int],
         "expectedRtoDescription": NotRequired[str],
         "expectedRtoInSecs": NotRequired[int],
     },
 )
+PermissionModelTypeDef = TypedDict(
+    "PermissionModelTypeDef",
+    {
+        "type": PermissionModelTypeType,
+        "crossAccountRoleArns": NotRequired[Sequence[str]],
+        "invokerRoleName": NotRequired[str],
+    },
+)
 CreateAppVersionAppComponentRequestRequestTypeDef = TypedDict(
     "CreateAppVersionAppComponentRequestRequestTypeDef",
     {
         "appArn": str,
         "name": str,
         "type": str,
         "additionalInfo": NotRequired[Mapping[str, Sequence[str]]],
@@ -478,14 +497,21 @@
 )
 DescribeResiliencyPolicyRequestRequestTypeDef = TypedDict(
     "DescribeResiliencyPolicyRequestRequestTypeDef",
     {
         "policyArn": str,
     },
 )
+EksSourceOutputTypeDef = TypedDict(
+    "EksSourceOutputTypeDef",
+    {
+        "eksClusterArn": str,
+        "namespaces": List[str],
+    },
+)
 EksSourceTypeDef = TypedDict(
     "EksSourceTypeDef",
     {
         "eksClusterArn": str,
         "namespaces": Sequence[str],
     },
 )
@@ -501,14 +527,30 @@
     "ListAppAssessmentComplianceDriftsRequestRequestTypeDef",
     {
         "assessmentArn": str,
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
 )
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": NotRequired[int],
+        "PageSize": NotRequired[int],
+        "StartingToken": NotRequired[str],
+    },
+)
+ListAppAssessmentResourceDriftsRequestRequestTypeDef = TypedDict(
+    "ListAppAssessmentResourceDriftsRequestRequestTypeDef",
+    {
+        "assessmentArn": str,
+        "maxResults": NotRequired[int],
+        "nextToken": NotRequired[str],
+    },
+)
 ListAppAssessmentsRequestRequestTypeDef = TypedDict(
     "ListAppAssessmentsRequestRequestTypeDef",
     {
         "appArn": NotRequired[str],
         "assessmentName": NotRequired[str],
         "assessmentStatus": NotRequired[Sequence[AssessmentStatusType]],
         "complianceStatus": NotRequired[ComplianceStatusType],
@@ -571,15 +613,15 @@
         "resolutionId": NotRequired[str],
     },
 )
 TimestampTypeDef = Union[datetime, str]
 ListRecommendationTemplatesRequestRequestTypeDef = TypedDict(
     "ListRecommendationTemplatesRequestRequestTypeDef",
     {
-        "assessmentArn": str,
+        "assessmentArn": NotRequired[str],
         "maxResults": NotRequired[int],
         "name": NotRequired[str],
         "nextToken": NotRequired[str],
         "recommendationTemplateArn": NotRequired[str],
         "reverseOrder": NotRequired[bool],
         "status": NotRequired[Sequence[RecommendationTemplateStatusType]],
     },
@@ -928,16 +970,16 @@
 ComplianceDriftTypeDef = TypedDict(
     "ComplianceDriftTypeDef",
     {
         "actualReferenceId": NotRequired[str],
         "actualValue": NotRequired[Dict[DisruptionTypeType, DisruptionComplianceTypeDef]],
         "appId": NotRequired[str],
         "appVersion": NotRequired[str],
-        "diffType": NotRequired[Literal["NotEqual"]],
-        "driftType": NotRequired[Literal["ApplicationCompliance"]],
+        "diffType": NotRequired[DifferenceTypeType],
+        "driftType": NotRequired[DriftTypeType],
         "entityId": NotRequired[str],
         "entityType": NotRequired[str],
         "expectedReferenceId": NotRequired[str],
         "expectedValue": NotRequired[Dict[DisruptionTypeType, DisruptionComplianceTypeDef]],
     },
 )
 CreateAppVersionAppComponentResponseTypeDef = TypedDict(
@@ -1025,48 +1067,23 @@
         "complianceStatus": NotRequired[AppComplianceStatusTypeType],
         "description": NotRequired[str],
         "driftStatus": NotRequired[AppDriftStatusTypeType],
         "eventSubscriptions": NotRequired[List[EventSubscriptionTypeDef]],
         "lastAppComplianceEvaluationTime": NotRequired[datetime],
         "lastDriftEvaluationTime": NotRequired[datetime],
         "lastResiliencyScoreEvaluationTime": NotRequired[datetime],
-        "permissionModel": NotRequired[PermissionModelTypeDef],
+        "permissionModel": NotRequired[PermissionModelOutputTypeDef],
         "policyArn": NotRequired[str],
         "resiliencyScore": NotRequired[float],
         "rpoInSecs": NotRequired[int],
         "rtoInSecs": NotRequired[int],
         "status": NotRequired[AppStatusTypeType],
         "tags": NotRequired[Dict[str, str]],
     },
 )
-CreateAppRequestRequestTypeDef = TypedDict(
-    "CreateAppRequestRequestTypeDef",
-    {
-        "name": str,
-        "assessmentSchedule": NotRequired[AppAssessmentScheduleTypeType],
-        "clientToken": NotRequired[str],
-        "description": NotRequired[str],
-        "eventSubscriptions": NotRequired[Sequence[EventSubscriptionTypeDef]],
-        "permissionModel": NotRequired[PermissionModelTypeDef],
-        "policyArn": NotRequired[str],
-        "tags": NotRequired[Mapping[str, str]],
-    },
-)
-UpdateAppRequestRequestTypeDef = TypedDict(
-    "UpdateAppRequestRequestTypeDef",
-    {
-        "appArn": str,
-        "assessmentSchedule": NotRequired[AppAssessmentScheduleTypeType],
-        "clearResiliencyPolicyArn": NotRequired[bool],
-        "description": NotRequired[str],
-        "eventSubscriptions": NotRequired[Sequence[EventSubscriptionTypeDef]],
-        "permissionModel": NotRequired[PermissionModelTypeDef],
-        "policyArn": NotRequired[str],
-    },
-)
 ListAppVersionsResponseTypeDef = TypedDict(
     "ListAppVersionsResponseTypeDef",
     {
         "appVersions": List[AppVersionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1104,14 +1121,40 @@
         "haArchitecture": NotRequired[HaArchitectureType],
         "recommendationCompliance": NotRequired[
             Dict[DisruptionTypeType, RecommendationDisruptionComplianceTypeDef]
         ],
         "suggestedChanges": NotRequired[List[str]],
     },
 )
+CreateAppRequestRequestTypeDef = TypedDict(
+    "CreateAppRequestRequestTypeDef",
+    {
+        "name": str,
+        "assessmentSchedule": NotRequired[AppAssessmentScheduleTypeType],
+        "clientToken": NotRequired[str],
+        "description": NotRequired[str],
+        "eventSubscriptions": NotRequired[Sequence[EventSubscriptionTypeDef]],
+        "permissionModel": NotRequired[PermissionModelTypeDef],
+        "policyArn": NotRequired[str],
+        "tags": NotRequired[Mapping[str, str]],
+    },
+)
+PermissionModelUnionTypeDef = Union[PermissionModelTypeDef, PermissionModelOutputTypeDef]
+UpdateAppRequestRequestTypeDef = TypedDict(
+    "UpdateAppRequestRequestTypeDef",
+    {
+        "appArn": str,
+        "assessmentSchedule": NotRequired[AppAssessmentScheduleTypeType],
+        "clearResiliencyPolicyArn": NotRequired[bool],
+        "description": NotRequired[str],
+        "eventSubscriptions": NotRequired[Sequence[EventSubscriptionTypeDef]],
+        "permissionModel": NotRequired[PermissionModelTypeDef],
+        "policyArn": NotRequired[str],
+    },
+)
 CreateAppVersionResourceRequestRequestTypeDef = TypedDict(
     "CreateAppVersionResourceRequestRequestTypeDef",
     {
         "appArn": str,
         "appComponents": Sequence[str],
         "logicalResourceId": LogicalResourceIdTypeDef,
         "physicalResourceId": str,
@@ -1143,14 +1186,21 @@
         "awsAccountId": NotRequired[str],
         "awsRegion": NotRequired[str],
         "logicalResourceId": NotRequired[LogicalResourceIdTypeDef],
         "physicalResourceId": NotRequired[str],
         "resourceName": NotRequired[str],
     },
 )
+ResourceIdentifierTypeDef = TypedDict(
+    "ResourceIdentifierTypeDef",
+    {
+        "logicalResourceId": NotRequired[LogicalResourceIdTypeDef],
+        "resourceType": NotRequired[str],
+    },
+)
 UpdateAppVersionResourceRequestRequestTypeDef = TypedDict(
     "UpdateAppVersionResourceRequestRequestTypeDef",
     {
         "appArn": str,
         "additionalInfo": NotRequired[Mapping[str, Sequence[str]]],
         "appComponents": NotRequired[Sequence[str]],
         "awsAccountId": NotRequired[str],
@@ -1195,36 +1245,34 @@
         "dataLocationConstraint": NotRequired[DataLocationConstraintType],
         "policy": NotRequired[Mapping[DisruptionTypeType, FailurePolicyTypeDef]],
         "policyDescription": NotRequired[str],
         "policyName": NotRequired[str],
         "tier": NotRequired[ResiliencyPolicyTierType],
     },
 )
-ImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
-    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
-    {
-        "appArn": str,
-        "eksSources": NotRequired[Sequence[EksSourceTypeDef]],
-        "importStrategy": NotRequired[ResourceImportStrategyTypeType],
-        "sourceArns": NotRequired[Sequence[str]],
-        "terraformSources": NotRequired[Sequence[TerraformSourceTypeDef]],
-    },
-)
 ImportResourcesToDraftAppVersionResponseTypeDef = TypedDict(
     "ImportResourcesToDraftAppVersionResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
-        "eksSources": List[EksSourceTypeDef],
+        "eksSources": List[EksSourceOutputTypeDef],
         "sourceArns": List[str],
         "status": ResourceImportStatusTypeType,
         "terraformSources": List[TerraformSourceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+EksSourceUnionTypeDef = Union[EksSourceTypeDef, EksSourceOutputTypeDef]
+ListAppAssessmentResourceDriftsRequestListAppAssessmentResourceDriftsPaginateTypeDef = TypedDict(
+    "ListAppAssessmentResourceDriftsRequestListAppAssessmentResourceDriftsPaginateTypeDef",
+    {
+        "assessmentArn": str,
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 ListAppVersionsRequestRequestTypeDef = TypedDict(
     "ListAppVersionsRequestRequestTypeDef",
     {
         "appArn": str,
         "endTime": NotRequired[TimestampTypeDef],
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
@@ -1412,14 +1460,24 @@
     "ComponentRecommendationTypeDef",
     {
         "appComponentName": str,
         "configRecommendations": List[ConfigRecommendationTypeDef],
         "recommendationStatus": RecommendationComplianceStatusType,
     },
 )
+ResourceDriftTypeDef = TypedDict(
+    "ResourceDriftTypeDef",
+    {
+        "appArn": NotRequired[str],
+        "appVersion": NotRequired[str],
+        "diffType": NotRequired[DifferenceTypeType],
+        "referenceId": NotRequired[str],
+        "resourceIdentifier": NotRequired[ResourceIdentifierTypeDef],
+    },
+)
 CreateResiliencyPolicyResponseTypeDef = TypedDict(
     "CreateResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1449,14 +1507,24 @@
 UpdateResiliencyPolicyResponseTypeDef = TypedDict(
     "UpdateResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
+    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    {
+        "appArn": str,
+        "eksSources": NotRequired[Sequence[EksSourceUnionTypeDef]],
+        "importStrategy": NotRequired[ResourceImportStrategyTypeType],
+        "sourceArns": NotRequired[Sequence[str]],
+        "terraformSources": NotRequired[Sequence[TerraformSourceTypeDef]],
+    },
+)
 CreateAppVersionResourceResponseTypeDef = TypedDict(
     "CreateAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1584,14 +1652,22 @@
     "ListAppComponentRecommendationsResponseTypeDef",
     {
         "componentRecommendations": List[ComponentRecommendationTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ListAppAssessmentResourceDriftsResponseTypeDef = TypedDict(
+    "ListAppAssessmentResourceDriftsResponseTypeDef",
+    {
+        "nextToken": str,
+        "resourceDrifts": List[ResourceDriftTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ListAppComponentCompliancesResponseTypeDef = TypedDict(
     "ListAppComponentCompliancesResponseTypeDef",
     {
         "componentCompliances": List[AppComponentComplianceTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub/type_defs.pyi` & `mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,18 @@
     AppStatusTypeType,
     AssessmentInvokerType,
     AssessmentStatusType,
     ComplianceStatusType,
     ConfigRecommendationOptimizationTypeType,
     CostFrequencyType,
     DataLocationConstraintType,
+    DifferenceTypeType,
     DisruptionTypeType,
     DriftStatusType,
+    DriftTypeType,
     EstimatedCostTierType,
     EventTypeType,
     ExcludeRecommendationReasonType,
     HaArchitectureType,
     PermissionModelTypeType,
     PhysicalIdentifierTypeType,
     RecommendationComplianceStatusType,
@@ -71,19 +73,20 @@
     "CostTypeDef",
     "DisruptionComplianceTypeDef",
     "AppComponentTypeDef",
     "EksSourceClusterNamespaceTypeDef",
     "TerraformSourceTypeDef",
     "AppSummaryTypeDef",
     "EventSubscriptionTypeDef",
-    "PermissionModelTypeDef",
+    "PermissionModelOutputTypeDef",
     "AppVersionSummaryTypeDef",
     "BatchUpdateRecommendationStatusFailedEntryTypeDef",
     "UpdateRecommendationStatusItemTypeDef",
     "RecommendationDisruptionComplianceTypeDef",
+    "PermissionModelTypeDef",
     "CreateAppVersionAppComponentRequestRequestTypeDef",
     "LogicalResourceIdTypeDef",
     "CreateRecommendationTemplateRequestRequestTypeDef",
     "FailurePolicyTypeDef",
     "DeleteAppAssessmentRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteAppVersionAppComponentRequestRequestTypeDef",
@@ -93,17 +96,20 @@
     "DescribeAppRequestRequestTypeDef",
     "DescribeAppVersionAppComponentRequestRequestTypeDef",
     "DescribeAppVersionRequestRequestTypeDef",
     "DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef",
     "DescribeAppVersionTemplateRequestRequestTypeDef",
     "DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef",
     "DescribeResiliencyPolicyRequestRequestTypeDef",
+    "EksSourceOutputTypeDef",
     "EksSourceTypeDef",
     "ListAlarmRecommendationsRequestRequestTypeDef",
     "ListAppAssessmentComplianceDriftsRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ListAppAssessmentResourceDriftsRequestRequestTypeDef",
     "ListAppAssessmentsRequestRequestTypeDef",
     "ListAppComponentCompliancesRequestRequestTypeDef",
     "ListAppComponentRecommendationsRequestRequestTypeDef",
     "ListAppInputSourcesRequestRequestTypeDef",
     "ListAppVersionAppComponentsRequestRequestTypeDef",
     "ListAppVersionResourceMappingsRequestRequestTypeDef",
     "ListAppVersionResourcesRequestRequestTypeDef",
@@ -152,29 +158,32 @@
     "DescribeAppVersionAppComponentResponseTypeDef",
     "ListAppVersionAppComponentsResponseTypeDef",
     "UpdateAppVersionAppComponentResponseTypeDef",
     "AppInputSourceTypeDef",
     "DeleteAppInputSourceRequestRequestTypeDef",
     "ListAppsResponseTypeDef",
     "AppTypeDef",
-    "CreateAppRequestRequestTypeDef",
-    "UpdateAppRequestRequestTypeDef",
     "ListAppVersionsResponseTypeDef",
     "BatchUpdateRecommendationStatusSuccessfulEntryTypeDef",
     "UpdateRecommendationStatusRequestEntryTypeDef",
     "ConfigRecommendationTypeDef",
+    "CreateAppRequestRequestTypeDef",
+    "PermissionModelUnionTypeDef",
+    "UpdateAppRequestRequestTypeDef",
     "CreateAppVersionResourceRequestRequestTypeDef",
     "DeleteAppVersionResourceRequestRequestTypeDef",
     "DescribeAppVersionResourceRequestRequestTypeDef",
+    "ResourceIdentifierTypeDef",
     "UpdateAppVersionResourceRequestRequestTypeDef",
     "CreateResiliencyPolicyRequestRequestTypeDef",
     "ResiliencyPolicyTypeDef",
     "UpdateResiliencyPolicyRequestRequestTypeDef",
-    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
     "ImportResourcesToDraftAppVersionResponseTypeDef",
+    "EksSourceUnionTypeDef",
+    "ListAppAssessmentResourceDriftsRequestListAppAssessmentResourceDriftsPaginateTypeDef",
     "ListAppVersionsRequestRequestTypeDef",
     "ListAppsRequestRequestTypeDef",
     "PhysicalResourceTypeDef",
     "ResourceMappingTypeDef",
     "UnsupportedResourceTypeDef",
     "RecommendationTemplateTypeDef",
     "ResiliencyScoreTypeDef",
@@ -188,46 +197,49 @@
     "ListAppInputSourcesResponseTypeDef",
     "CreateAppResponseTypeDef",
     "DescribeAppResponseTypeDef",
     "UpdateAppResponseTypeDef",
     "BatchUpdateRecommendationStatusResponseTypeDef",
     "BatchUpdateRecommendationStatusRequestRequestTypeDef",
     "ComponentRecommendationTypeDef",
+    "ResourceDriftTypeDef",
     "CreateResiliencyPolicyResponseTypeDef",
     "DescribeResiliencyPolicyResponseTypeDef",
     "ListResiliencyPoliciesResponseTypeDef",
     "ListSuggestedResiliencyPoliciesResponseTypeDef",
     "UpdateResiliencyPolicyResponseTypeDef",
+    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
     "CreateAppVersionResourceResponseTypeDef",
     "DeleteAppVersionResourceResponseTypeDef",
     "DescribeAppVersionResourceResponseTypeDef",
     "ListAppVersionResourcesResponseTypeDef",
     "UpdateAppVersionResourceResponseTypeDef",
     "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
     "AddDraftAppVersionResourceMappingsResponseTypeDef",
     "ListAppVersionResourceMappingsResponseTypeDef",
     "ListUnsupportedAppVersionResourcesResponseTypeDef",
     "CreateRecommendationTemplateResponseTypeDef",
     "ListRecommendationTemplatesResponseTypeDef",
     "AppComponentComplianceTypeDef",
     "AppAssessmentTypeDef",
     "ListAppComponentRecommendationsResponseTypeDef",
+    "ListAppAssessmentResourceDriftsResponseTypeDef",
     "ListAppComponentCompliancesResponseTypeDef",
     "DescribeAppAssessmentResponseTypeDef",
     "StartAppAssessmentResponseTypeDef",
 )
 
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
 RecommendationItemTypeDef = TypedDict(
     "RecommendationItemTypeDef",
     {
         "alreadyImplemented": NotRequired[bool],
         "excludeReason": NotRequired[ExcludeRecommendationReasonType],
@@ -303,19 +315,19 @@
     "EventSubscriptionTypeDef",
     {
         "eventType": EventTypeType,
         "name": str,
         "snsTopicArn": NotRequired[str],
     },
 )
-PermissionModelTypeDef = TypedDict(
-    "PermissionModelTypeDef",
+PermissionModelOutputTypeDef = TypedDict(
+    "PermissionModelOutputTypeDef",
     {
         "type": PermissionModelTypeType,
-        "crossAccountRoleArns": NotRequired[Sequence[str]],
+        "crossAccountRoleArns": NotRequired[List[str]],
         "invokerRoleName": NotRequired[str],
     },
 )
 AppVersionSummaryTypeDef = TypedDict(
     "AppVersionSummaryTypeDef",
     {
         "appVersion": str,
@@ -345,14 +357,22 @@
         "expectedComplianceStatus": ComplianceStatusType,
         "expectedRpoDescription": NotRequired[str],
         "expectedRpoInSecs": NotRequired[int],
         "expectedRtoDescription": NotRequired[str],
         "expectedRtoInSecs": NotRequired[int],
     },
 )
+PermissionModelTypeDef = TypedDict(
+    "PermissionModelTypeDef",
+    {
+        "type": PermissionModelTypeType,
+        "crossAccountRoleArns": NotRequired[Sequence[str]],
+        "invokerRoleName": NotRequired[str],
+    },
+)
 CreateAppVersionAppComponentRequestRequestTypeDef = TypedDict(
     "CreateAppVersionAppComponentRequestRequestTypeDef",
     {
         "appArn": str,
         "name": str,
         "type": str,
         "additionalInfo": NotRequired[Mapping[str, Sequence[str]]],
@@ -477,14 +497,21 @@
 )
 DescribeResiliencyPolicyRequestRequestTypeDef = TypedDict(
     "DescribeResiliencyPolicyRequestRequestTypeDef",
     {
         "policyArn": str,
     },
 )
+EksSourceOutputTypeDef = TypedDict(
+    "EksSourceOutputTypeDef",
+    {
+        "eksClusterArn": str,
+        "namespaces": List[str],
+    },
+)
 EksSourceTypeDef = TypedDict(
     "EksSourceTypeDef",
     {
         "eksClusterArn": str,
         "namespaces": Sequence[str],
     },
 )
@@ -500,14 +527,30 @@
     "ListAppAssessmentComplianceDriftsRequestRequestTypeDef",
     {
         "assessmentArn": str,
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
 )
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": NotRequired[int],
+        "PageSize": NotRequired[int],
+        "StartingToken": NotRequired[str],
+    },
+)
+ListAppAssessmentResourceDriftsRequestRequestTypeDef = TypedDict(
+    "ListAppAssessmentResourceDriftsRequestRequestTypeDef",
+    {
+        "assessmentArn": str,
+        "maxResults": NotRequired[int],
+        "nextToken": NotRequired[str],
+    },
+)
 ListAppAssessmentsRequestRequestTypeDef = TypedDict(
     "ListAppAssessmentsRequestRequestTypeDef",
     {
         "appArn": NotRequired[str],
         "assessmentName": NotRequired[str],
         "assessmentStatus": NotRequired[Sequence[AssessmentStatusType]],
         "complianceStatus": NotRequired[ComplianceStatusType],
@@ -570,15 +613,15 @@
         "resolutionId": NotRequired[str],
     },
 )
 TimestampTypeDef = Union[datetime, str]
 ListRecommendationTemplatesRequestRequestTypeDef = TypedDict(
     "ListRecommendationTemplatesRequestRequestTypeDef",
     {
-        "assessmentArn": str,
+        "assessmentArn": NotRequired[str],
         "maxResults": NotRequired[int],
         "name": NotRequired[str],
         "nextToken": NotRequired[str],
         "recommendationTemplateArn": NotRequired[str],
         "reverseOrder": NotRequired[bool],
         "status": NotRequired[Sequence[RecommendationTemplateStatusType]],
     },
@@ -927,16 +970,16 @@
 ComplianceDriftTypeDef = TypedDict(
     "ComplianceDriftTypeDef",
     {
         "actualReferenceId": NotRequired[str],
         "actualValue": NotRequired[Dict[DisruptionTypeType, DisruptionComplianceTypeDef]],
         "appId": NotRequired[str],
         "appVersion": NotRequired[str],
-        "diffType": NotRequired[Literal["NotEqual"]],
-        "driftType": NotRequired[Literal["ApplicationCompliance"]],
+        "diffType": NotRequired[DifferenceTypeType],
+        "driftType": NotRequired[DriftTypeType],
         "entityId": NotRequired[str],
         "entityType": NotRequired[str],
         "expectedReferenceId": NotRequired[str],
         "expectedValue": NotRequired[Dict[DisruptionTypeType, DisruptionComplianceTypeDef]],
     },
 )
 CreateAppVersionAppComponentResponseTypeDef = TypedDict(
@@ -1024,48 +1067,23 @@
         "complianceStatus": NotRequired[AppComplianceStatusTypeType],
         "description": NotRequired[str],
         "driftStatus": NotRequired[AppDriftStatusTypeType],
         "eventSubscriptions": NotRequired[List[EventSubscriptionTypeDef]],
         "lastAppComplianceEvaluationTime": NotRequired[datetime],
         "lastDriftEvaluationTime": NotRequired[datetime],
         "lastResiliencyScoreEvaluationTime": NotRequired[datetime],
-        "permissionModel": NotRequired[PermissionModelTypeDef],
+        "permissionModel": NotRequired[PermissionModelOutputTypeDef],
         "policyArn": NotRequired[str],
         "resiliencyScore": NotRequired[float],
         "rpoInSecs": NotRequired[int],
         "rtoInSecs": NotRequired[int],
         "status": NotRequired[AppStatusTypeType],
         "tags": NotRequired[Dict[str, str]],
     },
 )
-CreateAppRequestRequestTypeDef = TypedDict(
-    "CreateAppRequestRequestTypeDef",
-    {
-        "name": str,
-        "assessmentSchedule": NotRequired[AppAssessmentScheduleTypeType],
-        "clientToken": NotRequired[str],
-        "description": NotRequired[str],
-        "eventSubscriptions": NotRequired[Sequence[EventSubscriptionTypeDef]],
-        "permissionModel": NotRequired[PermissionModelTypeDef],
-        "policyArn": NotRequired[str],
-        "tags": NotRequired[Mapping[str, str]],
-    },
-)
-UpdateAppRequestRequestTypeDef = TypedDict(
-    "UpdateAppRequestRequestTypeDef",
-    {
-        "appArn": str,
-        "assessmentSchedule": NotRequired[AppAssessmentScheduleTypeType],
-        "clearResiliencyPolicyArn": NotRequired[bool],
-        "description": NotRequired[str],
-        "eventSubscriptions": NotRequired[Sequence[EventSubscriptionTypeDef]],
-        "permissionModel": NotRequired[PermissionModelTypeDef],
-        "policyArn": NotRequired[str],
-    },
-)
 ListAppVersionsResponseTypeDef = TypedDict(
     "ListAppVersionsResponseTypeDef",
     {
         "appVersions": List[AppVersionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1103,14 +1121,40 @@
         "haArchitecture": NotRequired[HaArchitectureType],
         "recommendationCompliance": NotRequired[
             Dict[DisruptionTypeType, RecommendationDisruptionComplianceTypeDef]
         ],
         "suggestedChanges": NotRequired[List[str]],
     },
 )
+CreateAppRequestRequestTypeDef = TypedDict(
+    "CreateAppRequestRequestTypeDef",
+    {
+        "name": str,
+        "assessmentSchedule": NotRequired[AppAssessmentScheduleTypeType],
+        "clientToken": NotRequired[str],
+        "description": NotRequired[str],
+        "eventSubscriptions": NotRequired[Sequence[EventSubscriptionTypeDef]],
+        "permissionModel": NotRequired[PermissionModelTypeDef],
+        "policyArn": NotRequired[str],
+        "tags": NotRequired[Mapping[str, str]],
+    },
+)
+PermissionModelUnionTypeDef = Union[PermissionModelTypeDef, PermissionModelOutputTypeDef]
+UpdateAppRequestRequestTypeDef = TypedDict(
+    "UpdateAppRequestRequestTypeDef",
+    {
+        "appArn": str,
+        "assessmentSchedule": NotRequired[AppAssessmentScheduleTypeType],
+        "clearResiliencyPolicyArn": NotRequired[bool],
+        "description": NotRequired[str],
+        "eventSubscriptions": NotRequired[Sequence[EventSubscriptionTypeDef]],
+        "permissionModel": NotRequired[PermissionModelTypeDef],
+        "policyArn": NotRequired[str],
+    },
+)
 CreateAppVersionResourceRequestRequestTypeDef = TypedDict(
     "CreateAppVersionResourceRequestRequestTypeDef",
     {
         "appArn": str,
         "appComponents": Sequence[str],
         "logicalResourceId": LogicalResourceIdTypeDef,
         "physicalResourceId": str,
@@ -1142,14 +1186,21 @@
         "awsAccountId": NotRequired[str],
         "awsRegion": NotRequired[str],
         "logicalResourceId": NotRequired[LogicalResourceIdTypeDef],
         "physicalResourceId": NotRequired[str],
         "resourceName": NotRequired[str],
     },
 )
+ResourceIdentifierTypeDef = TypedDict(
+    "ResourceIdentifierTypeDef",
+    {
+        "logicalResourceId": NotRequired[LogicalResourceIdTypeDef],
+        "resourceType": NotRequired[str],
+    },
+)
 UpdateAppVersionResourceRequestRequestTypeDef = TypedDict(
     "UpdateAppVersionResourceRequestRequestTypeDef",
     {
         "appArn": str,
         "additionalInfo": NotRequired[Mapping[str, Sequence[str]]],
         "appComponents": NotRequired[Sequence[str]],
         "awsAccountId": NotRequired[str],
@@ -1194,36 +1245,34 @@
         "dataLocationConstraint": NotRequired[DataLocationConstraintType],
         "policy": NotRequired[Mapping[DisruptionTypeType, FailurePolicyTypeDef]],
         "policyDescription": NotRequired[str],
         "policyName": NotRequired[str],
         "tier": NotRequired[ResiliencyPolicyTierType],
     },
 )
-ImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
-    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
-    {
-        "appArn": str,
-        "eksSources": NotRequired[Sequence[EksSourceTypeDef]],
-        "importStrategy": NotRequired[ResourceImportStrategyTypeType],
-        "sourceArns": NotRequired[Sequence[str]],
-        "terraformSources": NotRequired[Sequence[TerraformSourceTypeDef]],
-    },
-)
 ImportResourcesToDraftAppVersionResponseTypeDef = TypedDict(
     "ImportResourcesToDraftAppVersionResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
-        "eksSources": List[EksSourceTypeDef],
+        "eksSources": List[EksSourceOutputTypeDef],
         "sourceArns": List[str],
         "status": ResourceImportStatusTypeType,
         "terraformSources": List[TerraformSourceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+EksSourceUnionTypeDef = Union[EksSourceTypeDef, EksSourceOutputTypeDef]
+ListAppAssessmentResourceDriftsRequestListAppAssessmentResourceDriftsPaginateTypeDef = TypedDict(
+    "ListAppAssessmentResourceDriftsRequestListAppAssessmentResourceDriftsPaginateTypeDef",
+    {
+        "assessmentArn": str,
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 ListAppVersionsRequestRequestTypeDef = TypedDict(
     "ListAppVersionsRequestRequestTypeDef",
     {
         "appArn": str,
         "endTime": NotRequired[TimestampTypeDef],
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
@@ -1411,14 +1460,24 @@
     "ComponentRecommendationTypeDef",
     {
         "appComponentName": str,
         "configRecommendations": List[ConfigRecommendationTypeDef],
         "recommendationStatus": RecommendationComplianceStatusType,
     },
 )
+ResourceDriftTypeDef = TypedDict(
+    "ResourceDriftTypeDef",
+    {
+        "appArn": NotRequired[str],
+        "appVersion": NotRequired[str],
+        "diffType": NotRequired[DifferenceTypeType],
+        "referenceId": NotRequired[str],
+        "resourceIdentifier": NotRequired[ResourceIdentifierTypeDef],
+    },
+)
 CreateResiliencyPolicyResponseTypeDef = TypedDict(
     "CreateResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1448,14 +1507,24 @@
 UpdateResiliencyPolicyResponseTypeDef = TypedDict(
     "UpdateResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
+    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    {
+        "appArn": str,
+        "eksSources": NotRequired[Sequence[EksSourceUnionTypeDef]],
+        "importStrategy": NotRequired[ResourceImportStrategyTypeType],
+        "sourceArns": NotRequired[Sequence[str]],
+        "terraformSources": NotRequired[Sequence[TerraformSourceTypeDef]],
+    },
+)
 CreateAppVersionResourceResponseTypeDef = TypedDict(
     "CreateAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1583,14 +1652,22 @@
     "ListAppComponentRecommendationsResponseTypeDef",
     {
         "componentRecommendations": List[ComponentRecommendationTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ListAppAssessmentResourceDriftsResponseTypeDef = TypedDict(
+    "ListAppAssessmentResourceDriftsResponseTypeDef",
+    {
+        "nextToken": str,
+        "resourceDrifts": List[ResourceDriftTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ListAppComponentCompliancesResponseTypeDef = TypedDict(
     "ListAppComponentCompliancesResponseTypeDef",
     {
         "componentCompliances": List[AppComponentComplianceTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub.egg-info/PKG-INFO` & `mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resiliencehub
-Version: 1.34.0
-Summary: Type annotations for boto3.ResilienceHub 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.100
+Summary: Type annotations for boto3.ResilienceHub 1.34.100 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/
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
 
 <a id="mypy-boto3-resiliencehub"></a>
 
 # mypy-boto3-resiliencehub
 
 [![PyPI - mypy-boto3-resiliencehub](https://img.shields.io/pypi/v/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resiliencehub)](https://pepy.tech/project/mypy-boto3-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResilienceHub 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[boto3.ResilienceHub 1.34.100](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
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
 [mypy-boto3-resiliencehub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,14 +73,15 @@
     - [Emacs](#emacs)
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
+    - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
     - [Type definitions](#type-definitions)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
@@ -268,14 +269,36 @@
 from mypy_boto3_resiliencehub import ResilienceHubClient
 
 client: ResilienceHubClient = Session().client("resiliencehub")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
+<a id="paginators-annotations"></a>
+
+### Paginators annotations
+
+`mypy_boto3_resiliencehub.paginator` module contains type annotations for all
+paginators.
+
+```python
+from boto3.session import Session
+
+from mypy_boto3_resiliencehub import ResilienceHubClient
+from mypy_boto3_resiliencehub.paginator import ListAppAssessmentResourceDriftsPaginator
+
+client: ResilienceHubClient = Session().client("resiliencehub")
+
+# Explicit type annotations are optional here
+# Types should be correctly discovered by mypy and IDEs
+list_app_assessment_resource_drifts_paginator: ListAppAssessmentResourceDriftsPaginator = (
+    client.get_paginator("list_app_assessment_resource_drifts")
+)
+```
+
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_resiliencehub.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
```

### Comparing `mypy-boto3-resiliencehub-1.34.0/mypy_boto3_resiliencehub.egg-info/SOURCES.txt` & `mypy_boto3_resiliencehub-1.34.100/mypy_boto3_resiliencehub.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 mypy_boto3_resiliencehub/__init__.py
 mypy_boto3_resiliencehub/__init__.pyi
 mypy_boto3_resiliencehub/__main__.py
 mypy_boto3_resiliencehub/client.py
 mypy_boto3_resiliencehub/client.pyi
 mypy_boto3_resiliencehub/literals.py
 mypy_boto3_resiliencehub/literals.pyi
+mypy_boto3_resiliencehub/paginator.py
+mypy_boto3_resiliencehub/paginator.pyi
 mypy_boto3_resiliencehub/py.typed
 mypy_boto3_resiliencehub/type_defs.py
 mypy_boto3_resiliencehub/type_defs.pyi
 mypy_boto3_resiliencehub/version.py
 mypy_boto3_resiliencehub.egg-info/PKG-INFO
 mypy_boto3_resiliencehub.egg-info/SOURCES.txt
 mypy_boto3_resiliencehub.egg-info/dependency_links.txt
```

### Comparing `mypy-boto3-resiliencehub-1.34.0/setup.py` & `mypy_boto3_resiliencehub-1.34.100/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-resiliencehub",
-    version="1.34.0",
+    version="1.34.100",
     packages=["mypy_boto3_resiliencehub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.ResilienceHub 1.34.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
-    ),
+    description="Type annotations for boto3.ResilienceHub 1.34.100 service generated with mypy-boto3-builder 7.24.0",
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
     keywords="boto3 resiliencehub type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_resiliencehub": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

