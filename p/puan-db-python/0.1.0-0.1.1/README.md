# Comparing `tmp/puan_db_python-0.1.0.tar.gz` & `tmp/puan_db_python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puan_db_python-0.1.0.tar", max compression
+gzip compressed data, was "puan_db_python-0.1.1.tar", max compression
```

## Comparing `puan_db_python-0.1.0.tar` & `puan_db_python-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1913 2024-04-26 07:14:50.804168 puan_db_python-0.1.0/README.md
--rw-r--r--   0        0        0    11564 2024-04-26 11:18:51.281829 puan_db_python-0.1.0/puan_db_python/__init__.py
--rw-r--r--   0        0        0      313 2024-04-25 11:53:09.455616 puan_db_python-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2439 1970-01-01 00:00:00.000000 puan_db_python-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2131 2024-04-26 14:13:18.316480 puan_db_python-0.1.1/README.md
+-rw-r--r--   0        0        0    12558 2024-05-07 11:50:27.331963 puan_db_python-0.1.1/puan_db_python/__init__.py
+-rw-r--r--   0        0        0      313 2024-05-07 11:50:47.022961 puan_db_python-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 puan_db_python-0.1.1/PKG-INFO
```

### Comparing `puan_db_python-0.1.0/README.md` & `puan_db_python-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,25 @@
+# Puan DB Python Client
+## Install
+```bash
+pip install puan-db-python
+```
+
 # A quick what-is-dis
 A Python library for connecting to a `puan-db` instance. Puan DB is a logical reasoning database which draws conclusions from a model and finds combinations which satisfies a model while minimizing/maximizing some objective function.
 
 There are two types of variables to keep in mind: 
 - <b>Primitives</b>. These are defined by an ID given by you, and a lower and upper bound representing which integer values this variable may take in the future. The bound is a complex number so a boolean variable `x` would be declared with the bound `0+1j`, or just `1j`, as such `model.set_primitive("x", 1j)` 
 - <b>Composites</b>. These are created using one or more other primitives or composites as a connecter between them. For instance, an OR-connector is defined as `model.set_or(["x","y","z"])`.
 
 # Example
 ```python
 import puan_db_python
 
+# Connect to back end
 model = puan_db_python.PuanClient(
     host="localhost",
     port=50051,
     password=None,
     ssl=False
 )
 
@@ -35,9 +42,18 @@
 # Note that you must give the ID and not the alias when getting its value
 model.propagate_downstream({"x": 1+1j}).get(id) == 1+1j 
 
 # Or maybe we want to find a combination that trying
 # to not include x and even more not y, such that (x or y or z) must be true.
 # Note that we can send in multiple "objectives" and there's one solution returned
 # by each objective
-solutions = model.solve([{"x": -1, "y": -2}], {id: 1})
-```
+solutions = model.solve(
+    objectives=[
+        {
+            "x": -1, 
+            "y": -2,
+        }
+    ], 
+    fix={id: 1+1j}, 
+    solver=puan_db_python.Solver.GLPK,
+)
+```
```

### Comparing `puan_db_python-0.1.0/puan_db_python/__init__.py` & `puan_db_python-0.1.1/puan_db_python/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 
 @dataclass
 class PuanClient:
 
     host:       str
     port:       int
-    password:   Optional[str]
-    ssl:        Optional[bool]
+    password:   Optional[str] = None
+    ssl:        Optional[bool] = None
 
     @staticmethod
     def _bound_complex(bound: Optional[puan_db_pb2.Bound]) -> Optional[complex]:
         return complex(bound.lower, bound.upper) if bound else None
 
     @staticmethod
     def _complex_bound(cmplx: complex) -> puan_db_pb2.Bound:
@@ -235,36 +235,63 @@
             return stub.SetNot(
                 puan_db_pb2.Not(
                     references=references,
                     alias=alias
                 )
             ).id
         
+    def set_xor(self, references: List[str], alias: Optional[str] = None) -> str:
+        """
+            Set an xor constraint in the database.
+        """
+        with grpc.insecure_channel(f"{self.host}:{self.port}") as channel:
+            stub = puan_db_pb2_grpc.ModelingServiceStub(channel)
+            return stub.SetXor(
+                puan_db_pb2.Xor(
+                    references=references,
+                    alias=alias
+                )
+            ).id
+        
     def set_imply(self, condition: str, consequence: str, alias: Optional[str] = None) -> str:
         """
             Set an imply constraint in the database.
         """
         with grpc.insecure_channel(f"{self.host}:{self.port}") as channel:
             stub = puan_db_pb2_grpc.ModelingServiceStub(channel)
             return stub.SetImply(
                 puan_db_pb2.Imply(
                     condition=condition,
                     consequence=consequence,
                     alias=alias
                 )
             ).id
         
-    def propagate_downstream(self, query: Dict[str, complex] = {}) -> Dict[str, complex]:
+    def set_equal(self, lhs: str, rhs: str, alias: Optional[str] = None) -> str:
+        """
+            Set an equivalent constraint in the database.
+        """
+        with grpc.insecure_channel(f"{self.host}:{self.port}") as channel:
+            stub = puan_db_pb2_grpc.ModelingServiceStub(channel)
+            return stub.SetEqual(
+                puan_db_pb2.Equivalent(
+                    lhs=lhs,
+                    rhs=rhs,
+                    alias=alias
+                )
+            ).id
+        
+    def propagate(self, query: Dict[str, complex] = {}) -> Dict[str, complex]:
         """
             Propagate constraints downstream and returns the resulted bounds.
         """
         with grpc.insecure_channel(f"{self.host}:{self.port}") as channel:
             stub = puan_db_pb2_grpc.ModelingServiceStub(channel)
             return PuanClient._interpretation_dict(
-                stub.PropagateDownstream(
+                stub.Propagate(
                     PuanClient._dict_interpretation(query)
                 )
             )
         
     def propagate_upstream(self, query: Dict[str, complex] = {}) -> Dict[str, complex]:
         """
             Propagate constraints downstream and returns the resulted bounds.
@@ -285,15 +312,15 @@
             stub = puan_db_pb2_grpc.ModelingServiceStub(channel)
             return PuanClient._interpretation_dict(
                 stub.PropagateBidirectional(
                     PuanClient._dict_interpretation(query)
                 )
             )
         
-    def solve(self, objectives: List[Dict[str, int]], fix: Dict[str, int], solver: Solver) -> List[Dict[str, int]]:
+    def solve(self, objectives: List[Dict[str, int]], assume: Dict[str, int], solver: Solver) -> List[Dict[str, int]]:
         """
             Solves the objectives in the database and returns the optimal values.
 
             objectives:     List of objective dictionaries.
             fix:            Variables to be fixed before the optimization.
             solver:         Solver to be used.
 
@@ -303,13 +330,13 @@
             stub = puan_db_pb2_grpc.ModelingServiceStub(channel)
             return list(
                 map(
                     PuanClient._interpretation_dict,
                     stub.Solve(
                         puan_db_pb2.SolveRequest(
                             objectives=list(map(PuanClient._dict_objective, objectives)),
-                            fix=PuanClient._dict_interpretation(fix),
+                            assume=PuanClient._dict_interpretation(assume),
                             solver=solver
                         )
                     ).solutions
                 )
             )
```

### Comparing `puan_db_python-0.1.0/PKG-INFO` & `puan_db_python-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 Metadata-Version: 2.1
 Name: puan-db-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: grpcio (>=1.62.2,<2.0.0)
 Requires-Dist: grpcio-tools (>=1.62.2,<2.0.0)
 Description-Content-Type: text/markdown
 
+# Puan DB Python Client
+## Install
+```bash
+pip install puan-db-python
+```
+
 # A quick what-is-dis
 A Python library for connecting to a `puan-db` instance. Puan DB is a logical reasoning database which draws conclusions from a model and finds combinations which satisfies a model while minimizing/maximizing some objective function.
 
 There are two types of variables to keep in mind: 
 - <b>Primitives</b>. These are defined by an ID given by you, and a lower and upper bound representing which integer values this variable may take in the future. The bound is a complex number so a boolean variable `x` would be declared with the bound `0+1j`, or just `1j`, as such `model.set_primitive("x", 1j)` 
 - <b>Composites</b>. These are created using one or more other primitives or composites as a connecter between them. For instance, an OR-connector is defined as `model.set_or(["x","y","z"])`.
 
 # Example
 ```python
 import puan_db_python
 
+# Connect to back end
 model = puan_db_python.PuanClient(
     host="localhost",
     port=50051,
     password=None,
     ssl=False
 )
 
@@ -51,9 +58,19 @@
 # Note that you must give the ID and not the alias when getting its value
 model.propagate_downstream({"x": 1+1j}).get(id) == 1+1j 
 
 # Or maybe we want to find a combination that trying
 # to not include x and even more not y, such that (x or y or z) must be true.
 # Note that we can send in multiple "objectives" and there's one solution returned
 # by each objective
-solutions = model.solve([{"x": -1, "y": -2}], {id: 1})
+solutions = model.solve(
+    objectives=[
+        {
+            "x": -1, 
+            "y": -2,
+        }
+    ], 
+    fix={id: 1+1j}, 
+    solver=puan_db_python.Solver.GLPK,
+)
 ```
+
```

