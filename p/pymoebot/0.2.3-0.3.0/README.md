# Comparing `tmp/pymoebot-0.2.3.tar.gz` & `tmp/pymoebot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymoebot-0.2.3.tar", last modified: Mon Jul 24 11:57:39 2023, max compression
+gzip compressed data, was "pymoebot-0.3.0.tar", last modified: Tue May  7 12:05:35 2024, max compression
```

## Comparing `pymoebot-0.2.3.tar` & `pymoebot-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:39.703800 pymoebot-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-07-24 11:57:39.703800 pymoebot-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-24 11:57:28.000000 pymoebot-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:39.699800 pymoebot-0.2.3/pymoebot/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-24 11:57:28.000000 pymoebot-0.2.3/pymoebot/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-24 11:57:28.000000 pymoebot-0.2.3/pymoebot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:39.703800 pymoebot-0.2.3/pymoebot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-07-24 11:57:39.000000 pymoebot-0.2.3/pymoebot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-24 11:57:39.000000 pymoebot-0.2.3/pymoebot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 11:57:39.000000 pymoebot-0.2.3/pymoebot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 11:57:39.000000 pymoebot-0.2.3/pymoebot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 11:57:39.000000 pymoebot-0.2.3/pymoebot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 11:57:39.703800 pymoebot-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-24 11:57:28.000000 pymoebot-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:39.703800 pymoebot-0.2.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:28.000000 pymoebot-0.2.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-24 11:57:28.000000 pymoebot-0.2.3/test/model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:05:35.882056 pymoebot-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-05-07 12:05:35.882056 pymoebot-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-05-07 12:05:31.000000 pymoebot-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:05:35.882056 pymoebot-0.3.0/pymoebot/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-07 12:05:31.000000 pymoebot-0.3.0/pymoebot/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11065 2024-05-07 12:05:31.000000 pymoebot-0.3.0/pymoebot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:05:35.882056 pymoebot-0.3.0/pymoebot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-05-07 12:05:35.000000 pymoebot-0.3.0/pymoebot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-07 12:05:35.000000 pymoebot-0.3.0/pymoebot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 12:05:35.000000 pymoebot-0.3.0/pymoebot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 12:05:35.000000 pymoebot-0.3.0/pymoebot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-07 12:05:35.000000 pymoebot-0.3.0/pymoebot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 12:05:35.882056 pymoebot-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-07 12:05:31.000000 pymoebot-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:05:35.882056 pymoebot-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 12:05:31.000000 pymoebot-0.3.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-07 12:05:31.000000 pymoebot-0.3.0/test/model_test.py
```

### Comparing `pymoebot-0.2.3/PKG-INFO` & `pymoebot-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pymoebot
-Version: 0.2.3
+Version: 0.3.0
 Summary: A Python library intended to monitor and control MoeBot robotic lawn mowers.
 Home-page: https://github.com/Whytey/pymoebot
 Author: David Whyte
 Author-email: David@Whyte.xyz
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Requires-Dist: tinytuya
 
 # pymoebot
 
 A Python library intended to monitor (and control?) the [MoeBot](https://moebot.com.au/) robotic lawn mowers.
 
 * MoeBot are controllable over WiFi via the Tuya protocol, using the Tuya apps on your Apple/Android device.
 * Tested using an S5 model of MoeBot (which is identical to an S10 (and S20??) apart from battery size).
@@ -124,7 +125,10 @@
 The following appear to be sub-states for when the mower is in EMERGENCY state.  They are signified by a '103' DPS.
 
 * MOWER_LEAN
 * MOWER_EMERGENCY
 * MOWER_UI_LOCKED
 * PLACE_INSIDE_STATION
 * BATTERY_NOT_ENOUGH
+
+## Internals
+A Facebook user has opened the main case of the MoeBot and taken photos.  Refer to the images captured in the ['internals'](images/internals) folder.
```

### Comparing `pymoebot-0.2.3/README.md` & `pymoebot-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -113,7 +113,10 @@
 The following appear to be sub-states for when the mower is in EMERGENCY state.  They are signified by a '103' DPS.
 
 * MOWER_LEAN
 * MOWER_EMERGENCY
 * MOWER_UI_LOCKED
 * PLACE_INSIDE_STATION
 * BATTERY_NOT_ENOUGH
+
+## Internals
+A Facebook user has opened the main case of the MoeBot and taken photos.  Refer to the images captured in the ['internals'](images/internals) folder.
```

### Comparing `pymoebot-0.2.3/pymoebot.egg-info/PKG-INFO` & `pymoebot-0.3.0/pymoebot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pymoebot
-Version: 0.2.3
+Version: 0.3.0
 Summary: A Python library intended to monitor and control MoeBot robotic lawn mowers.
 Home-page: https://github.com/Whytey/pymoebot
 Author: David Whyte
 Author-email: David@Whyte.xyz
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Requires-Dist: tinytuya
 
 # pymoebot
 
 A Python library intended to monitor (and control?) the [MoeBot](https://moebot.com.au/) robotic lawn mowers.
 
 * MoeBot are controllable over WiFi via the Tuya protocol, using the Tuya apps on your Apple/Android device.
 * Tested using an S5 model of MoeBot (which is identical to an S10 (and S20??) apart from battery size).
@@ -124,7 +125,10 @@
 The following appear to be sub-states for when the mower is in EMERGENCY state.  They are signified by a '103' DPS.
 
 * MOWER_LEAN
 * MOWER_EMERGENCY
 * MOWER_UI_LOCKED
 * PLACE_INSIDE_STATION
 * BATTERY_NOT_ENOUGH
+
+## Internals
+A Facebook user has opened the main case of the MoeBot and taken photos.  Refer to the images captured in the ['internals'](images/internals) folder.
```

### Comparing `pymoebot-0.2.3/setup.py` & `pymoebot-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `pymoebot-0.2.3/test/model_test.py` & `pymoebot-0.3.0/test/model_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from unittest import mock
 
-from pymoebot import MoeBotConnectionError, MoeBot
+from pymoebot import MoeBot
 
 
 class TestMoeBot(unittest.TestCase):
     @mock.patch('tinytuya.Device.status')
     def test_no_device(self, mock_status):
         mock_status.return_value = {'Error': 'Network Error: Device Unreachable', 'Err': '905', 'Payload': None}
 
@@ -16,12 +16,9 @@
     @mock.patch('tinytuya.Device.status')
     def test_mock_device(self, mock_status):
         mock_status.return_value = {
             'dps': {'6': 100, '101': 'STANDBY', '102': 0, '103': 'MOWER_LEAN', '104': True, '105': 3, '106': 1111,
                     '114': 'AutoMode'}}
 
         m = MoeBot("RANDOM", "127.0.0.1", "RANDOM_KEY_ABCDE")
-        self.assertFalse(m.online)
-        self.assertIsNone(m.state)
-        m.poll()
         self.assertTrue(m.online)
-        self.assertIsNotNone(m.state)
+        self.assertIsNotNone(m.state)
```

