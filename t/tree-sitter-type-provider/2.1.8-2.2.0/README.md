# Comparing `tmp/tree_sitter_type_provider-2.1.8.tar.gz` & `tmp/tree_sitter_type_provider-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree_sitter_type_provider-2.1.8.tar", last modified: Wed Sep  7 12:22:48 2022, max compression
+gzip compressed data, was "tree_sitter_type_provider-2.2.0.tar", last modified: Tue May  7 19:41:39 2024, max compression
```

## Comparing `tree_sitter_type_provider-2.1.8.tar` & `tree_sitter_type_provider-2.2.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 12:22:48.817985 tree_sitter_type_provider-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-09-07 12:21:58.000000 tree_sitter_type_provider-2.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-09-07 12:21:58.000000 tree_sitter_type_provider-2.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2758 2022-09-07 12:22:48.817985 tree_sitter_type_provider-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2282 2022-09-07 12:21:58.000000 tree_sitter_type_provider-2.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1467 2022-09-07 12:21:58.000000 tree_sitter_type_provider-2.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-07 12:22:48.817985 tree_sitter_type_provider-2.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 12:22:48.817985 tree_sitter_type_provider-2.1.8/tree_sitter_type_provider/
--rw-r--r--   0 runner    (1001) docker     (121)    10696 2022-09-07 12:21:58.000000 tree_sitter_type_provider-2.1.8/tree_sitter_type_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8153 2022-09-07 12:21:58.000000 tree_sitter_type_provider-2.1.8/tree_sitter_type_provider/node_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     2112 2022-09-07 12:21:58.000000 tree_sitter_type_provider-2.1.8/tree_sitter_type_provider/parse_error.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-07 12:21:58.000000 tree_sitter_type_provider-2.1.8/tree_sitter_type_provider/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 12:22:48.817985 tree_sitter_type_provider-2.1.8/tree_sitter_type_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2758 2022-09-07 12:22:48.000000 tree_sitter_type_provider-2.1.8/tree_sitter_type_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-07 12:22:48.000000 tree_sitter_type_provider-2.1.8/tree_sitter_type_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-07 12:22:48.000000 tree_sitter_type_provider-2.1.8/tree_sitter_type_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-09-07 12:22:48.000000 tree_sitter_type_provider-2.1.8/tree_sitter_type_provider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-09-07 12:22:48.000000 tree_sitter_type_provider-2.1.8/tree_sitter_type_provider.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:41:39.254787 tree_sitter_type_provider-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-07 19:41:29.000000 tree_sitter_type_provider-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-05-07 19:41:39.254787 tree_sitter_type_provider-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-07 19:41:29.000000 tree_sitter_type_provider-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-07 19:41:29.000000 tree_sitter_type_provider-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 19:41:39.254787 tree_sitter_type_provider-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:41:39.250787 tree_sitter_type_provider-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:41:39.250787 tree_sitter_type_provider-2.2.0/src/tree_sitter_type_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)    12726 2024-05-07 19:41:29.000000 tree_sitter_type_provider-2.2.0/src/tree_sitter_type_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-05-07 19:41:29.000000 tree_sitter_type_provider-2.2.0/src/tree_sitter_type_provider/node_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:41:29.000000 tree_sitter_type_provider-2.2.0/src/tree_sitter_type_provider/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:41:39.254787 tree_sitter_type_provider-2.2.0/src/tree_sitter_type_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-05-07 19:41:39.000000 tree_sitter_type_provider-2.2.0/src/tree_sitter_type_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-07 19:41:39.000000 tree_sitter_type_provider-2.2.0/src/tree_sitter_type_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:41:39.000000 tree_sitter_type_provider-2.2.0/src/tree_sitter_type_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-07 19:41:39.000000 tree_sitter_type_provider-2.2.0/src/tree_sitter_type_provider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 19:41:39.000000 tree_sitter_type_provider-2.2.0/src/tree_sitter_type_provider.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:41:39.254787 tree_sitter_type_provider-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-07 19:41:29.000000 tree_sitter_type_provider-2.2.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-07 19:41:29.000000 tree_sitter_type_provider-2.2.0/tests/test_convert.py
```

### Comparing `tree_sitter_type_provider-2.1.8/LICENSE` & `tree_sitter_type_provider-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tree_sitter_type_provider-2.1.8/PKG-INFO` & `tree_sitter_type_provider-2.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,27 @@
-Metadata-Version: 2.1
-Name: tree_sitter_type_provider
-Version: 2.1.8
-Summary: Type providers for tree-sitter in Python
-Author: Wen Kokke
-Project-URL: repository, https://github.com/wenkokke/py-tree-sitter-type-provider
-Keywords: type-provider
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development :: Compilers
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-License-File: LICENSE
+![PyPI](https://img.shields.io/pypi/v/tree-sitter-type-provider)
+![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/wenkokke/py-tree-sitter-type-provider)
+[![GitHub Workflow Status](https://github.com/wenkokke/py-tree-sitter-type-provider/actions/workflows/ci.yml/badge.svg)](https://github.com/wenkokke/py-tree-sitter-talon/actions/workflows/ci.yml)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/wenkokke/py-tree-sitter-type-provider/dev.svg)](https://results.pre-commit.ci/latest/github/wenkokke/py-tree-sitter-type-provider/dev)
 
 # Type Providers for Tree Sitter
 
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/wenkokke/py-tree-sitter-type-provider/CI) ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/wenkokke/py-tree-sitter-type-provider) ![PyPI](https://img.shields.io/pypi/v/tree-sitter-type-provider)
-
 Create a type AST from any `node-types.json` file, as well as a generic visitor class and a transformer class, and a function to convert to the AST from the `tree_sitter.Node` type.
 
 For example, the following code defines a module named `tree_sitter_javascript` from `tree-sitter-javascript/src/nodes.json`:
 
 ```python
 import pathlib
 import tree_sitter_type_provider as tstp
 
 node_types_json = pathlib.Path("tree-sitter-javascript/src/node-types.json")
 node_types = tstp.NodeType.schema().loads(node_types_json.read_text(), many=True)
 
 def as_class_name(node_type_name: str) -> str:
-    class_name_parts: list[str] = ["Js"]
+    class_name_parts: typing.List[str] = ["Js"]
     for part in node_type_name.split("_"):
         class_name_parts.append(part.capitalize())
     return "".join(class_name_parts)
 
 sys.modules[__name__] = tstp.TreeSitterTypeProvider(
     "tree_sitter_javascript",
     node_types,
@@ -44,22 +32,23 @@
 ```
 
 The module contains a number of dataclasses which represent the AST nodes:
 
 ```python
 import tree_sitter as ts
 import tree_sitter_type_provider as tstp
+import typing
 
 @dataclass
 class JsArray(tstp.Node):
     text: str
     type_name: str
     start_position: tstp.Point
     end_position: tstp.Point
-    children: list[Union[JsExpression, JsSpreadElement]]
+    children: typing.List[typing.Union[JsExpression, JsSpreadElement]]
 
 @dataclass
 class JsDeclaration(tstp.Node):
     text: str
     type_name: str
     start_position: tstp.Point
     end_position: tstp.Point
@@ -75,9 +64,9 @@
 
 ...
 ```
 
 As well as a function to convert to the AST:
 
 ```python
-def from_tree_sitter(self, tsvalue: ts.Tree | ts.Node | ts.TreeCursor, *, encoding: str = 'utf-8') -> tstp.Node
+def from_tree_sitter(self, tsvalue: typing.Union[ts.Tree, ts.Node, ts.TreeCursor], *, encoding: str = 'utf-8') -> tstp.Node
 ```
```

### Comparing `tree_sitter_type_provider-2.1.8/tree_sitter_type_provider/__init__.py` & `tree_sitter_type_provider-2.2.0/src/tree_sitter_type_provider/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,82 +1,141 @@
-import collections.abc
-import types
-import typing
+from dataclasses import dataclass
+from types import ModuleType
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterator,
+    List,
+    Optional,
+    Sequence,
+    Type,
+    Union,
+    cast,
+)
 
-import tree_sitter  # type: ignore
+import tree_sitter
 
 from tree_sitter_type_provider.node_types import Branch as Branch
 from tree_sitter_type_provider.node_types import Leaf as Leaf
 from tree_sitter_type_provider.node_types import Node as Node
 from tree_sitter_type_provider.node_types import NodeArgsType as NodeArgsType
 from tree_sitter_type_provider.node_types import NodeFieldName as NodeFieldName
 from tree_sitter_type_provider.node_types import NodeType as NodeType
 from tree_sitter_type_provider.node_types import NodeTypeError as NodeTypeError
 from tree_sitter_type_provider.node_types import NodeTypeName as NodeTypeName
 from tree_sitter_type_provider.node_types import Point as Point
-from tree_sitter_type_provider.parse_error import ParseError
 
 
-class TreeSitterTypeProvider(types.ModuleType):
+@dataclass
+class ParseError(Exception, Branch):
+    children: List[Node]
+    contents: Optional[str] = None
+    filename: Optional[str] = None
+
+    @staticmethod
+    def _point_to_str(point: Point) -> str:
+        return f"line {point.line}, column {point.column}"
+
+    def _range(self) -> str:
+        if self.start_position.line == self.end_position.line:
+            return f"on line {self.start_position.line} between column {self.start_position.column} and {self.end_position.column}"
+        else:
+            return f" between {self._point_to_str(self.start_position)} and {self._point_to_str(self.end_position)}"
+
+    def _annotated_region(self) -> str:
+        if self.contents:
+
+            def _annotated_lines(
+                lines: Sequence[str],
+            ) -> Iterator[str]:
+                for l, line in enumerate(lines):
+                    yield line
+                    is_first_line = l == 0
+                    is_last_line = l == len(lines) - 1
+                    start = self.start_position.column if is_first_line else 0
+                    end = self.end_position.column if is_last_line else len(line)
+                    annotation: List[str] = []
+                    for c, _ in enumerate(line):
+                        if c < start or end < c:
+                            annotation.append(" ")
+                        else:
+                            annotation.append("^")
+                    yield "".join(annotation)
+
+            lines = self.contents.splitlines()
+            lines = lines[self.start_position.line : self.end_position.line + 1]
+            return "\n".join(_annotated_lines(lines))
+        else:
+            return self.text
+
+    def __str__(self) -> str:
+        return "".join(
+            (
+                f"Parse error ",
+                f"in {self.filename} " if self.filename else "",
+                f"{self._range()}:\n",
+                f"{self._annotated_region()}\n",
+            )
+        )
+
+
+class TreeSitterTypeProvider(ModuleType):
     def _node_type_name(
         self,
-        node: typing.Union[NodeTypeName, Node, NodeType, tree_sitter.Node],
+        node: Union[NodeTypeName, Node, NodeType, tree_sitter.Node],
     ) -> str:
         if isinstance(node, tree_sitter.Node):
-            return node.type
+            return cast(str, node.type)
         elif isinstance(node, Node):
             return node.type_name
         elif isinstance(node, NodeType):
             return node.type_name
         elif isinstance(node, str):
             return node
         else:
             raise NodeTypeError(
                 f"Cannot get node type name for object of type {type(node)}", node
             )
 
     def _node_type(
         self,
-        node: typing.Union[NodeTypeName, Node, NodeType, tree_sitter.Node],
+        node: Union[NodeTypeName, Node, NodeType, tree_sitter.Node],
     ) -> NodeType:
         node_type_name = self._node_type_name(node)
         node_type = self._node_types_by_type.get(node_type_name, None)
         if node_type is None:
             raise NodeTypeError(f"Could not find node type {node_type_name}")
         return node_type
 
     def _node_has_children(
         self,
-        node: typing.Union[NodeTypeName, Node, NodeType, tree_sitter.Node],
+        node: Union[NodeTypeName, Node, NodeType, tree_sitter.Node],
     ) -> bool:
         node_type = self._node_type(node)
         # NOTE: Any node with content can have extra nodes,
         #       even if the node only has fields and no children.
         return node_type.has_content
 
-    def _node_class(
-        self, node: typing.Union[Node, NodeType, tree_sitter.Node]
-    ) -> type[Node]:
+    def _node_class(self, node: Union[Node, NodeType, tree_sitter.Node]) -> Type[Node]:
         node_type_name = self._node_type_name(node)
         cls = self._node_classes_by_type.get(node_type_name, None)
         if cls is None:
             raise NodeTypeError(f"Could not find node type {node_type_name}")
         return cls
 
     def _node_hash(self, tsnode: tree_sitter.Node) -> int:
         return hash((tsnode.start_byte, tsnode.end_byte))
 
     def from_tree_sitter(
         self,
-        tsvalue: typing.Union[
-            tree_sitter.Tree, tree_sitter.Node, tree_sitter.TreeCursor
-        ],
+        tsvalue: Union[tree_sitter.Tree, tree_sitter.Node, tree_sitter.TreeCursor],
         *,
         encoding: str = "utf-8",
-        filename: typing.Optional[str] = None,
+        filename: Optional[str] = None,
         raise_parse_error: bool = False,
     ) -> Node:
         if isinstance(tsvalue, tree_sitter.Tree):
             tsvalue = tsvalue.root_node
         if isinstance(tsvalue, tree_sitter.Node):
             tsvalue = tsvalue.walk()
         return self._from_tree_cursor(
@@ -87,31 +146,34 @@
         )
 
     def _from_tree_cursor(
         self,
         tscursor: tree_sitter.TreeCursor,
         *,
         encoding: str = "utf-8",
-        filename: typing.Optional[str] = None,
+        filename: Optional[str] = None,
         raise_parse_error: bool,
     ) -> Node:
         if tscursor.node.is_named:
             # Convert basic information.
             text: str = tscursor.node.text.decode(encoding)
             type_name: str = tscursor.node.type
             node_type: NodeType = self._node_type(type_name)
             start_position: Point = Point.from_tree_sitter(tscursor.node.start_point)
             end_position: Point = Point.from_tree_sitter(tscursor.node.end_point)
 
             # Convert children.
-            fields: dict[str, typing.Union[None, Node, list[Node]]] = {}
-            children: list[Node] = []
+            fields: Dict[str, Union[None, Node, List[Node]]] = {}
+            children: List[Node] = []
 
-            def convert_child(tscursor: tree_sitter.TreeCursor):
-                field_name = tscursor.current_field_name()
+            def convert_child(tscursor: tree_sitter.TreeCursor) -> None:
+                try:
+                    field_name = tscursor.field_name
+                except AttributeError:
+                    field_name = tscursor.current_field_name()
                 child = self._from_tree_cursor(
                     tscursor,
                     encoding=encoding,
                     filename=filename,
                     raise_parse_error=raise_parse_error,
                 )
                 if field_name is None:
@@ -144,69 +206,69 @@
                 if not field_type.required and field_name not in fields:
                     if field_type.multiple:
                         fields[field_name] = []
                     else:
                         fields[field_name] = None
 
             # Create node instance
-            kwargs: dict[str, typing.Union[str, Point, None, Node, list[Node]]] = {}
+            kwargs: Dict[str, Union[str, Point, None, Node, List[Node]]] = {}
             kwargs["type_name"] = type_name
             kwargs["text"] = text
             kwargs["start_position"] = start_position
             kwargs["end_position"] = end_position
             if self._node_has_children(tscursor.node):
                 kwargs["children"] = children
-            kwargs |= fields
+            kwargs.update(fields)
 
             # Return the node with its field name.
             if raise_parse_error and type_name == "ERROR":
 
                 def _root_node(tsnode: tree_sitter.Node) -> str:
                     # TODO: node->tree isn't bound in tree_sitter_talon
                     if tsnode.parent:
                         return _root_node(tsnode.parent)
                     else:
-                        return tsnode.text.decode("utf-8")
+                        return cast(str, tsnode.text.decode("utf-8"))
 
                 contents = _root_node(tscursor.node)
                 raise ParseError(
                     text=text,
                     type_name=type_name,
                     start_position=start_position,
                     end_position=end_position,
                     children=children,
                     contents=contents,
                     filename=filename,
                 )
             else:
-                return self._node_class(tscursor.node)(**kwargs)  # type: ignore
+                return self._node_class(tscursor.node)(**kwargs)  # type: ignore[arg-type]
         else:
             raise TypeError(tscursor.node.type)
 
     def __init__(
         self,
         module_name: str,
-        node_types: typing.Sequence[NodeType],
+        node_types: Sequence[NodeType],
         *,
-        extra: typing.Sequence[NodeTypeName] = (),
-        as_class_name: typing.Optional[collections.abc.Callable[[str], str]] = None,
-        mixins: typing.Sequence[type] = (),
-        dataclass_kwargs: dict[str, typing.Any] = {},
+        extra: Sequence[NodeTypeName] = (),
+        as_class_name: Optional[Callable[[str], str]] = None,
+        mixins: Sequence[type] = (),
+        dataclass_kwargs: Dict[str, Any] = {},
     ):
         super().__init__(name=module_name)
 
         if as_class_name is None:
 
             def snake_to_pascal(node_type_name: str) -> str:
                 return "".join(map(str.capitalize, node_type_name.split("_")))
 
             as_class_name = snake_to_pascal
 
         # Dictionary of named node types
-        self._node_types_by_type: dict[str, NodeType] = {}
+        self._node_types_by_type: Dict[str, NodeType] = {}
         for node_type in node_types:
             if node_type.named:
                 self._node_types_by_type[node_type.type_name] = node_type
 
         # Insert node types for extra nodes
         for type_name in extra:
             if type_name not in self._node_types_by_type:
@@ -220,24 +282,24 @@
                 multiple=True,
                 required=True,
                 types=list(node_types),
             ),
         )
 
         # Create the list of extra node types
-        def _extra_node_types() -> collections.abc.Iterator[NodeType]:
+        def _extra_node_types() -> Iterator[NodeType]:
             for type_name in extra:
                 yield self._node_type(type_name)
             if "ERROR" not in extra:
                 yield self._node_type("ERROR")
 
-        self._extra: typing.Sequence = tuple(_extra_node_types())
+        self._extra: Sequence[NodeType] = tuple(_extra_node_types())
 
         # Dictionary of abstract classes
-        self._node_bases_by_type: dict[str, list[type[Node]]] = {}
+        self._node_bases_by_type: Dict[str, List[Type[Node]]] = {}
         for node_type in self._node_types_by_type.values():
             if node_type.is_abstract:
                 abscls = node_type.as_type(
                     as_class_name=as_class_name,
                     base=Node,
                     mixins=mixins,
                     extra=self._extra,
@@ -247,15 +309,15 @@
                 for subtype in node_type.subtypes:
                     if subtype.named:
                         if subtype.type_name not in self._node_bases_by_type:
                             self._node_bases_by_type[subtype.type_name] = []
                         self._node_bases_by_type[subtype.type_name].append(abscls)
 
         # Dictionary of dataclasses
-        self._node_classes_by_type: dict[str, type[Node]] = {}
+        self._node_classes_by_type: Dict[str, Type[Node]] = {}
         for node_type in self._node_types_by_type.values():
             if node_type.type_name == "ERROR":
                 self._node_classes_by_type["ERROR"] = ParseError
                 setattr(self, as_class_name(node_type.type_name), ParseError)
             else:
                 bases = self._node_bases_by_type.get(node_type.type_name, ())
                 cls = node_type.as_type(
```

### Comparing `tree_sitter_type_provider-2.1.8/tree_sitter_type_provider/node_types.py` & `tree_sitter_type_provider-2.2.0/src/tree_sitter_type_provider/node_types.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,218 +1,224 @@
-import abc
-import collections.abc
-import dataclasses
 import functools
 import itertools
-import typing
+from dataclasses import dataclass, field, make_dataclass
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
 
-import dataclasses_json
+from dataclasses_json import DataClassJsonMixin, config, dataclass_json
 
 
 class NodeTypeError(Exception):
     pass
 
 
-@dataclasses.dataclass
+@dataclass
 class Point:
     line: int
     column: int
 
     @staticmethod
-    def from_tree_sitter(tspoint: tuple[int, int]) -> "Point":
+    def from_tree_sitter(tspoint: Tuple[int, int]) -> "Point":
         return Point(line=tspoint[0], column=tspoint[1])
 
 
 NodeTypeName = str
 
 NodeFieldName = str
 
-AsClassName = collections.abc.Callable[[NodeTypeName], str]
+AsClassName = Callable[[NodeTypeName], str]
 
 
-@dataclasses.dataclass
-class Node(dataclasses_json.DataClassJsonMixin):
+@dataclass
+class Node(DataClassJsonMixin):
     text: str
-    type_name: NodeTypeName = dataclasses.field(
-        metadata=dataclasses_json.config(field_name="type")
-    )
+    type_name: NodeTypeName = field(metadata=config(field_name="type"))
     start_position: Point
     end_position: Point
 
     def is_equivalent(self, other: "Node") -> bool:
         try:
             self.assert_equivalent(other)
             return True
         except AssertionError:
             return False
 
-    def assert_equivalent(self, other: "Node"):
-        return NotImplemented
+    def assert_equivalent(self, other: "Node") -> None:
+        pass
 
 
-@dataclasses.dataclass
+@dataclass
 class Leaf(Node):
     pass
 
 
-@dataclasses.dataclass
+@dataclass
 class Branch(Node):
-    children: typing.Union[None, Node, typing.Sequence[Node]]
+    children: Union[None, Node, Sequence[Node]]
 
 
-@dataclasses_json.dataclass_json
-@dataclasses.dataclass
-class SimpleNodeType:
-    type_name: NodeTypeName = dataclasses.field(
-        metadata=dataclasses_json.config(field_name="type")
-    )
+@dataclass
+class SimpleNodeType(DataClassJsonMixin):
+    type_name: NodeTypeName = field(metadata=config(field_name="type"))
     named: bool
 
-    def is_extra(self, *, extra: typing.Sequence["SimpleNodeType"]) -> bool:
+    def is_extra(self, *, extra: Sequence["SimpleNodeType"]) -> bool:
         return any(self.type_name == other.type_name for other in extra)
 
-    def as_typehint(self, *, as_class_name: AsClassName) -> type[Node]:
+    def as_typehint(self, *, as_class_name: AsClassName) -> Type[Node]:
         if self.named:
-            return typing.cast(type, as_class_name(self.type_name))
+            return cast(type, as_class_name(self.type_name))
         raise ValueError(self)
 
     @staticmethod
     def many_as_typehint(
-        simple_node_types: typing.Sequence["SimpleNodeType"],
+        simple_node_types: Sequence["SimpleNodeType"],
         *,
         as_class_name: AsClassName,
-    ) -> typing.Optional[type[Node]]:
-        Ts: list[type] = []
+    ) -> Optional[Type[Node]]:
+        Ts: List[type] = []
         for simple_node_type in simple_node_types:
             if simple_node_type.named:
                 Ts.append(simple_node_type.as_typehint(as_class_name=as_class_name))
 
         if len(Ts) == 0:
             return None
 
         if len(Ts) == 1:
             return Ts[0]
 
-        return functools.reduce(lambda R, T: typing.cast(type, typing.Union[R, T]), Ts)
+        return functools.reduce(lambda R, T: cast(type, Union[R, T]), Ts)
 
 
-@dataclasses_json.dataclass_json
-@dataclasses.dataclass
+@dataclass_json
+@dataclass
 class NodeArgsType:
     multiple: bool = False
     required: bool = False
-    types: list[SimpleNodeType] = dataclasses.field(default_factory=list)
+    types: List[SimpleNodeType] = field(default_factory=list)
 
     @property
     def named(self) -> bool:
         return any(type.named for type in self.types)
 
     def __bool__(self) -> bool:
         return bool(self.types)
 
     def assert_equivalent(
         self,
-        node1: typing.Union[None, Node, typing.Sequence[Node]],
-        node2: typing.Union[None, Node, typing.Sequence[Node]],
+        node1: Union[None, Node, Sequence[Node]],
+        node2: Union[None, Node, Sequence[Node]],
     ) -> None:
-        if node1 is None:
-            assert node2 is None
-        elif isinstance(node1, Node):
-            assert isinstance(node2, Node)
-            node1.assert_equivalent(node2)
-        else:
-            assert isinstance(node2, typing.Sequence)
-            for child1, child2 in itertools.zip_longest(node1, node2):
-                assert isinstance(child1, Node)
-                assert isinstance(child2, Node)
-                child1.assert_equivalent(child2)
+        if self.named:
+            if node1 is None:
+                assert node2 is None
+            elif isinstance(node1, Node):
+                assert isinstance(node2, Node)
+                node1.assert_equivalent(node2)
+            else:
+                assert isinstance(node2, Sequence)
+                for child1, child2 in itertools.zip_longest(node1, node2):
+                    assert isinstance(child1, Node)
+                    assert isinstance(child2, Node)
+                    child1.assert_equivalent(child2)
 
     def as_typehint(
         self,
         *,
         is_field: bool,
         as_class_name: AsClassName,
-        extra: typing.Sequence[SimpleNodeType],
-    ) -> typing.Optional[type[Node]]:
+        extra: Sequence[SimpleNodeType],
+    ) -> Optional[Type[Node]]:
         if is_field:
             types_with_extra = tuple(self.types)
             multiple_with_extra = self.multiple
         else:
             # Add the extra nodes into the possible children
             types_with_extra = tuple((*self.types, *extra))
             # If there are extra nodes, a node can have any number of children
             multiple_with_extra = bool(extra) or self.multiple
         T = SimpleNodeType.many_as_typehint(
             types_with_extra, as_class_name=as_class_name
         )
         if T is not None:
             if multiple_with_extra:
-                return list[T]  # type: ignore
+                return List[T]  # type: ignore
             else:
                 if self.required:
                     return T
                 else:
-                    return typing.Optional[T]  # type: ignore
+                    return Optional[T]  # type: ignore
         else:
             return None
 
 
-@dataclasses_json.dataclass_json
-@dataclasses.dataclass
+@dataclass
 class NodeType(SimpleNodeType):
-    fields: dict[NodeFieldName, NodeArgsType] = dataclasses.field(default_factory=dict)
-    children: NodeArgsType = dataclasses.field(default_factory=NodeArgsType)
-    subtypes: list[SimpleNodeType] = dataclasses.field(default_factory=list)
+    fields: Dict[NodeFieldName, NodeArgsType] = field(default_factory=dict)
+    children: NodeArgsType = field(default_factory=NodeArgsType)
+    subtypes: List[SimpleNodeType] = field(default_factory=list)
 
-    def __post_init__(self, **kwargs):
+    def __post_init__(self, **kwargs: Any) -> None:
         assert not (
             self.is_abstract and self.has_content
         ), "Nodes can have either fields and children or subtypes, but not both."
 
     @property
     def is_abstract(self) -> bool:
         return len(self.subtypes) > 0
 
     @property
     def has_content(self) -> bool:
         return len(self.fields) > 0 or bool(self.children)
 
-    def assert_equivalent(self, node1: Node, node2: Node):
+    def assert_equivalent(self, node1: Node, node2: Node) -> None:
         if self.has_content:
             # compare children
             if hasattr(node1, "children"):
                 assert hasattr(node2, "children")
                 children1 = getattr(node1, "children")
                 children2 = getattr(node2, "children")
                 self.children.assert_equivalent(children1, children2)
             # compare fields
             for field_name, field_type in self.fields.items():
-                assert hasattr(node1, field_name)
-                assert hasattr(node2, field_name)
-                field1 = getattr(node1, field_name)
-                field2 = getattr(node2, field_name)
-                field_type.assert_equivalent(field1, field2)
+                if hasattr(node1, field_name):
+                    assert hasattr(node2, field_name)
+                    field1 = getattr(node1, field_name)
+                    field2 = getattr(node2, field_name)
+                    field_type.assert_equivalent(field1, field2)
+                else:
+                    assert not hasattr(node2, field_name)
         else:
-            return node1.text == node2.text
+            assert node1.text == node2.text
 
     def as_type(
         self,
         *,
         as_class_name: AsClassName,
-        mixins: typing.Sequence[type] = (),
-        extra: typing.Sequence[SimpleNodeType],
-        **kwargs,
-    ) -> type[Node]:
+        mixins: Sequence[type] = (),
+        extra: Sequence[SimpleNodeType],
+        **kwargs: Any,
+    ) -> Type[Node]:
         if self.named:
             cls_name = as_class_name(self.type_name)
             if self.is_abstract:
                 # TODO: should be a dynamic type alias
                 return type(cls_name, (Node,), {})
             else:
-                fields: dict[NodeFieldName, type] = {}
+                fields: Dict[NodeFieldName, Type[Any]] = {}
 
                 # Create fields for dataclass
                 for field_name, field in self.fields.items():
                     if field.named:
                         field_type = field.as_typehint(
                             is_field=True, as_class_name=as_class_name, extra=extra
                         )
@@ -223,36 +229,36 @@
                 if self.has_content:
                     children_type = self.children.as_typehint(
                         is_field=False, as_class_name=as_class_name, extra=extra
                     )
                     if children_type:
                         fields["children"] = children_type
                     else:
-                        fields["children"] = typing.cast(type, None)
+                        fields["children"] = cast(type, None)
 
                 # Create bases for dataclass
-                base: type[Node]
+                base: Type[Node]
                 if self.is_abstract:
                     base = Node
                 elif self.has_content:
                     base = Branch
                 else:
                     base = Leaf
 
                 # Create implementation of is_equivalent
                 node_type = self
 
-                def assert_equivalent(self, other: Node):
+                def _assert_equivalent(self: Node, other: Node) -> None:
                     node_type.assert_equivalent(self, other)
 
                 # Create and return dataclass
-                return dataclasses.make_dataclass(
+                return make_dataclass(
                     cls_name=cls_name,
                     fields=fields.items(),
                     bases=(base, *mixins),
                     namespace={
-                        "assert_equivalent": assert_equivalent,
+                        "assert_equivalent": _assert_equivalent,
                     },
                     **kwargs,
                 )
         else:
             raise ValueError(self)
```

