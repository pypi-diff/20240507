# Comparing `tmp/xbotext-0.1.2.tar.gz` & `tmp/xbotext-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbotext-0.1.2.tar", max compression
+gzip compressed data, was "xbotext-0.1.3.tar", max compression
```

## Comparing `xbotext-0.1.2.tar` & `xbotext-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-05-07 11:55:00.752903 xbotext-0.1.2/README.md
--rw-r--r--   0        0        0      255 2024-05-07 11:55:00.752903 xbotext-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-07 11:55:00.752903 xbotext-0.1.2/xbotext/__init__.py
--rw-r--r--   0        0        0     3248 2024-05-07 11:55:00.752903 xbotext-0.1.2/xbotext/cache.py
--rw-r--r--   0        0        0      522 2024-05-07 11:55:00.763736 xbotext-0.1.2/xbotext/chromium.py
--rw-r--r--   0        0        0      605 2024-05-07 11:55:00.763736 xbotext-0.1.2/xbotext/regedit.py
--rw-r--r--   0        0        0       20 2024-05-07 11:55:00.763736 xbotext-0.1.2/xbotext/sofaware.py
--rw-r--r--   0        0        0      101 2024-05-07 11:55:00.763736 xbotext-0.1.2/xbotext/system.py
--rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 xbotext-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-07 11:55:00.752903 xbotext-0.1.3/README.md
+-rw-r--r--   0        0        0      255 2024-05-07 12:13:11.059635 xbotext-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-07 11:55:00.752903 xbotext-0.1.3/xbotext/__init__.py
+-rw-r--r--   0        0        0     3336 2024-05-07 12:12:34.225851 xbotext-0.1.3/xbotext/cache.py
+-rw-r--r--   0        0        0      522 2024-05-07 11:55:00.763736 xbotext-0.1.3/xbotext/chromium.py
+-rw-r--r--   0        0        0      605 2024-05-07 11:55:00.763736 xbotext-0.1.3/xbotext/regedit.py
+-rw-r--r--   0        0        0       20 2024-05-07 11:55:00.763736 xbotext-0.1.3/xbotext/sofaware.py
+-rw-r--r--   0        0        0      101 2024-05-07 11:55:00.763736 xbotext-0.1.3/xbotext/system.py
+-rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 xbotext-0.1.3/PKG-INFO
```

### Comparing `xbotext-0.1.2/xbotext/cache.py` & `xbotext-0.1.3/xbotext/cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 
 
 def get_xbot_type():
     """获取机器人类型
     :retrun: app, activity
     """
     stack = inspect.stack()
-    calling_module_frame = stack[1]
-    calling_module_file_path = calling_module_frame.filename
+    for calling_module_frame in stack:
+        if "xbot_robot" in calling_module_frame.filename:
+            calling_module_file_path =  calling_module_frame.filename
+            break
     calling_module_dir, _ = os.path.split(calling_module_file_path)
     package_json_file_path = os.path.join(calling_module_dir, "package.json")
 
     with open(package_json_file_path) as f:
         package_json = json.load(f)
         robot_type = package_json.get("robot_type")
```

### Comparing `xbotext-0.1.2/xbotext/chromium.py` & `xbotext-0.1.3/xbotext/chromium.py`

 * *Files identical despite different names*

### Comparing `xbotext-0.1.2/xbotext/regedit.py` & `xbotext-0.1.3/xbotext/regedit.py`

 * *Files identical despite different names*

