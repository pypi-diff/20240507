# Comparing `tmp/pastperfect-0.0.2.tar.gz` & `tmp/pastperfect-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pastperfect-0.0.2.tar", max compression
+gzip compressed data, was "pastperfect-0.0.3.tar", max compression
```

## Comparing `pastperfect-0.0.2.tar` & `pastperfect-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2024-04-12 08:54:26.251362 pastperfect-0.0.2/LICENSE
--rw-r--r--   0        0        0      565 2024-04-12 20:39:41.605036 pastperfect-0.0.2/README.md
--rw-r--r--   0        0        0     1097 2024-04-12 20:40:24.011016 pastperfect-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       42 2024-04-12 20:39:18.086691 pastperfect-0.0.2/src/pastperfect/__init__.py
--rw-r--r--   0        0        0     2059 2024-04-12 20:39:18.094107 pastperfect-0.0.2/src/pastperfect/events.py
--rw-r--r--   0        0        0     1091 1970-01-01 00:00:00.000000 pastperfect-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-05-02 19:59:02.121990 pastperfect-0.0.3/LICENSE
+-rw-r--r--   0        0        0      870 2024-05-02 20:50:55.470882 pastperfect-0.0.3/README.md
+-rw-r--r--   0        0        0     1097 2024-05-07 20:26:14.579871 pastperfect-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-05-02 19:59:02.125536 pastperfect-0.0.3/src/pastperfect/__init__.py
+-rw-r--r--   0        0        0     2118 2024-05-07 20:22:28.929288 pastperfect-0.0.3/src/pastperfect/events.py
+-rw-r--r--   0        0        0     1396 1970-01-01 00:00:00.000000 pastperfect-0.0.3/PKG-INFO
```

### Comparing `pastperfect-0.0.2/LICENSE` & `pastperfect-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pastperfect-0.0.2/pyproject.toml` & `pastperfect-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 [tool.mypy]
 ignore_missing_imports = true
 # https://stackoverflow.com/questions/62265366/does-mypy-only-type-check-a-function-if-it-declares-a-return-type
 check_untyped_defs = true
 
 [tool.poetry]
 name = "pastperfect"
-version = "0.0.2"
+version = "0.0.3"
 description = "An experience on storing events."
 authors = ["Luís Miranda <luistm@gmail.com>"]
 license = "The Unlicense"
 readme = "README.md"
 packages = [{ include = "pastperfect", from = "src" }]
 exclude = ["**/*_test.py"]
```

### Comparing `pastperfect-0.0.2/src/pastperfect/events.py` & `pastperfect-0.0.3/src/pastperfect/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import json
 from dataclasses import dataclass, field
 from datetime import datetime
 from typing import Any, Iterator, Optional
 
 from turbofan.database import text  # type: ignore
 
@@ -25,27 +27,29 @@
 
     def __len__(self) -> int:
         sql_stmt = """SELECT COUNT(*) FROM event"""
         prepared_statement = text(sql_stmt)
         row = self._session.execute(prepared_statement).first()
         return row[0]
 
-    def append(self, event: Event) -> None:
+    def append(self, event: Event) -> Events:
         """
         Appends an event to the list of events.
         """
         sql_stmt = """INSERT INTO event (name, data, created_at) VALUES (:name, :data, :created_at)"""
         prepared_statement = text(sql_stmt)
         prepared_statement = prepared_statement.bindparams(
             name=event.name,
             data=json.dumps(event.data),
             created_at=event.created_at,
         )
         self._session.execute(prepared_statement)
 
+        return self
+
     def __getitem__(self, event_id: int) -> Event:
         sql_stmt = """SELECT id, name, data, created_at FROM event WHERE id = :item"""
         prepared_statement = text(sql_stmt)
         prepared_statement = prepared_statement.bindparams(item=event_id + 1)
         row = self._session.execute(prepared_statement).first()
         if not row:
             raise KeyError
```

