# Comparing `tmp/proboscis_async_events-0.1.3.tar.gz` & `tmp/proboscis_async_events-0.1.4.tar.gz`

## Comparing `proboscis_async_events-0.1.3.tar` & `proboscis_async_events-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/.python-version
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/requirements-dev.lock
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/requirements.lock
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/.idea/.gitignore
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/.idea/misc.xml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/.idea/modules.xml
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/.idea/proboscis-async-events.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/.idea/vcs.xml
--rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/.idea/workspace.xml
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/.idea/codeStyles/Project.xml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/src/proboscis_async_events/__init__.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/src/proboscis_async_events/messaging.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/test/test_messaging.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/.gitignore
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/README.md
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/.python-version
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/requirements-dev.lock
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/requirements.lock
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/.idea/.gitignore
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/.idea/misc.xml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/.idea/modules.xml
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/.idea/proboscis-async-events.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/.idea/vcs.xml
+-rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/.idea/workspace.xml
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/.idea/codeStyles/Project.xml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/src/proboscis_async_events/__init__.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/src/proboscis_async_events/messaging.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/test/test_messaging.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/.gitignore
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/README.md
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/PKG-INFO
```

### Comparing `proboscis_async_events-0.1.3/.idea/inspectionProfiles/Project_Default.xml` & `proboscis_async_events-0.1.4/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `proboscis_async_events-0.1.3/src/proboscis_async_events/messaging.py` & `proboscis_async_events-0.1.4/src/proboscis_async_events/messaging.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,77 @@
 import asyncio
 from asyncio import Event
 from dataclasses import dataclass, field
+from queue import Empty
 
 import pampy
 
 
 @dataclass
+class _Item:
+    header: str
+    value: object
+
+
+class MessageClosed(Exception):
+    pass
+
+
+@dataclass
 class Subscriber:
     src_handle: "Messages"
 
     def __post_init__(self):
         self.value_set = Event()
         self.value_empty = Event()
-        self.message = None
+        self.message = _Item("waiting", None)
 
-    async def tell(self, message):
-        assert not self.value_set.is_set()
-        self.message = message
-        self.value_empty.clear()
-        self.value_set.set()
+    async def tell(self, message: _Item):
+        assert self.message.header != 'end', "Cannot publish to a closed subscriber"
         await self.value_empty.wait()
+        match message:
+            case _Item('item', value):
+                self.message = message
+                self.value_empty.clear()
+                self.value_set.set()
+                await self.value_empty.wait()
+            case _Item('end', None):
+                self.message = message
+                self.value_empty.clear()
+                self.value_set.set()
 
-    async def get(self):
+    async def get_raw(self):
         await self.value_set.wait()
-        message = self.message
-        self.message = None
+        res = self.message
+        self.message = _Item("waiting", None)
         self.value_set.clear()
         self.value_empty.set()
-        return message
+        return res
+
+    async def get(self):
+        res = await self.get_raw()
+        match res:
+            case _Item('end', None):
+                raise MessageClosed()
+            case _Item('item', value):
+                return value
 
     def unsubscribe(self):
         self.src_handle.unsubscribe(self)
 
     def __aiter__(self):
         return self
 
     async def __anext__(self):
-        item = await self.get()
-        if item is None:
-            raise StopAsyncIteration
-        return item
+        item = await self.get_raw()
+        match item:
+            case _Item('end', None):
+                raise StopAsyncIteration
+            case _Item('item', value):
+                return value
 
     async def wait(self, pattern):
         from pampy import _
         matched = False
         while not matched:
             message = await self.get()
```

### Comparing `proboscis_async_events-0.1.3/test/test_messaging.py` & `proboscis_async_events-0.1.4/test/test_messaging.py`

 * *Files identical despite different names*

### Comparing `proboscis_async_events-0.1.3/pyproject.toml` & `proboscis_async_events-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "proboscis-async-events"
-version = "0.1.3"
+version = "0.1.4"
 description = "Add your description here"
 authors = [
     { name = "proboscis", email = "nameissoap@gmail.com" }
 ]
 dependencies = [
     "pampy>=0.3.0",
     "pytest>=8.2.0",
```

