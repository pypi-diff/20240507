# Comparing `tmp/printt-0.1.1.tar.gz` & `tmp/printt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "printt-0.1.1.tar", max compression
+gzip compressed data, was "printt-0.1.2.tar", max compression
```

## Comparing `printt-0.1.1.tar` & `printt-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1881 2024-05-06 08:30:37.348801 printt-0.1.1/README.md
--rw-r--r--   0        0        0      112 2024-05-06 08:27:19.365902 printt-0.1.1/printt/__init__.py
--rw-r--r--   0        0        0     1986 2024-05-06 08:52:28.944680 printt-0.1.1/printt/main.py
--rw-r--r--   0        0        0      344 2024-05-06 08:52:39.682509 printt-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2210 1970-01-01 00:00:00.000000 printt-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1881 2024-05-07 11:32:29.960510 printt-0.1.2/README.md
+-rw-r--r--   0        0        0      112 2024-05-07 11:32:29.960510 printt-0.1.2/printt/__init__.py
+-rw-r--r--   0        0        0     2157 2024-05-07 11:32:29.960510 printt-0.1.2/printt/main.py
+-rw-r--r--   0        0        0      344 2024-05-07 11:32:29.960510 printt-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2261 1970-01-01 00:00:00.000000 printt-0.1.2/PKG-INFO
```

### Comparing `printt-0.1.1/README.md` & `printt-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `printt-0.1.1/printt/main.py` & `printt-0.1.2/printt/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,45 @@
 import sys
-from typing import Any, Callable, Dict, Optional
+from typing import Any, Callable, Dict
 from rich import print as rprint
-
+import inspect
 # Set the default value for PRINT_ENABLED
 PRINT_ENABLED = True
 
-def get_var_name(var: Any) -> Optional[str]:
-    """Get the name of a variable."""
-    for name, val in globals().items():
-        if val is var:
-            return name
-    return None
+
+def get_var_name(var):
+    frame = inspect.currentframe().f_back
+    return [name for name, val in frame.f_locals.items() if val is var][0]
+
 
 def get_human_readable_size(num_bytes: int) -> str:
     """Convert the number of bytes to a human-readable string."""
     units = ['B', 'KB', 'MB', 'GB', 'TB', 'PB']
     unit_index = 0
     size = num_bytes
 
     while size >= 1024 and unit_index < len(units) - 1:
         size /= 1024
         unit_index += 1
 
     return f"{size:.2f} {units[unit_index]}"
 
-
 def get_var_size(x):
     return get_human_readable_size(sys.getsizeof(x))
 
-    
-def printt(x: Any, print_variable: bool = True) -> None:
+def printt(x: Any, print_variable: bool = True, include_methods: bool = False) -> None:
     """Prints details about a variable."""
     global PRINT_ENABLED  # Declare the global variable within the function
 
     if not PRINT_ENABLED:
         return  # Exit the function early if printing is disabled
 
     just_print: Dict[str, Any] = {
         "name": get_var_name(x),
-        "variable": x if print_variable else "print variable is disabled",
+        "value": x if print_variable else "print variable is disabled",
         "class": x.__class__.__name__,
     }
 
     rprint("-" * 60)
     for key, value in just_print.items():
         rprint(f"[bold blue]{key:15} ::[/bold blue] {value}")
     rprint("-" * 60)
@@ -50,24 +47,32 @@
     use_try: Dict[str, Callable] = {
         "type": type,
         "dir": dir,
         "len": len,
         "Memory Usage": get_var_size
     }
 
+    if include_methods:
+        use_try["Methods"] = dir
+
     for key, func in use_try.items():
         try:
-            rprint(f"[bold magenta]{key:15} ::[/bold magenta] {func(x)}")
+            if callable(func):
+                result = func(x)
+            else:
+                result = func
+            rprint(f"[bold magenta]{key:15} ::[/bold magenta] {result}")
             rprint("-" * 60)
         except Exception as e:
             rprint(f"[bold red]{key:15} ::[/bold red] not printed due to {e} !!!")
             rprint("-" * 60)
+            # pass
 
     rprint()
 
 def enable_printt():
     global PRINT_ENABLED
     PRINT_ENABLED = True
 
 def disable_printt():
     global PRINT_ENABLED
-    PRINT_ENABLED = False
+    PRINT_ENABLED = False
```

### Comparing `printt-0.1.1/PKG-INFO` & `printt-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: printt
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: tikendraw
 Author-email: tikendraksahu1029@gmail.com
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Description-Content-Type: text/markdown
 
 # **Printt (Detailed print)**
 
 **Description**
```

