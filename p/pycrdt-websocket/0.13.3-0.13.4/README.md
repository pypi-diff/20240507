# Comparing `tmp/pycrdt_websocket-0.13.3.tar.gz` & `tmp/pycrdt_websocket-0.13.4.tar.gz`

## Comparing `pycrdt_websocket-0.13.3.tar` & `pycrdt_websocket-0.13.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/pycrdt_websocket/__init__.py
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/pycrdt_websocket/asgi_server.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/pycrdt_websocket/awareness.py
--rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/pycrdt_websocket/django_channels_consumer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/pycrdt_websocket/py.typed
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/pycrdt_websocket/websocket.py
--rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/pycrdt_websocket/websocket_provider.py
--rw-r--r--   0        0        0     8412 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/pycrdt_websocket/websocket_server.py
--rw-r--r--   0        0        0    10700 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/pycrdt_websocket/yroom.py
--rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/pycrdt_websocket/ystore.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/pycrdt_websocket/yutils.py
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/tests/conftest.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/tests/package.json
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/tests/test_asgi.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/tests/test_pycrdt_yjs.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/tests/test_server.py
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/tests/test_yroom.py
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/tests/test_ystore.py
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/tests/utils.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/tests/yjs_client_0.js
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/tests/yjs_client_1.js
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/LICENSE
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/README.md
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/pyproject.toml
--rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/PKG-INFO
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/pycrdt_websocket/__init__.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/pycrdt_websocket/asgi_server.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/pycrdt_websocket/awareness.py
+-rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/pycrdt_websocket/django_channels_consumer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/pycrdt_websocket/py.typed
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/pycrdt_websocket/websocket.py
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/pycrdt_websocket/websocket_provider.py
+-rw-r--r--   0        0        0     8412 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/pycrdt_websocket/websocket_server.py
+-rw-r--r--   0        0        0    10772 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/pycrdt_websocket/yroom.py
+-rw-r--r--   0        0        0    16974 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/pycrdt_websocket/ystore.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/pycrdt_websocket/yutils.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/tests/conftest.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/tests/package.json
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/tests/test_asgi.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/tests/test_pycrdt_yjs.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/tests/test_server.py
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/tests/test_yroom.py
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/tests/test_ystore.py
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/tests/utils.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/tests/yjs_client_0.js
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/tests/yjs_client_1.js
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/LICENSE
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/README.md
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/pyproject.toml
+-rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.4/PKG-INFO
```

### Comparing `pycrdt_websocket-0.13.3/pycrdt_websocket/asgi_server.py` & `pycrdt_websocket-0.13.4/pycrdt_websocket/asgi_server.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.3/pycrdt_websocket/awareness.py` & `pycrdt_websocket-0.13.4/pycrdt_websocket/awareness.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.3/pycrdt_websocket/django_channels_consumer.py` & `pycrdt_websocket-0.13.4/pycrdt_websocket/django_channels_consumer.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.3/pycrdt_websocket/websocket.py` & `pycrdt_websocket-0.13.4/pycrdt_websocket/websocket.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.3/pycrdt_websocket/websocket_provider.py` & `pycrdt_websocket-0.13.4/pycrdt_websocket/websocket_provider.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.3/pycrdt_websocket/websocket_server.py` & `pycrdt_websocket-0.13.4/pycrdt_websocket/websocket_server.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.3/pycrdt_websocket/yroom.py` & `pycrdt_websocket-0.13.4/pycrdt_websocket/yroom.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,16 +130,18 @@
         Arguments:
             value: An optional callback to call when a message is received.
             If the callback returns True, the message is skipped.
         """
         self._on_message = value
 
     async def _broadcast_updates(self):
-        if self.ystore is not None and not self.ystore.started.is_set():
-            self._task_group.start_soon(self.ystore.start)
+        if self.ystore is not None:
+            async with self.ystore.start_lock:
+                if not self.ystore.started.is_set():
+                    await self._task_group.start(self.ystore.start)
 
         async with self._update_receive_stream:
             async for update in self._update_receive_stream:
                 if self._task_group.cancel_scope.cancel_called:
                     return
                 # broadcast internal ydoc's update to all clients, that includes changes from the
                 # clients and changes from the backend (out-of-band changes)
```

### Comparing `pycrdt_websocket-0.13.3/pycrdt_websocket/ystore.py` & `pycrdt_websocket-0.13.4/pycrdt_websocket/ystore.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 
 class BaseYStore(ABC):
     metadata_callback: Callable[[], Awaitable[bytes] | bytes] | None = None
     version = 2
     _started: Event | None = None
     _stopped: Event | None = None
     _task_group: TaskGroup | None = None
-    __start_lock: Lock | None = None
+    _public_start_lock: Lock | None = None
+    _private_start_lock: Lock | None = None
 
     @abstractmethod
     def __init__(
         self, path: str, metadata_callback: Callable[[], Awaitable[bytes] | bytes] | None = None
     ): ...
 
     @abstractmethod
@@ -54,18 +55,24 @@
     @property
     def stopped(self) -> Event:
         if self._stopped is None:
             self._stopped = Event()
         return self._stopped
 
     @property
+    def start_lock(self) -> Lock:
+        if self._public_start_lock is None:
+            self._public_start_lock = Lock()
+        return self._public_start_lock
+
+    @property
     def _start_lock(self) -> Lock:
-        if self.__start_lock is None:
-            self.__start_lock = Lock()
-        return self.__start_lock
+        if self._private_start_lock is None:
+            self._private_start_lock = Lock()
+        return self._private_start_lock
 
     async def __aenter__(self) -> BaseYStore:
         async with self._start_lock:
             if self._task_group is not None:
                 raise RuntimeError("YStore already running")
 
             async with AsyncExitStack() as exit_stack:
```

### Comparing `pycrdt_websocket-0.13.3/pycrdt_websocket/yutils.py` & `pycrdt_websocket-0.13.4/pycrdt_websocket/yutils.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.3/tests/conftest.py` & `pycrdt_websocket-0.13.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.3/tests/test_asgi.py` & `pycrdt_websocket-0.13.4/tests/test_asgi.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.3/tests/test_pycrdt_yjs.py` & `pycrdt_websocket-0.13.4/tests/test_pycrdt_yjs.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.3/tests/test_server.py` & `pycrdt_websocket-0.13.4/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.3/tests/test_yroom.py` & `pycrdt_websocket-0.13.4/tests/test_yroom.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.3/tests/test_ystore.py` & `pycrdt_websocket-0.13.4/tests/test_ystore.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.3/tests/utils.py` & `pycrdt_websocket-0.13.4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.3/tests/yjs_client_0.js` & `pycrdt_websocket-0.13.4/tests/yjs_client_0.js`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.3/tests/yjs_client_1.js` & `pycrdt_websocket-0.13.4/tests/yjs_client_1.js`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.3/.gitignore` & `pycrdt_websocket-0.13.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.3/LICENSE` & `pycrdt_websocket-0.13.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.3/README.md` & `pycrdt_websocket-0.13.4/README.md`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.3/pyproject.toml` & `pycrdt_websocket-0.13.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.3/PKG-INFO` & `pycrdt_websocket-0.13.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pycrdt-websocket
-Version: 0.13.3
+Version: 0.13.4
 Summary: WebSocket connector for pycrdt
 Project-URL: Homepage, https://github.com/jupyter-server/pycrdt-websocket
 Project-URL: Source, https://github.com/jupyter-server/pycrdt-websocket
 Project-URL: Issues, https://github.com/jupyter-server/pycrdt-websocket/issues
 Project-URL: Pypi, https://pypi.org/project/pycrdt-websocket
 Author-email: David Brochart <david.brochart@gmail.com>
 License: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: pycrdt-websocket Version: 0.13.3 Summary: WebSocket
+Metadata-Version: 2.3 Name: pycrdt-websocket Version: 0.13.4 Summary: WebSocket
 connector for pycrdt Project-URL: Homepage, https://github.com/jupyter-server/
 pycrdt-websocket Project-URL: Source, https://github.com/jupyter-server/pycrdt-
 websocket Project-URL: Issues, https://github.com/jupyter-server/pycrdt-
 websocket/issues Project-URL: Pypi, https://pypi.org/project/pycrdt-websocket
 Author-email: David Brochart
 gmail.com> License: MIT License Copyright (c) 2022 David Brochart Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
```

