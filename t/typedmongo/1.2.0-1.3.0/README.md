# Comparing `tmp/typedmongo-1.2.0.tar.gz` & `tmp/typedmongo-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedmongo-1.2.0.tar", last modified: Mon May  6 01:46:10 2024, max compression
+gzip compressed data, was "typedmongo-1.3.0.tar", last modified: Tue May  7 08:45:25 2024, max compression
```

## Comparing `typedmongo-1.2.0.tar` & `typedmongo-1.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2024-05-06 01:45:52.892057 typedmongo-1.2.0/LICENSE
--rw-r--r--   0        0        0     3808 2024-05-06 01:45:52.892057 typedmongo-1.2.0/README.md
--rw-r--r--   0        0        0     1441 2024-05-06 01:46:10.243988 typedmongo-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-06 01:45:52.892057 typedmongo-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 01:45:52.892057 typedmongo-1.2.0/tests/asyncio/__init__.py
--rw-r--r--   0        0        0     5575 2024-05-06 01:45:52.892057 typedmongo-1.2.0/tests/asyncio/test_client.py
--rw-r--r--   0        0        0     4233 2024-05-06 01:45:52.896057 typedmongo-1.2.0/tests/asyncio/test_table.py
--rw-r--r--   0        0        0     1218 2024-05-06 01:45:52.896057 typedmongo-1.2.0/tests/sync.py
--rw-r--r--   0        0        0     5335 2024-05-06 01:45:52.896057 typedmongo-1.2.0/tests/test_client.py
--rw-r--r--   0        0        0     2930 2024-05-06 01:45:52.896057 typedmongo-1.2.0/tests/test_expressions.py
--rw-r--r--   0        0        0      582 2024-05-06 01:45:52.896057 typedmongo-1.2.0/tests/test_marshamallow.py
--rw-r--r--   0        0        0     4225 2024-05-06 01:45:52.896057 typedmongo-1.2.0/tests/test_table.py
--rw-r--r--   0        0        0      811 2024-05-06 01:45:52.896057 typedmongo-1.2.0/typedmongo/__init__.py
--rw-r--r--   0        0        0      811 2024-05-06 01:45:52.896057 typedmongo-1.2.0/typedmongo/asyncio/__init__.py
--rw-r--r--   0        0        0    10328 2024-05-06 01:45:52.896057 typedmongo-1.2.0/typedmongo/asyncio/client.py
--rw-r--r--   0        0        0     9999 2024-05-06 01:45:52.896057 typedmongo-1.2.0/typedmongo/asyncio/fields.py
--rw-r--r--   0        0        0     8527 2024-05-06 01:45:52.896057 typedmongo-1.2.0/typedmongo/asyncio/table.py
--rw-r--r--   0        0        0    10122 2024-05-06 01:45:52.896057 typedmongo-1.2.0/typedmongo/client.py
--rw-r--r--   0        0        0      163 2024-05-06 01:45:52.896057 typedmongo-1.2.0/typedmongo/exceptions.py
--rw-r--r--   0        0        0     5452 2024-05-06 01:45:52.896057 typedmongo-1.2.0/typedmongo/expressions.py
--rw-r--r--   0        0        0     9999 2024-05-06 01:45:52.896057 typedmongo-1.2.0/typedmongo/fields.py
--rw-r--r--   0        0        0      849 2024-05-06 01:45:52.896057 typedmongo-1.2.0/typedmongo/marshamallow.py
--rw-r--r--   0        0        0     1325 2024-05-06 01:45:52.896057 typedmongo-1.2.0/typedmongo/sync.py
--rw-r--r--   0        0        0     8527 2024-05-06 01:45:52.896057 typedmongo-1.2.0/typedmongo/table.py
--rw-r--r--   0        0        0     4181 1970-01-01 00:00:00.000000 typedmongo-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-07 08:45:14.284598 typedmongo-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3808 2024-05-07 08:45:14.284598 typedmongo-1.3.0/README.md
+-rw-r--r--   0        0        0     1441 2024-05-07 08:45:25.828545 typedmongo-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-07 08:45:14.284598 typedmongo-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 08:45:14.284598 typedmongo-1.3.0/tests/asyncio/__init__.py
+-rw-r--r--   0        0        0     5575 2024-05-07 08:45:14.284598 typedmongo-1.3.0/tests/asyncio/test_client.py
+-rw-r--r--   0        0        0     4229 2024-05-07 08:45:14.284598 typedmongo-1.3.0/tests/asyncio/test_table.py
+-rw-r--r--   0        0        0     1218 2024-05-07 08:45:14.284598 typedmongo-1.3.0/tests/sync.py
+-rw-r--r--   0        0        0     5335 2024-05-07 08:45:14.284598 typedmongo-1.3.0/tests/test_client.py
+-rw-r--r--   0        0        0     2930 2024-05-07 08:45:14.284598 typedmongo-1.3.0/tests/test_expressions.py
+-rw-r--r--   0        0        0      582 2024-05-07 08:45:14.288598 typedmongo-1.3.0/tests/test_marshamallow.py
+-rw-r--r--   0        0        0     4221 2024-05-07 08:45:14.288598 typedmongo-1.3.0/tests/test_table.py
+-rw-r--r--   0        0        0      811 2024-05-07 08:45:14.288598 typedmongo-1.3.0/typedmongo/__init__.py
+-rw-r--r--   0        0        0      811 2024-05-07 08:45:14.288598 typedmongo-1.3.0/typedmongo/asyncio/__init__.py
+-rw-r--r--   0        0        0    10328 2024-05-07 08:45:14.288598 typedmongo-1.3.0/typedmongo/asyncio/client.py
+-rw-r--r--   0        0        0     9999 2024-05-07 08:45:14.288598 typedmongo-1.3.0/typedmongo/asyncio/fields.py
+-rw-r--r--   0        0        0     8494 2024-05-07 08:45:14.288598 typedmongo-1.3.0/typedmongo/asyncio/table.py
+-rw-r--r--   0        0        0    10122 2024-05-07 08:45:14.288598 typedmongo-1.3.0/typedmongo/client.py
+-rw-r--r--   0        0        0      163 2024-05-07 08:45:14.288598 typedmongo-1.3.0/typedmongo/exceptions.py
+-rw-r--r--   0        0        0     5452 2024-05-07 08:45:14.288598 typedmongo-1.3.0/typedmongo/expressions.py
+-rw-r--r--   0        0        0     9999 2024-05-07 08:45:14.288598 typedmongo-1.3.0/typedmongo/fields.py
+-rw-r--r--   0        0        0      849 2024-05-07 08:45:14.288598 typedmongo-1.3.0/typedmongo/marshamallow.py
+-rw-r--r--   0        0        0     1325 2024-05-07 08:45:14.288598 typedmongo-1.3.0/typedmongo/sync.py
+-rw-r--r--   0        0        0     8494 2024-05-07 08:45:14.288598 typedmongo-1.3.0/typedmongo/table.py
+-rw-r--r--   0        0        0     4181 1970-01-01 00:00:00.000000 typedmongo-1.3.0/PKG-INFO
```

### Comparing `typedmongo-1.2.0/LICENSE` & `typedmongo-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typedmongo-1.2.0/README.md` & `typedmongo-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `typedmongo-1.2.0/pyproject.toml` & `typedmongo-1.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "typedmongo"
-version = "1.2.0"
+version = "1.3.0"
 description = "A production-ready modern Python MongoDB ODM"
 authors = [
     { name = "abersheeran", email = "me@abersheeran.com" },
 ]
 dependencies = [
     "pymongo>=4.6.3",
     "motor>=3.4.0",
```

### Comparing `typedmongo-1.2.0/tests/asyncio/test_client.py` & `typedmongo-1.3.0/tests/asyncio/test_client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.2.0/tests/asyncio/test_table.py` & `typedmongo-1.3.0/tests/asyncio/test_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     assert isinstance(user._id, str)
     assert isinstance(user.created_at, datetime.datetime)
 
     user = User(
         name="Aber", age=18, tags=["a", "b"], wallet=Wallet(balance=100), children=[]
     )
     assert hasattr(user, "_id")
-    assert isinstance(user.dump(user)["_id"], str)
+    assert isinstance(User.dump(user)["_id"], str)
     assert isinstance(user.created_at, datetime.datetime)
 
 
 def test_recursion_field():
     user = User.load(
         {
             "name": "Aber",
@@ -149,13 +149,13 @@
             "tags": ["a", "b"],
             "wallet": {"balance": 100},
             "children": [],
             "extra": {"a": "b"},
         }
     )
     assert user.extra == {"a": "b"}
-    assert user.dump(user)["extra"] == {"a": "b"}
+    assert user.dump()["extra"] == {"a": "b"}
 
 
 def test_datetime_field():
     user = User.load(dict(created_at=datetime.datetime.now()), partial=True)
     assert isinstance(user.created_at, datetime.datetime)
```

### Comparing `typedmongo-1.2.0/tests/sync.py` & `typedmongo-1.3.0/tests/sync.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.2.0/tests/test_client.py` & `typedmongo-1.3.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.2.0/tests/test_expressions.py` & `typedmongo-1.3.0/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.2.0/tests/test_marshamallow.py` & `typedmongo-1.3.0/tests/test_marshamallow.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.2.0/tests/test_table.py` & `typedmongo-1.3.0/tests/test_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     assert isinstance(user._id, str)
     assert isinstance(user.created_at, datetime.datetime)
 
     user = User(
         name="Aber", age=18, tags=["a", "b"], wallet=Wallet(balance=100), children=[]
     )
     assert hasattr(user, "_id")
-    assert isinstance(user.dump(user)["_id"], str)
+    assert isinstance(User.dump(user)["_id"], str)
     assert isinstance(user.created_at, datetime.datetime)
 
 
 def test_recursion_field():
     user = User.load(
         {
             "name": "Aber",
@@ -149,13 +149,13 @@
             "tags": ["a", "b"],
             "wallet": {"balance": 100},
             "children": [],
             "extra": {"a": "b"},
         }
     )
     assert user.extra == {"a": "b"}
-    assert user.dump(user)["extra"] == {"a": "b"}
+    assert user.dump()["extra"] == {"a": "b"}
 
 
 def test_datetime_field():
     user = User.load(dict(created_at=datetime.datetime.now()), partial=True)
     assert isinstance(user.created_at, datetime.datetime)
```

### Comparing `typedmongo-1.2.0/typedmongo/__init__.py` & `typedmongo-1.3.0/typedmongo/__init__.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.2.0/typedmongo/asyncio/__init__.py` & `typedmongo-1.3.0/typedmongo/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.2.0/typedmongo/asyncio/client.py` & `typedmongo-1.3.0/typedmongo/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.2.0/typedmongo/asyncio/fields.py` & `typedmongo-1.3.0/typedmongo/asyncio/fields.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.2.0/typedmongo/asyncio/table.py` & `typedmongo-1.3.0/typedmongo/asyncio/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,24 +227,23 @@
         validated: dict[str, Any] = cls.__schema__.load(data=data, partial=partial)  # type: ignore
         loaded = {
             key: getattr(cls.__fields__[key], "load")(value, partial=partial)
             for key, value in validated.items()
         }
         return cls(**loaded)
 
-    @classmethod
-    def dump(cls, instance: Self) -> dict[str, Any]:
+    def dump(self: Self) -> dict[str, Any]:
         """
         Dump the instance to jsonable dict.
         """
         dumped = {
-            key: getattr(instance.__fields__[key], "dump")(value)
-            for key, value in instance.__dict__.items()
+            key: getattr(self.__fields__[key], "dump")(value)
+            for key, value in self.__dict__.items()
         }
-        return cls.__schema__.dump(dumped)  # type: ignore
+        return self.__schema__.dump(dumped)  # type: ignore
 
     @classmethod
     def indexes(cls) -> list[Index]:
         return []
 
     def to_mongo(self) -> dict[str, Any]:
         """
```

### Comparing `typedmongo-1.2.0/typedmongo/client.py` & `typedmongo-1.3.0/typedmongo/client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.2.0/typedmongo/expressions.py` & `typedmongo-1.3.0/typedmongo/expressions.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.2.0/typedmongo/fields.py` & `typedmongo-1.3.0/typedmongo/fields.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.2.0/typedmongo/marshamallow.py` & `typedmongo-1.3.0/typedmongo/marshamallow.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.2.0/typedmongo/sync.py` & `typedmongo-1.3.0/typedmongo/sync.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.2.0/typedmongo/table.py` & `typedmongo-1.3.0/typedmongo/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,24 +227,23 @@
         validated: dict[str, Any] = cls.__schema__.load(data=data, partial=partial)  # type: ignore
         loaded = {
             key: getattr(cls.__fields__[key], "load")(value, partial=partial)
             for key, value in validated.items()
         }
         return cls(**loaded)
 
-    @classmethod
-    def dump(cls, instance: Self) -> dict[str, Any]:
+    def dump(self: Self) -> dict[str, Any]:
         """
         Dump the instance to jsonable dict.
         """
         dumped = {
-            key: getattr(instance.__fields__[key], "dump")(value)
-            for key, value in instance.__dict__.items()
+            key: getattr(self.__fields__[key], "dump")(value)
+            for key, value in self.__dict__.items()
         }
-        return cls.__schema__.dump(dumped)  # type: ignore
+        return self.__schema__.dump(dumped)  # type: ignore
 
     @classmethod
     def indexes(cls) -> list[Index]:
         return []
 
     def to_mongo(self) -> dict[str, Any]:
         """
```

### Comparing `typedmongo-1.2.0/PKG-INFO` & `typedmongo-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedmongo
-Version: 1.2.0
+Version: 1.3.0
 Summary: A production-ready modern Python MongoDB ODM
 Author-Email: abersheeran <me@abersheeran.com>
 License: Apache2.0
 Requires-Python: >=3.10
 Requires-Dist: pymongo>=4.6.3
 Requires-Dist: motor>=3.4.0
 Requires-Dist: marshmallow>=3.21.1
```

