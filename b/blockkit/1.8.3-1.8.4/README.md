# Comparing `tmp/blockkit-1.8.3.tar.gz` & `tmp/blockkit-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockkit-1.8.3.tar", last modified: Wed Mar 20 13:27:31 2024, max compression
+gzip compressed data, was "blockkit-1.8.4.tar", last modified: Tue May  7 11:00:18 2024, max compression
```

## Comparing `blockkit-1.8.3.tar` & `blockkit-1.8.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:27:31.968002 blockkit-1.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-20 13:27:27.000000 blockkit-1.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-20 13:27:27.000000 blockkit-1.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-03-20 13:27:31.964002 blockkit-1.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-03-20 13:27:27.000000 blockkit-1.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:27:31.964002 blockkit-1.8.3/blockkit/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-20 13:27:27.000000 blockkit-1.8.3/blockkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-03-20 13:27:27.000000 blockkit-1.8.3/blockkit/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-03-20 13:27:27.000000 blockkit-1.8.3/blockkit/components.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-20 13:27:27.000000 blockkit-1.8.3/blockkit/display.py
--rw-r--r--   0 runner    (1001) docker     (127)    22902 2024-03-20 13:27:27.000000 blockkit-1.8.3/blockkit/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-20 13:27:27.000000 blockkit-1.8.3/blockkit/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-03-20 13:27:27.000000 blockkit-1.8.3/blockkit/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-03-20 13:27:27.000000 blockkit-1.8.3/blockkit/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-03-20 13:27:27.000000 blockkit-1.8.3/blockkit/surfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-03-20 13:27:27.000000 blockkit-1.8.3/blockkit/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:27:31.964002 blockkit-1.8.3/blockkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-03-20 13:27:31.000000 blockkit-1.8.3/blockkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-20 13:27:31.000000 blockkit-1.8.3/blockkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 13:27:31.000000 blockkit-1.8.3/blockkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-20 13:27:31.000000 blockkit-1.8.3/blockkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-20 13:27:31.000000 blockkit-1.8.3/blockkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 13:27:31.968002 blockkit-1.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-03-20 13:27:27.000000 blockkit-1.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:27:31.964002 blockkit-1.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13378 2024-03-20 13:27:27.000000 blockkit-1.8.3/tests/test_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-03-20 13:27:27.000000 blockkit-1.8.3/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (127)    52104 2024-03-20 13:27:27.000000 blockkit-1.8.3/tests/test_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)    51891 2024-03-20 13:27:27.000000 blockkit-1.8.3/tests/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8591 2024-03-20 13:27:27.000000 blockkit-1.8.3/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     9112 2024-03-20 13:27:27.000000 blockkit-1.8.3/tests/test_surfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:00:18.614948 blockkit-1.8.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-07 11:00:14.000000 blockkit-1.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 11:00:14.000000 blockkit-1.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-07 11:00:18.614948 blockkit-1.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-05-07 11:00:14.000000 blockkit-1.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:00:18.610948 blockkit-1.8.4/blockkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-07 11:00:14.000000 blockkit-1.8.4/blockkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-07 11:00:14.000000 blockkit-1.8.4/blockkit/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-07 11:00:14.000000 blockkit-1.8.4/blockkit/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-07 11:00:14.000000 blockkit-1.8.4/blockkit/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22902 2024-05-07 11:00:14.000000 blockkit-1.8.4/blockkit/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-07 11:00:14.000000 blockkit-1.8.4/blockkit/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-05-07 11:00:14.000000 blockkit-1.8.4/blockkit/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-05-07 11:00:14.000000 blockkit-1.8.4/blockkit/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-05-07 11:00:14.000000 blockkit-1.8.4/blockkit/surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-07 11:00:14.000000 blockkit-1.8.4/blockkit/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:00:18.614948 blockkit-1.8.4/blockkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-07 11:00:18.000000 blockkit-1.8.4/blockkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-07 11:00:18.000000 blockkit-1.8.4/blockkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 11:00:18.000000 blockkit-1.8.4/blockkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 11:00:18.000000 blockkit-1.8.4/blockkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 11:00:18.000000 blockkit-1.8.4/blockkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 11:00:18.614948 blockkit-1.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-07 11:00:14.000000 blockkit-1.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:00:18.614948 blockkit-1.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13379 2024-05-07 11:00:14.000000 blockkit-1.8.4/tests/test_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-07 11:00:14.000000 blockkit-1.8.4/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52104 2024-05-07 11:00:14.000000 blockkit-1.8.4/tests/test_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51891 2024-05-07 11:00:14.000000 blockkit-1.8.4/tests/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8591 2024-05-07 11:00:14.000000 blockkit-1.8.4/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9112 2024-05-07 11:00:14.000000 blockkit-1.8.4/tests/test_surfaces.py
```

### Comparing `blockkit-1.8.3/LICENSE` & `blockkit-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.3/PKG-INFO` & `blockkit-1.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockkit
-Version: 1.8.3
+Version: 1.8.4
 Summary: A fast way to build Block Kit interfaces in Python.
 Home-page: https://github.com/imryche/blockkit
 Author: Dmitry Chernyshov
 Author-email: imryche13@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `blockkit-1.8.3/README.md` & `blockkit-1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.3/blockkit/blocks.py` & `blockkit-1.8.4/blockkit/blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 class Block(Component):
     block_id: Optional[str] = Field(None, min_length=1, max_length=255)
 
 
 class Actions(Block):
     type: str = "actions"
-    elements: List[ActionElement] = Field(..., min_length=1, max_length=5)
+    elements: List[ActionElement] = Field(..., min_length=1, max_length=25)
 
     def __init__(
         self, *, elements: List[ActionElement], block_id: Optional[str] = None
     ):
         super().__init__(elements=elements, block_id=block_id)
 
 
@@ -151,15 +151,15 @@
     MultiConversationsSelect,
     ChannelsSelect,
     MultiChannelsSelect,
     DatePicker,
     DatetimePicker,
     TimePicker,
     NumberInput,
-    FileInput
+    FileInput,
 ]
 
 
 class Input(Block):
     type: str = "input"
     label: Union[PlainText, str]
     element: InputElement
```

### Comparing `blockkit-1.8.3/blockkit/components.py` & `blockkit-1.8.4/blockkit/components.py`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.3/blockkit/display.py` & `blockkit-1.8.4/blockkit/display.py`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.3/blockkit/elements.py` & `blockkit-1.8.4/blockkit/elements.py`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.3/blockkit/generators.py` & `blockkit-1.8.4/blockkit/generators.py`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.3/blockkit/objects.py` & `blockkit-1.8.4/blockkit/objects.py`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.3/blockkit/surfaces.py` & `blockkit-1.8.4/blockkit/surfaces.py`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.3/blockkit/validators.py` & `blockkit-1.8.4/blockkit/validators.py`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.3/blockkit.egg-info/PKG-INFO` & `blockkit-1.8.4/blockkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockkit
-Version: 1.8.3
+Version: 1.8.4
 Summary: A fast way to build Block Kit interfaces in Python.
 Home-page: https://github.com/imryche/blockkit
 Author: Dmitry Chernyshov
 Author-email: imryche13@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `blockkit-1.8.3/blockkit.egg-info/SOURCES.txt` & `blockkit-1.8.4/blockkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.3/setup.py` & `blockkit-1.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Package meta-data.
 NAME = "blockkit"
 DESCRIPTION = "A fast way to build Block Kit interfaces in Python."
 URL = "https://github.com/imryche/blockkit"
 EMAIL = "imryche13@gmail.com"
 AUTHOR = "Dmitry Chernyshov"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "1.8.3"
+VERSION = "1.8.4"
 
 REQUIRED = ["pydantic>=2,<3"]
 EXTRAS = {"gen": ["black"]}
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import the README and use it as the long-description.
```

### Comparing `blockkit-1.8.3/tests/test_blocks.py` & `blockkit-1.8.4/tests/test_blocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 
 def test_actions_excessive_elements_raise_exception():
     with pytest.raises(ValidationError):
         Actions(
             elements=[
                 Button(text=PlainText(text="text"), action_id="action_id")
-                for _ in range(6)
+                for _ in range(26)
             ]
         )
 
 
 def test_builds_context():
     assert Context(
         elements=[
```

### Comparing `blockkit-1.8.3/tests/test_components.py` & `blockkit-1.8.4/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.3/tests/test_elements.py` & `blockkit-1.8.4/tests/test_elements.py`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.3/tests/test_generators.py` & `blockkit-1.8.4/tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.3/tests/test_objects.py` & `blockkit-1.8.4/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.3/tests/test_surfaces.py` & `blockkit-1.8.4/tests/test_surfaces.py`

 * *Files identical despite different names*

