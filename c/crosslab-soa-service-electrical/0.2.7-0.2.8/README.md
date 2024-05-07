# Comparing `tmp/crosslab_soa_service_electrical-0.2.7.tar.gz` & `tmp/crosslab_soa_service_electrical-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_soa_service_electrical-0.2.7.tar", last modified: Fri Apr  5 09:17:07 2024, max compression
+gzip compressed data, was "crosslab_soa_service_electrical-0.2.8.tar", last modified: Tue May  7 16:54:25 2024, max compression
```

## Comparing `crosslab_soa_service_electrical-0.2.7.tar` & `crosslab_soa_service_electrical-0.2.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:07.842567 crosslab_soa_service_electrical-0.2.7/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      410 2024-04-05 09:17:07.842567 crosslab_soa_service_electrical-0.2.7/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.7/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)      585 2024-04-05 09:17:07.842567 crosslab_soa_service_electrical-0.2.7/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)       37 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.7/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:07.838567 crosslab_soa_service_electrical-0.2.7/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:07.838567 crosslab_soa_service_electrical-0.2.7/src/crosslab/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:07.838567 crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:07.842567 crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      256 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5236 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/electrical_connection_service.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      745 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/messages.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/py.typed
--rw-r--r--   0 vscode    (1000) vscode    (1000)      614 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/signal_interface.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:07.842567 crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/signal_interfaces/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/signal_interfaces/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3001 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/signal_interfaces/gpio.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:07.842567 crosslab_soa_service_electrical-0.2.7/src/crosslab_soa_service_electrical.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      410 2024-04-05 09:17:07.000000 crosslab_soa_service_electrical-0.2.7/src/crosslab_soa_service_electrical.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      770 2024-04-05 09:17:07.000000 crosslab_soa_service_electrical-0.2.7/src/crosslab_soa_service_electrical.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-04-05 09:17:07.000000 crosslab_soa_service_electrical-0.2.7/src/crosslab_soa_service_electrical.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       25 2024-04-05 09:17:07.000000 crosslab_soa_service_electrical-0.2.7/src/crosslab_soa_service_electrical.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2024-04-05 09:17:07.000000 crosslab_soa_service_electrical-0.2.7/src/crosslab_soa_service_electrical.egg-info/top_level.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-05 09:17:07.842567 crosslab_soa_service_electrical-0.2.7/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4098 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.7/tests/test_gpio.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      810 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.7/tests/test_standard.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 16:54:25.402405 crosslab_soa_service_electrical-0.2.8/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      410 2024-05-07 16:54:25.402405 crosslab_soa_service_electrical-0.2.8/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.8/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      585 2024-05-07 16:54:25.402405 crosslab_soa_service_electrical-0.2.8/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       37 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.8/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 16:54:25.398405 crosslab_soa_service_electrical-0.2.8/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 16:54:25.398405 crosslab_soa_service_electrical-0.2.8/src/crosslab/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 16:54:25.398405 crosslab_soa_service_electrical-0.2.8/src/crosslab/soa_services/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 16:54:25.398405 crosslab_soa_service_electrical-0.2.8/src/crosslab/soa_services/electrical/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      256 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.8/src/crosslab/soa_services/electrical/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5279 2024-05-07 16:28:32.000000 crosslab_soa_service_electrical-0.2.8/src/crosslab/soa_services/electrical/electrical_connection_service.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      745 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.8/src/crosslab/soa_services/electrical/messages.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.8/src/crosslab/soa_services/electrical/py.typed
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      614 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.8/src/crosslab/soa_services/electrical/signal_interface.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 16:54:25.398405 crosslab_soa_service_electrical-0.2.8/src/crosslab/soa_services/electrical/signal_interfaces/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.8/src/crosslab/soa_services/electrical/signal_interfaces/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3001 2023-11-08 12:05:40.000000 crosslab_soa_service_electrical-0.2.8/src/crosslab/soa_services/electrical/signal_interfaces/gpio.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 16:54:25.402405 crosslab_soa_service_electrical-0.2.8/src/crosslab_soa_service_electrical.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      410 2024-05-07 16:54:25.000000 crosslab_soa_service_electrical-0.2.8/src/crosslab_soa_service_electrical.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      770 2024-05-07 16:54:25.000000 crosslab_soa_service_electrical-0.2.8/src/crosslab_soa_service_electrical.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-05-07 16:54:25.000000 crosslab_soa_service_electrical-0.2.8/src/crosslab_soa_service_electrical.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       25 2024-05-07 16:54:25.000000 crosslab_soa_service_electrical-0.2.8/src/crosslab_soa_service_electrical.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2024-05-07 16:54:25.000000 crosslab_soa_service_electrical-0.2.8/src/crosslab_soa_service_electrical.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-07 16:54:25.402405 crosslab_soa_service_electrical-0.2.8/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4394 2024-05-07 16:28:32.000000 crosslab_soa_service_electrical-0.2.8/tests/test_gpio.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      962 2024-05-07 16:28:32.000000 crosslab_soa_service_electrical-0.2.8/tests/test_standard.py
```

### Comparing `crosslab_soa_service_electrical-0.2.7/setup.cfg` & `crosslab_soa_service_electrical-0.2.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_soa_service_electrical
-version = 0.2.7
+version = 0.2.8
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab SOA Electrical Service
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
 	Operating System :: OS Independent
```

### Comparing `crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/electrical_connection_service.py` & `crosslab_soa_service_electrical-0.2.8/src/crosslab/soa_services/electrical/electrical_connection_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import json
 from dataclasses import dataclass
 from typing import Callable, Dict, Set
 
 from crosslab.soa_client.connection import Connection, DataChannel
 from crosslab.soa_client.service import Service
-from pyee.asyncio import AsyncIOEventEmitter
-
 from crosslab.soa_services.electrical import (
     ConstructableSignalInterface,
     SignalInterface,
 )
 from crosslab.soa_services.electrical.messages import (
     ElectricalServiceConfig,
     SignalInterfaceConfig,
 )
+from pyee.asyncio import AsyncIOEventEmitter
 
 
 @dataclass
 class SignalInterfaceMeta:
     upstreamDataFuns: Set[Callable]
     busIds: Set[str]
     id: str
@@ -103,15 +102,16 @@
 
             interface_meta = SignalInterfaceMeta(
                 id=id, busIds=set(), upstreamDataFuns=set()
             )
             connection_meta.interface_meta[interface] = interface_meta
             self._interface_id_ref_counter[id] += 1
 
-            def upstreamDataFun(data, busId=busId):
+            async def upstreamDataFun(data, busId=busId):
+                await channel.ready()
                 channel.send(json.dumps({"busId": busId, "data": data}))
 
             interface.on("upstreamData", upstreamDataFun)
             interface_meta.upstreamDataFuns.add(upstreamDataFun)
             interface_meta.busIds.add(busId)
 
             self._connection_meta[connection].interfaces.add(interface)
```

### Comparing `crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/messages.py` & `crosslab_soa_service_electrical-0.2.8/src/crosslab/soa_services/electrical/messages.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/signal_interface.py` & `crosslab_soa_service_electrical-0.2.8/src/crosslab/soa_services/electrical/signal_interface.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_electrical-0.2.7/src/crosslab/soa_services/electrical/signal_interfaces/gpio.py` & `crosslab_soa_service_electrical-0.2.8/src/crosslab/soa_services/electrical/signal_interfaces/gpio.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_electrical-0.2.7/src/crosslab_soa_service_electrical.egg-info/SOURCES.txt` & `crosslab_soa_service_electrical-0.2.8/src/crosslab_soa_service_electrical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_electrical-0.2.7/tests/test_gpio.py` & `crosslab_soa_service_electrical-0.2.8/tests/test_gpio.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,35 @@
+import asyncio
+from asyncio import sleep
 from typing import Any
 
 import pytest
 from crosslab.soa_client.test_helper import ConnectionStub
 from data import serviceConfig
 
 from crosslab.soa_services.electrical import ElectricalConnectionService
 from crosslab.soa_services.electrical.messages import ElectricalServiceConfig
 from crosslab.soa_services.electrical.signal_interfaces.gpio import (
     ConstractableGPIOInterface,
     GPIOInterface,
 )
+from tests.helper import running_tasks
 
 
 def test_gpio_meta():
     gci = ConstractableGPIOInterface(["S1", "S2"])
-    assert gci.getDescription() == {"availableSignals": {"gpio": ["S1", "S2"]}, "direction": "inout"}
+    assert gci.getDescription() == {
+        "availableSignals": {"gpio": ["S1", "S2"]},
+        "direction": "inout",
+    }
 
 
 @pytest.mark.parametrize("tiebreaker", [True, False])
-def test_gpio_interface_creation(tiebreaker):
+@pytest.mark.asyncio
+async def test_gpio_interface_creation(tiebreaker):
     con = ConnectionStub(tiebreaker)
     ecs = ElectricalConnectionService("test")
     gci = ConstractableGPIOInterface(["S1", "S2"])
     ecs.addInterface(gci)
 
     interface: Any = None
 
@@ -31,18 +38,20 @@
         assert interface is None
         interface = _interface
         assert isinstance(interface, GPIOInterface)
 
     ecs.on("newInterface", newInterface)
 
     ecs.setupConnection(con, serviceConfig)
+    await asyncio.wait(running_tasks())
 
 
 @pytest.mark.parametrize("tiebreaker", [True, False])
-def test_gpio_changeDriver(tiebreaker):
+@pytest.mark.asyncio
+async def test_gpio_changeDriver(tiebreaker):
     con = ConnectionStub(tiebreaker)
     ecs = ElectricalConnectionService("test")
     gci = ConstractableGPIOInterface(["S1", "S2"])
     ecs.addInterface(gci)
 
     interface: Any = None
 
@@ -53,24 +62,27 @@
     ecs.on("newInterface", newInterface)
 
     ecs.setupConnection(con, serviceConfig)
 
     assert isinstance(interface, GPIOInterface)
     interface.changeDriver("highZ")
 
+    await asyncio.wait(running_tasks())
+
     assert con.messages == {
         "data": [
             '{"busId": "0", "data": {"driver": "default", "state": "unknown"}}',
             '{"busId": "0", "data": {"driver": "default", "state": "highZ"}}',
         ]
     }
 
 
 @pytest.mark.parametrize("tiebreaker", [True, False])
-def test_gpio_signalChange(tiebreaker):
+@pytest.mark.asyncio
+async def test_gpio_signalChange(tiebreaker):
     con = ConnectionStub(tiebreaker)
     ecs = ElectricalConnectionService("test")
     gci = ConstractableGPIOInterface(["S1", "S2"])
     ecs.addInterface(gci)
 
     signalChanges = []
 
@@ -80,14 +92,15 @@
 
     ecs.on("newInterface", newInterface)
     ecs.setupConnection(con, serviceConfig)
     con.channels["data"].emit(
         "data", '{"busId": "0", "data": {"driver": "default", "state": "weakH"}}'
     )
     assert signalChanges == ["weakH"]
+    await asyncio.wait(running_tasks())
 
 
 def test_gpip_signal_evaluation():
     gpio = GPIOInterface({})  # type: ignore
 
     gpio.driverStates = {"S1": "highZ", "S2": "unknown"}
     gpio.evaluateSignalState()
@@ -128,8 +141,7 @@
     gpio.driverStates = {"S1": "weakH", "S2": "error"}
     gpio.evaluateSignalState()
     assert gpio.signalState == "error"
 
     gpio.driverStates = {"S1": "weakH", "S2": "unknown"}
     gpio.evaluateSignalState()
     assert gpio.signalState == "unknown"
-    pass
```

