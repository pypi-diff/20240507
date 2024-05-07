# Comparing `tmp/ucbreq-2.0.4.tar.gz` & `tmp/ucbreq-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucbreq-2.0.4.tar", last modified: Tue Jan  3 20:33:58 2023, max compression
+gzip compressed data, was "ucbreq-2.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ucbreq-2.0.4.tar` & `ucbreq-2.0.5.tar`

### file list

```diff
@@ -1,5 +1,16 @@
--rw-r--r--   0        0        0     2200 2020-11-17 18:33:59.501340 ucbreq-2.0.4/README.rst
--rw-r--r--   0        0        0      900 2023-01-03 20:33:16.357681 ucbreq-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     6626 2023-01-03 20:11:37.399159 ucbreq-2.0.4/src/ucbreq/__init__.py
--rw-r--r--   0        0        0        0 2023-01-03 20:30:57.135519 ucbreq-2.0.4/src/ucbreq/py.typed
--rw-r--r--   0        0        0     3020 1970-01-01 00:00:00.000000 ucbreq-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1203 2023-01-03 20:25:46.635158 ucbreq-2.0.5/.gitignore
+-rw-r--r--   0        0        0     1077 2020-11-17 17:50:42.897269 ucbreq-2.0.5/LICENSE
+-rw-r--r--   0        0        0     2200 2020-11-17 18:33:59.501340 ucbreq-2.0.5/README.rst
+-rw-r--r--   0        0        0      634 2023-01-03 20:22:44.540946 ucbreq-2.0.5/docs/Makefile
+-rw-r--r--   0        0        0     1999 2023-01-03 20:23:48.213020 ucbreq-2.0.5/docs/conf.py
+-rw-r--r--   0        0        0      443 2023-01-03 20:25:21.480129 ucbreq-2.0.5/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-01-03 20:17:19.216566 ucbreq-2.0.5/docs/make.bat
+-rw-r--r--   0        0        0      106 2023-01-03 20:21:18.144846 ucbreq-2.0.5/docs/ucbreq.rst
+-rw-r--r--   0        0        0      901 2024-05-07 15:00:04.431699 ucbreq-2.0.5/pyproject.toml
+-rwxr-xr-x   0        0        0      371 2023-01-11 22:54:01.700981 ucbreq-2.0.5/run_all_tests.sh
+-rw-r--r--   0        0        0     6569 2024-04-30 20:51:05.733753 ucbreq-2.0.5/src/ucbreq/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:30:57.135519 ucbreq-2.0.5/src/ucbreq/py.typed
+-rw-r--r--   0        0        0        0 2020-11-17 17:50:42.897269 ucbreq-2.0.5/test/__init__.py
+-rw-r--r--   0        0        0      960 2023-01-03 17:20:11.375187 ucbreq-2.0.5/test/test_dump.py
+-rw-r--r--   0        0        0     1899 2023-01-03 18:23:40.467748 ucbreq-2.0.5/test/test_load.py
+-rw-r--r--   0        0        0     3021 1970-01-01 00:00:00.000000 ucbreq-2.0.5/PKG-INFO
```

### Comparing `ucbreq-2.0.4/README.rst` & `ucbreq-2.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `ucbreq-2.0.4/pyproject.toml` & `ucbreq-2.0.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = 'ucbreq'
 description = 'Simple format for serialization, similar to CSV.  Not useful for most general use.'
-version = '2.0.4'
+version = '2.0.5'
 readme = 'README.rst'
 requires-python = '>= 3.5, < 4'
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
@@ -13,16 +13,16 @@
     'Programming Language :: Python :: 3.5',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Software Development :: Libraries',
 ]
 
 [[project.authors]]
 name = "Taylor C. Richberger"
-email = "tcr@absolute-performance.com"
+email = "taylor.richberger@procern.com"
 
 [project.urls]
-repository  = 'https://github.com/absperf/ucbreq'
+repository  = 'https://github.com/ProCern/ucbreq'
 documentation = 'https://ucbreq.readthedocs.io/'
 
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.2,<4", 'wheel']
```

### Comparing `ucbreq-2.0.4/src/ucbreq/__init__.py` & `ucbreq-2.0.5/src/ucbreq/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 values.
 
 Effectively, the format is a list of ``key|value`` lines, where keys may be
 made into a list by either repeating them or suffixing them with an _1 index,
 incrementing.
 '''
 from collections.abc import Sequence
-from io import BytesIO, StringIO
-import codecs
-from typing import Dict, Union, Generic, TypeVar, Mapping, Sequence, TextIO, Optional, Tuple, Callable, MutableMapping, MutableSequence, cast, NamedTuple, List
+from io import StringIO
+from typing import Union, Mapping, Sequence, TextIO, Optional, Tuple, Callable, MutableMapping, MutableSequence, List
 
 ValueList = Sequence[str]
 Value = Union[str, ValueList]
 Object = Mapping[str, Value]
 
 # Mutable list that can be appended to.
 MutableList = MutableSequence[str]
@@ -29,15 +28,15 @@
 
     These conditions are technically illegal, but we don't enforce them.
     '''
 
     def __init__(
         self,
         plain: Optional[MutableSequence] = None,
-        indexed: Optional[List[Tuple[int, str]]] = None):
+        indexed: Optional[List[Tuple[int, str]]] = None) -> None:
         if plain is None:
             plain = []
         if indexed is None:
             indexed = []
 
         self.plain = plain
         self.indexed = indexed
@@ -86,24 +85,24 @@
     if startindex < 0:
         raise ValueError('startindex must be non-negative, but was {}'.format(startindex))
 
     keys = set()
 
     for key, value in obj.items():
         if isinstance(value, str):
-            if not key in keys:
+            if key not in keys:
                 fp.write(key)
                 fp.write(separator)
                 fp.write(value)
                 fp.write('\n')
                 keys.add(key)
         else:
             for index, item in enumerate(value, start=startindex):
                 k = index_separator.join((key, str(index)))
-                if not k in keys:
+                if k not in keys:
                     fp.write(k)
                     fp.write(separator)
                     fp.write(item)
                     fp.write('\n')
                     keys.add(k)
 
 def dumps(obj: Object, startindex: int = 1, separator: str = '|', index_separator: str = '_') -> str:
```

### Comparing `ucbreq-2.0.4/PKG-INFO` & `ucbreq-2.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ucbreq
-Version: 2.0.4
+Version: 2.0.5
 Summary: Simple format for serialization, similar to CSV.  Not useful for most general use.
-Author-email: "Taylor C. Richberger" <tcr@absolute-performance.com>
+Author-email: "Taylor C. Richberger" <taylor.richberger@procern.com>
 Requires-Python: >= 3.5, < 4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Project-URL: documentation, https://ucbreq.readthedocs.io/
-Project-URL: repository, https://github.com/absperf/ucbreq
+Project-URL: repository, https://github.com/ProCern/ucbreq
 
 python-req
 ==========
 
 Simple python module for loading and dumping structures in req format, a very
 simple {string: (string|list(string))} format.
```

