# Comparing `tmp/fastapi_filter-1.1.0.tar.gz` & `tmp/fastapi_filter-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_filter-1.1.0.tar", max compression
+gzip compressed data, was "fastapi_filter-2.0.0.tar", max compression
```

## Comparing `fastapi_filter-1.1.0.tar` & `fastapi_filter-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2024-01-04 21:52:51.528231 fastapi_filter-1.1.0/LICENSE
--rw-r--r--   0        0        0     1935 2024-01-04 21:52:51.528231 fastapi_filter-1.1.0/README.md
--rw-r--r--   0        0        0      107 2024-01-04 21:52:51.532231 fastapi_filter-1.1.0/fastapi_filter/__init__.py
--rw-r--r--   0        0        0        0 2024-01-04 21:52:51.532231 fastapi_filter-1.1.0/fastapi_filter/base/__init__.py
--rw-r--r--   0        0        0     9059 2024-01-04 21:52:51.532231 fastapi_filter-1.1.0/fastapi_filter/base/filter.py
--rw-r--r--   0        0        0        0 2024-01-04 21:52:51.532231 fastapi_filter-1.1.0/fastapi_filter/contrib/__init__.py
--rw-r--r--   0        0        0       50 2024-01-04 21:52:51.532231 fastapi_filter-1.1.0/fastapi_filter/contrib/mongoengine/__init__.py
--rw-r--r--   0        0        0     2770 2024-01-04 21:52:51.532231 fastapi_filter-1.1.0/fastapi_filter/contrib/mongoengine/filter.py
--rw-r--r--   0        0        0       50 2024-01-04 21:52:51.532231 fastapi_filter-1.1.0/fastapi_filter/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     4782 2024-01-04 21:52:51.532231 fastapi_filter-1.1.0/fastapi_filter/contrib/sqlalchemy/filter.py
--rw-r--r--   0        0        0        0 2024-01-04 21:52:51.532231 fastapi_filter-1.1.0/fastapi_filter/py.typed
--rw-r--r--   0        0        0     3178 2024-01-04 21:52:51.532231 fastapi_filter-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3180 1970-01-01 00:00:00.000000 fastapi_filter-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-07 19:13:39.481577 fastapi_filter-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1935 2024-05-07 19:13:39.481577 fastapi_filter-2.0.0/README.md
+-rw-r--r--   0        0        0      107 2024-05-07 19:13:39.481577 fastapi_filter-2.0.0/fastapi_filter/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:13:39.481577 fastapi_filter-2.0.0/fastapi_filter/base/__init__.py
+-rw-r--r--   0        0        0     8713 2024-05-07 19:13:39.481577 fastapi_filter-2.0.0/fastapi_filter/base/filter.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:13:39.481577 fastapi_filter-2.0.0/fastapi_filter/contrib/__init__.py
+-rw-r--r--   0        0        0       50 2024-05-07 19:13:39.481577 fastapi_filter-2.0.0/fastapi_filter/contrib/mongoengine/__init__.py
+-rw-r--r--   0        0        0     2770 2024-05-07 19:13:39.481577 fastapi_filter-2.0.0/fastapi_filter/contrib/mongoengine/filter.py
+-rw-r--r--   0        0        0       50 2024-05-07 19:13:39.481577 fastapi_filter-2.0.0/fastapi_filter/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     4758 2024-05-07 19:13:39.481577 fastapi_filter-2.0.0/fastapi_filter/contrib/sqlalchemy/filter.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:13:39.481577 fastapi_filter-2.0.0/fastapi_filter/py.typed
+-rw-r--r--   0        0        0     3511 2024-05-07 19:13:39.485577 fastapi_filter-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3130 1970-01-01 00:00:00.000000 fastapi_filter-2.0.0/PKG-INFO
```

### Comparing `fastapi_filter-1.1.0/LICENSE` & `fastapi_filter-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_filter-1.1.0/README.md` & `fastapi_filter-2.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # FastAPI filter
 
 ## Compatibility
 
 **Required:**
 
-- Python: >=3.8, <4.0
+- Python: >=3.9, <4.0
 - Fastapi: >=0.100, <1.0
 - Pydantic: >=2.0.0, <3.0.0
 
 **Optional**
 
 - MongoEngine: >=0.24.1, <0.28.0
 - SQLAlchemy: >=1.4.36, <2.1.0
```

### Comparing `fastapi_filter-1.1.0/fastapi_filter/base/filter.py` & `fastapi_filter-2.0.0/fastapi_filter/base/filter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import sys
 from collections import defaultdict
+from collections.abc import Iterable
 from copy import deepcopy
-from typing import Any, Dict, Iterable, List, Optional, Tuple, Type, Union, get_args, get_origin
+from typing import Any, Optional, Union, get_args, get_origin
 
 from fastapi import Depends
 from fastapi.exceptions import RequestValidationError
 from pydantic import BaseModel, ConfigDict, ValidationError, ValidationInfo, create_model, field_validator
 from pydantic.fields import FieldInfo
 
-UNION_TYPES: List = [Union]
+UNION_TYPES: list = [Union]
 
 if sys.version_info >= (3, 10):
     from types import UnionType
 
     UNION_TYPES.append(UnionType)
 
 
@@ -40,20 +41,20 @@
     ## Query string examples:
 
         >>> "?my_field__gt=12&my_other_field=Tomato"
         >>> "?my_field__in=12,13,15&my_other_field__not_in=Tomato,Pepper"
     """
 
     class Constants:  # pragma: no cover
-        model: Type
+        model: Any
         ordering_field_name: str = "order_by"
-        search_model_fields: List[str]
+        search_model_fields: list[str]
         search_field_name: str = "search"
         prefix: str
-        original_filter: Type["BaseFilterModel"]
+        original_filter: type["BaseFilterModel"]
 
     def filter(self, query):  # pragma: no cover
         ...
 
     @property
     def filtering_fields(self):
         fields = self.model_dump(exclude_none=True, exclude_unset=True)
@@ -123,15 +124,15 @@
                 f"Field names can appear at most once for {cls.Constants.ordering_field_name}. "
                 f"The following was ambiguous: {ambiguous_field_names}."
             )
 
         return value
 
 
-def with_prefix(prefix: str, Filter: Type[BaseFilterModel]) -> Type[BaseFilterModel]:
+def with_prefix(prefix: str, Filter: type[BaseFilterModel]) -> type[BaseFilterModel]:
     """Allow re-using existing filter under a prefix.
 
     Example:
         ```python
         from pydantic import BaseModel
 
         from fastapi_filter.filter import FilterDepends
@@ -178,16 +179,16 @@
 
     NestedFilter.Constants.prefix = prefix
     NestedFilter.Constants.original_filter = Filter
 
     return NestedFilter
 
 
-def _list_to_str_fields(Filter: Type[BaseFilterModel]):
-    ret: Dict[str, Tuple[Union[object, Type], Optional[FieldInfo]]] = {}
+def _list_to_str_fields(Filter: type[BaseFilterModel]):
+    ret: dict[str, tuple[Union[object, type], Optional[FieldInfo]]] = {}
     for name, f in Filter.model_fields.items():
         field_info = deepcopy(f)
         annotation = f.annotation
 
         if get_origin(annotation) in UNION_TYPES:
             annotation_args: list = list(get_args(f.annotation))
             if type(None) in annotation_args:
@@ -207,41 +208,35 @@
             ret[name] = (str if f.is_required() else Optional[str], field_info)
         else:
             ret[name] = (f.annotation, field_info)
 
     return ret
 
 
-def FilterDepends(Filter: Type[BaseFilterModel], *, by_alias: bool = False, use_cache: bool = True) -> Any:
+def FilterDepends(Filter: type[BaseFilterModel], *, by_alias: bool = False, use_cache: bool = True) -> Any:
     """Use a hack to support lists in filters.
 
     FastAPI doesn't support it yet: https://github.com/tiangolo/fastapi/issues/50
 
     What we do is loop through the fields of a filter and change any `list` field to a `str` one so that it won't be
     excluded from the possible query parameters.
 
     When we apply the filter, we build the original filter to properly validate the data (i.e. can the string be parsed
     and formatted as a list of <type>?)
     """
     fields = _list_to_str_fields(Filter)
-    GeneratedFilter: Type[BaseFilterModel] = create_model(Filter.__class__.__name__, **fields)
+    GeneratedFilter: type[BaseFilterModel] = create_model(Filter.__class__.__name__, **fields)
 
     class FilterWrapper(GeneratedFilter):  # type: ignore[misc,valid-type]
         def __new__(cls, *args, **kwargs):
             try:
                 instance = GeneratedFilter(*args, **kwargs)
                 data = instance.model_dump(exclude_unset=True, exclude_defaults=True, by_alias=by_alias)
                 if original_filter := getattr(Filter.Constants, "original_filter", None):
                     prefix = f"{Filter.Constants.prefix}__"
-                    stripped = {}
-                    # TODO: replace with `removeprefix` when python 3.8 is no longer supported
-                    # stripped = {k.removeprefix(NestedFilter.Constants.prefix): v for k, v in value.items()}
-                    for k, v in data.items():
-                        if k.startswith(prefix):
-                            k = k.replace(prefix, "", 1)
-                        stripped[k] = v
+                    stripped = {k.removeprefix(prefix): v for k, v in data.items()}
                     return original_filter(**stripped)
                 return Filter(**data)
             except ValidationError as e:
                 raise RequestValidationError(e.errors()) from e
 
     return Depends(FilterWrapper)
```

### Comparing `fastapi_filter-1.1.0/fastapi_filter/contrib/mongoengine/filter.py` & `fastapi_filter-2.0.0/fastapi_filter/contrib/mongoengine/filter.py`

 * *Files identical despite different names*

### Comparing `fastapi_filter-1.1.0/fastapi_filter/contrib/sqlalchemy/filter.py` & `fastapi_filter-2.0.0/fastapi_filter/contrib/sqlalchemy/filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from enum import Enum
 from typing import Union
 from warnings import warn
 
 from pydantic import ValidationInfo, field_validator
 from sqlalchemy import or_
 from sqlalchemy.orm import Query
```

### Comparing `fastapi_filter-1.1.0/pyproject.toml` & `fastapi_filter-2.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -24,117 +24,127 @@
   "bson.objectid",
   "mongoengine.*",
   "uvicorn.*",
 ]
 ignore_missing_imports = true
 
 [tool.ruff]
+line-length = 120
+# Assume Python 3.9 to be compatible with typing.
+target-version = "py39"
+# Exclude a variety of commonly ignored directories.
+exclude = [
+    ".git",
+    ".mypy_cache",
+    ".nox",
+    ".ruff_cache",
+]
+
+
+[tool.ruff.lint]
 select = [
   "A",
   "B",
   "C",
   "D",
   "E",
-  "F"
+  "F",
+  "I",
+  "SIM",
+  "UP",
 ]
 ignore = [
   "A003",  # Argument name should be lowercase.
   "B008",  # Do not perform function calls in argument defaults.
   "D1",  # Missing docstring https://www.pydocstyle.org/en/2.1.1/error_codes.html.
   "D203",  # 1 blank line required before class docstring.
   "D213",  # Multi-line docstring summary should start at the second line.
 ]
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 fixable = ["A", "B", "C", "D", "E", "F"]
 unfixable = []
 
-# Exclude a variety of commonly ignored directories.
-exclude = [
-    ".git",
-    ".mypy_cache",
-    ".nox",
-    ".ruff_cache",
-]
-
-line-length = 120
-
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
-# Assume Python 3.12.
-target-version = "py312"
-
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
+[tool.ruff.format]
+# Like Black, use double quotes for strings.
+quote-style = "double"
+# Like Black, indent with spaces, rather than tabs.
+indent-style = "space"
+# Like Black, respect magic trailing commas.
+skip-magic-trailing-comma = false
+# Like Black, automatically detect the appropriate line ending.
+line-ending = "auto"
+
 [tool.poetry]
 name = "fastapi-filter"
-version = "1.1.0"
+version = "2.0.0"
 description = "FastAPI filter"
 authors = ["Arthur Rio <arthur.rio44@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/arthurio/fastapi-filter"
 classifiers = [
     "Natural Language :: English",
     "Framework :: FastAPI",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
 ]
 
 [tool.poetry.dependencies]
 SQLAlchemy = {version = ">=1.4.36,<2.1.0", optional = true}
 fastapi = ">=0.100.0,<1.0"
 mongoengine = {version = ">=0.24.1,<0.28.0", optional = true}
 pydantic = ">=2.0.0,<3.0.0"
-python = ">=3.8,<4.0"
+python = ">=3.9,<4.0"
 
 [tool.poetry.dev-dependencies]
-Faker = "^20.0.0"
+Faker = "^22.7.0"
 SQLAlchemy-Utils = "^0.41.0"
 aiosqlite = "^0.19.0"
-bandit = "^1.7.5"
-black = "^23.1.0"
-flynt = "^1.0.0"
-greenlet = "^3.0.0"
-httpx = "^0.25.0"
-ipython = "^8.11.0"
-isort = "^5.12.0"
-mkdocs-material = "^9.1.2"
-mypy = "^1.1"
+bandit = "^1.7.8"
+flynt = "^1.0.1"
+greenlet = "^3.0.3"
+httpx = "^0.26.0"
+ipython = "^8.11.0,<8.24.0"
+mkdocs-material = "^9.5.21"
+mypy = "^1.10.0"
 mypy-extensions = "^1.0.0"
-pre-commit = "^3.1.1"
-pudb = "^2022.1.3"
-pytest = "^7.2.2"
+pre-commit = "^3.7.0"
+pudb = "^2024.1"
+pytest = "^7.4.4"
 pytest-asyncio = "^0.23.0"
-pytest-cov = "^4.0.0"
+pytest-cov = "^4.1.0"
 pytest-pudb = "^0.7.0"
-python-lsp-server = "^1.7.4"
-requests = "^2.28.2"
+python-lsp-server = "^1.11.0"
+requests = "^2.31.0"
 tomli = "^2.0.1"
 types-click = "^7.1.8"
-types-setuptools = "^68.1.0.0"
-typing-extensions = "^4.5.0"
-uvicorn = "^0.24.0"
-pydantic = {extras = ["email"], version="^2.0.0"}
+types-setuptools = "^68.2.0.2"
+typing-extensions = "^4.11.0"
+uvicorn = "^0.29.0"
+pydantic = {extras = ["email"], version="^2.7.1"}
 
 [tool.poetry.extras]
 mongoengine = ["mongoengine"]
 sqlalchemy = ["SQLAlchemy"]
 all = ["mongoengine", "SQLAlchemy"]
 
 [tool.poetry.group.dev.dependencies]
 nox = "^2023.0.0"
-ruff = "^0.1.0"
-urllib3 = "<=2.0"
+ruff = "^0.4.0"
+urllib3 = "<=2.1.0"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `fastapi_filter-1.1.0/PKG-INFO` & `fastapi_filter-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: fastapi-filter
-Version: 1.1.0
+Version: 2.0.0
 Summary: FastAPI filter
 Home-page: https://github.com/arthurio/fastapi-filter
 License: MIT
 Author: Arthur Rio
 Author-email: arthur.rio44@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Framework :: FastAPI
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Provides-Extra: all
 Provides-Extra: mongoengine
@@ -36,15 +35,15 @@
 
 # FastAPI filter
 
 ## Compatibility
 
 **Required:**
 
-- Python: >=3.8, <4.0
+- Python: >=3.9, <4.0
 - Fastapi: >=0.100, <1.0
 - Pydantic: >=2.0.0, <3.0.0
 
 **Optional**
 
 - MongoEngine: >=0.24.1, <0.28.0
 - SQLAlchemy: >=1.4.36, <2.1.0
```

