# Comparing `tmp/redis_om-0.3.0.tar.gz` & `tmp/redis_om-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_om-0.3.0.tar", max compression
+gzip compressed data, was "redis_om-0.3.1.tar", max compression
```

## Comparing `redis_om-0.3.0.tar` & `redis_om-0.3.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1071 2024-05-02 14:37:48.558696 redis_om-0.3.0/LICENSE
--rw-r--r--   0        0        0    13159 2024-05-02 14:37:48.558696 redis_om-0.3.0/README.md
--rw-r--r--   0        0        0      463 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/__init__.py
--rw-r--r--   0        0        0     2995 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/_compat.py
--rw-r--r--   0        0        0       35 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/async_redis.py
--rw-r--r--   0        0        0      751 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/checks.py
--rw-r--r--   0        0        0      524 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/connections.py
--rw-r--r--   0        0        0      223 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/model/__init__.py
--rw-r--r--   0        0        0        0 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/model/cli/__init__.py
--rw-r--r--   0        0        0      448 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/model/cli/migrate.py
--rw-r--r--   0        0        0     6544 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/model/encoders.py
--rw-r--r--   0        0        0        0 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/model/migrations/__init__.py
--rw-r--r--   0        0        0     5204 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/model/migrations/migrator.py
--rw-r--r--   0        0        0    77675 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/model/model.py
--rw-r--r--   0        0        0     2230 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/model/query_resolver.py
--rw-r--r--   0        0        0     2246 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/model/render_tree.py
--rw-r--r--   0        0        0      855 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/model/token_escaper.py
--rw-r--r--   0        0        0       13 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/sync_redis.py
--rw-r--r--   0        0        0      234 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/util.py
--rw-r--r--   0        0        0     3717 2024-05-02 14:37:48.558696 redis_om-0.3.0/docs/connections.md
--rw-r--r--   0        0        0     6704 2024-05-02 14:37:48.558696 redis_om-0.3.0/docs/errors.md
--rw-r--r--   0        0        0     7510 2024-05-02 14:37:48.558696 redis_om-0.3.0/docs/fastapi_integration.md
--rw-r--r--   0        0        0    21897 2024-05-02 14:37:48.558696 redis_om-0.3.0/docs/getting_started.md
--rw-r--r--   0        0        0      973 2024-05-02 14:37:48.558696 redis_om-0.3.0/docs/index.md
--rw-r--r--   0        0        0    11595 2024-05-02 14:37:48.558696 redis_om-0.3.0/docs/models.md
--rw-r--r--   0        0        0     1674 2024-05-02 14:37:48.562696 redis_om-0.3.0/docs/redis_modules.md
--rw-r--r--   0        0        0     3688 2024-05-02 14:37:48.562696 redis_om-0.3.0/docs/validation.md
--rw-r--r--   0        0        0     3577 2024-05-02 14:37:48.562696 redis_om-0.3.0/images/logo.svg
--rw-r--r--   0        0        0     1931 2024-05-02 14:37:48.986699 redis_om-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      462 2024-05-02 14:38:20.770891 redis_om-0.3.0/redis_om/__init__.py
--rw-r--r--   0        0        0     2995 2024-05-02 14:38:20.774891 redis_om-0.3.0/redis_om/_compat.py
--rw-r--r--   0        0        0       35 2024-05-02 14:38:20.770891 redis_om-0.3.0/redis_om/async_redis.py
--rw-r--r--   0        0        0      714 2024-05-02 14:38:20.770891 redis_om-0.3.0/redis_om/checks.py
--rw-r--r--   0        0        0      524 2024-05-02 14:38:20.770891 redis_om-0.3.0/redis_om/connections.py
--rw-r--r--   0        0        0      223 2024-05-02 14:38:20.782891 redis_om-0.3.0/redis_om/model/__init__.py
--rw-r--r--   0        0        0        0 2024-05-02 14:38:20.838892 redis_om-0.3.0/redis_om/model/cli/__init__.py
--rw-r--r--   0        0        0      446 2024-05-02 14:38:20.838892 redis_om-0.3.0/redis_om/model/cli/migrate.py
--rw-r--r--   0        0        0     6544 2024-05-02 14:38:20.778891 redis_om-0.3.0/redis_om/model/encoders.py
--rw-r--r--   0        0        0        0 2024-05-02 14:38:20.842892 redis_om-0.3.0/redis_om/model/migrations/__init__.py
--rw-r--r--   0        0        0     5101 2024-05-02 14:38:20.842892 redis_om-0.3.0/redis_om/model/migrations/migrator.py
--rw-r--r--   0        0        0    77350 2024-05-02 14:38:20.834892 redis_om-0.3.0/redis_om/model/model.py
--rw-r--r--   0        0        0     2229 2024-05-02 14:38:20.774891 redis_om-0.3.0/redis_om/model/query_resolver.py
--rw-r--r--   0        0        0     2246 2024-05-02 14:38:20.838892 redis_om-0.3.0/redis_om/model/render_tree.py
--rw-r--r--   0        0        0      855 2024-05-02 14:38:20.774891 redis_om-0.3.0/redis_om/model/token_escaper.py
--rw-r--r--   0        0        0       13 2024-05-02 14:38:20.766891 redis_om-0.3.0/redis_om/sync_redis.py
--rw-r--r--   0        0        0      228 2024-05-02 14:38:20.770891 redis_om-0.3.0/redis_om/util.py
--rw-r--r--   0        0        0    14712 1970-01-01 00:00:00.000000 redis_om-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-07 21:00:12.788866 redis_om-0.3.1/LICENSE
+-rw-r--r--   0        0        0    13159 2024-05-07 21:00:12.788866 redis_om-0.3.1/README.md
+-rw-r--r--   0        0        0      463 2024-05-07 21:00:12.788866 redis_om-0.3.1/aredis_om/__init__.py
+-rw-r--r--   0        0        0     2995 2024-05-07 21:00:12.788866 redis_om-0.3.1/aredis_om/_compat.py
+-rw-r--r--   0        0        0       35 2024-05-07 21:00:12.788866 redis_om-0.3.1/aredis_om/async_redis.py
+-rw-r--r--   0        0        0      751 2024-05-07 21:00:12.788866 redis_om-0.3.1/aredis_om/checks.py
+-rw-r--r--   0        0        0      524 2024-05-07 21:00:12.788866 redis_om-0.3.1/aredis_om/connections.py
+-rw-r--r--   0        0        0      223 2024-05-07 21:00:12.788866 redis_om-0.3.1/aredis_om/model/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 21:00:12.788866 redis_om-0.3.1/aredis_om/model/cli/__init__.py
+-rw-r--r--   0        0        0      448 2024-05-07 21:00:12.788866 redis_om-0.3.1/aredis_om/model/cli/migrate.py
+-rw-r--r--   0        0        0     6544 2024-05-07 21:00:12.788866 redis_om-0.3.1/aredis_om/model/encoders.py
+-rw-r--r--   0        0        0        0 2024-05-07 21:00:12.788866 redis_om-0.3.1/aredis_om/model/migrations/__init__.py
+-rw-r--r--   0        0        0     5204 2024-05-07 21:00:12.788866 redis_om-0.3.1/aredis_om/model/migrations/migrator.py
+-rw-r--r--   0        0        0    80741 2024-05-07 21:00:12.792866 redis_om-0.3.1/aredis_om/model/model.py
+-rw-r--r--   0        0        0     2230 2024-05-07 21:00:12.792866 redis_om-0.3.1/aredis_om/model/query_resolver.py
+-rw-r--r--   0        0        0     2246 2024-05-07 21:00:12.792866 redis_om-0.3.1/aredis_om/model/render_tree.py
+-rw-r--r--   0        0        0      855 2024-05-07 21:00:12.792866 redis_om-0.3.1/aredis_om/model/token_escaper.py
+-rw-r--r--   0        0        0       13 2024-05-07 21:00:12.792866 redis_om-0.3.1/aredis_om/sync_redis.py
+-rw-r--r--   0        0        0      234 2024-05-07 21:00:12.792866 redis_om-0.3.1/aredis_om/util.py
+-rw-r--r--   0        0        0     3717 2024-05-07 21:00:12.792866 redis_om-0.3.1/docs/connections.md
+-rw-r--r--   0        0        0     6704 2024-05-07 21:00:12.792866 redis_om-0.3.1/docs/errors.md
+-rw-r--r--   0        0        0     7510 2024-05-07 21:00:12.792866 redis_om-0.3.1/docs/fastapi_integration.md
+-rw-r--r--   0        0        0    22328 2024-05-07 21:00:12.792866 redis_om-0.3.1/docs/getting_started.md
+-rw-r--r--   0        0        0      973 2024-05-07 21:00:12.792866 redis_om-0.3.1/docs/index.md
+-rw-r--r--   0        0        0    11639 2024-05-07 21:00:12.792866 redis_om-0.3.1/docs/models.md
+-rw-r--r--   0        0        0     1674 2024-05-07 21:00:12.792866 redis_om-0.3.1/docs/redis_modules.md
+-rw-r--r--   0        0        0     3688 2024-05-07 21:00:12.792866 redis_om-0.3.1/docs/validation.md
+-rw-r--r--   0        0        0     3577 2024-05-07 21:00:12.792866 redis_om-0.3.1/images/logo.svg
+-rw-r--r--   0        0        0     1931 2024-05-07 21:00:13.240869 redis_om-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      462 2024-05-07 21:00:51.541038 redis_om-0.3.1/redis_om/__init__.py
+-rw-r--r--   0        0        0     2995 2024-05-07 21:00:51.545038 redis_om-0.3.1/redis_om/_compat.py
+-rw-r--r--   0        0        0       35 2024-05-07 21:00:51.541038 redis_om-0.3.1/redis_om/async_redis.py
+-rw-r--r--   0        0        0      714 2024-05-07 21:00:51.545038 redis_om-0.3.1/redis_om/checks.py
+-rw-r--r--   0        0        0      524 2024-05-07 21:00:51.541038 redis_om-0.3.1/redis_om/connections.py
+-rw-r--r--   0        0        0      223 2024-05-07 21:00:51.557038 redis_om-0.3.1/redis_om/model/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 21:00:51.625039 redis_om-0.3.1/redis_om/model/cli/__init__.py
+-rw-r--r--   0        0        0      446 2024-05-07 21:00:51.625039 redis_om-0.3.1/redis_om/model/cli/migrate.py
+-rw-r--r--   0        0        0     6544 2024-05-07 21:00:51.557038 redis_om-0.3.1/redis_om/model/encoders.py
+-rw-r--r--   0        0        0        0 2024-05-07 21:00:51.629039 redis_om-0.3.1/redis_om/model/migrations/__init__.py
+-rw-r--r--   0        0        0     5101 2024-05-07 21:00:51.629039 redis_om-0.3.1/redis_om/model/migrations/migrator.py
+-rw-r--r--   0        0        0    80416 2024-05-07 21:00:51.625039 redis_om-0.3.1/redis_om/model/model.py
+-rw-r--r--   0        0        0     2229 2024-05-07 21:00:51.549039 redis_om-0.3.1/redis_om/model/query_resolver.py
+-rw-r--r--   0        0        0     2246 2024-05-07 21:00:51.625039 redis_om-0.3.1/redis_om/model/render_tree.py
+-rw-r--r--   0        0        0      855 2024-05-07 21:00:51.549039 redis_om-0.3.1/redis_om/model/token_escaper.py
+-rw-r--r--   0        0        0       13 2024-05-07 21:00:51.541038 redis_om-0.3.1/redis_om/sync_redis.py
+-rw-r--r--   0        0        0      228 2024-05-07 21:00:51.545038 redis_om-0.3.1/redis_om/util.py
+-rw-r--r--   0        0        0    14712 1970-01-01 00:00:00.000000 redis_om-0.3.1/PKG-INFO
```

### Comparing `redis_om-0.3.0/LICENSE` & `redis_om-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/README.md` & `redis_om-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/aredis_om/_compat.py` & `redis_om-0.3.1/aredis_om/_compat.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/aredis_om/checks.py` & `redis_om-0.3.1/aredis_om/checks.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/aredis_om/connections.py` & `redis_om-0.3.1/aredis_om/connections.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/aredis_om/model/encoders.py` & `redis_om-0.3.1/aredis_om/model/encoders.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/aredis_om/model/migrations/migrator.py` & `redis_om-0.3.1/aredis_om/model/migrations/migrator.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/aredis_om/model/model.py` & `redis_om-0.3.1/aredis_om/model/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     Sequence,
     Set,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
-from typing import get_args as typing_get_args, no_type_check
+from typing import get_args as typing_get_args
+from typing import no_type_check
 
 from more_itertools import ichunked
 from redis.commands.json.path import Path
 from redis.exceptions import ResponseError
 from typing_extensions import Protocol, get_args, get_origin
 from ulid import ULID
 
@@ -78,14 +79,16 @@
 def get_outer_type(field):
     if hasattr(field, "outer_type_"):
         return field.outer_type_
     elif isinstance(field.annotation, type) or is_supported_container_type(
         field.annotation
     ):
         return field.annotation
+    elif not hasattr(field.annotation, "__args__"):
+        return None
     else:
         return field.annotation.__args__[0]
 
 
 class RedisModelError(Exception):
     """Raised when a problem exists in the definition of a RedisModel."""
 
@@ -108,14 +111,19 @@
     OR = 7
     AND = 8
     NOT = 9
     IN = 10
     NOT_IN = 11
     LIKE = 12
     ALL = 13
+    STARTSWITH = 14
+    ENDSWITH = 15
+    CONTAINS = 16
+    TRUE = 17
+    FALSE = 18
 
     def __str__(self):
         return str(self.name)
 
 
 ExpressionOrModelField = Union[
     "Expression", "NegatedExpression", ModelField, PydanticFieldInfo
@@ -342,14 +350,29 @@
         )
 
     def __rshift__(self, other: Any) -> Expression:
         return Expression(
             left=self.field, op=Operators.NOT_IN, right=other, parents=self.parents
         )
 
+    def startswith(self, other: Any) -> Expression:
+        return Expression(
+            left=self.field, op=Operators.STARTSWITH, right=other, parents=self.parents
+        )
+
+    def endswith(self, other: Any) -> Expression:
+        return Expression(
+            left=self.field, op=Operators.ENDSWITH, right=other, parents=self.parents
+        )
+
+    def contains(self, other: Any) -> Expression:
+        return Expression(
+            left=self.field, op=Operators.CONTAINS, right=other, parents=self.parents
+        )
+
     def __getattr__(self, item):
         if item.startswith("__"):
             raise AttributeError("cannot invoke __getattr__ with reserved field")
         outer_type = outer_type_or_annotation(self.field)
         if is_supported_container_type(outer_type):
             embedded_cls = get_args(outer_type)
             if not embedded_cls:
@@ -559,14 +582,16 @@
             # within the model inside the list marked as `index=True`.
             return RediSearchFieldTypes.TAG
         elif container_type is not None:
             raise QuerySyntaxError(
                 "Only lists and tuples are supported for multi-value fields. "
                 f"Docs: {ERRORS_URL}#E4"
             )
+        elif field_type is bool:
+            return RediSearchFieldTypes.TAG
         elif any(issubclass(field_type, t) for t in NUMERIC_TYPES):
             # Index numeric Python types as NUMERIC fields, so we can support
             # range queries.
             return RediSearchFieldTypes.NUMERIC
         else:
             # TAG fields are the default field type and support equality and
             # membership queries, though membership (and the multi-value nature
@@ -653,15 +678,19 @@
                         "an alternative query that uses a string containing more than "
                         "just the character %s.",
                         field_name,
                         separator_char,
                         separator_char,
                     )
                     return ""
-                if isinstance(value, int):
+                if isinstance(value, bool):
+                    result = "@{field_name}:{{{value}}}".format(
+                        field_name=field_name, value=value
+                    )
+                elif isinstance(value, int):
                     # This if will hit only if the field is a primary key of type int
                     result = f"@{field_name}:[{value} {value}]"
                 elif separator_char in value:
                     # The value contains the TAG field separator. We can work
                     # around this by breaking apart the values and unioning them
                     # with multiple field:{} queries.
                     values: filter = filter(None, value.split(separator_char))
@@ -687,14 +716,29 @@
                 )
             elif op is Operators.NOT_IN:
                 # TODO: Implement NOT_IN, test this...
                 expanded_value = cls.expand_tag_value(value)
                 result += "-(@{field_name}:{{{expanded_value}}})".format(
                     field_name=field_name, expanded_value=expanded_value
                 )
+            elif op is Operators.STARTSWITH:
+                expanded_value = cls.expand_tag_value(value)
+                result += "(@{field_name}:{{{expanded_value}*}})".format(
+                    field_name=field_name, expanded_value=expanded_value
+                )
+            elif op is Operators.ENDSWITH:
+                expanded_value = cls.expand_tag_value(value)
+                result += "(@{field_name}:{{*{expanded_value}}})".format(
+                    field_name=field_name, expanded_value=expanded_value
+                )
+            elif op is Operators.CONTAINS:
+                expanded_value = cls.expand_tag_value(value)
+                result += "(@{field_name}:{{*{expanded_value}*}})".format(
+                    field_name=field_name, expanded_value=expanded_value
+                )
 
         return result
 
     def resolve_redisearch_pagination(self):
         """Resolve pagination options for a query."""
         return ["LIMIT", self.offset, self.limit]
 
@@ -1028,20 +1072,22 @@
     return lambda a: a
 
 
 class FieldInfo(PydanticFieldInfo):
     def __init__(self, default: Any = Undefined, **kwargs: Any) -> None:
         primary_key = kwargs.pop("primary_key", False)
         sortable = kwargs.pop("sortable", Undefined)
+        case_sensitive = kwargs.pop("case_sensitive", Undefined)
         index = kwargs.pop("index", Undefined)
         full_text_search = kwargs.pop("full_text_search", Undefined)
         vector_options = kwargs.pop("vector_options", None)
         super().__init__(default=default, **kwargs)
         self.primary_key = primary_key
         self.sortable = sortable
+        self.case_sensitive = case_sensitive
         self.index = index
         self.full_text_search = full_text_search
         self.vector_options = vector_options
 
 
 class RelationshipInfo(Representation):
     def __init__(
@@ -1165,14 +1211,15 @@
     max_items: Optional[int] = None,
     min_length: Optional[int] = None,
     max_length: Optional[int] = None,
     allow_mutation: bool = True,
     regex: Optional[str] = None,
     primary_key: bool = False,
     sortable: Union[bool, UndefinedType] = Undefined,
+    case_sensitive: Union[bool, UndefinedType] = Undefined,
     index: Union[bool, UndefinedType] = Undefined,
     full_text_search: Union[bool, UndefinedType] = Undefined,
     vector_options: Optional[VectorFieldOptions] = None,
     schema_extra: Optional[Dict[str, Any]] = None,
 ) -> Any:
     current_schema_extra = schema_extra or {}
     field_info = FieldInfo(
@@ -1193,14 +1240,15 @@
         max_items=max_items,
         min_length=min_length,
         max_length=max_length,
         allow_mutation=allow_mutation,
         regex=regex,
         primary_key=primary_key,
         sortable=sortable,
+        case_sensitive=case_sensitive,
         index=index,
         full_text_search=full_text_search,
         vector_options=vector_options,
         **current_schema_extra,
     )
     return field_info
 
@@ -1586,14 +1634,19 @@
         from pydantic.version import VERSION as PYDANTIC_VERSION
 
         PYDANTIC_V2 = PYDANTIC_VERSION.startswith("2.")
         if not PYDANTIC_V2:
             *_, validation_error = validate_model(self.__class__, self.__dict__)
             if validation_error:
                 raise validation_error
+        else:
+            from pydantic import TypeAdapter
+
+            adapter = TypeAdapter(self.__class__)
+            adapter.validate_python(self.__dict__)
 
 
 class HashModel(RedisModel, abc.ABC):
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
 
         if hasattr(cls, "__annotations__"):
@@ -1638,14 +1691,17 @@
 
     async def save(
         self: "Model", pipeline: Optional[redis.client.Pipeline] = None
     ) -> "Model":
         self.check()
         db = self._get_db(pipeline)
         document = jsonable_encoder(self.dict())
+
+        # filter out values which are `None` because they are not valid in a HSET
+        document = {k: v for k, v in document.items() if v is not None}
         # TODO: Wrap any Redis response errors in a custom exception?
         await db.hset(self.key(), mapping=document)
         return self
 
     @classmethod
     async def all_pks(cls):  # type: ignore
         key_prefix = cls.make_key(cls._meta.primary_key_pattern.format(pk=""))
@@ -1760,25 +1816,28 @@
         #  a List[int] gets indexed as TAG instead of NUMERICAL.
         # TODO: Raise error if user embeds a model field or list and makes it
         #  sortable. Instead, the embedded model should mark individual fields
         #  as sortable.
         # TODO: Abstract string-building logic for each type (TAG, etc.) into
         #  classes that take a field name.
         sortable = getattr(field_info, "sortable", False)
+        case_sensitive = getattr(field_info, "case_sensitive", False)
 
         if is_supported_container_type(typ):
             embedded_cls = get_args(typ)
             if not embedded_cls:
                 # TODO: Test if this can really happen.
                 log.warning(
                     "Model %s defined an empty list or tuple field: %s", cls, name
                 )
                 return ""
             embedded_cls = embedded_cls[0]
             schema = cls.schema_for_type(name, embedded_cls, field_info)
+        elif typ is bool:
+            schema = f"{name} TAG"
         elif any(issubclass(typ, t) for t in NUMERIC_TYPES):
             vector_options: Optional[VectorFieldOptions] = getattr(
                 field_info, "vector_options", None
             )
             if vector_options:
                 schema = f"{name} {vector_options.schema}"
             else:
@@ -1800,14 +1859,17 @@
                     )
                 )
             schema = " ".join(sub_fields)
         else:
             schema = f"{name} TAG SEPARATOR {SINGLE_VALUE_TAG_FIELD_SEPARATOR}"
         if schema and sortable is True:
             schema += " SORTABLE"
+        if schema and case_sensitive is True:
+            schema += " CASESENSITIVE"
+
         return schema
 
 
 class JsonModel(RedisModel, abc.ABC):
     def __init_subclass__(cls, **kwargs):
         # Generate the RediSearch schema once to validate fields.
         cls.redisearch_schema()
@@ -1897,14 +1959,17 @@
         for name, field in cls.__annotations__.items():
             if name in fields:
                 continue
             fields[name] = PydanticFieldInfo.from_annotation(field)
 
         for name, field in fields.items():
             _type = get_outer_type(field)
+            if _type is None:
+                continue
+
             if (
                 not isinstance(field, FieldInfo)
                 and hasattr(field, "metadata")
                 and len(field.metadata) > 0
                 and isinstance(field.metadata[0], FieldInfo)
             ):
                 field = field.metadata[0]
@@ -2042,14 +2107,15 @@
                 # If we're indexing the this field as a JavaScript array, then
                 # the currently built-up JSONPath expression will be
                 # "field_name[*]", which is what we want to use.
                 path = json_path
             else:
                 path = f"{json_path}.{name}"
             sortable = getattr(field_info, "sortable", False)
+            case_sensitive = getattr(field_info, "case_sensitive", False)
             full_text_search = getattr(field_info, "full_text_search", False)
             sortable_tag_error = RedisModelError(
                 "In this Preview release, TAG fields cannot "
                 f"be marked as sortable. Problem field: {name}. "
                 "See docs: TODO"
             )
 
@@ -2072,14 +2138,18 @@
                     raise RedisModelError(
                         "List and tuple fields cannot be indexed for full-text "
                         f"search. Problem field: {name}. See docs: TODO"
                     )
                 schema = f"{path} AS {index_field_name} TAG SEPARATOR {SINGLE_VALUE_TAG_FIELD_SEPARATOR}"
                 if sortable is True:
                     raise sortable_tag_error
+                if case_sensitive is True:
+                    schema += " CASESENSITIVE"
+            elif typ is bool:
+                schema = f"{path} AS {index_field_name} TAG"
             elif any(issubclass(typ, t) for t in NUMERIC_TYPES):
                 schema = f"{path} AS {index_field_name} NUMERIC"
             elif issubclass(typ, str):
                 if full_text_search is True:
                     schema = (
                         f"{path} AS {index_field_name} TAG SEPARATOR {SINGLE_VALUE_TAG_FIELD_SEPARATOR} "
                         f"{path} AS {index_field_name}_fts TEXT"
@@ -2087,22 +2157,27 @@
                     if sortable is True:
                         # NOTE: With the current preview release, making a field
                         # full-text searchable and sortable only makes the TEXT
                         # field sortable. This means that results for full-text
                         # search queries can be sorted, but not exact match
                         # queries.
                         schema += " SORTABLE"
+                    if case_sensitive is True:
+                        raise RedisModelError("Text fields cannot be case-sensitive.")
                 else:
                     schema = f"{path} AS {index_field_name} TAG SEPARATOR {SINGLE_VALUE_TAG_FIELD_SEPARATOR}"
                     if sortable is True:
                         raise sortable_tag_error
+                    if case_sensitive is True:
+                        schema += " CASESENSITIVE"
             else:
                 schema = f"{path} AS {index_field_name} TAG SEPARATOR {SINGLE_VALUE_TAG_FIELD_SEPARATOR}"
                 if sortable is True:
                     raise sortable_tag_error
+
             return schema
         return ""
 
 
 class EmbeddedJsonModel(JsonModel, abc.ABC):
     class Meta:
         embedded = True
```

### Comparing `redis_om-0.3.0/aredis_om/model/query_resolver.py` & `redis_om-0.3.1/aredis_om/model/query_resolver.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/aredis_om/model/render_tree.py` & `redis_om-0.3.1/aredis_om/model/render_tree.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/aredis_om/model/token_escaper.py` & `redis_om-0.3.1/aredis_om/model/token_escaper.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/docs/connections.md` & `redis_om-0.3.1/docs/connections.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/docs/errors.md` & `redis_om-0.3.1/docs/errors.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/docs/fastapi_integration.md` & `redis_om-0.3.1/docs/fastapi_integration.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/docs/getting_started.md` & `redis_om-0.3.1/docs/getting_started.md`

 * *Files 2% similar despite different names*

```diff
@@ -698,14 +698,35 @@
 # Find all customers whose last name is "Brookins" OR whose age is
 # 100 AND whose last name is "Smith"
 Customer.find((Customer.last_name == "Brookins") | (
         Customer.age == 100
 ) & (Customer.last_name == "Smith")).all()
 ```
 
+### Saving and querying Boolean values
+
+For historical reasons, saving and querying Boolean values is not supported in `HashModels`, however in JSON models,
+you may store and query Boolean values using the `==` syntax:
+
+```python
+from redis_om import (
+    Field,
+    JsonModel,
+    Migrator
+)
+
+class Demo(JsonModel):
+    b: bool = Field(index=True)
+
+Migrator().run()
+d = Demo(b=True)
+d.save()
+res = Demo.find(Demo.b == True)
+```
+
 ## Calling Other Redis Commands
 
 Sometimes you'll need to run a Redis command directly.  Redis OM supports this through the `db` method on your model's class.  This returns a connected Redis client instance which exposes a function named for each Redis command.  For example, let's perform some basic set operations:
 
 ```python
 from redis_om import HashModel
```

### Comparing `redis_om-0.3.0/docs/index.md` & `redis_om-0.3.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/docs/models.md` & `redis_om-0.3.1/docs/models.md`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 ### All Settings Supported by the Meta Object
 
 Here is a table of the settings available in the Meta object and what they control.
 
 | Setting                 | Description                                                                                                                                                                                                                                                 | Default                                                         |
 | ----------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------- |
 | global_key_prefix       | A string prefix applied to every Redis key that the model manages. This could be something like your application's name.                                                                                                                                    | ""                                                              |
-| model_key_prefix        | A string prefix applied to the Redis key representing every model. For example, the Redis Hash key for a HashModel. This prefix is also added to the redisearch index created for every model with indexed fields.                                          | ""                                                              |
+| model_key_prefix        | A string prefix applied to the Redis key representing every model. For example, the Redis Hash key for a HashModel. This prefix is also added to the redisearch index created for every model with indexed fields.                                          | f"{new_class.__module__}.{new_class.__name__}"                                                              |
 | primary_key_pattern     | A format string producing the base string for a Redis key representing this model. This string should accept a "pk" format argument. **Note:** This is a "new style" format string, which will be called with `.format()`.                                  | "{pk}"                                                           |
 | database                | A redis.asyncio.Redis or redis.Redis client instance that the model will use to communicate with Redis.                                                                                                                                                         | A new instance created with connections.get_redis_connection(). |
 | primary_key_creator_cls | A class that adheres to the PrimaryKeyCreator protocol, which Redis OM will use to create a primary key for a new model instance.                                                                                                                           | UlidPrimaryKey                                                  |
 | index_name              | The RediSearch index name to use for this model. Only used if at least one of the model's fields are marked as indexable (`index=True`).                                                                                                                    | "{global_key_prefix}:{model_key_prefix}:index"                  |
 | embedded                | Whether or not this model is "embedded." Embedded models are not included in migrations that create and destroy indexes. Instead, their indexed fields are included in the index for the parent model. **Note**: Only `JsonModel` can have embedded models. | False                                                           |
 | encoding                | The default encoding to use for strings. This encoding is given to redis-py at the connection level. In both cases, Redis OM will decode binary strings from Redis using your chosen encoding.                                                  | "utf-8"                                                         |
 ## Configuring Pydantic
```

### Comparing `redis_om-0.3.0/docs/redis_modules.md` & `redis_om-0.3.1/docs/redis_modules.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/docs/validation.md` & `redis_om-0.3.1/docs/validation.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/images/logo.svg` & `redis_om-0.3.1/images/logo.svg`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/pyproject.toml` & `redis_om-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redis-om"
-version = "0.3.0"
+version = "0.3.1"
 description = "Object mappings, and more, for Redis."
 authors = [ "Redis OSS <oss@redis.com>" ]
 maintainers = [ "Redis OSS <oss@redis.com>" ]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/redis/redis-om-python"
 classifiers = [
```

### Comparing `redis_om-0.3.0/redis_om/_compat.py` & `redis_om-0.3.1/redis_om/_compat.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/redis_om/checks.py` & `redis_om-0.3.1/redis_om/checks.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/redis_om/connections.py` & `redis_om-0.3.1/redis_om/connections.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/redis_om/model/encoders.py` & `redis_om-0.3.1/redis_om/model/encoders.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/redis_om/model/migrations/migrator.py` & `redis_om-0.3.1/redis_om/model/migrations/migrator.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/redis_om/model/model.py` & `redis_om-0.3.1/redis_om/model/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     Sequence,
     Set,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
-from typing import get_args as typing_get_args, no_type_check
+from typing import get_args as typing_get_args
+from typing import no_type_check
 
 from more_itertools import ichunked
 from redis.commands.json.path import Path
 from redis.exceptions import ResponseError
 from typing_extensions import Protocol, get_args, get_origin
 from ulid import ULID
 
@@ -78,14 +79,16 @@
 def get_outer_type(field):
     if hasattr(field, "outer_type_"):
         return field.outer_type_
     elif isinstance(field.annotation, type) or is_supported_container_type(
         field.annotation
     ):
         return field.annotation
+    elif not hasattr(field.annotation, "__args__"):
+        return None
     else:
         return field.annotation.__args__[0]
 
 
 class RedisModelError(Exception):
     """Raised when a problem exists in the definition of a RedisModel."""
 
@@ -108,14 +111,19 @@
     OR = 7
     AND = 8
     NOT = 9
     IN = 10
     NOT_IN = 11
     LIKE = 12
     ALL = 13
+    STARTSWITH = 14
+    ENDSWITH = 15
+    CONTAINS = 16
+    TRUE = 17
+    FALSE = 18
 
     def __str__(self):
         return str(self.name)
 
 
 ExpressionOrModelField = Union[
     "Expression", "NegatedExpression", ModelField, PydanticFieldInfo
@@ -342,14 +350,29 @@
         )
 
     def __rshift__(self, other: Any) -> Expression:
         return Expression(
             left=self.field, op=Operators.NOT_IN, right=other, parents=self.parents
         )
 
+    def startswith(self, other: Any) -> Expression:
+        return Expression(
+            left=self.field, op=Operators.STARTSWITH, right=other, parents=self.parents
+        )
+
+    def endswith(self, other: Any) -> Expression:
+        return Expression(
+            left=self.field, op=Operators.ENDSWITH, right=other, parents=self.parents
+        )
+
+    def contains(self, other: Any) -> Expression:
+        return Expression(
+            left=self.field, op=Operators.CONTAINS, right=other, parents=self.parents
+        )
+
     def __getattr__(self, item):
         if item.startswith("__"):
             raise AttributeError("cannot invoke __getattr__ with reserved field")
         outer_type = outer_type_or_annotation(self.field)
         if is_supported_container_type(outer_type):
             embedded_cls = get_args(outer_type)
             if not embedded_cls:
@@ -559,14 +582,16 @@
             # within the model inside the list marked as `index=True`.
             return RediSearchFieldTypes.TAG
         elif container_type is not None:
             raise QuerySyntaxError(
                 "Only lists and tuples are supported for multi-value fields. "
                 f"Docs: {ERRORS_URL}#E4"
             )
+        elif field_type is bool:
+            return RediSearchFieldTypes.TAG
         elif any(issubclass(field_type, t) for t in NUMERIC_TYPES):
             # Index numeric Python types as NUMERIC fields, so we can support
             # range queries.
             return RediSearchFieldTypes.NUMERIC
         else:
             # TAG fields are the default field type and support equality and
             # membership queries, though membership (and the multi-value nature
@@ -653,15 +678,19 @@
                         "an alternative query that uses a string containing more than "
                         "just the character %s.",
                         field_name,
                         separator_char,
                         separator_char,
                     )
                     return ""
-                if isinstance(value, int):
+                if isinstance(value, bool):
+                    result = "@{field_name}:{{{value}}}".format(
+                        field_name=field_name, value=value
+                    )
+                elif isinstance(value, int):
                     # This if will hit only if the field is a primary key of type int
                     result = f"@{field_name}:[{value} {value}]"
                 elif separator_char in value:
                     # The value contains the TAG field separator. We can work
                     # around this by breaking apart the values and unioning them
                     # with multiple field:{} queries.
                     values: filter = filter(None, value.split(separator_char))
@@ -687,14 +716,29 @@
                 )
             elif op is Operators.NOT_IN:
                 # TODO: Implement NOT_IN, test this...
                 expanded_value = cls.expand_tag_value(value)
                 result += "-(@{field_name}:{{{expanded_value}}})".format(
                     field_name=field_name, expanded_value=expanded_value
                 )
+            elif op is Operators.STARTSWITH:
+                expanded_value = cls.expand_tag_value(value)
+                result += "(@{field_name}:{{{expanded_value}*}})".format(
+                    field_name=field_name, expanded_value=expanded_value
+                )
+            elif op is Operators.ENDSWITH:
+                expanded_value = cls.expand_tag_value(value)
+                result += "(@{field_name}:{{*{expanded_value}}})".format(
+                    field_name=field_name, expanded_value=expanded_value
+                )
+            elif op is Operators.CONTAINS:
+                expanded_value = cls.expand_tag_value(value)
+                result += "(@{field_name}:{{*{expanded_value}*}})".format(
+                    field_name=field_name, expanded_value=expanded_value
+                )
 
         return result
 
     def resolve_redisearch_pagination(self):
         """Resolve pagination options for a query."""
         return ["LIMIT", self.offset, self.limit]
 
@@ -1028,20 +1072,22 @@
     return lambda a: a
 
 
 class FieldInfo(PydanticFieldInfo):
     def __init__(self, default: Any = Undefined, **kwargs: Any) -> None:
         primary_key = kwargs.pop("primary_key", False)
         sortable = kwargs.pop("sortable", Undefined)
+        case_sensitive = kwargs.pop("case_sensitive", Undefined)
         index = kwargs.pop("index", Undefined)
         full_text_search = kwargs.pop("full_text_search", Undefined)
         vector_options = kwargs.pop("vector_options", None)
         super().__init__(default=default, **kwargs)
         self.primary_key = primary_key
         self.sortable = sortable
+        self.case_sensitive = case_sensitive
         self.index = index
         self.full_text_search = full_text_search
         self.vector_options = vector_options
 
 
 class RelationshipInfo(Representation):
     def __init__(
@@ -1165,14 +1211,15 @@
     max_items: Optional[int] = None,
     min_length: Optional[int] = None,
     max_length: Optional[int] = None,
     allow_mutation: bool = True,
     regex: Optional[str] = None,
     primary_key: bool = False,
     sortable: Union[bool, UndefinedType] = Undefined,
+    case_sensitive: Union[bool, UndefinedType] = Undefined,
     index: Union[bool, UndefinedType] = Undefined,
     full_text_search: Union[bool, UndefinedType] = Undefined,
     vector_options: Optional[VectorFieldOptions] = None,
     schema_extra: Optional[Dict[str, Any]] = None,
 ) -> Any:
     current_schema_extra = schema_extra or {}
     field_info = FieldInfo(
@@ -1193,14 +1240,15 @@
         max_items=max_items,
         min_length=min_length,
         max_length=max_length,
         allow_mutation=allow_mutation,
         regex=regex,
         primary_key=primary_key,
         sortable=sortable,
+        case_sensitive=case_sensitive,
         index=index,
         full_text_search=full_text_search,
         vector_options=vector_options,
         **current_schema_extra,
     )
     return field_info
 
@@ -1586,14 +1634,19 @@
         from pydantic.version import VERSION as PYDANTIC_VERSION
 
         PYDANTIC_V2 = PYDANTIC_VERSION.startswith("2.")
         if not PYDANTIC_V2:
             *_, validation_error = validate_model(self.__class__, self.__dict__)
             if validation_error:
                 raise validation_error
+        else:
+            from pydantic import TypeAdapter
+
+            adapter = TypeAdapter(self.__class__)
+            adapter.validate_python(self.__dict__)
 
 
 class HashModel(RedisModel, abc.ABC):
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
 
         if hasattr(cls, "__annotations__"):
@@ -1638,14 +1691,17 @@
 
     def save(
         self: "Model", pipeline: Optional[redis.client.Pipeline] = None
     ) -> "Model":
         self.check()
         db = self._get_db(pipeline)
         document = jsonable_encoder(self.dict())
+
+        # filter out values which are `None` because they are not valid in a HSET
+        document = {k: v for k, v in document.items() if v is not None}
         # TODO: Wrap any Redis response errors in a custom exception?
         db.hset(self.key(), mapping=document)
         return self
 
     @classmethod
     def all_pks(cls):  # type: ignore
         key_prefix = cls.make_key(cls._meta.primary_key_pattern.format(pk=""))
@@ -1760,25 +1816,28 @@
         #  a List[int] gets indexed as TAG instead of NUMERICAL.
         # TODO: Raise error if user embeds a model field or list and makes it
         #  sortable. Instead, the embedded model should mark individual fields
         #  as sortable.
         # TODO: Abstract string-building logic for each type (TAG, etc.) into
         #  classes that take a field name.
         sortable = getattr(field_info, "sortable", False)
+        case_sensitive = getattr(field_info, "case_sensitive", False)
 
         if is_supported_container_type(typ):
             embedded_cls = get_args(typ)
             if not embedded_cls:
                 # TODO: Test if this can really happen.
                 log.warning(
                     "Model %s defined an empty list or tuple field: %s", cls, name
                 )
                 return ""
             embedded_cls = embedded_cls[0]
             schema = cls.schema_for_type(name, embedded_cls, field_info)
+        elif typ is bool:
+            schema = f"{name} TAG"
         elif any(issubclass(typ, t) for t in NUMERIC_TYPES):
             vector_options: Optional[VectorFieldOptions] = getattr(
                 field_info, "vector_options", None
             )
             if vector_options:
                 schema = f"{name} {vector_options.schema}"
             else:
@@ -1800,14 +1859,17 @@
                     )
                 )
             schema = " ".join(sub_fields)
         else:
             schema = f"{name} TAG SEPARATOR {SINGLE_VALUE_TAG_FIELD_SEPARATOR}"
         if schema and sortable is True:
             schema += " SORTABLE"
+        if schema and case_sensitive is True:
+            schema += " CASESENSITIVE"
+
         return schema
 
 
 class JsonModel(RedisModel, abc.ABC):
     def __init_subclass__(cls, **kwargs):
         # Generate the RediSearch schema once to validate fields.
         cls.redisearch_schema()
@@ -1897,14 +1959,17 @@
         for name, field in cls.__annotations__.items():
             if name in fields:
                 continue
             fields[name] = PydanticFieldInfo.from_annotation(field)
 
         for name, field in fields.items():
             _type = get_outer_type(field)
+            if _type is None:
+                continue
+
             if (
                 not isinstance(field, FieldInfo)
                 and hasattr(field, "metadata")
                 and len(field.metadata) > 0
                 and isinstance(field.metadata[0], FieldInfo)
             ):
                 field = field.metadata[0]
@@ -2042,14 +2107,15 @@
                 # If we're indexing the this field as a JavaScript array, then
                 # the currently built-up JSONPath expression will be
                 # "field_name[*]", which is what we want to use.
                 path = json_path
             else:
                 path = f"{json_path}.{name}"
             sortable = getattr(field_info, "sortable", False)
+            case_sensitive = getattr(field_info, "case_sensitive", False)
             full_text_search = getattr(field_info, "full_text_search", False)
             sortable_tag_error = RedisModelError(
                 "In this Preview release, TAG fields cannot "
                 f"be marked as sortable. Problem field: {name}. "
                 "See docs: TODO"
             )
 
@@ -2072,14 +2138,18 @@
                     raise RedisModelError(
                         "List and tuple fields cannot be indexed for full-text "
                         f"search. Problem field: {name}. See docs: TODO"
                     )
                 schema = f"{path} AS {index_field_name} TAG SEPARATOR {SINGLE_VALUE_TAG_FIELD_SEPARATOR}"
                 if sortable is True:
                     raise sortable_tag_error
+                if case_sensitive is True:
+                    schema += " CASESENSITIVE"
+            elif typ is bool:
+                schema = f"{path} AS {index_field_name} TAG"
             elif any(issubclass(typ, t) for t in NUMERIC_TYPES):
                 schema = f"{path} AS {index_field_name} NUMERIC"
             elif issubclass(typ, str):
                 if full_text_search is True:
                     schema = (
                         f"{path} AS {index_field_name} TAG SEPARATOR {SINGLE_VALUE_TAG_FIELD_SEPARATOR} "
                         f"{path} AS {index_field_name}_fts TEXT"
@@ -2087,22 +2157,27 @@
                     if sortable is True:
                         # NOTE: With the current preview release, making a field
                         # full-text searchable and sortable only makes the TEXT
                         # field sortable. This means that results for full-text
                         # search queries can be sorted, but not exact match
                         # queries.
                         schema += " SORTABLE"
+                    if case_sensitive is True:
+                        raise RedisModelError("Text fields cannot be case-sensitive.")
                 else:
                     schema = f"{path} AS {index_field_name} TAG SEPARATOR {SINGLE_VALUE_TAG_FIELD_SEPARATOR}"
                     if sortable is True:
                         raise sortable_tag_error
+                    if case_sensitive is True:
+                        schema += " CASESENSITIVE"
             else:
                 schema = f"{path} AS {index_field_name} TAG SEPARATOR {SINGLE_VALUE_TAG_FIELD_SEPARATOR}"
                 if sortable is True:
                     raise sortable_tag_error
+
             return schema
         return ""
 
 
 class EmbeddedJsonModel(JsonModel, abc.ABC):
     class Meta:
         embedded = True
```

### Comparing `redis_om-0.3.0/redis_om/model/query_resolver.py` & `redis_om-0.3.1/redis_om/model/query_resolver.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/redis_om/model/render_tree.py` & `redis_om-0.3.1/redis_om/model/render_tree.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/redis_om/model/token_escaper.py` & `redis_om-0.3.1/redis_om/model/token_escaper.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.3.0/PKG-INFO` & `redis_om-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-om
-Version: 0.3.0
+Version: 0.3.1
 Summary: Object mappings, and more, for Redis.
 Home-page: https://github.com/redis/redis-om-python
 License: BSD-3-Clause
 Author: Redis OSS
 Author-email: oss@redis.com
 Maintainer: Redis OSS
 Maintainer-email: oss@redis.com
```

