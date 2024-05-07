# Comparing `tmp/aistudio_cognition-3.5.0.1.tar.gz` & `tmp/aistudio_cognition-3.5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aistudio_cognition-3.5.0.1.tar", max compression
+gzip compressed data, was "aistudio_cognition-3.5.0.2.tar", max compression
```

## Comparing `aistudio_cognition-3.5.0.1.tar` & `aistudio_cognition-3.5.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    16129 2024-05-03 11:55:58.409004 aistudio_cognition-3.5.0.1/aistudio_cognition/cognibot/models.py
--rw-r--r--   0        0        0       46 2024-03-15 08:14:34.225844 aistudio_cognition-3.5.0.1/aistudio_cognition/models/__init__.py
--rw-r--r--   0        0        0      141 2024-03-15 08:14:34.225844 aistudio_cognition-3.5.0.1/aistudio_cognition/models/response_status.py
--rw-r--r--   0        0        0       82 2024-03-15 08:14:34.225844 aistudio_cognition-3.5.0.1/aistudio_cognition/nlu/luis/__init__.py
--rw-r--r--   0        0        0     7059 2024-03-15 08:14:34.225844 aistudio_cognition-3.5.0.1/aistudio_cognition/nlu/luis/luis.py
--rw-r--r--   0        0        0       47 2024-03-15 08:14:34.225844 aistudio_cognition-3.5.0.1/aistudio_cognition/nlu/luis/models/__init__.py
--rw-r--r--   0        0        0      467 2024-03-15 08:14:34.225844 aistudio_cognition-3.5.0.1/aistudio_cognition/nlu/luis/models/luis_settings.py
--rw-r--r--   0        0        0     2830 2024-03-15 08:14:34.225844 aistudio_cognition-3.5.0.1/aistudio_cognition/nlu/luis/prediction.py
--rw-r--r--   0        0        0     5207 2024-03-15 08:14:34.225844 aistudio_cognition-3.5.0.1/aistudio_cognition/nlu/luis/rule.py
--rw-r--r--   0        0        0      674 2024-03-15 08:14:34.225844 aistudio_cognition-3.5.0.1/aistudio_cognition/nlu/models.py
--rw-r--r--   0        0        0      357 2024-05-03 11:55:58.409004 aistudio_cognition-3.5.0.1/pyproject.toml
--rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 aistudio_cognition-3.5.0.1/PKG-INFO
+-rw-r--r--   0        0        0    16148 2024-05-07 11:02:37.284458 aistudio_cognition-3.5.0.2/aistudio_cognition/cognibot/models.py
+-rw-r--r--   0        0        0       46 2024-05-06 11:33:00.390232 aistudio_cognition-3.5.0.2/aistudio_cognition/models/__init__.py
+-rw-r--r--   0        0        0      141 2024-05-06 11:33:00.390232 aistudio_cognition-3.5.0.2/aistudio_cognition/models/response_status.py
+-rw-r--r--   0        0        0       82 2024-05-06 11:33:00.390232 aistudio_cognition-3.5.0.2/aistudio_cognition/nlu/luis/__init__.py
+-rw-r--r--   0        0        0     7059 2024-05-06 11:33:00.390232 aistudio_cognition-3.5.0.2/aistudio_cognition/nlu/luis/luis.py
+-rw-r--r--   0        0        0       47 2024-05-06 11:33:00.390232 aistudio_cognition-3.5.0.2/aistudio_cognition/nlu/luis/models/__init__.py
+-rw-r--r--   0        0        0      467 2024-05-06 11:33:00.390232 aistudio_cognition-3.5.0.2/aistudio_cognition/nlu/luis/models/luis_settings.py
+-rw-r--r--   0        0        0     2830 2024-05-06 11:33:00.390232 aistudio_cognition-3.5.0.2/aistudio_cognition/nlu/luis/prediction.py
+-rw-r--r--   0        0        0     5207 2024-05-06 11:33:00.390232 aistudio_cognition-3.5.0.2/aistudio_cognition/nlu/luis/rule.py
+-rw-r--r--   0        0        0      674 2024-05-06 11:33:00.390232 aistudio_cognition-3.5.0.2/aistudio_cognition/nlu/models.py
+-rw-r--r--   0        0        0      357 2024-05-07 11:02:37.284458 aistudio_cognition-3.5.0.2/pyproject.toml
+-rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 aistudio_cognition-3.5.0.2/PKG-INFO
```

### Comparing `aistudio_cognition-3.5.0.1/aistudio_cognition/cognibot/models.py` & `aistudio_cognition-3.5.0.2/aistudio_cognition/cognibot/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -656,14 +656,15 @@
 
 @dataclass_json
 @dataclass
 class Cognibot:
     cognibot_settings: CognibotSettings
     version: str
     skills: list[Skill]
+    ae_app_id: str
     connections: list[Connection] = field(default_factory=list)
     credentials: list[Credential] = field(default_factory=list)
     nlu_settings: list[AIStudioNLU] = field(default_factory=list)
     schedules: list[Schedule] = field(default_factory=list)
 
 
 @dataclass_json
```

### Comparing `aistudio_cognition-3.5.0.1/aistudio_cognition/nlu/luis/luis.py` & `aistudio_cognition-3.5.0.2/aistudio_cognition/nlu/luis/luis.py`

 * *Files identical despite different names*

### Comparing `aistudio_cognition-3.5.0.1/aistudio_cognition/nlu/luis/prediction.py` & `aistudio_cognition-3.5.0.2/aistudio_cognition/nlu/luis/prediction.py`

 * *Files identical despite different names*

### Comparing `aistudio_cognition-3.5.0.1/aistudio_cognition/nlu/luis/rule.py` & `aistudio_cognition-3.5.0.2/aistudio_cognition/nlu/luis/rule.py`

 * *Files identical despite different names*

### Comparing `aistudio_cognition-3.5.0.1/aistudio_cognition/nlu/models.py` & `aistudio_cognition-3.5.0.2/aistudio_cognition/nlu/models.py`

 * *Files identical despite different names*

### Comparing `aistudio_cognition-3.5.0.1/PKG-INFO` & `aistudio_cognition-3.5.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aistudio-cognition
-Version: 3.5.0.1
+Version: 3.5.0.2
 Summary: NLU and KM prediction utility for AIStudio
 Author: Ankita Nair
 Author-email: ankita.nair@automationedge.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

