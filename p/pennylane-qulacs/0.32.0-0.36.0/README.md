# Comparing `tmp/pennylane_qulacs-0.32.0-py3-none-any.whl.zip` & `tmp/pennylane_qulacs-0.36.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 13912 bytes, number of entries: 9
--rw-r--r--  2.0 unx      668 b- defN 23-Aug-28 19:05 pennylane_qulacs/__init__.py
--rw-r--r--  2.0 unx      692 b- defN 23-Aug-28 19:05 pennylane_qulacs/_version.py
--rw-r--r--  2.0 unx    13434 b- defN 23-Aug-28 19:05 pennylane_qulacs/qulacs_device.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Aug-28 19:05 pennylane_qulacs-0.32.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     8423 b- defN 23-Aug-28 19:05 pennylane_qulacs-0.32.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-28 19:05 pennylane_qulacs-0.32.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       84 b- defN 23-Aug-28 19:05 pennylane_qulacs-0.32.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 23-Aug-28 19:05 pennylane_qulacs-0.32.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      801 b- defN 23-Aug-28 19:05 pennylane_qulacs-0.32.0.dist-info/RECORD
-9 files, 35568 bytes uncompressed, 12510 bytes compressed:  64.8%
+Zip file size: 13956 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      668 b- defN 24-May-06 23:16 pennylane_qulacs/__init__.py
+-rw-r--r--  2.0 unx      692 b- defN 24-May-06 23:16 pennylane_qulacs/_version.py
+-rw-r--r--  2.0 unx    13594 b- defN 24-May-06 23:16 pennylane_qulacs/qulacs_device.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-06 23:16 pennylane_qulacs-0.36.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8442 b- defN 24-May-06 23:16 pennylane_qulacs-0.36.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-06 23:16 pennylane_qulacs-0.36.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       84 b- defN 24-May-06 23:16 pennylane_qulacs-0.36.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 24-May-06 23:16 pennylane_qulacs-0.36.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      801 b- defN 24-May-06 23:16 pennylane_qulacs-0.36.0.dist-info/RECORD
+9 files, 35747 bytes uncompressed, 12554 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: pennylane_qulacs/_version.py
 Comment: 
 
 Filename: pennylane_qulacs/qulacs_device.py
 Comment: 
 
-Filename: pennylane_qulacs-0.32.0.dist-info/LICENSE
+Filename: pennylane_qulacs-0.36.0.dist-info/LICENSE
 Comment: 
 
-Filename: pennylane_qulacs-0.32.0.dist-info/METADATA
+Filename: pennylane_qulacs-0.36.0.dist-info/METADATA
 Comment: 
 
-Filename: pennylane_qulacs-0.32.0.dist-info/WHEEL
+Filename: pennylane_qulacs-0.36.0.dist-info/WHEEL
 Comment: 
 
-Filename: pennylane_qulacs-0.32.0.dist-info/entry_points.txt
+Filename: pennylane_qulacs-0.36.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: pennylane_qulacs-0.32.0.dist-info/top_level.txt
+Filename: pennylane_qulacs-0.36.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pennylane_qulacs-0.32.0.dist-info/RECORD
+Filename: pennylane_qulacs-0.36.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pennylane_qulacs/_version.py

```diff
@@ -12,8 +12,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Version information.
    Version number (major.minor.patch[-label])
 """
 
-__version__ = "0.32.0"
+__version__ = "0.36.0"
```

## pennylane_qulacs/qulacs_device.py

```diff
@@ -118,14 +118,15 @@
     _observable_map = {
         "PauliX": "X",
         "PauliY": "Y",
         "PauliZ": "Z",
         "Identity": "I",
         "Hadamard": None,
         "Hermitian": None,
+        "Prod": None,
     }
 
     operations = _operation_map.keys()
     observables = _observable_map.keys()
 
     # Add inverse gates to _operation_map
     _operation_map.update({k + ".inv": v for k, v in _operation_map.items()})
@@ -344,14 +345,16 @@
         return prob
 
     def expval(self, observable, **kwargs):
         if self.shots is None:
             qulacs_observable = Observable(self.num_wires)
             if isinstance(observable.name, list):
                 observables = [self._observable_map[obs] for obs in observable.name]
+            elif observable.name == "Prod":
+                observables = [self._observable_map[obs.name] for obs in observable.operands]
             else:
                 observables = [self._observable_map[observable.name]]
 
             if None not in observables:
                 applied_wires = self.map_wires(observable.wires).tolist()
                 opp = " ".join([f"{obs} {applied_wires[i]}" for i, obs in enumerate(observables)])
```

## Comparing `pennylane_qulacs-0.32.0.dist-info/LICENSE` & `pennylane_qulacs-0.36.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pennylane_qulacs-0.32.0.dist-info/METADATA` & `pennylane_qulacs-0.36.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pennylane-qulacs
-Version: 0.32.0
+Version: 0.36.0
 Summary: PennyLane plugin for Qulacs.
 Home-page: http://xanadu.ai
 Maintainer: Xanadu Inc.
 Maintainer-email: software@xanadu.ai
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -34,15 +34,15 @@
 Provides-Extra: gpu
 Requires-Dist: qulacs-gpu >=0.1.10.1 ; extra == 'gpu'
 
 PennyLane-Qulacs Plugin
 #######################
 
 
-.. image:: https://img.shields.io/github/workflow/status/PennyLaneAI/pennylane-qulacs/Tests/master?logo=github&style=flat-square
+.. image:: https://img.shields.io/github/actions/workflow/status/PennyLaneAI/pennylane-qulacs/tests.yml?branch=master&logo=github&style=flat-square
     :alt: GitHub Workflow Status (branch)
     :target: https://github.com/PennyLaneAI/pennylane-qulacs/actions?query=workflow%3ATests
 
 .. image:: https://img.shields.io/codecov/c/github/PennyLaneAI/pennylane-qulacs/master.svg?logo=codecov&style=flat-square
     :alt: Codecov coverage
     :target: https://codecov.io/gh/PennyLaneAI/pennylane-qulacs
```

## Comparing `pennylane_qulacs-0.32.0.dist-info/RECORD` & `pennylane_qulacs-0.36.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 pennylane_qulacs/__init__.py,sha256=k6FHqdErObJWrCN7bLPrq6vlz_gfzNEc8VsCR64tzyg,668
-pennylane_qulacs/_version.py,sha256=_-mOZ65SLoL5OTGULQfUCOxJIBdPAfIz4GfDpogEIVQ,692
-pennylane_qulacs/qulacs_device.py,sha256=OOshU1Tah4NLLd8qLVO16i4kLoKUcfz3W_xtNG08d_w,13434
-pennylane_qulacs-0.32.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-pennylane_qulacs-0.32.0.dist-info/METADATA,sha256=Xo3IexQjx3J_md01xqK-ZS6xfWtIvy_qdqHyXddtqhk,8423
-pennylane_qulacs-0.32.0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-pennylane_qulacs-0.32.0.dist-info/entry_points.txt,sha256=EwihxFbiPOC0_lUgm4eZvFgo2arPJo0Xo0k1KlfuED4,84
-pennylane_qulacs-0.32.0.dist-info/top_level.txt,sha256=Q5_9psFP563yaHmGoR1awUjhsxBwe39b68vVr2ba-Rw,17
-pennylane_qulacs-0.32.0.dist-info/RECORD,,
+pennylane_qulacs/_version.py,sha256=bffOyMAzTLgpfpQZnltKEg0YwlYfnA7klmmYOn_VRDA,692
+pennylane_qulacs/qulacs_device.py,sha256=uRboOmJcTGYJAIl3Oy9IVAqo1MYNkSAegjEkqLdXg00,13594
+pennylane_qulacs-0.36.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pennylane_qulacs-0.36.0.dist-info/METADATA,sha256=2J28zHkfRsk3n8ajT1KJjWoYV07WVsuaqFndfb3TI1s,8442
+pennylane_qulacs-0.36.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pennylane_qulacs-0.36.0.dist-info/entry_points.txt,sha256=EwihxFbiPOC0_lUgm4eZvFgo2arPJo0Xo0k1KlfuED4,84
+pennylane_qulacs-0.36.0.dist-info/top_level.txt,sha256=Q5_9psFP563yaHmGoR1awUjhsxBwe39b68vVr2ba-Rw,17
+pennylane_qulacs-0.36.0.dist-info/RECORD,,
```

