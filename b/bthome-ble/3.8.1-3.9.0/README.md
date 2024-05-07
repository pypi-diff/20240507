# Comparing `tmp/bthome_ble-3.8.1.tar.gz` & `tmp/bthome_ble-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bthome_ble-3.8.1.tar", max compression
+gzip compressed data, was "bthome_ble-3.9.0.tar", max compression
```

## Comparing `bthome_ble-3.8.1.tar` & `bthome_ble-3.9.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2024-03-18 07:59:03.586130 bthome_ble-3.8.1/LICENSE
--rw-r--r--   0        0        0     3675 2024-03-18 07:59:03.586130 bthome_ble-3.8.1/README.md
--rw-r--r--   0        0        0     2378 2024-03-18 07:59:04.230122 bthome_ble-3.8.1/pyproject.toml
--rw-r--r--   0        0        0      610 2024-03-18 07:59:04.202123 bthome_ble-3.8.1/src/bthome_ble/__init__.py
--rw-r--r--   0        0        0     3604 2024-03-18 07:59:03.586130 bthome_ble-3.8.1/src/bthome_ble/bthome_v1_encryption.py
--rw-r--r--   0        0        0     3765 2024-03-18 07:59:03.586130 bthome_ble-3.8.1/src/bthome_ble/bthome_v2_encryption.py
--rw-r--r--   0        0        0    11758 2024-03-18 07:59:03.586130 bthome_ble-3.8.1/src/bthome_ble/const.py
--rw-r--r--   0        0        0      649 2024-03-18 07:59:03.586130 bthome_ble-3.8.1/src/bthome_ble/event.py
--rw-r--r--   0        0        0    27216 2024-03-18 07:59:03.586130 bthome_ble-3.8.1/src/bthome_ble/parser.py
--rw-r--r--   0        0        0        0 2024-03-18 07:59:03.586130 bthome_ble-3.8.1/src/bthome_ble/py.typed
--rw-r--r--   0        0        0     5179 1970-01-01 00:00:00.000000 bthome_ble-3.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-07 17:50:02.112908 bthome_ble-3.9.0/LICENSE
+-rw-r--r--   0        0        0     3675 2024-05-07 17:50:02.112908 bthome_ble-3.9.0/README.md
+-rw-r--r--   0        0        0     2378 2024-05-07 17:50:02.828912 bthome_ble-3.9.0/pyproject.toml
+-rw-r--r--   0        0        0      610 2024-05-07 17:50:02.804912 bthome_ble-3.9.0/src/bthome_ble/__init__.py
+-rw-r--r--   0        0        0     3604 2024-05-07 17:50:02.116908 bthome_ble-3.9.0/src/bthome_ble/bthome_v1_encryption.py
+-rw-r--r--   0        0        0     3765 2024-05-07 17:50:02.116908 bthome_ble-3.9.0/src/bthome_ble/bthome_v2_encryption.py
+-rw-r--r--   0        0        0    11758 2024-05-07 17:50:02.116908 bthome_ble-3.9.0/src/bthome_ble/const.py
+-rw-r--r--   0        0        0      673 2024-05-07 17:50:02.116908 bthome_ble-3.9.0/src/bthome_ble/event.py
+-rw-r--r--   0        0        0    27216 2024-05-07 17:50:02.116908 bthome_ble-3.9.0/src/bthome_ble/parser.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:50:02.116908 bthome_ble-3.9.0/src/bthome_ble/py.typed
+-rw-r--r--   0        0        0     5179 1970-01-01 00:00:00.000000 bthome_ble-3.9.0/PKG-INFO
```

### Comparing `bthome_ble-3.8.1/LICENSE` & `bthome_ble-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bthome_ble-3.8.1/README.md` & `bthome_ble-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `bthome_ble-3.8.1/pyproject.toml` & `bthome_ble-3.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bthome-ble"
-version = "3.8.1"
+version = "3.9.0"
 description = "BThome BLE support"
 authors = ["Ernst Klamer <e.klamer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bluetooth-devices/bthome-ble"
 documentation = "https://bthome-ble.readthedocs.io"
 classifiers = [
```

### Comparing `bthome_ble-3.8.1/src/bthome_ble/__init__.py` & `bthome_ble-3.9.0/src/bthome_ble/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     SensorUpdate,
     SensorValue,
     Units,
 )
 
 from .parser import BTHomeBluetoothDeviceData
 
-__version__ = "3.8.1"
+__version__ = "3.9.0"
 
 __all__ = [
     "BinarySensorDeviceClass",
     "BTHomeBluetoothDeviceData",
     "DeviceClass",
     "DeviceKey",
     "SensorDescription",
```

### Comparing `bthome_ble-3.8.1/src/bthome_ble/bthome_v1_encryption.py` & `bthome_ble-3.9.0/src/bthome_ble/bthome_v1_encryption.py`

 * *Files identical despite different names*

### Comparing `bthome_ble-3.8.1/src/bthome_ble/bthome_v2_encryption.py` & `bthome_ble-3.9.0/src/bthome_ble/bthome_v2_encryption.py`

 * *Files identical despite different names*

### Comparing `bthome_ble-3.8.1/src/bthome_ble/const.py` & `bthome_ble-3.9.0/src/bthome_ble/const.py`

 * *Files identical despite different names*

### Comparing `bthome_ble-3.8.1/src/bthome_ble/parser.py` & `bthome_ble-3.9.0/src/bthome_ble/parser.py`

 * *Files identical despite different names*

### Comparing `bthome_ble-3.8.1/PKG-INFO` & `bthome_ble-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bthome-ble
-Version: 3.8.1
+Version: 3.9.0
 Summary: BThome BLE support
 Home-page: https://github.com/bluetooth-devices/bthome-ble
 License: MIT
 Author: Ernst Klamer
 Author-email: e.klamer@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bthome-ble Version: 3.8.1 Summary: BThome BLE
+Metadata-Version: 2.1 Name: bthome-ble Version: 3.9.0 Summary: BThome BLE
 support Home-page: https://github.com/bluetooth-devices/bthome-ble License: MIT
 Author: Ernst Klamer Author-email: e.klamer@gmail.com Requires-Python:
 >=3.9,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

