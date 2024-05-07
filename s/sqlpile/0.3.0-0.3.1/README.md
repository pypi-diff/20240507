# Comparing `tmp/sqlpile-0.3.0.tar.gz` & `tmp/sqlpile-0.3.1.tar.gz`

## Comparing `sqlpile-0.3.0.tar` & `sqlpile-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 sqlpile-0.3.0/.python-version
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 sqlpile-0.3.0/requirements-dev.lock
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 sqlpile-0.3.0/requirements.lock
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sqlpile-0.3.0/.vscode/settings.json
--rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 sqlpile-0.3.0/docs/CODE_STYLE.md
--rw-r--r--   0        0        0  2731400 2020-02-02 00:00:00.000000 sqlpile-0.3.0/docs/imgs/good-oop.png
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 sqlpile-0.3.0/src/sqlpile/__init__.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 sqlpile-0.3.0/src/sqlpile/abcs.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 sqlpile-0.3.0/src/sqlpile/config.py
--rw-r--r--   0        0        0    18034 2020-02-02 00:00:00.000000 sqlpile-0.3.0/src/sqlpile/core.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 sqlpile-0.3.0/src/sqlpile/database.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 sqlpile-0.3.0/src/sqlpile/main.py
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 sqlpile-0.3.0/src/sqlpile/utils.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 sqlpile-0.3.0/.gitignore
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 sqlpile-0.3.0/README.md
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 sqlpile-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 sqlpile-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 sqlpile-0.3.1/.python-version
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 sqlpile-0.3.1/requirements-dev.lock
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 sqlpile-0.3.1/requirements.lock
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sqlpile-0.3.1/.vscode/settings.json
+-rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 sqlpile-0.3.1/docs/CODE_STYLE.md
+-rw-r--r--   0        0        0  2731400 2020-02-02 00:00:00.000000 sqlpile-0.3.1/docs/imgs/good-oop.png
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 sqlpile-0.3.1/src/sqlpile/__init__.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 sqlpile-0.3.1/src/sqlpile/abcs.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 sqlpile-0.3.1/src/sqlpile/config.py
+-rw-r--r--   0        0        0    18041 2020-02-02 00:00:00.000000 sqlpile-0.3.1/src/sqlpile/core.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 sqlpile-0.3.1/src/sqlpile/database.py
+-rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 sqlpile-0.3.1/src/sqlpile/main.py
+-rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 sqlpile-0.3.1/src/sqlpile/utils.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 sqlpile-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 sqlpile-0.3.1/README.md
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 sqlpile-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 sqlpile-0.3.1/PKG-INFO
```

### Comparing `sqlpile-0.3.0/requirements-dev.lock` & `sqlpile-0.3.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `sqlpile-0.3.0/requirements.lock` & `sqlpile-0.3.1/requirements.lock`

 * *Files identical despite different names*

### Comparing `sqlpile-0.3.0/docs/CODE_STYLE.md` & `sqlpile-0.3.1/docs/CODE_STYLE.md`

 * *Files identical despite different names*

### Comparing `sqlpile-0.3.0/docs/imgs/good-oop.png` & `sqlpile-0.3.1/docs/imgs/good-oop.png`

 * *Files identical despite different names*

### Comparing `sqlpile-0.3.0/src/sqlpile/abcs.py` & `sqlpile-0.3.1/src/sqlpile/abcs.py`

 * *Files identical despite different names*

### Comparing `sqlpile-0.3.0/src/sqlpile/config.py` & `sqlpile-0.3.1/src/sqlpile/config.py`

 * *Files identical despite different names*

### Comparing `sqlpile-0.3.0/src/sqlpile/core.py` & `sqlpile-0.3.1/src/sqlpile/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -504,15 +504,15 @@
     def __enter__(self):
         self.init_executor()
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.executor.shutdown()
 
-    def get(self, key):
+    def get(self, key) -> Any:
         result = self.localz.get(key)
 
         if result is None:
             result = self.remote.get(key)
             if result is not None:
                 self.localz.set(key, result)
```

### Comparing `sqlpile-0.3.0/src/sqlpile/database.py` & `sqlpile-0.3.1/src/sqlpile/database.py`

 * *Files identical despite different names*

### Comparing `sqlpile-0.3.0/README.md` & `sqlpile-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `sqlpile-0.3.0/pyproject.toml` & `sqlpile-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sqlpile"
-version = "0.3.0"
+version = "0.3.1"
 description = "Add your description here"
 authors = [{ name = "Kevin Hill", email = "kivo360@gmail.com" }]
 dependencies = [
     "sqlalchemy>=2.0.29",
     "psycopg[binary]>=3.1.18",
     "cloudpickle>=3.0.0",
     "lz4>=4.3.3",
```

### Comparing `sqlpile-0.3.0/PKG-INFO` & `sqlpile-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sqlpile
-Version: 0.3.0
+Version: 0.3.1
 Summary: Add your description here
 Author-email: Kevin Hill <kivo360@gmail.com>
 Requires-Python: >=3.8
 Requires-Dist: aiosqlite>=0.20.0
 Requires-Dist: asyncer>=0.0.7
 Requires-Dist: cloudpickle>=3.0.0
 Requires-Dist: cytoolz>=0.12.3
```

