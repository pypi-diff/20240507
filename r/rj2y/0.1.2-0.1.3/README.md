# Comparing `tmp/rj2y-0.1.2.tar.gz` & `tmp/rj2y-0.1.3.tar.gz`

## Comparing `rj2y-0.1.2.tar` & `rj2y-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 rj2y-0.1.2/.python-version
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 rj2y-0.1.2/Makefile
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 rj2y-0.1.2/requirements-dev.lock
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 rj2y-0.1.2/requirements.lock
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 rj2y-0.1.2/tmp.json
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 rj2y-0.1.2/tmp.yaml
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 rj2y-0.1.2/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rj2y-0.1.2/src/rj2y/__init__.py
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 rj2y-0.1.2/src/rj2y/main.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 rj2y-0.1.2/tests/unittest/test_main.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 rj2y-0.1.2/.gitignore
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 rj2y-0.1.2/README.md
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 rj2y-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 rj2y-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 rj2y-0.1.3/.python-version
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 rj2y-0.1.3/Makefile
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 rj2y-0.1.3/requirements-dev.lock
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 rj2y-0.1.3/requirements.lock
+-rw-r--r--   0        0        0    88550 2020-02-02 00:00:00.000000 rj2y-0.1.3/tmp.json
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 rj2y-0.1.3/tmp.yaml
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 rj2y-0.1.3/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rj2y-0.1.3/src/rj2y/__init__.py
+-rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 rj2y-0.1.3/src/rj2y/main.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 rj2y-0.1.3/tests/unittest/test_main.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 rj2y-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 rj2y-0.1.3/README.md
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 rj2y-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 rj2y-0.1.3/PKG-INFO
```

### Comparing `rj2y-0.1.2/tmp.yaml` & `rj2y-0.1.3/tmp.yaml`

 * *Files identical despite different names*

### Comparing `rj2y-0.1.2/src/rj2y/main.py` & `rj2y-0.1.3/src/rj2y/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,26 @@
         return None
 
     @abstractmethod
     def dump(self) -> str:
         pass
 
 
+class NullYamlNode(YamlNode):
+    def __init__(self, value: None):
+        self.value = value
+
+    @property
+    def tag(self) -> str:
+        return ""
+
+    def dump(self) -> str:
+        return "null"
+
+
 class StrYamlNode(YamlNode):
     def __init__(self, value: str):
         self.value = value
 
     @property
     def tag(self) -> str:
         if len(self.value.split("\n")) > 1:
@@ -138,14 +150,16 @@
             return MappingYamlNode.parse(decoded_json)
         elif isinstance(decoded_json, list):
             return ListYamlNode.parse(decoded_json)
     return StrYamlNode(obj)
 
 
 def parse_to_yaml_node(v: YamlGeneralValueType) -> YamlNode:
+    if v is None:
+        return NullYamlNode(v)
     if isinstance(v, str):
         return parse_embedded_json_string(v)
     if isinstance(v, bool):  # note: bool should be checked before int because bool is a subclass of int
         return BoolYamlNode(v)
     if isinstance(v, int):
         return IntYamlNode(v)
     if isinstance(v, float):
```

### Comparing `rj2y-0.1.2/tests/unittest/test_main.py` & `rj2y-0.1.3/tests/unittest/test_main.py`

 * *Files identical despite different names*

### Comparing `rj2y-0.1.2/README.md` & `rj2y-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,34 @@
 
 [![PyPI](https://img.shields.io/pypi/v/rj2y)](https://pypi.org/project/rj2y/)
 [![PyPI Python Versions](https://img.shields.io/pypi/pyversions/rj2y)](https://pypi.org/project/rj2y/)
 [![Downloads](https://pepy.tech/badge/rj2y)](https://pepy.tech/project/rj2y)
 
 This CLI tool is a simple utility to convert JSON to YAML. Especially useful when you want to convert JSON including JSON-embedded string.
 
+```json
+{
+  "iii": "{\"i\":\"{\\\"ii\\\": \\\"ii\\\"}\",\"ii\":\"ii\"}",
+  "kkk": "{\"k\": \"{\\\"kk\\\": \\\"kk1\\\\nkk2\\\\nkk3\\\\n\\\"}\"}"
+}
+```
+
+```yaml
+iii:
+  i:
+    ii: !!str ii
+  ii: !!str ii
+kkk:
+  k:
+    kk: !!str |-
+      kk1
+      kk2
+      kk3
+```
+
 It may be convenient to reading server logs. Using with [`jq`](https://github.com/jqlang/jq) and [`yq`](https://github.com/mikefarah/yq) is recommended.
 
 ## Installation
 
 ```bash
 pipx install rj2y
 ```
```

### Comparing `rj2y-0.1.2/pyproject.toml` & `rj2y-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rj2y"
-version = "0.1.2"
+version = "0.1.3"
 description = "Recursively convert JSON including json-string to YAML"
 authors = [{ name = "pollenjp", email = "polleninjp@gmail.com" }]
 dependencies = ["click>=8.1.7"]
 readme = "README.md"
 requires-python = ">= 3.10"
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `rj2y-0.1.2/PKG-INFO` & `rj2y-0.1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rj2y
-Version: 0.1.2
+Version: 0.1.3
 Summary: Recursively convert JSON including json-string to YAML
 Project-URL: Homepage, https://github.com/pollenjp/rj2y-py
 Project-URL: Repository, https://github.com/pollenjp/rj2y-py
 Author-email: pollenjp <polleninjp@gmail.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -18,14 +18,34 @@
 
 [![PyPI](https://img.shields.io/pypi/v/rj2y)](https://pypi.org/project/rj2y/)
 [![PyPI Python Versions](https://img.shields.io/pypi/pyversions/rj2y)](https://pypi.org/project/rj2y/)
 [![Downloads](https://pepy.tech/badge/rj2y)](https://pepy.tech/project/rj2y)
 
 This CLI tool is a simple utility to convert JSON to YAML. Especially useful when you want to convert JSON including JSON-embedded string.
 
+```json
+{
+  "iii": "{\"i\":\"{\\\"ii\\\": \\\"ii\\\"}\",\"ii\":\"ii\"}",
+  "kkk": "{\"k\": \"{\\\"kk\\\": \\\"kk1\\\\nkk2\\\\nkk3\\\\n\\\"}\"}"
+}
+```
+
+```yaml
+iii:
+  i:
+    ii: !!str ii
+  ii: !!str ii
+kkk:
+  k:
+    kk: !!str |-
+      kk1
+      kk2
+      kk3
+```
+
 It may be convenient to reading server logs. Using with [`jq`](https://github.com/jqlang/jq) and [`yq`](https://github.com/mikefarah/yq) is recommended.
 
 ## Installation
 
 ```bash
 pipx install rj2y
 ```
```

