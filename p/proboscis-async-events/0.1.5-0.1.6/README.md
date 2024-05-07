# Comparing `tmp/proboscis_async_events-0.1.5.tar.gz` & `tmp/proboscis_async_events-0.1.6.tar.gz`

## Comparing `proboscis_async_events-0.1.5.tar` & `proboscis_async_events-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/.python-version
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/requirements-dev.lock
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/requirements.lock
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/.idea/.gitignore
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/.idea/misc.xml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/.idea/modules.xml
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/.idea/proboscis-async-events.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/.idea/vcs.xml
--rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/.idea/workspace.xml
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/.idea/codeStyles/Project.xml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/src/proboscis_async_events/__init__.py
--rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/src/proboscis_async_events/messaging.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/test/test_messaging.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/.gitignore
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/README.md
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/.python-version
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/requirements-dev.lock
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/requirements.lock
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/.idea/.gitignore
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/.idea/misc.xml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/.idea/modules.xml
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/.idea/proboscis-async-events.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/.idea/vcs.xml
+-rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/.idea/workspace.xml
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/.idea/codeStyles/Project.xml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/src/proboscis_async_events/__init__.py
+-rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/src/proboscis_async_events/messaging.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/test/test_messaging.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/.gitignore
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/README.md
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/PKG-INFO
```

### Comparing `proboscis_async_events-0.1.5/.idea/proboscis-async-events.iml` & `proboscis_async_events-0.1.6/.idea/proboscis-async-events.iml`

 * *Files identical despite different names*

### Comparing `proboscis_async_events-0.1.5/.idea/workspace.xml` & `proboscis_async_events-0.1.6/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `proboscis_async_events-0.1.5/.idea/inspectionProfiles/Project_Default.xml` & `proboscis_async_events-0.1.6/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `proboscis_async_events-0.1.5/src/proboscis_async_events/messaging.py` & `proboscis_async_events-0.1.6/src/proboscis_async_events/messaging.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,16 +23,25 @@
     src_handle: "Messages"
 
     def __post_init__(self):
         self.value_set = Event()
         self.value_set.clear()
         self.value_empty = Event()
         self.value_empty.set()
+        self.entered = Event()
         self.message = _Item("waiting", None)
 
+    async def __aenter__(self):
+        self.entered.set()
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        await self.unsubscribe()
+        self.entered.clear()
+
+
     async def tell(self, message: _Item):
         assert self.message.header != 'end', "Cannot publish to a closed subscriber"
         await self.value_empty.wait()
         self.message = message
         self.value_empty.clear()
         # print(f'Subscriber{id(self)}: setting value_set signal')
         self.value_set.set()
@@ -46,14 +55,15 @@
                 # print(f"subscriber: closing subscriber due to {message.header}")
                 pass
             case _:
                 raise ValueError(f"Invalid message type {message}")
 
     async def get_raw(self):
         # print(f'Subscriber{id(self)}: waiting for value_set signal:{self.value_set.is_set()}:{id(self.value_set)}')
+        assert self.entered.is_set(), "Subscriber must be entered with async with statement"
         await self.value_set.wait()
         # print('Subscriber: waited for value_set signal')
         res = self.message
         self.message = _Item("waiting", None)
         self.value_set.clear()
         self.value_empty.set()
         # print('Subscriber: value_set signal cleared')
@@ -111,16 +121,25 @@
 
     def subscribe(self) -> Subscriber:
         subscriber = Subscriber(self)
         self.subscribers.append(subscriber)
         return subscriber
 
     async def publish(self, message):
-        for subscriber in self.subscribers:
+        assert not isinstance(message, _Item), "Cannot publish a _Item"
+        #print(f'Messages: publishing {message} to {len(self.subscribers)} subscribers')
+        for subscriber in list(self.subscribers):
             await subscriber.tell(_Item('item', message))
+        #print(f'Messages: published {message} to {len(self.subscribers)} subscribers')
 
     async def unsubscribe(self, subscriber: Subscriber):
+        #print(f'Messages: unsubscribing {id(subscriber)} from {self.subscribers}')
         self.subscribers.remove(subscriber)
         await subscriber.tell(_Item('unsubscribe', None))
+        #print(f'Messages: unsubscription done for {id(subscriber)}')
+        #print(f'Messages: remaining subscribers:{[id(s) for s in self.subscribers]}')
 
     async def close(self):
-        await self.publish(_Item('end', None))
+        for subscriber in list(self.subscribers):
+            #print(f'Messages: closing subscriber:{subscriber}')
+            await subscriber.tell(_Item('end', None))
+            #print('Messages: closed subscriber')
```

### Comparing `proboscis_async_events-0.1.5/pyproject.toml` & `proboscis_async_events-0.1.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "proboscis-async-events"
-version = "0.1.5"
+version = "0.1.6"
 description = "Add your description here"
 authors = [
     { name = "proboscis", email = "nameissoap@gmail.com" }
 ]
 dependencies = [
     "pampy>=0.3.0",
     "pytest>=8.2.0",
```

