# Comparing `tmp/sqlmodel_filters-0.0.7.tar.gz` & `tmp/sqlmodel_filters-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmodel_filters-0.0.7.tar", max compression
+gzip compressed data, was "sqlmodel_filters-0.0.8.tar", max compression
```

## Comparing `sqlmodel_filters-0.0.7.tar` & `sqlmodel_filters-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-05-03 00:29:09.341392 sqlmodel_filters-0.0.7/LICENSE
--rw-r--r--   0        0        0     8433 2024-05-03 00:29:09.341392 sqlmodel_filters-0.0.7/README.md
--rw-r--r--   0        0        0     1022 2024-05-03 00:29:25.205609 sqlmodel_filters-0.0.7/pyproject.toml
--rw-r--r--   0        0        0       82 2024-05-03 00:29:09.341392 sqlmodel_filters-0.0.7/sqlmodel_filters/__init__.py
--rw-r--r--   0        0        0     7467 2024-05-03 00:29:09.341392 sqlmodel_filters-0.0.7/sqlmodel_filters/builder.py
--rw-r--r--   0        0        0     6941 2024-05-03 00:29:09.341392 sqlmodel_filters-0.0.7/sqlmodel_filters/components.py
--rw-r--r--   0        0        0      165 2024-05-03 00:29:09.341392 sqlmodel_filters-0.0.7/sqlmodel_filters/exceptions.py
--rw-r--r--   0        0        0      391 2024-05-03 00:29:09.341392 sqlmodel_filters-0.0.7/sqlmodel_filters/utils.py
--rw-r--r--   0        0        0     9018 1970-01-01 00:00:00.000000 sqlmodel_filters-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-07 10:42:02.201348 sqlmodel_filters-0.0.8/LICENSE
+-rw-r--r--   0        0        0     8433 2024-05-07 10:42:02.201348 sqlmodel_filters-0.0.8/README.md
+-rw-r--r--   0        0        0     1022 2024-05-07 10:42:15.889348 sqlmodel_filters-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0       82 2024-05-07 10:42:02.201348 sqlmodel_filters-0.0.8/sqlmodel_filters/__init__.py
+-rw-r--r--   0        0        0     7919 2024-05-07 10:42:02.201348 sqlmodel_filters-0.0.8/sqlmodel_filters/builder.py
+-rw-r--r--   0        0        0     7419 2024-05-07 10:42:02.201348 sqlmodel_filters-0.0.8/sqlmodel_filters/components.py
+-rw-r--r--   0        0        0      165 2024-05-07 10:42:02.201348 sqlmodel_filters-0.0.8/sqlmodel_filters/exceptions.py
+-rw-r--r--   0        0        0      391 2024-05-07 10:42:02.201348 sqlmodel_filters-0.0.8/sqlmodel_filters/utils.py
+-rw-r--r--   0        0        0     9018 1970-01-01 00:00:00.000000 sqlmodel_filters-0.0.8/PKG-INFO
```

### Comparing `sqlmodel_filters-0.0.7/LICENSE` & `sqlmodel_filters-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmodel_filters-0.0.7/README.md` & `sqlmodel_filters-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `sqlmodel_filters-0.0.7/pyproject.toml` & `sqlmodel_filters-0.0.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlmodel-filters"
-version = "0.0.7"
+version = "0.0.8"
 description = "A Lucene query like fliltering for SQLModel"
 authors = ["Manabu Niseki <manabu.niseki@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `sqlmodel_filters-0.0.7/sqlmodel_filters/builder.py` & `sqlmodel_filters-0.0.8/sqlmodel_filters/builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 import contextlib
 from collections.abc import Callable
 from types import MappingProxyType
 from typing import Any, TypeVar
 
 from luqum.thread import parse
-from luqum.tree import AndOperation, Group, Item, Not, OrOperation, SearchField, UnknownOperation, Word
+from luqum.tree import (
+    AndOperation,
+    Group,
+    Item,
+    Not,
+    OrOperation,
+    Phrase,
+    SearchField,
+    Term,
+    UnknownOperation,
+    Word,
+)
 from luqum.visitor import TreeVisitor
 from pydantic.fields import FieldInfo
 from sqlalchemy.sql._typing import _ColumnExpressionArgument
 from sqlmodel import SQLModel, and_, not_, or_, select
 from sqlmodel.sql.expression import Select, SelectOfScalar
 
 from sqlmodel_filters.exceptions import IllegalFilterError
 
-from .components import SearchFieldNode, WordNode
+from .components import PhraseNode, SearchFieldNode, WordNode
 
 ModelType = TypeVar("ModelType", bound=SQLModel)
 
 
 class ExpressionsBuilder(TreeVisitor):
     def __init__(
         self,
@@ -121,35 +132,44 @@
         for child in node.children:
             yield from self.get_expressions(child)
 
     def visit_unknown_operation(self, node: UnknownOperation, context: dict):
         self.expressions.extend(list(self.get_expressions(node)))
         yield from super().generic_visit(node, context)
 
-    def _handle_top_level_word(self, node: Word):
+    def _handle_top_level_term(self, node: Term):
         pos = node.pos or -1
         if self.is_analyzed(pos):
             return
 
         self.update_analyzed_positions(pos)
 
-        wrapper = WordNode(node, model=self.model, default_fields=self.default_fields)
+        def get_wrapper():
+            match node:
+                case Word():
+                    return WordNode(node, model=self.model, default_fields=self.default_fields)
+                case Phrase():
+                    return PhraseNode(node, model=self.model, default_fields=self.default_fields)
+                case unknown:
+                    raise IllegalFilterError(f"Top level {unknown.__class__} is not supported yet")
+
+        wrapper = get_wrapper()
         yield from wrapper.get_expressions()
 
-    def visit_word(self, node: Word, context: dict):
+    def visit_term(self, node: Term, context: dict):
         parents: tuple[Any] = context.get("parents", ())
         is_top_level = len(parents) == 0
 
         if not is_top_level:
             with contextlib.suppress(Exception):
                 last = parents[-1][-1]
                 is_top_level = last == node
 
         if is_top_level:
-            self.expressions.extend(list(self._handle_top_level_word(node)))
+            self.expressions.extend(list(self._handle_top_level_term(node)))
 
         yield from super().generic_visit(node, context)
 
     def __call__(self, tree: Item):
         # NOTE: initialize expressions and _processed_positions to ensure idempotency
         self.expressions = []
         self._analyzed_positions = set()
```

### Comparing `sqlmodel_filters-0.0.7/sqlmodel_filters/components.py` & `sqlmodel_filters-0.0.8/sqlmodel_filters/components.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import contextlib
 from functools import cached_property
 from types import MappingProxyType
-from typing import Annotated, Any, TypeVar
+from typing import Annotated, Any, Generic, TypeVar
 
 from luqum.tree import From, Item, Phrase, Range, Regex, To, Word
 from pydantic import TypeAdapter
 from pydantic.fields import FieldInfo
 from sqlalchemy.orm.attributes import InstrumentedAttribute
 from sqlalchemy.sql._typing import _ColumnExpressionArgument
 from sqlmodel import SQLModel, and_
 
 from .exceptions import IllegalFieldError, IllegalFilterError
 from .utils import dequote, deslash
 
 ModelType = TypeVar("ModelType", bound=SQLModel)
+NodeType = TypeVar("NodeType", bound=Item)
 
 
 def replace_wildcards(s: str, *, mapping: MappingProxyType[str, str]):
     for k, v in mapping.items():
         s = s.replace(k, v)
 
     return s
@@ -181,30 +182,42 @@
                 yield from self._to_expression(self.node)
             case Regex():
                 yield from self._regex_expression(self.node)
             case unknown:
                 raise IllegalFilterError(f"{unknown.__class__} is not supported yet")
 
 
-class WordNode:
-    def __init__(self, node: Word, *, model: type[ModelType], default_fields: dict[str, FieldInfo] | None = None):
+class BaseNode(Generic[NodeType]):
+    def __init__(self, node: NodeType, *, model: type[ModelType], default_fields: dict[str, FieldInfo] | None = None):
         self.node = node
         self.model = model
         self.default_fields = default_fields or model.model_fields
 
     def get_field(self, name) -> InstrumentedAttribute:
         return getattr(self.model, name)
 
+
+class WordNode(BaseNode[Word]):
     def get_expressions(self):
         for name in self.default_fields:
             model_field = ModelField(self.model, name=name)
             with contextlib.suppress(Exception):
                 field = self.get_field(name)
 
                 if self.node.value == "*":
                     yield field.isnot(None)
                 else:
                     casted = model_field.cast(self.node.value)
                     if isinstance(casted, str):
                         yield field.like(str(LikeWord(casted)))
                     else:
                         yield field == casted
+
+
+class PhraseNode(BaseNode[Phrase]):
+    def get_expressions(self):
+        for name in self.default_fields:
+            model_field = ModelField(self.model, name=name)
+            with contextlib.suppress(Exception):
+                field = self.get_field(name)
+                casted = model_field.cast(dequote(self.node.value))
+                yield field == casted
```

### Comparing `sqlmodel_filters-0.0.7/PKG-INFO` & `sqlmodel_filters-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlmodel-filters
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Lucene query like fliltering for SQLModel
 License: MIT
 Author: Manabu Niseki
 Author-email: manabu.niseki@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

