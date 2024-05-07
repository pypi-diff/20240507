# Comparing `tmp/itemadapter-0.7.0.tar.gz` & `tmp/itemadapter-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itemadapter-0.7.0.tar", last modified: Tue Aug  2 17:45:43 2022, max compression
+gzip compressed data, was "itemadapter-0.8.0.tar", last modified: Thu Mar 30 19:15:13 2023, max compression
```

## Comparing `itemadapter-0.7.0.tar` & `itemadapter-0.8.0.tar`

### file list

```diff
@@ -1,18 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 17:45:43.852445 itemadapter-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-08-02 17:45:33.000000 itemadapter-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-02 17:45:33.000000 itemadapter-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    16945 2022-08-02 17:45:43.852445 itemadapter-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15962 2022-08-02 17:45:33.000000 itemadapter-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 17:45:43.848446 itemadapter-0.7.0/itemadapter/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-08-02 17:45:33.000000 itemadapter-0.7.0/itemadapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      978 2022-08-02 17:45:33.000000 itemadapter-0.7.0/itemadapter/_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)    13282 2022-08-02 17:45:33.000000 itemadapter-0.7.0/itemadapter/adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4007 2022-08-02 17:45:33.000000 itemadapter-0.7.0/itemadapter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 17:45:43.848446 itemadapter-0.7.0/itemadapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16945 2022-08-02 17:45:43.000000 itemadapter-0.7.0/itemadapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-08-02 17:45:43.000000 itemadapter-0.7.0/itemadapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-02 17:45:43.000000 itemadapter-0.7.0/itemadapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-02 17:45:43.000000 itemadapter-0.7.0/itemadapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-08-02 17:45:33.000000 itemadapter-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-08-02 17:45:43.852445 itemadapter-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-08-02 17:45:33.000000 itemadapter-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:15:13.236836 itemadapter-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-03-30 19:15:04.000000 itemadapter-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-30 19:15:04.000000 itemadapter-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17757 2023-03-30 19:15:13.236836 itemadapter-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16773 2023-03-30 19:15:04.000000 itemadapter-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:15:13.236836 itemadapter-0.8.0/itemadapter/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-30 19:15:04.000000 itemadapter-0.8.0/itemadapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-30 19:15:04.000000 itemadapter-0.8.0/itemadapter/_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12992 2023-03-30 19:15:04.000000 itemadapter-0.8.0/itemadapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 19:15:04.000000 itemadapter-0.8.0/itemadapter/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-03-30 19:15:04.000000 itemadapter-0.8.0/itemadapter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:15:13.236836 itemadapter-0.8.0/itemadapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17757 2023-03-30 19:15:13.000000 itemadapter-0.8.0/itemadapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-03-30 19:15:13.000000 itemadapter-0.8.0/itemadapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 19:15:13.000000 itemadapter-0.8.0/itemadapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-30 19:15:13.000000 itemadapter-0.8.0/itemadapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-30 19:15:04.000000 itemadapter-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-30 19:15:13.236836 itemadapter-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-30 19:15:04.000000 itemadapter-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:15:13.236836 itemadapter-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-03-30 19:15:04.000000 itemadapter-0.8.0/tests/test_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-03-30 19:15:04.000000 itemadapter-0.8.0/tests/test_adapter_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-03-30 19:15:04.000000 itemadapter-0.8.0/tests/test_adapter_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-03-30 19:15:04.000000 itemadapter-0.8.0/tests/test_adapter_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-03-30 19:15:04.000000 itemadapter-0.8.0/tests/test_adapter_scrapy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-03-30 19:15:04.000000 itemadapter-0.8.0/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-30 19:15:04.000000 itemadapter-0.8.0/tests/test_itemadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-03-30 19:15:04.000000 itemadapter-0.8.0/tests/test_utils.py
```

### Comparing `itemadapter-0.7.0/LICENSE` & `itemadapter-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `itemadapter-0.7.0/PKG-INFO` & `itemadapter-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: itemadapter
-Version: 0.7.0
+Version: 0.8.0
 Summary: Common interface for data container classes
 Home-page: https://github.com/scrapy/itemadapter
 Author: Eugenio Lacuesta
 Author-email: eugenio.lacuesta@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Scrapy
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # itemadapter
 [![version](https://img.shields.io/pypi/v/itemadapter.svg)](https://pypi.python.org/pypi/itemadapter)
 [![pyversions](https://img.shields.io/pypi/pyversions/itemadapter.svg)](https://pypi.python.org/pypi/itemadapter)
 [![actions](https://github.com/scrapy/itemadapter/workflows/Tests/badge.svg)](https://github.com/scrapy/itemadapter/actions)
@@ -45,19 +45,16 @@
 Additionally, interaction with arbitrary types is supported, by implementing
 a pre-defined interface (see [extending `itemadapter`](#extending-itemadapter)).
 
 ---
 
 ## Requirements
 
-* Python 3.6+
+* Python 3.7+
 * [`scrapy`](https://scrapy.org/): optional, needed to interact with `scrapy` items
-* `dataclasses` ([stdlib](https://docs.python.org/3/library/dataclasses.html) in Python 3.7+,
-  or its [backport](https://pypi.org/project/dataclasses/) in Python 3.6): optional, needed
-  to interact with `dataclass`-based items
 * [`attrs`](https://pypi.org/project/attrs/): optional, needed to interact with `attrs`-based items
 * [`pydantic`](https://pypi.org/project/pydantic/): optional, needed to interact with `pydantic`-based items
 
 ---
 
 ## Installation
 
@@ -398,14 +395,54 @@
 >>> item = FakeItemClass()
 >>> adapter = ItemAdapter(item)
 >>> adapter
 <ItemAdapter for FakeItemClass()>
 >>>
 ```
 
+### Multiple adapter classes
+
+If you need to have different handlers and/or priorities for different cases
+you can subclass the `ItemAdapter` class and set the `ADAPTER_CLASSES`
+attribute as needed:
+
+
+**Example**
+```python
+>>> from collections import deque
+>>> from itemadapter.adapter import (
+...     ItemAdapter,
+...     AttrsAdapter,
+...     DataclassAdapter,
+...     DictAdapter,
+...     PydanticAdapter,
+...     ScrapyItemAdapter,
+... )
+>>> from scrapy.item import Item, Field
+>>>
+>>> class BuiltinTypesItemAdapter(ItemAdapter):
+...     ADAPTER_CLASSES = deque([DictAdapter, DataclassAdapter])
+...
+>>> class ThirdPartyTypesItemAdapter(ItemAdapter):
+...     ADAPTER_CLASSES = deque([AttrsAdapter, PydanticAdapter, ScrapyItemAdapter])
+...
+>>> class ScrapyItem(Item):
+...     foo = Field()
+...
+>>> BuiltinTypesItemAdapter.is_item(dict())
+True
+>>> ThirdPartyTypesItemAdapter.is_item(dict())
+False
+>>> BuiltinTypesItemAdapter.is_item(ScrapyItem(foo="bar"))
+False
+>>> ThirdPartyTypesItemAdapter.is_item(ScrapyItem(foo="bar"))
+True
+>>>
+```
+
 ---
 
 ## More examples
 
 ### `scrapy.item.Item` objects
 
 ```python
```

### Comparing `itemadapter-0.7.0/README.md` & `itemadapter-0.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,19 +20,16 @@
 Additionally, interaction with arbitrary types is supported, by implementing
 a pre-defined interface (see [extending `itemadapter`](#extending-itemadapter)).
 
 ---
 
 ## Requirements
 
-* Python 3.6+
+* Python 3.7+
 * [`scrapy`](https://scrapy.org/): optional, needed to interact with `scrapy` items
-* `dataclasses` ([stdlib](https://docs.python.org/3/library/dataclasses.html) in Python 3.7+,
-  or its [backport](https://pypi.org/project/dataclasses/) in Python 3.6): optional, needed
-  to interact with `dataclass`-based items
 * [`attrs`](https://pypi.org/project/attrs/): optional, needed to interact with `attrs`-based items
 * [`pydantic`](https://pypi.org/project/pydantic/): optional, needed to interact with `pydantic`-based items
 
 ---
 
 ## Installation
 
@@ -373,14 +370,54 @@
 >>> item = FakeItemClass()
 >>> adapter = ItemAdapter(item)
 >>> adapter
 <ItemAdapter for FakeItemClass()>
 >>>
 ```
 
+### Multiple adapter classes
+
+If you need to have different handlers and/or priorities for different cases
+you can subclass the `ItemAdapter` class and set the `ADAPTER_CLASSES`
+attribute as needed:
+
+
+**Example**
+```python
+>>> from collections import deque
+>>> from itemadapter.adapter import (
+...     ItemAdapter,
+...     AttrsAdapter,
+...     DataclassAdapter,
+...     DictAdapter,
+...     PydanticAdapter,
+...     ScrapyItemAdapter,
+... )
+>>> from scrapy.item import Item, Field
+>>>
+>>> class BuiltinTypesItemAdapter(ItemAdapter):
+...     ADAPTER_CLASSES = deque([DictAdapter, DataclassAdapter])
+...
+>>> class ThirdPartyTypesItemAdapter(ItemAdapter):
+...     ADAPTER_CLASSES = deque([AttrsAdapter, PydanticAdapter, ScrapyItemAdapter])
+...
+>>> class ScrapyItem(Item):
+...     foo = Field()
+...
+>>> BuiltinTypesItemAdapter.is_item(dict())
+True
+>>> ThirdPartyTypesItemAdapter.is_item(dict())
+False
+>>> BuiltinTypesItemAdapter.is_item(ScrapyItem(foo="bar"))
+False
+>>> ThirdPartyTypesItemAdapter.is_item(ScrapyItem(foo="bar"))
+True
+>>>
+```
+
 ---
 
 ## More examples
 
 ### `scrapy.item.Item` objects
 
 ```python
```

### Comparing `itemadapter-0.7.0/itemadapter/_imports.py` & `itemadapter-0.8.0/itemadapter/_imports.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,19 +14,14 @@
         _base_item_cls = getattr(scrapy.item, "_BaseItem", scrapy.item.BaseItem)
     except AttributeError:
         _scrapy_item_classes = (scrapy.item.Item,)
     else:
         _scrapy_item_classes = (scrapy.item.Item, _base_item_cls)
 
 try:
-    import dataclasses  # pylint: disable=W0611 (unused-import)
-except ImportError:
-    dataclasses = None  # type: ignore [assignment]
-
-try:
     import attr  # pylint: disable=W0611 (unused-import)
 except ImportError:
     attr = None  # type: ignore [assignment]
 
 try:
     import pydantic  # pylint: disable=W0611 (unused-import)
 except ImportError:
```

### Comparing `itemadapter-0.7.0/itemadapter/adapter.py` & `itemadapter-0.8.0/itemadapter/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
+import dataclasses
 from abc import abstractmethod, ABCMeta
 from collections import deque
 from collections.abc import KeysView, MutableMapping
 from types import MappingProxyType
 from typing import Any, Deque, Iterator, Type, Optional, List
 
 from itemadapter.utils import (
     _get_pydantic_model_metadata,
     _is_attrs_class,
-    _is_dataclass,
     _is_pydantic_model,
 )
 
-from itemadapter._imports import attr, dataclasses, _scrapy_item_classes
+from itemadapter._imports import attr, _scrapy_item_classes
 
 
 __all__ = [
     "AdapterInterface",
     "AttrsAdapter",
     "DataclassAdapter",
     "DictAdapter",
@@ -135,40 +135,34 @@
             raise RuntimeError("attr module is not available")
         return [a.name for a in attr.fields(item_class)]
 
 
 class DataclassAdapter(_MixinAttrsDataclassAdapter, AdapterInterface):
     def __init__(self, item: Any) -> None:
         super().__init__(item)
-        if dataclasses is None:
-            raise RuntimeError("dataclasses module is not available")
         # store a reference to the item's fields to avoid O(n) lookups and O(n^2) traversals
         self._fields_dict = {field.name: field for field in dataclasses.fields(self.item)}
 
     @classmethod
     def is_item(cls, item: Any) -> bool:
-        return _is_dataclass(item) and not isinstance(item, type)
+        return dataclasses.is_dataclass(item) and not isinstance(item, type)
 
     @classmethod
     def is_item_class(cls, item_class: type) -> bool:
-        return _is_dataclass(item_class)
+        return dataclasses.is_dataclass(item_class)
 
     @classmethod
     def get_field_meta_from_class(cls, item_class: type, field_name: str) -> MappingProxyType:
-        if dataclasses is None:
-            raise RuntimeError("dataclasses module is not available")
         for field in dataclasses.fields(item_class):
             if field.name == field_name:
                 return field.metadata  # type: ignore
         raise KeyError(f"{item_class.__name__} does not support field: {field_name}")
 
     @classmethod
     def get_field_names_from_class(cls, item_class: type) -> Optional[List[str]]:
-        if dataclasses is None:
-            raise RuntimeError("dataclasses module is not available")
         return [a.name for a in dataclasses.fields(item_class)]
 
 
 class PydanticAdapter(AdapterInterface):
 
     item: Any
 
@@ -357,21 +351,20 @@
         """Return read-only key view with the names of all the defined fields for the item."""
         return self.adapter.field_names()
 
     def asdict(self) -> dict:
         """Return a dict object with the contents of the adapter. This works slightly different
         than calling `dict(adapter)`: it's applied recursively to nested items (if there are any).
         """
-        return {key: _asdict(value) for key, value in self.items()}
+        return {key: self._asdict(value) for key, value in self.items()}
 
-
-def _asdict(obj: Any) -> Any:
-    """Helper for ItemAdapter.asdict()."""
-    if isinstance(obj, dict):
-        return {key: _asdict(value) for key, value in obj.items()}
-    if isinstance(obj, (list, set, tuple)):
-        return obj.__class__(_asdict(x) for x in obj)
-    if isinstance(obj, ItemAdapter):
-        return obj.asdict()
-    if ItemAdapter.is_item(obj):
-        return ItemAdapter(obj).asdict()
-    return obj
+    @classmethod
+    def _asdict(cls, obj: Any) -> Any:
+        if isinstance(obj, dict):
+            return {key: cls._asdict(value) for key, value in obj.items()}
+        if isinstance(obj, (list, set, tuple)):
+            return obj.__class__(cls._asdict(x) for x in obj)
+        if isinstance(obj, cls):
+            return obj.asdict()
+        if cls.is_item(obj):
+            return cls(obj).asdict()
+        return obj
```

### Comparing `itemadapter-0.7.0/itemadapter/utils.py` & `itemadapter-0.8.0/itemadapter/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,18 @@
 import warnings
 
 from types import MappingProxyType
 from typing import Any
 
-from itemadapter._imports import attr, dataclasses, pydantic
+from itemadapter._imports import attr, pydantic
 
 
 __all__ = ["is_item", "get_field_meta_from_class"]
 
 
-def _is_dataclass(obj: Any) -> bool:
-    """In py36, this returns False if the "dataclasses" backport module is not installed."""
-    if dataclasses is None:
-        return False
-    return dataclasses.is_dataclass(obj)
-
-
 def _is_attrs_class(obj: Any) -> bool:
     if attr is None:
         return False
     return attr.has(obj)
 
 
 def _is_pydantic_model(obj: Any) -> bool:
```

### Comparing `itemadapter-0.7.0/itemadapter.egg-info/PKG-INFO` & `itemadapter-0.8.0/itemadapter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: itemadapter
-Version: 0.7.0
+Version: 0.8.0
 Summary: Common interface for data container classes
 Home-page: https://github.com/scrapy/itemadapter
 Author: Eugenio Lacuesta
 Author-email: eugenio.lacuesta@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Scrapy
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # itemadapter
 [![version](https://img.shields.io/pypi/v/itemadapter.svg)](https://pypi.python.org/pypi/itemadapter)
 [![pyversions](https://img.shields.io/pypi/pyversions/itemadapter.svg)](https://pypi.python.org/pypi/itemadapter)
 [![actions](https://github.com/scrapy/itemadapter/workflows/Tests/badge.svg)](https://github.com/scrapy/itemadapter/actions)
@@ -45,19 +45,16 @@
 Additionally, interaction with arbitrary types is supported, by implementing
 a pre-defined interface (see [extending `itemadapter`](#extending-itemadapter)).
 
 ---
 
 ## Requirements
 
-* Python 3.6+
+* Python 3.7+
 * [`scrapy`](https://scrapy.org/): optional, needed to interact with `scrapy` items
-* `dataclasses` ([stdlib](https://docs.python.org/3/library/dataclasses.html) in Python 3.7+,
-  or its [backport](https://pypi.org/project/dataclasses/) in Python 3.6): optional, needed
-  to interact with `dataclass`-based items
 * [`attrs`](https://pypi.org/project/attrs/): optional, needed to interact with `attrs`-based items
 * [`pydantic`](https://pypi.org/project/pydantic/): optional, needed to interact with `pydantic`-based items
 
 ---
 
 ## Installation
 
@@ -398,14 +395,54 @@
 >>> item = FakeItemClass()
 >>> adapter = ItemAdapter(item)
 >>> adapter
 <ItemAdapter for FakeItemClass()>
 >>>
 ```
 
+### Multiple adapter classes
+
+If you need to have different handlers and/or priorities for different cases
+you can subclass the `ItemAdapter` class and set the `ADAPTER_CLASSES`
+attribute as needed:
+
+
+**Example**
+```python
+>>> from collections import deque
+>>> from itemadapter.adapter import (
+...     ItemAdapter,
+...     AttrsAdapter,
+...     DataclassAdapter,
+...     DictAdapter,
+...     PydanticAdapter,
+...     ScrapyItemAdapter,
+... )
+>>> from scrapy.item import Item, Field
+>>>
+>>> class BuiltinTypesItemAdapter(ItemAdapter):
+...     ADAPTER_CLASSES = deque([DictAdapter, DataclassAdapter])
+...
+>>> class ThirdPartyTypesItemAdapter(ItemAdapter):
+...     ADAPTER_CLASSES = deque([AttrsAdapter, PydanticAdapter, ScrapyItemAdapter])
+...
+>>> class ScrapyItem(Item):
+...     foo = Field()
+...
+>>> BuiltinTypesItemAdapter.is_item(dict())
+True
+>>> ThirdPartyTypesItemAdapter.is_item(dict())
+False
+>>> BuiltinTypesItemAdapter.is_item(ScrapyItem(foo="bar"))
+False
+>>> ThirdPartyTypesItemAdapter.is_item(ScrapyItem(foo="bar"))
+True
+>>>
+```
+
 ---
 
 ## More examples
 
 ### `scrapy.item.Item` objects
 
 ```python
```

### Comparing `itemadapter-0.7.0/setup.py` & `itemadapter-0.8.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,33 +3,37 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="itemadapter",
-    version="0.7.0",
+    version="0.8.0",
     license="BSD",
     description="Common interface for data container classes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Eugenio Lacuesta",
     author_email="eugenio.lacuesta@gmail.com",
     url="https://github.com/scrapy/itemadapter",
     packages=["itemadapter"],
-    python_requires=">=3.6",
+    package_data={
+        "itemadapter": ["py.typed"],
+    },
+    include_package_data=True,
+    python_requires=">=3.7",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Framework :: Scrapy",
         "Intended Audience :: Developers",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

