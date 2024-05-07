# Comparing `tmp/sqlfactory-1.0.3.tar.gz` & `tmp/sqlfactory-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlfactory-1.0.3.tar", max compression
+gzip compressed data, was "sqlfactory-1.1.0.tar", max compression
```

## Comparing `sqlfactory-1.0.3.tar` & `sqlfactory-1.1.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1069 2024-04-12 12:59:25.607004 sqlfactory-1.0.3/LICENSE
--rw-r--r--   0        0        0     7889 2024-04-12 12:59:25.607004 sqlfactory-1.0.3/README.md
--rw-r--r--   0        0        0     1293 2024-04-12 12:59:26.162997 sqlfactory-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      303 2024-04-12 12:59:25.607004 sqlfactory-1.0.3/sqlfactory/__init__.py
--rw-r--r--   0        0        0      324 2024-04-12 12:59:25.607004 sqlfactory-1.0.3/sqlfactory/condition/__init__.py
--rw-r--r--   0        0        0     5049 2024-04-12 12:59:25.607004 sqlfactory-1.0.3/sqlfactory/condition/base.py
--rw-r--r--   0        0        0     1787 2024-04-12 12:59:25.607004 sqlfactory-1.0.3/sqlfactory/condition/between.py
--rw-r--r--   0        0        0     4920 2024-04-12 12:59:25.607004 sqlfactory-1.0.3/sqlfactory/condition/in_condition.py
--rw-r--r--   0        0        0     1274 2024-04-12 12:59:25.607004 sqlfactory-1.0.3/sqlfactory/condition/like.py
--rw-r--r--   0        0        0     5510 2024-04-12 12:59:25.607004 sqlfactory-1.0.3/sqlfactory/condition/simple.py
--rw-r--r--   0        0        0       68 2024-04-12 12:59:25.607004 sqlfactory-1.0.3/sqlfactory/delete/__init__.py
--rw-r--r--   0        0        0     1951 2024-04-12 12:59:25.607004 sqlfactory-1.0.3/sqlfactory/delete/delete.py
--rw-r--r--   0        0        0     7691 2024-04-12 12:59:25.607004 sqlfactory-1.0.3/sqlfactory/entities.py
--rw-r--r--   0        0        0     7543 2024-04-12 12:59:25.607004 sqlfactory-1.0.3/sqlfactory/execute.py
--rw-r--r--   0        0        0        0 2024-04-12 12:59:25.635004 sqlfactory-1.0.3/sqlfactory/func/__init__.py
--rw-r--r--   0        0        0     2240 2024-04-12 12:59:25.607004 sqlfactory-1.0.3/sqlfactory/func/agg.py
--rw-r--r--   0        0        0      987 2024-04-12 12:59:25.607004 sqlfactory-1.0.3/sqlfactory/func/base.py
--rw-r--r--   0        0        0      979 2024-04-12 12:59:25.611004 sqlfactory-1.0.3/sqlfactory/func/control.py
--rw-r--r--   0        0        0    15497 2024-04-12 12:59:25.611004 sqlfactory-1.0.3/sqlfactory/func/datetime.py
--rw-r--r--   0        0        0     4359 2024-04-12 12:59:25.611004 sqlfactory-1.0.3/sqlfactory/func/enc.py
--rw-r--r--   0        0        0     4726 2024-04-12 12:59:25.611004 sqlfactory-1.0.3/sqlfactory/func/info.py
--rw-r--r--   0        0        0     4601 2024-04-12 12:59:25.611004 sqlfactory-1.0.3/sqlfactory/func/misc.py
--rw-r--r--   0        0        0     7156 2024-04-12 12:59:25.611004 sqlfactory-1.0.3/sqlfactory/func/numeric.py
--rw-r--r--   0        0        0     7741 2024-04-12 12:59:25.611004 sqlfactory-1.0.3/sqlfactory/func/str.py
--rw-r--r--   0        0        0       95 2024-04-12 12:59:25.611004 sqlfactory-1.0.3/sqlfactory/insert/__init__.py
--rw-r--r--   0        0        0     6349 2024-04-12 12:59:25.611004 sqlfactory-1.0.3/sqlfactory/insert/insert.py
--rw-r--r--   0        0        0      601 2024-04-12 12:59:25.611004 sqlfactory-1.0.3/sqlfactory/insert/values.py
--rw-r--r--   0        0        0      115 2024-04-12 12:59:25.611004 sqlfactory-1.0.3/sqlfactory/logger.py
--rw-r--r--   0        0        0      271 2024-04-12 12:59:25.611004 sqlfactory-1.0.3/sqlfactory/mixins/__init__.py
--rw-r--r--   0        0        0     3822 2024-04-12 12:59:25.611004 sqlfactory-1.0.3/sqlfactory/mixins/limit.py
--rw-r--r--   0        0        0     2498 2024-04-12 12:59:25.611004 sqlfactory-1.0.3/sqlfactory/mixins/order.py
--rw-r--r--   0        0        0      824 2024-04-12 12:59:25.611004 sqlfactory-1.0.3/sqlfactory/mixins/where.py
--rw-r--r--   0        0        0      244 2024-04-12 12:59:25.611004 sqlfactory-1.0.3/sqlfactory/select/__init__.py
--rw-r--r--   0        0        0     1200 2024-04-12 12:59:25.611004 sqlfactory-1.0.3/sqlfactory/select/aliased.py
--rw-r--r--   0        0        0     2119 2024-04-12 12:59:25.611004 sqlfactory-1.0.3/sqlfactory/select/column_list.py
--rw-r--r--   0        0        0     1846 2024-04-12 12:59:25.611004 sqlfactory-1.0.3/sqlfactory/select/join.py
--rw-r--r--   0        0        0     7224 2024-04-12 12:59:25.611004 sqlfactory-1.0.3/sqlfactory/select/select.py
--rw-r--r--   0        0        0     3861 2024-04-12 12:59:25.611004 sqlfactory-1.0.3/sqlfactory/statement.py
--rw-r--r--   0        0        0       68 2024-04-12 12:59:25.611004 sqlfactory-1.0.3/sqlfactory/update/__init__.py
--rw-r--r--   0        0        0     4867 2024-04-12 12:59:25.611004 sqlfactory-1.0.3/sqlfactory/update/update.py
--rw-r--r--   0        0        0     9002 1970-01-01 00:00:00.000000 sqlfactory-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-18 13:46:10.653117 sqlfactory-1.1.0/LICENSE
+-rw-r--r--   0        0        0     7889 2024-04-18 13:46:10.653117 sqlfactory-1.1.0/README.md
+-rw-r--r--   0        0        0     1293 2024-04-18 13:46:11.641105 sqlfactory-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      303 2024-04-18 13:46:10.653117 sqlfactory-1.1.0/sqlfactory/__init__.py
+-rw-r--r--   0        0        0      324 2024-04-18 13:46:10.653117 sqlfactory-1.1.0/sqlfactory/condition/__init__.py
+-rw-r--r--   0        0        0     5049 2024-04-18 13:46:10.653117 sqlfactory-1.1.0/sqlfactory/condition/base.py
+-rw-r--r--   0        0        0     1787 2024-04-18 13:46:10.653117 sqlfactory-1.1.0/sqlfactory/condition/between.py
+-rw-r--r--   0        0        0     4920 2024-04-18 13:46:10.653117 sqlfactory-1.1.0/sqlfactory/condition/in_condition.py
+-rw-r--r--   0        0        0     1274 2024-04-18 13:46:10.653117 sqlfactory-1.1.0/sqlfactory/condition/like.py
+-rw-r--r--   0        0        0     5510 2024-04-18 13:46:10.653117 sqlfactory-1.1.0/sqlfactory/condition/simple.py
+-rw-r--r--   0        0        0       68 2024-04-18 13:46:10.653117 sqlfactory-1.1.0/sqlfactory/delete/__init__.py
+-rw-r--r--   0        0        0     1951 2024-04-18 13:46:10.653117 sqlfactory-1.1.0/sqlfactory/delete/delete.py
+-rw-r--r--   0        0        0     7691 2024-04-18 13:46:10.653117 sqlfactory-1.1.0/sqlfactory/entities.py
+-rw-r--r--   0        0        0     7543 2024-04-18 13:46:10.653117 sqlfactory-1.1.0/sqlfactory/execute.py
+-rw-r--r--   0        0        0        0 2024-04-18 13:46:10.685117 sqlfactory-1.1.0/sqlfactory/func/__init__.py
+-rw-r--r--   0        0        0     2240 2024-04-18 13:46:10.653117 sqlfactory-1.1.0/sqlfactory/func/agg.py
+-rw-r--r--   0        0        0      987 2024-04-18 13:46:10.653117 sqlfactory-1.1.0/sqlfactory/func/base.py
+-rw-r--r--   0        0        0      979 2024-04-18 13:46:10.653117 sqlfactory-1.1.0/sqlfactory/func/control.py
+-rw-r--r--   0        0        0    15497 2024-04-18 13:46:10.653117 sqlfactory-1.1.0/sqlfactory/func/datetime.py
+-rw-r--r--   0        0        0     4359 2024-04-18 13:46:10.657117 sqlfactory-1.1.0/sqlfactory/func/enc.py
+-rw-r--r--   0        0        0     4726 2024-04-18 13:46:10.657117 sqlfactory-1.1.0/sqlfactory/func/info.py
+-rw-r--r--   0        0        0     4601 2024-04-18 13:46:10.657117 sqlfactory-1.1.0/sqlfactory/func/misc.py
+-rw-r--r--   0        0        0     7156 2024-04-18 13:46:10.657117 sqlfactory-1.1.0/sqlfactory/func/numeric.py
+-rw-r--r--   0        0        0     7741 2024-04-18 13:46:10.657117 sqlfactory-1.1.0/sqlfactory/func/str.py
+-rw-r--r--   0        0        0       95 2024-04-18 13:46:10.657117 sqlfactory-1.1.0/sqlfactory/insert/__init__.py
+-rw-r--r--   0        0        0     6349 2024-04-18 13:46:10.657117 sqlfactory-1.1.0/sqlfactory/insert/insert.py
+-rw-r--r--   0        0        0      601 2024-04-18 13:46:10.657117 sqlfactory-1.1.0/sqlfactory/insert/values.py
+-rw-r--r--   0        0        0      115 2024-04-18 13:46:10.657117 sqlfactory-1.1.0/sqlfactory/logger.py
+-rw-r--r--   0        0        0      271 2024-04-18 13:46:10.657117 sqlfactory-1.1.0/sqlfactory/mixins/__init__.py
+-rw-r--r--   0        0        0     3822 2024-04-18 13:46:10.657117 sqlfactory-1.1.0/sqlfactory/mixins/limit.py
+-rw-r--r--   0        0        0     2498 2024-04-18 13:46:10.657117 sqlfactory-1.1.0/sqlfactory/mixins/order.py
+-rw-r--r--   0        0        0      824 2024-04-18 13:46:10.657117 sqlfactory-1.1.0/sqlfactory/mixins/where.py
+-rw-r--r--   0        0        0      244 2024-04-18 13:46:10.657117 sqlfactory-1.1.0/sqlfactory/select/__init__.py
+-rw-r--r--   0        0        0     1200 2024-04-18 13:46:10.657117 sqlfactory-1.1.0/sqlfactory/select/aliased.py
+-rw-r--r--   0        0        0     2115 2024-04-18 13:46:10.657117 sqlfactory-1.1.0/sqlfactory/select/column_list.py
+-rw-r--r--   0        0        0     1846 2024-04-18 13:46:10.657117 sqlfactory-1.1.0/sqlfactory/select/join.py
+-rw-r--r--   0        0        0     7502 2024-04-18 13:46:10.657117 sqlfactory-1.1.0/sqlfactory/select/select.py
+-rw-r--r--   0        0        0     3861 2024-04-18 13:46:10.657117 sqlfactory-1.1.0/sqlfactory/statement.py
+-rw-r--r--   0        0        0       68 2024-04-18 13:46:10.657117 sqlfactory-1.1.0/sqlfactory/update/__init__.py
+-rw-r--r--   0        0        0     4867 2024-04-18 13:46:10.657117 sqlfactory-1.1.0/sqlfactory/update/update.py
+-rw-r--r--   0        0        0     9002 1970-01-01 00:00:00.000000 sqlfactory-1.1.0/PKG-INFO
```

### Comparing `sqlfactory-1.0.3/LICENSE` & `sqlfactory-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/README.md` & `sqlfactory-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/pyproject.toml` & `sqlfactory-1.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlfactory"
-version = "v1.0.3"
+version = "v1.1.0"
 description = "Convenient classes for building SQL queries in Python. Main purpose of this library is to ease construction of SQL queries in Python code. It is not an ORM (and don't intend to be), just a plain SQL query builder with syntax as similar to actual SQL as possible."
 authors = ["Michal Kuchta <niximor@gmail.com>"]
 readme = "README.md"
 packages = [{include = "sqlfactory"}]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 5 - Production/Stable",
```

### Comparing `sqlfactory-1.0.3/sqlfactory/condition/base.py` & `sqlfactory-1.1.0/sqlfactory/condition/base.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/condition/between.py` & `sqlfactory-1.1.0/sqlfactory/condition/between.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/condition/in_condition.py` & `sqlfactory-1.1.0/sqlfactory/condition/in_condition.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/condition/like.py` & `sqlfactory-1.1.0/sqlfactory/condition/like.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/condition/simple.py` & `sqlfactory-1.1.0/sqlfactory/condition/simple.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/delete/delete.py` & `sqlfactory-1.1.0/sqlfactory/delete/delete.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/entities.py` & `sqlfactory-1.1.0/sqlfactory/entities.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/execute.py` & `sqlfactory-1.1.0/sqlfactory/execute.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/func/agg.py` & `sqlfactory-1.1.0/sqlfactory/func/agg.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/func/base.py` & `sqlfactory-1.1.0/sqlfactory/func/base.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/func/control.py` & `sqlfactory-1.1.0/sqlfactory/func/control.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/func/datetime.py` & `sqlfactory-1.1.0/sqlfactory/func/datetime.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/func/enc.py` & `sqlfactory-1.1.0/sqlfactory/func/enc.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/func/info.py` & `sqlfactory-1.1.0/sqlfactory/func/info.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/func/misc.py` & `sqlfactory-1.1.0/sqlfactory/func/misc.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/func/numeric.py` & `sqlfactory-1.1.0/sqlfactory/func/numeric.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/func/str.py` & `sqlfactory-1.1.0/sqlfactory/func/str.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/insert/insert.py` & `sqlfactory-1.1.0/sqlfactory/insert/insert.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/insert/values.py` & `sqlfactory-1.1.0/sqlfactory/insert/values.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/mixins/limit.py` & `sqlfactory-1.1.0/sqlfactory/mixins/limit.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/mixins/order.py` & `sqlfactory-1.1.0/sqlfactory/mixins/order.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/mixins/where.py` & `sqlfactory-1.1.0/sqlfactory/mixins/where.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/select/aliased.py` & `sqlfactory-1.1.0/sqlfactory/select/aliased.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/select/column_list.py` & `sqlfactory-1.1.0/sqlfactory/select/column_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,19 +19,22 @@
             ))
         else:
             super().__init__()
 
     def __contains__(self, other: Statement):
         """This needs custom implementation over default list.__contains__ because we need to compare Column objects,
         which would generate Eq() instances instead of doing comparison."""
+        if isinstance(other, Column):
+            other = str(other)
+
         for item in self:
-            if isinstance(item, Column) and isinstance(other, Column):
-                if str(item) == str(other):
-                    return True
-            elif item == other:
+            if isinstance(item, Column):
+                item = str(item)
+
+            if item == other:
                 return True
 
         return False
 
     def add(self, element: Statement | str) -> ColumnList:
         """Add new columns to the set."""
         return self.append(element)
```

### Comparing `sqlfactory-1.0.3/sqlfactory/select/join.py` & `sqlfactory-1.1.0/sqlfactory/select/join.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/select/select.py` & `sqlfactory-1.1.0/sqlfactory/select/select.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """SELECT statement builder."""
 
 from __future__ import annotations
 
 from collections.abc import Collection
+from functools import reduce
 from typing import Any, overload
 
 from .column_list import ColumnList
 from .join import Join, LeftJoin
 from ..entities import ColumnArg, Table
 from ..condition.base import ConditionBase
 from ..execute import ExecutableStatementWithArgs
@@ -33,15 +34,15 @@
       user to ensure that JOINs are unique. This may be changed in the future, but it is not simple task, as joins
       needs to be in certain order.
     """
     def __init__(
             self,
             *columns: Statement | ColumnArg,
             select: ColumnList = None,
-            table: Table | str | Statement = None,
+            table: Table | str | Statement | Collection[Table | str | Statement] = None,
             join: Collection[Join] = None,
             where: ConditionBase = None,
             group_by: ColumnList | Collection[Statement | ColumnArg] = None,
             having: ConditionBase = None,
             order: OrderArg = None,
             limit: Limit = None
     ):
@@ -66,15 +67,18 @@
 
         self.columns = select or ColumnList(columns)
 
         if not table:
             self.table = ""
             raise AttributeError("Missing required keyword argument table.")
 
-        self.table = Table(table) if isinstance(table, str) else table
+        if not isinstance(table, Collection) or isinstance(table, str):
+            table = [table]
+
+        self.table = [Table(t) if isinstance(t, str) else t for t in table]
         self._join = list(join) if join is not None else None
         self._group_by = ColumnList(group_by) if group_by is not None and not isinstance(group_by, ColumnList) else group_by
         self._having = having
 
     def add(self, column: Statement | Any) -> Select:
         """Add new statement or column to the set of selected columns"""
         self.columns.add(column)
@@ -149,15 +153,15 @@
 
     # pylint: disable=invalid-name
     def HAVING(self, condition: ConditionBase) -> Select:
         """Alias for having() to be more SQL-like with all capitals."""
         return self.having(condition)
 
     def __str__(self):
-        out = ["SELECT", str(self.columns), f"FROM {str(self.table)}"]
+        out = ["SELECT", str(self.columns), f"FROM {', '.join(map(str, self.table))}"]
 
         if self._join:
             out.extend(map(str, self._join))
 
         if self._where:
             out.append("WHERE")
             out.append(str(self._where))
@@ -184,15 +188,19 @@
 
         if self._join:
             for join in self._join:
                 out.extend(join.args)
 
         return (
             out +
-            (self.table.args if isinstance(self.table, StatementWithArgs) else []) +
+            reduce(
+                lambda acc, t: acc + (t.args if isinstance(t, StatementWithArgs) else []),
+                self.table,
+                []
+            ) +
             (self._where.args if self._where else []) +
             (self._group_by.args if self._group_by else []) +
             (self._having.args if self._having else []) +
             (self._order.args if self._order else []) +
             (self._limit.args if self._limit else [])
         )
```

### Comparing `sqlfactory-1.0.3/sqlfactory/statement.py` & `sqlfactory-1.1.0/sqlfactory/statement.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/sqlfactory/update/update.py` & `sqlfactory-1.1.0/sqlfactory/update/update.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.0.3/PKG-INFO` & `sqlfactory-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfactory
-Version: 1.0.3
+Version: 1.1.0
 Summary: Convenient classes for building SQL queries in Python. Main purpose of this library is to ease construction of SQL queries in Python code. It is not an ORM (and don't intend to be), just a plain SQL query builder with syntax as similar to actual SQL as possible.
 Author: Michal Kuchta
 Author-email: niximor@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

