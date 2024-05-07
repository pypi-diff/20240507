# Comparing `tmp/datasiphon-0.2.2.tar.gz` & `tmp/datasiphon-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasiphon-0.2.2.tar", last modified: Mon Mar  4 08:48:34 2024, max compression
+gzip compressed data, was "datasiphon-0.2.3.tar", last modified: Tue May  7 09:12:53 2024, max compression
```

## Comparing `datasiphon-0.2.2.tar` & `datasiphon-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-03-04 08:48:34.806654 datasiphon-0.2.2/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-03-04 08:48:34.806654 datasiphon-0.2.2/PKG-INFO
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5119 2024-03-04 08:16:45.000000 datasiphon-0.2.2/README.md
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     1318 2024-01-29 12:20:19.000000 datasiphon-0.2.2/pyproject.toml
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)       38 2024-03-04 08:48:34.806654 datasiphon-0.2.2/setup.cfg
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-03-04 08:48:34.805654 datasiphon-0.2.2/src/
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-03-04 08:48:34.806654 datasiphon-0.2.2/src/datasiphon.egg-info/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-03-04 08:48:34.000000 datasiphon-0.2.2/src/datasiphon.egg-info/PKG-INFO
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)      311 2024-03-04 08:48:34.000000 datasiphon-0.2.2/src/datasiphon.egg-info/SOURCES.txt
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)        1 2024-03-04 08:48:34.000000 datasiphon-0.2.2/src/datasiphon.egg-info/dependency_links.txt
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)       33 2024-03-04 08:48:34.000000 datasiphon-0.2.2/src/datasiphon.egg-info/requires.txt
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)        7 2024-03-04 08:48:34.000000 datasiphon-0.2.2/src/datasiphon.egg-info/top_level.txt
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-03-04 08:48:34.806654 datasiphon-0.2.2/src/siphon/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)      211 2024-03-04 08:48:03.000000 datasiphon-0.2.2/src/siphon/__init__.py
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     1125 2024-01-29 12:20:19.000000 datasiphon-0.2.2/src/siphon/base.py
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     4319 2023-12-12 12:45:44.000000 datasiphon-0.2.2/src/siphon/nosql.py
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)    20912 2024-03-04 08:48:03.000000 datasiphon-0.2.2/src/siphon/sql.py
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-03-04 08:48:34.806654 datasiphon-0.2.2/tests/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)    17143 2024-03-04 08:48:03.000000 datasiphon-0.2.2/tests/test_sql.py
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-07 09:12:53.441638 datasiphon-0.2.3/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-07 09:12:53.441638 datasiphon-0.2.3/PKG-INFO
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5119 2024-03-04 08:16:45.000000 datasiphon-0.2.3/README.md
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     1318 2024-01-29 12:20:19.000000 datasiphon-0.2.3/pyproject.toml
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)       38 2024-05-07 09:12:53.441638 datasiphon-0.2.3/setup.cfg
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-07 09:12:53.439638 datasiphon-0.2.3/src/
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-07 09:12:53.441638 datasiphon-0.2.3/src/datasiphon.egg-info/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-07 09:12:53.000000 datasiphon-0.2.3/src/datasiphon.egg-info/PKG-INFO
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)      311 2024-05-07 09:12:53.000000 datasiphon-0.2.3/src/datasiphon.egg-info/SOURCES.txt
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)        1 2024-05-07 09:12:53.000000 datasiphon-0.2.3/src/datasiphon.egg-info/dependency_links.txt
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)       33 2024-05-07 09:12:53.000000 datasiphon-0.2.3/src/datasiphon.egg-info/requires.txt
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)        7 2024-05-07 09:12:53.000000 datasiphon-0.2.3/src/datasiphon.egg-info/top_level.txt
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-07 09:12:53.440638 datasiphon-0.2.3/src/siphon/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)      211 2024-05-07 09:10:52.000000 datasiphon-0.2.3/src/siphon/__init__.py
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     1127 2024-05-07 09:10:36.000000 datasiphon-0.2.3/src/siphon/base.py
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     4314 2024-05-07 09:10:38.000000 datasiphon-0.2.3/src/siphon/nosql.py
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)    22292 2024-05-07 09:10:59.000000 datasiphon-0.2.3/src/siphon/sql.py
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-07 09:12:53.441638 datasiphon-0.2.3/tests/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)    16693 2024-05-07 09:11:07.000000 datasiphon-0.2.3/tests/test_sql.py
```

### Comparing `datasiphon-0.2.2/PKG-INFO` & `datasiphon-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasiphon
-Version: 0.2.2
+Version: 0.2.3
 Summary: Dynamic building of filtered database queries
 Author-email: Marek Nemeth <99m.nemeth@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/Nemulo/libs-datasiphon
 Project-URL: Bug Tracker, https://github.com/Nemulo/libs-datasiphon/issues
 Project-URL: Documentation, https://github.com/Nemulo/libs-datasiphon/blob/main/README.md
 Keywords: database,sql,filtering,query
```

### Comparing `datasiphon-0.2.2/README.md` & `datasiphon-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `datasiphon-0.2.2/pyproject.toml` & `datasiphon-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datasiphon-0.2.2/src/datasiphon.egg-info/PKG-INFO` & `datasiphon-0.2.3/src/datasiphon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasiphon
-Version: 0.2.2
+Version: 0.2.3
 Summary: Dynamic building of filtered database queries
 Author-email: Marek Nemeth <99m.nemeth@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/Nemulo/libs-datasiphon
 Project-URL: Bug Tracker, https://github.com/Nemulo/libs-datasiphon/issues
 Project-URL: Documentation, https://github.com/Nemulo/libs-datasiphon/blob/main/README.md
 Keywords: database,sql,filtering,query
```

### Comparing `datasiphon-0.2.2/src/siphon/base.py` & `datasiphon-0.2.3/src/siphon/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typing as t
 
 
 class QueryBuilder:
-    OPS = ['eq', 'ne', 'gt', 'ge', 'lt', 'le', 'in_', 'nin']
+    OPS = ["eq", "ne", "gt", "ge", "lt", "le", "in_", "nin"]
 
     @staticmethod
     def eq(column: t.Any, value: t.Any) -> t.Any:
         pass
 
     @staticmethod
     def ne(column: t.Any, value: t.Any) -> t.Any:
@@ -56,9 +56,10 @@
 class InvalidOperatorError(SiphonError):
     pass
 
 
 class InvalidValueError(SiphonError):
     pass
 
+
 class InvalidRestrictionModel(SiphonError):
-    pass
+    pass
```

### Comparing `datasiphon-0.2.2/src/siphon/nosql.py` & `datasiphon-0.2.3/src/siphon/nosql.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,49 +5,48 @@
 import typing as t
 
 
 class Mongo(QueryBuilder):
     """
     Mongo query builder
     """
+
     @staticmethod
     def get_arg(model: dict) -> t.Tuple[str, t.Any]:
         """
         Yield the first key-value pair of a dict for mongo document filter
 
         :param model: The model to get the argument from
 
         :return: The first key-value pair of the model
         """
         for key, value in model.items():
             if not isinstance(value, dict):
                 if key in Mongo.OPS:
-                    yield (None, {f'${key}': value})
+                    yield (None, {f"${key}": value})
                 else:
                     yield (key, value)
             else:
                 for k, v in Mongo.get_arg(value):
                     if k is None:
                         yield (key, v)
                     else:
-                        yield (f'{key}.{k}', v)
+                        yield (f"{key}.{k}", v)
 
     @staticmethod
     def validate_fmt(model: dict) -> tuple[dict, dict]:
         """
         Validate the format of the model, also transform operators in model into mongo-filter operators
 
         :param model: The model to validate
 
         :return: The validated and transformed model
         """
         kw = Mongo.get_kw(model)
-        args = {
-            processed_key: processed_value for processed_key, processed_value in Mongo.get_arg(model)
-        }
+        args = {processed_key: processed_value for processed_key, processed_value in Mongo.get_arg(model)}
         return args, kw
 
     @staticmethod
     def get_kw(model: dict) -> dict:
         """
         Get the keyword arguments from the model
 
@@ -76,16 +75,20 @@
 
         :return: The built query
         """
         raise NotImplementedError()  # Noqa
         if not isinstance(collection, pc.Collection):
             raise TypeError(f"Invalid collection: {collection}")
         parsed_model, kw = cls.validate_fmt(model)
-        cursor = collection.find(parsed_model, projection=projection).sort(
-            kw.get('order_by', {})).skip(kw.get('offset', 0)).limit(kw.get('limit', 0))
+        cursor = (
+            collection.find(parsed_model, projection=projection)
+            .sort(kw.get("order_by", {}))
+            .skip(kw.get("offset", 0))
+            .limit(kw.get("limit", 0))
+        )
         return cursor
 
     @classmethod
     def _kw(cls, key: str, value: t.Any) -> t.Any:
         return getattr(cls, key)(value)
 
     @staticmethod
@@ -96,18 +99,15 @@
         :param value: The value to transform
 
         :return: The transformed value
         """
         order_dict = {}
         if not isinstance(value, dict):
             raise FilterFormatError(f"Invalid format: order_by -> {value}")
-        ordering = {
-            'asc': 1,
-            'desc': -1
-        }
+        ordering = {"asc": 1, "desc": -1}
         try:
             for direction, col in value.items():
                 order_dict[col] = ordering[direction]
         except KeyError:
             raise InvalidValueError(f"Invalid value: order_by -> {value}")
         return order_dict
```

### Comparing `datasiphon-0.2.2/src/siphon/sql.py` & `datasiphon-0.2.3/src/siphon/sql.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,61 +1,67 @@
-from .base import QueryBuilder, FilterFormatError, FilterColumnError, InvalidOperatorError, InvalidValueError, InvalidRestrictionModel, SiphonError
+from .base import (
+    QueryBuilder,
+    FilterFormatError,
+    FilterColumnError,
+    InvalidOperatorError,
+    InvalidValueError,
+    InvalidRestrictionModel,
+    SiphonError,
+)
 import sqlalchemy as sa
 import typing as t
 from pydantic import BaseModel, model_validator, ValidationError
 from pydantic.fields import FieldInfo
 import re
 from copy import copy
 from sqlalchemy.sql.base import ReadOnlyColumnCollection
+import datetime as dt
 
 
 class SqlOrderFilter(BaseModel):
     direction: str = None
     column: str = None
 
-    @model_validator(mode='after')
+    @model_validator(mode="after")
     def check_values(self):
         if self.direction is None or self.column is None:
             # Can happen only if created manually
             raise ValueError("Both direction and column must be set")
 
     @classmethod
-    def parse(cls, data: str | list[str]) -> list['SqlOrderFilter']:
+    def parse(cls, data: str | list[str]) -> list["SqlOrderFilter"]:
         """
         Parse the order_by string
 
         :param data: The string to parse
 
         :raises InvalidValueError: If the string is invalid
 
         :return: The parsed string
         """
-        direction_options = {
-            'asc': 'asc',
-            'desc': 'desc',
-            '+': 'asc',
-            '-': 'desc'
-        }
+        direction_options = {"asc": "asc", "desc": "desc", "+": "asc", "-": "desc"}
         # Can happen only if created manually - user error
         if not isinstance(data, (str, list)):
             raise FilterFormatError(
-                f"Invalid value for order_by: {data} - expected string, one of (asc|desc)(<column>), (+|-)(<column>), (<column>).(asc|desc)")
+                f"Invalid value for order_by: {data} - expected string, one of (asc|desc)(<column>), (+|-)(<column>), (<column>).(asc|desc)"
+            )
         if isinstance(data, str):
             data = [data]
         parsed_data = []
         for item in data:
-            if match := re.match(r'(asc|desc)\((.+)\)', item):
+            if match := re.match(r"(asc|desc)\((.+)\)", item):
                 parsed_data.append(cls(direction=match.group(1), column=match.group(2)))
-            elif match := re.match(r'(\+|-)(.+)', item):
+            elif match := re.match(r"(\+|-)(.+)", item):
                 parsed_data.append(cls(direction=direction_options[match.group(1)], column=match.group(2)))
-            elif match := re.match(r'(.+)\.(asc|desc)', item):
+            elif match := re.match(r"(.+)\.(asc|desc)", item):
                 parsed_data.append(cls(direction=direction_options[match.group(2)], column=match.group(1)))
             else:
                 raise InvalidValueError(
-                    f"Invalid value for order_by: {item} - expected one of (asc|desc)(<column>), (+|-)(<column>), (<column>).(asc|desc)")
+                    f"Invalid value for order_by: {item} - expected one of (asc|desc)(<column>), (+|-)(<column>), (<column>).(asc|desc)"
+                )
         return parsed_data
 
 
 class KeywordFilter(BaseModel):
     order_by: list = None
     limit: int = None
     offset: int = None
@@ -107,62 +113,85 @@
         # remove all sql fields from `all_fields`
         for field in sql_fields:
             _ = all_fields.pop(field, None)
         return all_fields
 
     @property
     def filter_order_by(self) -> list[str] | None:
-        return getattr(self, 'order_by', [])
+        return getattr(self, "order_by", [])
 
     @property
     def filter_limit(self) -> bool:
-        return getattr(self, 'limit', False)
+        return getattr(self, "limit", False)
 
     @property
     def filter_offset(self) -> bool:
-        return getattr(self, 'offset', False)
+        return getattr(self, "offset", False)
 
-    @model_validator(mode='after')
+    @model_validator(mode="after")
     def check_values(self):
         """
         Check the values of the model
 
         :raises ValueError: If the model has invalid values
         """
         for field_info in self.sql_fields.values():
             # this validation is strictly for user error - if it happens, it's user error
             if field_info.annotation != list[str]:
                 raise ValueError(
-                    f"Invalid type: {field_info.annotation} for {field_info}, required: list of operators (list[str])")
+                    f"Invalid type: {field_info.annotation} for {field_info}, required: list of operators (list[str])"
+                )
         for keyword_field, field_info in self.sql_keywords.items():
             if field_info.annotation != SQL.__sql_kwargs__[keyword_field]:
                 raise ValueError(
-                    f"Invalid type: {field_info.annotation} for {field_info}, required: {SQL.__sql_kwargs__[keyword_field]}")
+                    f"Invalid type: {field_info.annotation} for {field_info}, required: {SQL.__sql_kwargs__[keyword_field]}"
+                )
+
+
+class FilterTypeParser:
+    """
+    Class for parsing filter types
+    """
+
+    @staticmethod
+    def parse_type(type_: t.Type) -> t.Callable:
+        """
+        Parse the type string
+
+        :param type_str: The string to parse
+
+        :raises ValueError: If the string is invalid
+
+        :return: The parsed string
+        """
+        if type_ in [int, float, str, bool]:
+            return type_
+        elif type_ == dt.datetime:
+            return dt.datetime.fromisoformat
+        else:
+            raise ValueError(f"Unparsable type: {type_}")
 
 
 class FilterBuilder:
-    junctionMapping = {
-        'and': sa.and_,
-        'or': sa.or_
-    }
+    junctionMapping = {"and": sa.and_, "or": sa.or_}
 
     """
     Class for processing incoming filter (parsed by qstion package), no initial fields,
     but storing all incoming fields in extra field
     """
 
     @staticmethod
     def construct_clause(data: dict, query_columns: ReadOnlyColumnCollection) -> list[sa.ColumnElement]:
         current_clause = []
         for key, value in data.items():
             match key:
                 case str() as keyword if keyword in SQL.__sql_kwargs__:
                     # not processing keywords in clause
                     continue
-                case str() as junction if junction in ['and', 'or']:
+                case str() as junction if junction in ["and", "or"]:
                     clause_result = FilterBuilder.construct_clause(value, query_columns)
                     if len(clause_result) == 1:
                         current_clause.append(clause_result[0])
                     else:
                         current_clause.append(FilterBuilder.junctionMapping[junction](*clause_result))
                 case str() as column_name:
                     column = query_columns[column_name]
@@ -173,68 +202,69 @@
     @staticmethod
     def construct_column_clause(column: sa.Column, data: dict) -> sa.ColumnElement:
         current_clause = []
         for key, value in data.items():
             match key:
                 case str() as op if op in SQL.OPS:
                     current_clause.append(SQL._op(op)(column, value))
-                case str() as junction if junction in ['and', 'or']:
+                case str() as junction if junction in ["and", "or"]:
                     clause_result = FilterBuilder.construct_column_clause(column, value)
                     if len(clause_result) == 1:
                         current_clause.append(clause_result[0])
                     else:
                         current_clause.append(FilterBuilder.junctionMapping[junction](*clause_result))
         return current_clause
 
     @staticmethod
     def extract_keywords(data: dict) -> KeywordFilter:
         exported_data = {}
         for item in data:
             match item:
-                case 'order_by':
+                case "order_by":
                     exported_data[item] = SqlOrderFilter.parse(data[item])
-                case 'limit':
+                case "limit":
                     exported_data[item] = data[item]
-                case 'offset':
+                case "offset":
                     exported_data[item] = data[item]
         return KeywordFilter(**exported_data)
 
     @staticmethod
-    def check_values(
-            data: dict, query_columns: ReadOnlyColumnCollection, /, filter_model: RestrictionModel):
+    def check_values(data: dict, query_columns: ReadOnlyColumnCollection, /, filter_model: RestrictionModel):
         """
         Check the values of the model verifying that all fields are valid
 
         :param data: The data to check
 
         :raises ValueError: If the model has invalid values
 
         """
         junction_included = False
         for filter_key, filter_body in data.items():
             match filter_key:
-                case str() as limit_or_offset if limit_or_offset in ['limit', 'offset']:
+                case str() as limit_or_offset if limit_or_offset in ["limit", "offset"]:
                     if not isinstance(filter_body, int):
                         raise FilterFormatError(
-                            f"Invalid value: {filter_body} - expected integer for {limit_or_offset}")
+                            f"Invalid value: {filter_body} - expected integer for {limit_or_offset}"
+                        )
                     if filter_model is not None:
                         if not getattr(filter_model, filter_key, False):
-                            raise FilterColumnError(
-                                f"Usage of keyword disabled by restriction model: {filter_key}")
-                case 'order_by':
+                            raise FilterColumnError(f"Usage of keyword disabled by restriction model: {filter_key}")
+                case "order_by":
                     if not isinstance(filter_body, (list, str)):
                         raise FilterFormatError(
-                            f"Invalid value: {filter_body} - expected list of strings or string for order_by")
+                            f"Invalid value: {filter_body} - expected list of strings or string for order_by"
+                        )
                     parsed_order_by = SqlOrderFilter.parse(filter_body)
                     for order_instance in parsed_order_by:
                         if filter_model is not None:
                             if order_instance.column not in filter_model.filter_order_by:
                                 raise FilterColumnError(
-                                    f"Column filtering disabled by restriction model: {order_instance.column}")
-                case str() as junction if junction in ['and', 'or']:
+                                    f"Column filtering disabled by restriction model: {order_instance.column}"
+                                )
+                case str() as junction if junction in ["and", "or"]:
                     if junction_included:
                         raise FilterFormatError(f"Invalid filter: {filter_key} - expected only one of (and, or)")
                     junction_included = True
                     # do not pass key because it's not column name
                     FilterBuilder.check_nested(filter_body, query_columns, filter_model)
                 case str() as column_name:
                     if filter_key not in query_columns:
@@ -242,77 +272,81 @@
                     if filter_model is not None:
                         if filter_key not in filter_model.sql_fields:
                             raise FilterColumnError(f"Column filtering disabled by restriction model: {filter_key}")
                     FilterBuilder.check_nested(filter_body, query_columns, filter_model, column_name)
                 case _:
                     # nothing else is allowed
                     raise ValueError(
-                        f"Invalid keyword: {filter_key} - expected one of (limit, offset, order_by, and, or) or column name")
+                        f"Invalid keyword: {filter_key} - expected one of (limit, offset, order_by, and, or) or column name"
+                    )
 
     @staticmethod
-    def check_nested(data: dict, query_columns: ReadOnlyColumnCollection, /, filter_model: RestrictionModel,
-                     current_key: str = None) -> None:
+    def check_nested(
+        data: dict, query_columns: ReadOnlyColumnCollection, /, filter_model: RestrictionModel, current_key: str = None
+    ) -> None:
         """
         Check the values of the model verifying that all fields are valid
 
         :param data: The data to check
 
         :raises ValueError: If the model has invalid values
         """
         junction_included = False
         if not isinstance(data, dict):
             raise FilterFormatError(f"Invalid filter: {data} - expected dictionary")
         for key, value in data.items():
             match key:
-                case str() as junction if junction in ['and', 'or']:
+                case str() as junction if junction in ["and", "or"]:
                     if junction_included:
                         raise FilterFormatError(f"Invalid filter: {key} - expected only one of (and, or)")
                     junction_included = True
                     FilterBuilder.check_nested(value, query_columns, filter_model, current_key)
                 case str() as op if op in SQL.OPS:
                     if current_key is None:
                         raise FilterFormatError(
-                            f"Don't have column name to apply operation: {op} - expected column name")
+                            f"Don't have column name to apply operation: {op} - expected column name"
+                        )
                     if filter_model is not None:
-                        if getattr(
-                                filter_model, current_key) != [] and op not in getattr(
-                                filter_model, current_key):
+                        if getattr(filter_model, current_key) != [] and op not in getattr(filter_model, current_key):
                             raise InvalidOperatorError(
-                                f"Invalid operator: {op} - not allowed for column: {current_key}, allowed: {getattr(filter_model, current_key)}")
-                    if op in ['in_', 'nin']:
+                                f"Invalid operator: {op} - not allowed for column: {current_key}, allowed: {getattr(filter_model, current_key)}"
+                            )
+                    if op in ["in_", "nin"]:
                         if not isinstance(value, (list, tuple)):
-                            raise InvalidValueError(
-                                f"Invalid value: {value} - expected list or tuple for {op}")
+                            raise InvalidValueError(f"Invalid value: {value} - expected list or tuple for {op}")
                         # instead of checking if each value has correct type, we will use constructor to do it and catch any type errors with InvalidValueError
                         try:
                             _ = [query_columns[current_key].type.python_type(item) for item in value]
                         except TypeError:
                             raise InvalidValueError(
-                                f"Invalid value type for {current_key}: {value} - expected {query_columns[current_key].type.python_type}")
+                                f"Invalid value type for {current_key}: {value} - expected {query_columns[current_key].type.python_type}"
+                            )
                     else:
                         try:
-                            _ = query_columns[current_key].type.python_type(value)
-                        except TypeError:
+                            parse_func = FilterTypeParser.parse_type(query_columns[current_key].type.python_type)
+                            _ = parse_func(value)
+                        except (TypeError, ValueError):
                             raise InvalidValueError(
-                                f"Cannot construct {current_key}'s {value=} - expected {query_columns[current_key].type.python_type}")
+                                f"Cannot construct {current_key}'s {value=} - expected {query_columns[current_key].type.python_type}"
+                            )
                 case str() as column_name:
                     if current_key is not None:
                         raise FilterFormatError(
-                            f"Invalid filter: {data} - expected one of (and, or) or operator for column: {current_key}, got: {column_name}")
+                            f"Invalid filter: {data} - expected one of (and, or) or operator for column: {current_key}, got: {column_name}"
+                        )
                     else:  # VSCode - Insiders bug showing this as dead code
                         FilterBuilder.check_nested(value, query_columns, filter_model, column_name)
 
 
 class SQL(QueryBuilder):
     """
     SQL query builder
     """
-    __sql_kwargs__ = {
-        'order_by': list[str], 'limit': bool, 'offset': bool
-    }
+
+    __sql_kwargs__ = {"order_by": list[str], "limit": bool, "offset": bool}
 
     @staticmethod
     def dump_query_columns(query: sa.Select) -> ReadOnlyColumnCollection:
         """
         Dump all selected columns to dictionary
 
         :param query: The query to dump
@@ -329,32 +363,35 @@
         :param filter_model: The model to validate
         :param column_collection: The columns to validate against
 
         :raises FilterColumnError: If the model has invalid columns
         """
         # Only for user error - if it happens, it's user error
         if not (isinstance(filter_model, RestrictionModel)):
-            raise InvalidRestrictionModel(
-                f"Invalid type: {type(filter_model)}, required: `RestrictionModel`")
+            raise InvalidRestrictionModel(f"Invalid type: {type(filter_model)}, required: `RestrictionModel`")
         if not set(filter_model.sql_fields.keys()).issubset(set(column_collection.keys())):
             raise InvalidRestrictionModel(
-                f"Invalid column: {set(filter_model.sql_fields.keys()) - set(column_collection.keys())} not found in select statement")
+                f"Invalid column: {set(filter_model.sql_fields.keys()) - set(column_collection.keys())} not found in select statement"
+            )
         for field_name in filter_model.sql_fields:
             # Only for user error - if it happens, it's user error
             if not isinstance(getattr(filter_model, field_name), list):
                 raise InvalidRestrictionModel(
-                    f"Invalid type: {type(getattr(filter_model, field_name))}, required: list")
+                    f"Invalid type: {type(getattr(filter_model, field_name))}, required: list"
+                )
             if not set(getattr(filter_model, field_name)).issubset(set(SQL.OPS)):
                 raise InvalidOperatorError(
-                    f"Invalid operator in filter model: {set(getattr(filter_model, field_name)) - set(SQL.OPS)}")
+                    f"Invalid operator in filter model: {set(getattr(filter_model, field_name)) - set(SQL.OPS)}"
+                )
         # verify that all order_by columns (if present) ar in query columns
         if filter_model.filter_order_by:
             if not set(filter_model.filter_order_by).issubset(set(column_collection.keys())):
                 raise InvalidRestrictionModel(
-                    f"Invalid column: {set(filter_model.filter_order_by) - set(column_collection.keys())} not found in select statement")
+                    f"Invalid column: {set(filter_model.filter_order_by) - set(column_collection.keys())} not found in select statement"
+                )
 
     @classmethod
     def build(cls, query: sa.Select, qs_filter: dict, filter_model: RestrictionModel = None) -> sa.Select:
         """
         Build a SQL query from a model
 
         :param query: The statement to build from
@@ -381,50 +418,58 @@
         query = query.where(*filter_data)
         keyword_data = FilterBuilder.extract_keywords(qs_filter)
         query = keyword_data.apply_on_query(query)
         return query
 
     @staticmethod
     def eq(column: sa.Column, value: t.Any) -> sa.ColumnElement:
-        return column == column.type.python_type(value)
+        process_type_func = FilterTypeParser.parse_type(column.type.python_type)
+        return column == process_type_func(value)
 
     @staticmethod
     def ne(column: sa.Column, value: t.Any) -> sa.ColumnElement:
-        return column != column.type.python_type(value)
+        process_type_func = FilterTypeParser.parse_type(column.type.python_type)
+        return column != process_type_func(value)
 
     @staticmethod
     def gt(column: sa.Column, value: t.Any) -> sa.ColumnElement:
-        return column > column.type.python_type(value)
+        process_type_func = FilterTypeParser.parse_type(column.type.python_type)
+        return column > process_type_func(value)
 
     @staticmethod
     def ge(column: sa.Column, value: t.Any) -> sa.ColumnElement:
-        return column >= column.type.python_type(value)
+        process_type_func = FilterTypeParser.parse_type(column.type.python_type)
+        return column >= process_type_func(value)
 
     @staticmethod
     def lt(column: sa.Column, value: t.Any) -> sa.ColumnElement:
-        return column < column.type.python_type(value)
+        process_type_func = FilterTypeParser.parse_type(column.type.python_type)
+        return column < process_type_func(value)
 
     @staticmethod
     def le(column: sa.Column, value: t.Any) -> sa.ColumnElement:
-        return column <= column.type.python_type(value)
+        process_type_func = FilterTypeParser.parse_type(column.type.python_type)
+        return column <= process_type_func(value)
 
     @staticmethod
     def in_(column: sa.Column, value: t.Any) -> sa.ColumnElement:
+        process_type_func = FilterTypeParser.parse_type(column.type.python_type)
         # last chance to sanitize the value
         if not isinstance(value, (list, tuple)):
-            value = [column.type.python_type(value)]
+            value = [process_type_func(value)]
         else:
             value = [column.type.python_type(item) for item in value]
         return column.in_(value)
 
     @staticmethod
     def nin(column: sa.Column, value: t.Any) -> sa.ColumnElement:
+        process_type_func = FilterTypeParser.parse_type(column.type.python_type)
         # last chance to sanitize the value
         if not isinstance(value, (list, tuple)):
-            value = [column.type.python_type(value)]
+            value = [process_type_func(value)]
         else:
             value = [column.type.python_type(item) for item in value]
         return ~column.in_(value)
 
     @classmethod
     def _kw(cls, kw: str, stm: sa.Select, value: t.Any) -> sa.Select:
         return getattr(cls, kw)(stm, value)
@@ -437,18 +482,15 @@
         :param stm: The statement to apply to
         :param value: The order_by to apply
 
         :raises InvalidOperatorError: If the order_by has an invalid operator
 
         :return: The statement with the order_by applied
         """
-        ordering = {
-            'asc': sa.asc,
-            'desc': sa.desc
-        }
+        ordering = {"asc": sa.asc, "desc": sa.desc}
         for order_instance in values:
             stm = stm.order_by(ordering[order_instance.direction](stm.exported_columns[order_instance.column]))
         return stm
 
     @staticmethod
     def limit(stm: sa.Select, value: int) -> sa.Select:
         """
```

### Comparing `datasiphon-0.2.2/tests/test_sql.py` & `datasiphon-0.2.3/tests/test_sql.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import unittest
 import sys
 import data
 from pydantic import BaseModel
 import sqlalchemy as sa
+
 sys.path.append(".")
 
 # TODO support for ignore and strict keyword deprecated
 
 
 class SQLTest(unittest.TestCase):
 
@@ -14,480 +15,437 @@
         import src.siphon as ds
 
         # Test filtering - format
         # 1. not a select
         with self.assertRaises(ds.base.SiphonError):
             ds.sql.SQL.build(
                 data.test_table,
-                {'name': {'eq': 'John'}},
+                {"name": {"eq": "John"}},
             )
 
         # 2. keyword with invalid value
         with self.assertRaises(ds.sql.FilterFormatError):
             ds.sql.SQL.build(
                 data.tt_select,
-                {'limit': 'John'},
+                {"limit": "John"},
             )
 
         # 3. keyword order_by with invalid value
         with self.assertRaises(ds.sql.InvalidValueError):
             ds.sql.SQL.build(
                 data.tt_select,
-                {'order_by': 'name'},
+                {"order_by": "name"},
             )
 
         # 5. non-keyword with invalid value
         with self.assertRaises(ds.sql.FilterFormatError):
             ds.sql.SQL.build(
                 data.tt_select,
-                {'name': 'John'},
+                {"name": "John"},
             )
 
         # 6. non-operator key
 
         with self.assertRaises(ds.sql.FilterFormatError):
             ds.sql.SQL.build(
                 data.tt_select,
-                {'name': {'invalid': 'John'}},
+                {"name": {"invalid": "John"}},
             )
 
         # Test filtering - columns
         # 1. column not in select
 
         with self.assertRaises(ds.sql.FilterColumnError):
             ds.sql.SQL.build(
                 data.tt_select,
-                {'invalid': {'eq': 'John'}},
+                {"invalid": {"eq": "John"}},
             )
 
         # Test filtering - correct
         # 1. No filter
         self.assertEqual(
             str(ds.sql.SQL.build(data.tt_select, {})),
             str(data.tt_select),
         )
 
         # 2. Simple filter
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select,
-                {'name': {'eq': 'John'}}
-            )),
-            str(data.tt_select.where(data.test_table.c.name == 'John')))
+            str(ds.sql.SQL.build(data.tt_select, {"name": {"eq": "John"}})),
+            str(data.tt_select.where(data.test_table.c.name == "John")),
+        )
 
         # 3. Multiple filters
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select,
-                {'name': {'eq': 'John'}, 'age': {'eq': 20}})
-                ),
-            str(data.tt_select.where(
-                (data.test_table.c.name == 'John') &
-                (data.test_table.c.age == 20))))
+            str(ds.sql.SQL.build(data.tt_select, {"name": {"eq": "John"}, "age": {"eq": 20}})),
+            str(data.tt_select.where((data.test_table.c.name == "John") & (data.test_table.c.age == 20))),
+        )
 
         # 4. keyword limit
 
-        self.assertEqual(
-            str(ds.sql.SQL.build(data.tt_select, {'limit': 3})),
-            str(data.tt_select.limit(3))
-        )
+        self.assertEqual(str(ds.sql.SQL.build(data.tt_select, {"limit": 3})), str(data.tt_select.limit(3)))
 
         # 5. keyword offset
-        self.assertEqual(
-            str(ds.sql.SQL.build(data.tt_select, {'offset': 3})),
-            str(data.tt_select.offset(3))
-        )
+        self.assertEqual(str(ds.sql.SQL.build(data.tt_select, {"offset": 3})), str(data.tt_select.offset(3)))
 
         # 6. keyword order_by
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select, {'order_by': 'name.desc'})),
-            str(data.tt_select.order_by(data.test_table.c.name.desc()))
+            str(ds.sql.SQL.build(data.tt_select, {"order_by": "name.desc"})),
+            str(data.tt_select.order_by(data.test_table.c.name.desc())),
         )
 
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select, {'order_by': 'name.asc'})),
-            str(data.tt_select.order_by(data.test_table.c.name.asc()))
+            str(ds.sql.SQL.build(data.tt_select, {"order_by": "name.asc"})),
+            str(data.tt_select.order_by(data.test_table.c.name.asc())),
         )
 
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select,
-                {'order_by': '+name'})),
-            str(data.tt_select.order_by(data.test_table.c.name.asc())))
+            str(ds.sql.SQL.build(data.tt_select, {"order_by": "+name"})),
+            str(data.tt_select.order_by(data.test_table.c.name.asc())),
+        )
 
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select,
-                {'order_by': '-name'})),
-            str(data.tt_select.order_by(data.test_table.c.name.desc()))
+            str(ds.sql.SQL.build(data.tt_select, {"order_by": "-name"})),
+            str(data.tt_select.order_by(data.test_table.c.name.desc())),
         )
 
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select,
-                {'order_by': 'asc(name)'})),
-            str(data.tt_select.order_by(data.test_table.c.name.asc()))
+            str(ds.sql.SQL.build(data.tt_select, {"order_by": "asc(name)"})),
+            str(data.tt_select.order_by(data.test_table.c.name.asc())),
         )
 
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select,
-                {'order_by': 'desc(name)'})),
-            str(data.tt_select.order_by(data.test_table.c.name.desc()))
+            str(ds.sql.SQL.build(data.tt_select, {"order_by": "desc(name)"})),
+            str(data.tt_select.order_by(data.test_table.c.name.desc())),
         )
 
         # Test every operator
         # 1. eq
 
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select, {'name': {'eq': 'John'}})),
-            str(data.tt_select.where(data.test_table.c.name == 'John')))
+            str(ds.sql.SQL.build(data.tt_select, {"name": {"eq": "John"}})),
+            str(data.tt_select.where(data.test_table.c.name == "John")),
+        )
 
         # 2. ne
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select, {'name': {'ne': 'John'}})),
-            str(data.tt_select.where(data.test_table.c.name != 'John')))
+            str(ds.sql.SQL.build(data.tt_select, {"name": {"ne": "John"}})),
+            str(data.tt_select.where(data.test_table.c.name != "John")),
+        )
 
         # 3. gt
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select, {'age': {'gt': 20}})),
-            str(data.tt_select.where(data.test_table.c.age > 20)))
+            str(ds.sql.SQL.build(data.tt_select, {"age": {"gt": 20}})),
+            str(data.tt_select.where(data.test_table.c.age > 20)),
+        )
 
         # 4. ge
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select, {'age': {'ge': 20}})),
-            str(data.tt_select.where(data.test_table.c.age >= 20)))
+            str(ds.sql.SQL.build(data.tt_select, {"age": {"ge": 20}})),
+            str(data.tt_select.where(data.test_table.c.age >= 20)),
+        )
 
         # 5. lt
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select, {'age': {'lt': 20}})),
-            str(data.tt_select.where(data.test_table.c.age < 20)))
+            str(ds.sql.SQL.build(data.tt_select, {"age": {"lt": 20}})),
+            str(data.tt_select.where(data.test_table.c.age < 20)),
+        )
 
         # 6. le
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select, {'age': {'le': 20}})),
-            str(data.tt_select.where(data.test_table.c.age <= 20)))
+            str(ds.sql.SQL.build(data.tt_select, {"age": {"le": 20}})),
+            str(data.tt_select.where(data.test_table.c.age <= 20)),
+        )
 
         # 7. in_
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select, {'age': {'in_': [20, 21]}})),
-            str(data.tt_select.where(data.test_table.c.age.in_([20, 21]))))
+            str(ds.sql.SQL.build(data.tt_select, {"age": {"in_": [20, 21]}})),
+            str(data.tt_select.where(data.test_table.c.age.in_([20, 21]))),
+        )
 
         # 8. nin
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select, {'age': {'nin': [20, 21]}})),
-            str(data.tt_select.where(~data.test_table.c.age.in_([20, 21]))))
+            str(ds.sql.SQL.build(data.tt_select, {"age": {"nin": [20, 21]}})),
+            str(data.tt_select.where(~data.test_table.c.age.in_([20, 21]))),
+        )
 
         # test filter value is of incorrect type
         # NOTE functionality updated v 0.2.2 - will not raise error, str is convertable to int
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select, {'age': {'eq': '20'}})),
-            str(data.tt_select.where(data.test_table.c.age == 20))
+            str(ds.sql.SQL.build(data.tt_select, {"age": {"eq": "20"}})),
+            str(data.tt_select.where(data.test_table.c.age == 20)),
         )
 
     def test_advanced_select(self):
         import src.siphon as ds
 
         # test combined tables - should raise error since value is of type string
         # NOTE functionality updated v 0.1.0
         # NOTE functionality updated v 0.2.2 - will not raise error, int is convertable to string
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.st_tt_select, {'value': {'in_': [1, 2, 3]}},
-            )),
-            str(data.st_tt_select.where(data.secondary_test.c.value.in_(['1', '2', '3'])))
+            str(
+                ds.sql.SQL.build(
+                    data.st_tt_select,
+                    {"value": {"in_": [1, 2, 3]}},
+                )
+            ),
+            str(data.st_tt_select.where(data.secondary_test.c.value.in_(["1", "2", "3"]))),
         )
 
         # combined tables correct select
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.st_tt_select, {'value': {'in_': ['abc', 'def']}, 'name': {'eq': 'John'}})),
-            str(data.st_tt_select.where(
-                (data.secondary_test.c.value.in_(['abc', 'def'])) &
-                (data.test_table.c.name == 'John')))
+            str(ds.sql.SQL.build(data.st_tt_select, {"value": {"in_": ["abc", "def"]}, "name": {"eq": "John"}})),
+            str(
+                data.st_tt_select.where(
+                    (data.secondary_test.c.value.in_(["abc", "def"])) & (data.test_table.c.name == "John")
+                )
+            ),
         )
 
         # test base table select
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.base_select, {'name': {'eq': 'John'}})),
-            str(data.base_select.where(data.test_table.c.name == 'John'))
+            str(ds.sql.SQL.build(data.base_select, {"name": {"eq": "John"}})),
+            str(data.base_select.where(data.test_table.c.name == "John")),
         )
 
     def test_invalid_inputs(self):
         import src.siphon as ds
 
         # test invalid inputs
         # parsed dict with invalid operators
         with self.assertRaises(ds.base.SiphonError):
-            ds.sql.SQL.build({'name': {'invalid': 'John'}}, ds.sql.SQL, data.tt_select)
+            ds.sql.SQL.build({"name": {"invalid": "John"}}, ds.sql.SQL, data.tt_select)
 
         # parsed dict which is not nested
         with self.assertRaises(ds.base.SiphonError):
-            ds.sql.SQL.build({'name': 'John'}, ds.sql.SQL, data.tt_select)
+            ds.sql.SQL.build({"name": "John"}, ds.sql.SQL, data.tt_select)
 
         # mistyped input
         with self.assertRaises(ds.base.SiphonError):
-            ds.sql.SQL.build({'name[eq': 'John'}, ds.sql.SQL, data.tt_select)
+            ds.sql.SQL.build({"name[eq": "John"}, ds.sql.SQL, data.tt_select)
 
         # order by is not list
         with self.assertRaises(ds.sql.FilterFormatError):
             ds.sql.SQL.build(
                 data.tt_select,
-                {'order_by': {"name.desc": True}},
+                {"order_by": {"name.desc": True}},
             )
 
         # in is not actaully a list
         with self.assertRaises(ds.sql.InvalidValueError):
             ds.sql.SQL.build(
                 data.tt_select,
-                {'age': {'in_': 20}},
+                {"age": {"in_": 20}},
             )
 
     def test_restricted_inputs(self):
         import src.siphon as ds
 
         # simple restriction with no operators
 
         class SimpleUserRestriction(ds.sql.RestrictionModel):
             name: list[str] = []
 
         restriction = SimpleUserRestriction()
         with self.assertRaises(ds.sql.FilterColumnError):
-            ds.sql.SQL.build(data.tt_select, {'age': {'eq': 20}}, filter_model=restriction)
+            ds.sql.SQL.build(data.tt_select, {"age": {"eq": 20}}, filter_model=restriction)
 
         self.assertEqual(
-            str(ds.sql.SQL.build(data.tt_select, {'name': {'eq': 'John'}}, filter_model=restriction)),
-            str(data.tt_select.where(data.test_table.c.name == 'John'))
+            str(ds.sql.SQL.build(data.tt_select, {"name": {"eq": "John"}}, filter_model=restriction)),
+            str(data.tt_select.where(data.test_table.c.name == "John")),
         )
 
         self.assertEqual(
-            str(ds.sql.SQL.build(data.tt_select, {'name': {'in_': ['John', 'Alex']}}, filter_model=restriction)),
-            str(data.tt_select.where(data.test_table.c.name.in_(['John', 'Alex'])))
+            str(ds.sql.SQL.build(data.tt_select, {"name": {"in_": ["John", "Alex"]}}, filter_model=restriction)),
+            str(data.tt_select.where(data.test_table.c.name.in_(["John", "Alex"]))),
         )
 
         # restrictions on filters
         class BaseUserRestriction(ds.sql.RestrictionModel):
-            name: list[str] = ['eq', 'ne']
+            name: list[str] = ["eq", "ne"]
 
         restriction = BaseUserRestriction()
 
         # test restricted select with single order by
         with self.assertRaises(ds.sql.FilterColumnError):
-            ds.sql.SQL.build(data.tt_select, {'order_by': 'name.desc'}, filter_model=restriction)
+            ds.sql.SQL.build(data.tt_select, {"order_by": "name.desc"}, filter_model=restriction)
 
         with self.assertRaises(ds.sql.FilterColumnError):
-            ds.sql.SQL.build(data.tt_select, {'age': {'eq': 20}}, filter_model=restriction)
+            ds.sql.SQL.build(data.tt_select, {"age": {"eq": 20}}, filter_model=restriction)
 
         # test restricted select
         with self.assertRaises(ds.sql.InvalidOperatorError):
-            ds.sql.SQL.build(data.tt_select, {'name': {'in_': 'John'}}, filter_model=restriction)
+            ds.sql.SQL.build(data.tt_select, {"name": {"in_": "John"}}, filter_model=restriction)
 
         class AdvancedUserRestriction(ds.sql.RestrictionModel):
-            name: list[str] = ['eq', 'ne']
-            age: list[str] = ['eq', 'ne', 'in_']
-            value: list[str] = ['in_']
-            order_by: list[str] = ['name', 'age']
+            name: list[str] = ["eq", "ne"]
+            age: list[str] = ["eq", "ne", "in_"]
+            value: list[str] = ["in_"]
+            order_by: list[str] = ["name", "age"]
             limit: bool = True
 
         restriction = AdvancedUserRestriction()
 
         # test restricted select with single order by
         self.assertEqual(
-            str(ds.sql.SQL.build(data.st_tt_select, {'order_by': 'name.desc'}, filter_model=restriction)),
-            str(data.st_tt_select.order_by(data.test_table.c.name.desc()))
+            str(ds.sql.SQL.build(data.st_tt_select, {"order_by": "name.desc"}, filter_model=restriction)),
+            str(data.st_tt_select.order_by(data.test_table.c.name.desc())),
         )
 
         # test restricted select
         self.assertEqual(
-            str(ds.sql.SQL.build(data.st_tt_select, {'name': {'eq': 'John'}}, filter_model=restriction)),
-            str(data.st_tt_select.where(data.test_table.c.name == 'John'))
+            str(ds.sql.SQL.build(data.st_tt_select, {"name": {"eq": "John"}}, filter_model=restriction)),
+            str(data.st_tt_select.where(data.test_table.c.name == "John")),
         )
 
         # test restricted limit
         class LimitRestriction(ds.sql.RestrictionModel):
             limit: bool = False
 
         restriction = LimitRestriction()
 
         with self.assertRaises(ds.sql.FilterColumnError):
-            ds.sql.SQL.build(data.tt_select, {'limit': 3}, filter_model=restriction)
+            ds.sql.SQL.build(data.tt_select, {"limit": 3}, filter_model=restriction)
 
         # test invalid order by column
         with self.assertRaises(ds.sql.FilterColumnError):
-            ds.sql.SQL.build(data.tt_select, {'order_by': 'name.desc'}, filter_model=restriction)
+            ds.sql.SQL.build(data.tt_select, {"order_by": "name.desc"}, filter_model=restriction)
 
         class InvalidRestrictionOperators(ds.sql.RestrictionModel):
-            name: list[str] = ['eq', 'ne', 'invalid']
+            name: list[str] = ["eq", "ne", "invalid"]
 
         restriction = InvalidRestrictionOperators()
 
         with self.assertRaises(ds.sql.InvalidOperatorError):
-            ds.sql.SQL.build(data.tt_select, {'name': {'eq': 'John'}}, filter_model=restriction)
+            ds.sql.SQL.build(data.tt_select, {"name": {"eq": "John"}}, filter_model=restriction)
 
         class InvalidOrderByColumns(ds.sql.RestrictionModel):
-            order_by: list[str] = ['name', 'invalid']
+            order_by: list[str] = ["name", "invalid"]
 
         restriction = InvalidOrderByColumns()
 
         with self.assertRaises(ds.sql.InvalidRestrictionModel):
-            ds.sql.SQL.build(data.tt_select, {'order_by': 'name.desc'}, filter_model=restriction)
+            ds.sql.SQL.build(data.tt_select, {"order_by": "name.desc"}, filter_model=restriction)
 
         class NonExistentCol(ds.sql.RestrictionModel):
-            invalid: list[str] = ['eq', 'ne']
+            invalid: list[str] = ["eq", "ne"]
 
         restriction = NonExistentCol()
 
         with self.assertRaises(ds.sql.InvalidRestrictionModel):
-            ds.sql.SQL.build(data.tt_select, {'invalid': {'eq': 'John'}}, filter_model=restriction)
+            ds.sql.SQL.build(data.tt_select, {"invalid": {"eq": "John"}}, filter_model=restriction)
 
     def test_multiple_order_by(self):
         import src.siphon as ds
 
         # test multiple order by's
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select, {'order_by': ['name.desc', 'age.asc']})),
-            str(data.tt_select.order_by(data.test_table.c.name.desc(), data.test_table.c.age.asc()))
+            str(ds.sql.SQL.build(data.tt_select, {"order_by": ["name.desc", "age.asc"]})),
+            str(data.tt_select.order_by(data.test_table.c.name.desc(), data.test_table.c.age.asc())),
         )
 
         # test multiple order by's with invalid column
         with self.assertRaises(ds.sql.InvalidValueError):
-            ds.sql.SQL.build(
-                data.tt_select, {'order_by': ['name.desc', 'invalid']})
+            ds.sql.SQL.build(data.tt_select, {"order_by": ["name.desc", "invalid"]})
 
         # test multiple order by's with invalid operator
         with self.assertRaises(ds.sql.InvalidValueError):
-            ds.sql.SQL.build(
-                data.tt_select, {'order_by': ['name.desc', 'age.invalid']})
+            ds.sql.SQL.build(data.tt_select, {"order_by": ["name.desc", "age.invalid"]})
 
     def test_and_or_junctions(self):
         import src.siphon as ds
 
         # simple and junction
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select, {'and': {'name': {'eq': 'John'}, 'age': {'eq': 20}}})
-                ),
-            str(data.tt_select.where(
-                (data.test_table.c.name == 'John') & (data.test_table.c.age == 20))
-                )
+            str(ds.sql.SQL.build(data.tt_select, {"and": {"name": {"eq": "John"}, "age": {"eq": 20}}})),
+            str(data.tt_select.where((data.test_table.c.name == "John") & (data.test_table.c.age == 20))),
         )
 
         # simple or junction
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select, {'or': {'name': {'eq': 'John'}, 'age': {'eq': 20}}})
-                ),
-            str(data.tt_select.where(
-                (data.test_table.c.name == 'John') | (data.test_table.c.age == 20))
-                )
+            str(ds.sql.SQL.build(data.tt_select, {"or": {"name": {"eq": "John"}, "age": {"eq": 20}}})),
+            str(data.tt_select.where((data.test_table.c.name == "John") | (data.test_table.c.age == 20))),
         )
 
         # test stacked and junctions - which logically results in simple junction
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select, {'and': {'and': {'name': {'eq': 'John'}, 'age': {'eq': 20}}}})
-                ),
-            str(data.tt_select.where(
-                (data.test_table.c.name == 'John') & (data.test_table.c.age == 20))
-                )
+            str(ds.sql.SQL.build(data.tt_select, {"and": {"and": {"name": {"eq": "John"}, "age": {"eq": 20}}}})),
+            str(data.tt_select.where((data.test_table.c.name == "John") & (data.test_table.c.age == 20))),
         )
 
         # test stacked or junctions - which logically results in simple junction
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select, {'or': {'or': {'name': {'eq': 'John'}}}})
-                ),
-            str(data.tt_select.where(
-                (data.test_table.c.name == 'John'))
-                )
+            str(ds.sql.SQL.build(data.tt_select, {"or": {"or": {"name": {"eq": "John"}}}})),
+            str(data.tt_select.where((data.test_table.c.name == "John"))),
         )
 
         # test multiple junctions on same level
         with self.assertRaises(ds.sql.FilterFormatError):
-            ds.sql.SQL.build(
-                data.tt_select, {'and': {'name': {'eq': 'John'}}, 'or': {'age': {'eq': 20}}}
-            )
+            ds.sql.SQL.build(data.tt_select, {"and": {"name": {"eq": "John"}}, "or": {"age": {"eq": 20}}})
 
         # test multiple junctions on same nested level
         with self.assertRaises(ds.sql.FilterFormatError):
-            ds.sql.SQL.build(
-                data.tt_select, {'name': {'and': {'eq': 'John', 'ne': 'John'}, 'or': {'age': {'eq': 20}}}}
-            )
+            ds.sql.SQL.build(data.tt_select, {"name": {"and": {"eq": "John", "ne": "John"}, "or": {"age": {"eq": 20}}}})
 
         # test nested junction with missing column name
         with self.assertRaises(ds.sql.FilterFormatError):
-            ds.sql.SQL.build(
-                data.tt_select, {'or': {'eq': 'John', 'ne': 'John'}, 'age': {'eq': 20}}
-            )
+            ds.sql.SQL.build(data.tt_select, {"or": {"eq": "John", "ne": "John"}, "age": {"eq": 20}})
 
         # test nested junction
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select, {'name': {'or': {'eq': 'John', 'ne': 'John'}}, 'age': {'eq': 20}}
-            )),
-            str(data.tt_select.where(
-                ((data.test_table.c.name == 'John') | (data.test_table.c.name != 'John')) & (data.test_table.c.age == 20))
+            str(ds.sql.SQL.build(data.tt_select, {"name": {"or": {"eq": "John", "ne": "John"}}, "age": {"eq": 20}})),
+            str(
+                data.tt_select.where(
+                    ((data.test_table.c.name == "John") | (data.test_table.c.name != "John"))
+                    & (data.test_table.c.age == 20)
                 )
+            ),
         )
 
         # test nested single
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select, {'name': {'or': {'eq': 'John'}}}
-            )),
-            str(data.tt_select.where(
-                (data.test_table.c.name == 'John'))
-                )
+            str(ds.sql.SQL.build(data.tt_select, {"name": {"or": {"eq": "John"}}})),
+            str(data.tt_select.where((data.test_table.c.name == "John"))),
         )
 
         # test extremely nested junction
         self.assertEqual(
-            str(ds.sql.SQL.build(
-                data.tt_select,
-                {
-                    'or': {
-                        'name': {
-                            'or': {
-                                'and': {
-                                    'eq': 'John',
-                                    'ne': 'John'
-                                },
-                                'gt': 'Alex'
-                            },
-                            'eq': 'John'
-                        },
-                        'age': {'eq': 20}
-                    }
-                },
-            )),
-            str(data.tt_select.where(
-                sa.or_(
+            str(
+                ds.sql.SQL.build(
+                    data.tt_select,
+                    {
+                        "or": {
+                            "name": {"or": {"and": {"eq": "John", "ne": "John"}, "gt": "Alex"}, "eq": "John"},
+                            "age": {"eq": 20},
+                        }
+                    },
+                )
+            ),
+            str(
+                data.tt_select.where(
                     sa.or_(
-                        sa.and_(
-                            data.test_table.c.name == 'John',
-                            data.test_table.c.name != 'John'
+                        sa.or_(
+                            sa.and_(data.test_table.c.name == "John", data.test_table.c.name != "John"),
+                            data.test_table.c.name > "Alex",
                         ),
-                        data.test_table.c.name > 'Alex'
-                    ),
-                    data.test_table.c.name == 'John',
-                    data.test_table.c.age == 20
+                        data.test_table.c.name == "John",
+                        data.test_table.c.age == 20,
+                    )
                 )
-            )
-            )
+            ),
+        )
+
+    def test_parse_time_stamp_from_str(self):
+        import src.siphon as ds
+
+        # test invalid time stamp
+        with self.assertRaises(ds.sql.InvalidValueError):
+            ds.sql.SQL.build(data.timestamp_table_select, {"created_at": {"eq": "2021-0101 12:00:00"}})
+
+        # test valid time stamp
+        self.assertEqual(
+            str(ds.sql.SQL.build(data.timestamp_table_select, {"created_at": {"eq": "2021-01-01T12:00:00"}})),
+            str(data.timestamp_table_select.where(data.table_with_time_stamp.c.created_at == "2021-01-01T12:00:00")),
         )
 
 
 if __name__ == "__main__":
     unittest.main()
```

