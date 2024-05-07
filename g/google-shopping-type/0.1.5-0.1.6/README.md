# Comparing `tmp/google-shopping-type-0.1.5.tar.gz` & `tmp/google-shopping-type-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-shopping-type-0.1.5.tar", last modified: Wed Mar 27 20:24:43 2024, max compression
+gzip compressed data, was "google-shopping-type-0.1.6.tar", last modified: Tue May  7 20:44:08 2024, max compression
```

## Comparing `google-shopping-type-0.1.5.tar` & `google-shopping-type-0.1.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 20:24:43.230777 google-shopping-type-0.1.5/
--rw-rw-r--   0 root         (0)     1003    11358 2024-03-27 20:21:42.000000 google-shopping-type-0.1.5/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-03-27 20:21:42.000000 google-shopping-type-0.1.5/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5072 2024-03-27 20:24:43.230777 google-shopping-type-0.1.5/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3708 2024-03-27 20:21:42.000000 google-shopping-type-0.1.5/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 20:24:43.222776 google-shopping-type-0.1.5/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 20:24:43.222776 google-shopping-type-0.1.5/google/shopping/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 20:24:43.226777 google-shopping-type-0.1.5/google/shopping/type/
--rw-rw-r--   0 root         (0)     1003      908 2024-03-27 20:21:42.000000 google-shopping-type-0.1.5/google/shopping/type/__init__.py
--rw-rw-r--   0 root         (0)     1003      229 2024-03-27 20:21:42.000000 google-shopping-type-0.1.5/google/shopping/type/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-03-27 20:21:42.000000 google-shopping-type-0.1.5/google/shopping/type/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       81 2024-03-27 20:21:42.000000 google-shopping-type-0.1.5/google/shopping/type/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 20:24:43.226777 google-shopping-type-0.1.5/google/shopping/type/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-27 20:21:42.000000 google-shopping-type-0.1.5/google/shopping/type/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 20:24:43.226777 google-shopping-type-0.1.5/google/shopping/type/types/
--rw-rw-r--   0 root         (0)     1003      791 2024-03-27 20:21:42.000000 google-shopping-type-0.1.5/google/shopping/type/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     8543 2024-03-27 20:21:42.000000 google-shopping-type-0.1.5/google/shopping/type/types/types.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 20:24:43.226777 google-shopping-type-0.1.5/google_shopping_type.egg-info/
--rw-r--r--   0 root         (0)     1003     5072 2024-03-27 20:24:43.000000 google-shopping-type-0.1.5/google_shopping_type.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003      699 2024-03-27 20:24:43.000000 google-shopping-type-0.1.5/google_shopping_type.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-27 20:24:43.000000 google-shopping-type-0.1.5/google_shopping_type.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-27 20:24:43.000000 google-shopping-type-0.1.5/google_shopping_type.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      305 2024-03-27 20:24:43.000000 google-shopping-type-0.1.5/google_shopping_type.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-03-27 20:24:43.000000 google-shopping-type-0.1.5/google_shopping_type.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-03-27 20:24:43.230777 google-shopping-type-0.1.5/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3163 2024-03-27 20:21:42.000000 google-shopping-type-0.1.5/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 20:24:43.226777 google-shopping-type-0.1.5/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-27 20:21:42.000000 google-shopping-type-0.1.5/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 20:24:43.226777 google-shopping-type-0.1.5/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-27 20:21:42.000000 google-shopping-type-0.1.5/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 20:24:43.226777 google-shopping-type-0.1.5/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-27 20:21:42.000000 google-shopping-type-0.1.5/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 20:24:43.226777 google-shopping-type-0.1.5/tests/unit/gapic/type/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-27 20:21:42.000000 google-shopping-type-0.1.5/tests/unit/gapic/type/__init__.py
--rw-rw-r--   0 root         (0)     1003      779 2024-03-27 20:21:42.000000 google-shopping-type-0.1.5/tests/unit/gapic/type/test_type.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:44:08.164540 google-shopping-type-0.1.6/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-05-07 20:40:13.000000 google-shopping-type-0.1.6/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-05-07 20:40:13.000000 google-shopping-type-0.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5072 2024-05-07 20:44:08.164540 google-shopping-type-0.1.6/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3708 2024-05-07 20:40:13.000000 google-shopping-type-0.1.6/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:44:08.160540 google-shopping-type-0.1.6/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:44:08.160540 google-shopping-type-0.1.6/google/shopping/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:44:08.160540 google-shopping-type-0.1.6/google/shopping/type/
+-rw-rw-r--   0 root         (0)     1003      959 2024-05-07 20:40:13.000000 google-shopping-type-0.1.6/google/shopping/type/__init__.py
+-rw-rw-r--   0 root         (0)     1003      229 2024-05-07 20:40:13.000000 google-shopping-type-0.1.6/google/shopping/type/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-07 20:40:13.000000 google-shopping-type-0.1.6/google/shopping/type/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       81 2024-05-07 20:40:13.000000 google-shopping-type-0.1.6/google/shopping/type/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:44:08.160540 google-shopping-type-0.1.6/google/shopping/type/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:13.000000 google-shopping-type-0.1.6/google/shopping/type/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:44:08.164540 google-shopping-type-0.1.6/google/shopping/type/types/
+-rw-rw-r--   0 root         (0)     1003      842 2024-05-07 20:40:13.000000 google-shopping-type-0.1.6/google/shopping/type/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9800 2024-05-07 20:40:13.000000 google-shopping-type-0.1.6/google/shopping/type/types/types.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:44:08.164540 google-shopping-type-0.1.6/google_shopping_type.egg-info/
+-rw-r--r--   0 root         (0)     1003     5072 2024-05-07 20:44:08.000000 google-shopping-type-0.1.6/google_shopping_type.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003      699 2024-05-07 20:44:08.000000 google-shopping-type-0.1.6/google_shopping_type.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-07 20:44:08.000000 google-shopping-type-0.1.6/google_shopping_type.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-07 20:44:08.000000 google-shopping-type-0.1.6/google_shopping_type.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      305 2024-05-07 20:44:08.000000 google-shopping-type-0.1.6/google_shopping_type.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-05-07 20:44:08.000000 google-shopping-type-0.1.6/google_shopping_type.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-05-07 20:44:08.168541 google-shopping-type-0.1.6/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3163 2024-05-07 20:40:13.000000 google-shopping-type-0.1.6/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:44:08.164540 google-shopping-type-0.1.6/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:13.000000 google-shopping-type-0.1.6/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:44:08.164540 google-shopping-type-0.1.6/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:13.000000 google-shopping-type-0.1.6/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:44:08.164540 google-shopping-type-0.1.6/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:13.000000 google-shopping-type-0.1.6/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:44:08.164540 google-shopping-type-0.1.6/tests/unit/gapic/type/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:13.000000 google-shopping-type-0.1.6/tests/unit/gapic/type/__init__.py
+-rw-rw-r--   0 root         (0)     1003      779 2024-05-07 20:40:13.000000 google-shopping-type-0.1.6/tests/unit/gapic/type/test_type.py
```

### Comparing `google-shopping-type-0.1.5/LICENSE` & `google-shopping-type-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `google-shopping-type-0.1.5/MANIFEST.in` & `google-shopping-type-0.1.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-shopping-type-0.1.5/PKG-INFO` & `google-shopping-type-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-shopping-type
-Version: 0.1.5
+Version: 0.1.6
 Summary: Google Shopping Type API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-type
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-shopping-type-0.1.5/README.rst` & `google-shopping-type-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `google-shopping-type-0.1.5/google/shopping/type/__init__.py` & `google-shopping-type-0.1.6/google/shopping/type/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,16 +14,24 @@
 # limitations under the License.
 #
 from google.shopping.type import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
-from .types.types import Channel, CustomAttribute, Destination, Price, ReportingContext
+from .types.types import (
+    Channel,
+    CustomAttribute,
+    Destination,
+    Price,
+    ReportingContext,
+    Weight,
+)
 
 __all__ = (
     "Channel",
     "CustomAttribute",
     "Destination",
     "Price",
     "ReportingContext",
+    "Weight",
 )
```

### Comparing `google-shopping-type-0.1.5/google/shopping/type/gapic_version.py` & `google-shopping-type-0.1.6/google/shopping/type/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.5"  # {x-release-please-version}
+__version__ = "0.1.6"  # {x-release-please-version}
```

### Comparing `google-shopping-type-0.1.5/google/shopping/type/services/__init__.py` & `google-shopping-type-0.1.6/google/shopping/type/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-type-0.1.5/google/shopping/type/types/__init__.py` & `google-shopping-type-0.1.6/tests/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,16 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from .types import Channel, CustomAttribute, Destination, Price, ReportingContext
-
-__all__ = (
-    "Channel",
-    "CustomAttribute",
-    "Destination",
-    "Price",
-    "ReportingContext",
-)
```

### Comparing `google-shopping-type-0.1.5/google/shopping/type/types/types.py` & `google-shopping-type-0.1.6/google/shopping/type/types/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,37 +18,83 @@
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.shopping.type",
     manifest={
+        "Weight",
         "Price",
         "CustomAttribute",
         "Destination",
         "ReportingContext",
         "Channel",
     },
 )
 
 
+class Weight(proto.Message):
+    r"""The weight represented as the value in string and the unit.
+
+    .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
+
+    Attributes:
+        amount_micros (int):
+            Required. The weight represented as a number
+            in micros (1 million micros is an equivalent to
+            one's currency standard unit, for example, 1 kg
+            = 1000000 micros).
+            This field can also be set as infinity by
+            setting to -1. This field only support -1 and
+            positive value.
+
+            This field is a member of `oneof`_ ``_amount_micros``.
+        unit (google.shopping.type.types.Weight.WeightUnit):
+            Required. The weight unit.
+            Acceptable values are: kg and lb
+    """
+
+    class WeightUnit(proto.Enum):
+        r"""The weight unit.
+
+        Values:
+            WEIGHT_UNIT_UNSPECIFIED (0):
+                unit unspecified
+            POUND (1):
+                lb unit.
+            KILOGRAM (2):
+                kg unit.
+        """
+        WEIGHT_UNIT_UNSPECIFIED = 0
+        POUND = 1
+        KILOGRAM = 2
+
+    amount_micros: int = proto.Field(
+        proto.INT64,
+        number=1,
+        optional=True,
+    )
+    unit: WeightUnit = proto.Field(
+        proto.ENUM,
+        number=2,
+        enum=WeightUnit,
+    )
+
+
 class Price(proto.Message):
     r"""The price represented as a number and currency.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         amount_micros (int):
             The price represented as a number in micros
             (1 million micros is an equivalent to one's
             currency standard unit, for example, 1 USD =
             1000000 micros).
-            This field can also be set as infinity by
-            setting to -1. This field only support -1 and
-            positive value.
 
             This field is a member of `oneof`_ ``_amount_micros``.
         currency_code (str):
             The currency of the price using three-letter acronyms
             according to `ISO
             4217 <http://en.wikipedia.org/wiki/ISO_4217>`__.
```

### Comparing `google-shopping-type-0.1.5/google_shopping_type.egg-info/PKG-INFO` & `google-shopping-type-0.1.6/google_shopping_type.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-shopping-type
-Version: 0.1.5
+Version: 0.1.6
 Summary: Google Shopping Type API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-type
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-shopping-type-0.1.5/google_shopping_type.egg-info/SOURCES.txt` & `google-shopping-type-0.1.6/google_shopping_type.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-shopping-type-0.1.5/setup.py` & `google-shopping-type-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `google-shopping-type-0.1.5/tests/__init__.py` & `google-shopping-type-0.1.6/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-type-0.1.5/tests/unit/__init__.py` & `google-shopping-type-0.1.6/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-type-0.1.5/tests/unit/gapic/__init__.py` & `google-shopping-type-0.1.6/tests/unit/gapic/type/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-type-0.1.5/tests/unit/gapic/type/__init__.py` & `google-shopping-type-0.1.6/tests/unit/gapic/type/test_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 # -*- coding: utf-8 -*-
-# Copyright 2024 Google LLC
+# Copyright 2021 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+
+from google.shopping import type
+
+# NOTE: These are dummy tests to reach 100% coverage
+# They simply check that the message can be created.
+
+
+def test_type():
+    type.Channel()
```

### Comparing `google-shopping-type-0.1.5/tests/unit/gapic/type/test_type.py` & `google-shopping-type-0.1.6/google/shopping/type/types/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 # -*- coding: utf-8 -*-
-# Copyright 2021 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from .types import (
+    Channel,
+    CustomAttribute,
+    Destination,
+    Price,
+    ReportingContext,
+    Weight,
+)
 
-from google.shopping import type
-
-# NOTE: These are dummy tests to reach 100% coverage
-# They simply check that the message can be created.
-
-
-def test_type():
-    type.Channel()
+__all__ = (
+    "Channel",
+    "CustomAttribute",
+    "Destination",
+    "Price",
+    "ReportingContext",
+    "Weight",
+)
```

