# Comparing `tmp/eastmoneypy-0.1.5.tar.gz` & `tmp/eastmoneypy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eastmoneypy-0.1.5.tar", last modified: Sat Apr 27 15:02:55 2024, max compression
+gzip compressed data, was "eastmoneypy-0.1.6.tar", last modified: Tue May  7 14:29:38 2024, max compression
```

## Comparing `eastmoneypy-0.1.5.tar` & `eastmoneypy-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:02:55.818216 eastmoneypy-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-27 15:02:49.000000 eastmoneypy-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-27 15:02:49.000000 eastmoneypy-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-27 15:02:55.818216 eastmoneypy-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-27 15:02:49.000000 eastmoneypy-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:02:55.818216 eastmoneypy-0.1.5/eastmoneypy/
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-27 15:02:49.000000 eastmoneypy-0.1.5/eastmoneypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-04-27 15:02:49.000000 eastmoneypy-0.1.5/eastmoneypy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-27 15:02:49.000000 eastmoneypy-0.1.5/eastmoneypy/config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:02:55.818216 eastmoneypy-0.1.5/eastmoneypy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-27 15:02:55.000000 eastmoneypy-0.1.5/eastmoneypy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-27 15:02:55.000000 eastmoneypy-0.1.5/eastmoneypy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 15:02:55.000000 eastmoneypy-0.1.5/eastmoneypy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-27 15:02:55.000000 eastmoneypy-0.1.5/eastmoneypy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-27 15:02:55.000000 eastmoneypy-0.1.5/eastmoneypy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 15:02:55.818216 eastmoneypy-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-04-27 15:02:49.000000 eastmoneypy-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:02:55.818216 eastmoneypy-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-27 15:02:49.000000 eastmoneypy-0.1.5/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:29:38.216158 eastmoneypy-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-07 14:29:34.000000 eastmoneypy-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-07 14:29:34.000000 eastmoneypy-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-07 14:29:38.212158 eastmoneypy-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-07 14:29:34.000000 eastmoneypy-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:29:38.212158 eastmoneypy-0.1.6/eastmoneypy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-07 14:29:34.000000 eastmoneypy-0.1.6/eastmoneypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-05-07 14:29:34.000000 eastmoneypy-0.1.6/eastmoneypy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 14:29:34.000000 eastmoneypy-0.1.6/eastmoneypy/config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:29:38.212158 eastmoneypy-0.1.6/eastmoneypy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-07 14:29:38.000000 eastmoneypy-0.1.6/eastmoneypy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-07 14:29:38.000000 eastmoneypy-0.1.6/eastmoneypy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:29:38.000000 eastmoneypy-0.1.6/eastmoneypy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 14:29:38.000000 eastmoneypy-0.1.6/eastmoneypy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 14:29:38.000000 eastmoneypy-0.1.6/eastmoneypy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:29:38.216158 eastmoneypy-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-05-07 14:29:34.000000 eastmoneypy-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:29:38.212158 eastmoneypy-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 14:29:34.000000 eastmoneypy-0.1.6/tests/test_api.py
```

### Comparing `eastmoneypy-0.1.5/LICENSE` & `eastmoneypy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `eastmoneypy-0.1.5/PKG-INFO` & `eastmoneypy-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eastmoneypy
-Version: 0.1.5
+Version: 0.1.6
 Summary: python lib for operating eastmoney
 Home-page: https://github.com/zvtvz/eastmoneypy
 Author: foolcage
 Author-email: 5533061@qq.com
 Project-URL: Bug Reports, https://github.com/zvtvz/eastmoneypy/issues
 Project-URL: Funding, https://www.foolcage.com
 Project-URL: Say Thanks!, https://saythanks.io/to/foolcage
```

### Comparing `eastmoneypy-0.1.5/README.md` & `eastmoneypy-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `eastmoneypy-0.1.5/eastmoneypy/__init__.py` & `eastmoneypy-0.1.6/eastmoneypy/__init__.py`

 * *Files identical despite different names*

### Comparing `eastmoneypy-0.1.5/eastmoneypy/api.py` & `eastmoneypy-0.1.6/eastmoneypy/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     lines = src.split("\n")
     header = {}
     if lines:
         for line in lines:
             try:
                 index = line.index(":")
                 key = line[:index]
-                value = line[index + 1 :]
+                value = line[index + 1:]
                 if key and value:
                     header.setdefault(key.strip(), value.strip())
             except Exception:
                 pass
     return header
 
 
@@ -40,15 +40,15 @@
         raise Exception(f"code:{resp.status_code},msg:{resp.content}")
     # {
     #   "re": true,
     #   "message": "",
     #   "result": {}
     # }
     result = resp.text
-    js_text = result[result.index("(") + 1 : result.index(")")]
+    js_text = result[result.index("(") + 1: result.index(")")]
 
     ret = demjson3.decode(js_text)
     logger.info(f"ret:{ret}")
     data = ret.get("data")
     if data and key:
         result_value = data.get(key)
     else:
@@ -112,16 +112,16 @@
     else:
         resp = requests.get(url, headers=HEADER)
 
     ret, _ = parse_resp(resp, key=None)
     return ret
 
 
-def get_group_id(group_name):
-    groups = get_groups()
+def get_group_id(group_name, session=None):
+    groups = get_groups(session=session)
     groups = [group for group in groups if group["gname"] == group_name]
     if groups:
         return groups[0]["gid"]
     return None
 
 
 def list_entities(group_name=None, group_id=None, session: Session = None):
@@ -140,15 +140,15 @@
 
     _, result = parse_resp(resp)
     datas = result["stkinfolist"]
     return [data["security"].split("$")[1] for data in datas]
 
 
 def add_to_group(
-    code, entity_type="stock", group_name=None, group_id=None, session: Session = None
+        code, entity_type="stock", group_name=None, group_id=None, session: Session = None
 ):
     if not group_id:
         assert group_name is not None
         group_id = get_group_id(group_name)
         if not group_id:
             raise Exception(f"could not find group:{group_name}")
     code = to_eastmoney_code(code, entity_type=entity_type)
```

### Comparing `eastmoneypy-0.1.5/eastmoneypy.egg-info/PKG-INFO` & `eastmoneypy-0.1.6/eastmoneypy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eastmoneypy
-Version: 0.1.5
+Version: 0.1.6
 Summary: python lib for operating eastmoney
 Home-page: https://github.com/zvtvz/eastmoneypy
 Author: foolcage
 Author-email: 5533061@qq.com
 Project-URL: Bug Reports, https://github.com/zvtvz/eastmoneypy/issues
 Project-URL: Funding, https://www.foolcage.com
 Project-URL: Say Thanks!, https://saythanks.io/to/foolcage
```

### Comparing `eastmoneypy-0.1.5/setup.py` & `eastmoneypy-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.1.5',  # Required
+    version='0.1.6',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='python lib for operating eastmoney',  # Required
 
     # This is an optional longer description of your project that represents
```

