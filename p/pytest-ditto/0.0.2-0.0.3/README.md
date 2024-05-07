# Comparing `tmp/pytest_ditto-0.0.2.tar.gz` & `tmp/pytest_ditto-0.0.3.tar.gz`

## Comparing `pytest_ditto-0.0.2.tar` & `pytest_ditto-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/ditto/__init__.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/ditto/_unittest.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/ditto/_version.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/ditto/plugin.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/ditto/snapshot.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/ditto/io/__init__.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/ditto/io/_json.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/ditto/io/_pandas_parquet.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/ditto/io/_pickle.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/ditto/io/_protocol.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/ditto/io/_yaml.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/.gitignore
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/README.md
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pytest_ditto-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/ditto/__init__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/ditto/_unittest.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/ditto/_version.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/ditto/exceptions.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/ditto/plugin.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/ditto/snapshot.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/ditto/io/__init__.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/ditto/io/_json.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/ditto/io/_pandas_parquet.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/ditto/io/_pickle.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/ditto/io/_protocol.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/ditto/io/_yaml.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/LICENSE
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/README.md
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pytest_ditto-0.0.3/PKG-INFO
```

### Comparing `pytest_ditto-0.0.2/ditto/_unittest.py` & `pytest_ditto-0.0.3/ditto/_unittest.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,10 +20,9 @@
     @property
     def snapshot(self) -> Snapshot:
         path = _calling_test_path() / ".ditto"
         path.mkdir(exist_ok=True)
 
         return Snapshot(
             path=path,
-            name=".".join(self.id().split(".")[-3:]),
-            record=self.record,
+            group_name=".".join(self.id().split(".")[-3:]),
         )
```

### Comparing `pytest_ditto-0.0.2/ditto/io/__init__.py` & `pytest_ditto-0.0.3/ditto/io/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,40 @@
+from enum import Enum
+
 from ditto.io._protocol import Base
 from ditto.io._yaml import Yaml
 from ditto.io._json import Json
 from ditto.io._pickle import Pickle
 from ditto.io._pandas_parquet import PandasParquet
 
 
 __all__ = [
-    "Base" "Yaml",
+    "Base",
+    "Yaml",
     "Json",
     "Pickle",
     "PandasParquet",
     "register",
     "get",
     "default",
 ]
 
 
+class IO(str, Enum):
+    PICKLE = "pickle"
+    JSON = "json"
+    YAML = "yaml"
+    PANDAS_PARQUET = "pandas_parquet"
+
+
 _NAME_IO_MAP: dict[str, type[Base]] = {
-    "pkl": Pickle,
-    "json": Json,
-    "yaml": Yaml,
-    "pandas_parquet": PandasParquet,
+    IO.PICKLE: Pickle,
+    IO.JSON: Json,
+    IO.YAML: Yaml,
+    IO.PANDAS_PARQUET: PandasParquet,
 }
 
 
 def register(name: str, io: type[Base]) -> None:
     _NAME_IO_MAP[name] = io
```

### Comparing `pytest_ditto-0.0.2/pyproject.toml` & `pytest_ditto-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "pytest-ditto"
 dynamic = [
     "version",
 ]
-description = ""
-keywords = ["pytest"]
+description = "Snapshot testing pytest plugin with minimal ceremony and flexible persistence formats."
+keywords = ["pytest" , "testing"]
 authors = [{ name = "Lachlan Taylor", email = "lachlanbtaylor@proton.me" }]
 maintainers = [{ name = "Lachlan Taylor", email = "lachlanbtaylor@proton.me" }]
 requires-python = ">=3.10"
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -64,15 +64,15 @@
 [tool.hatch.envs.default]
 python = "3.10"
 dependencies = [
   "pytest",
 ]
 
 [tool.hatch.envs.default.scripts]
-test = "pytest {args:tests}"
+test = "pytest {args:tests/ci}"
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.10", "3.11", "3.12"]
 
 
 [tool.pytest.ini_options]
 testpaths = "tests"
```

