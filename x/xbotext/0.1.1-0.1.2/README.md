# Comparing `tmp/xbotext-0.1.1.tar.gz` & `tmp/xbotext-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbotext-0.1.1.tar", max compression
+gzip compressed data, was "xbotext-0.1.2.tar", max compression
```

## Comparing `xbotext-0.1.1.tar` & `xbotext-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0      269 2023-10-24 07:52:35.639133 xbotext-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-09-20 04:52:09.471482 xbotext-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-09-20 04:52:09.470987 xbotext-0.1.1/xbotext/__init__.py
--rw-r--r--   0        0        0      617 2023-10-24 07:50:46.828602 xbotext-0.1.1/xbotext/sys.py
--rw-r--r--   0        0        0       30 2023-09-20 05:00:48.158777 xbotext-0.1.1/xbotext/utils.py
--rw-r--r--   0        0        0      193 2023-09-20 05:08:02.686782 xbotext-0.1.1/xbotext/validators.py
--rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 xbotext-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-07 11:55:00.752903 xbotext-0.1.2/README.md
+-rw-r--r--   0        0        0      255 2024-05-07 11:55:00.752903 xbotext-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-07 11:55:00.752903 xbotext-0.1.2/xbotext/__init__.py
+-rw-r--r--   0        0        0     3248 2024-05-07 11:55:00.752903 xbotext-0.1.2/xbotext/cache.py
+-rw-r--r--   0        0        0      522 2024-05-07 11:55:00.763736 xbotext-0.1.2/xbotext/chromium.py
+-rw-r--r--   0        0        0      605 2024-05-07 11:55:00.763736 xbotext-0.1.2/xbotext/regedit.py
+-rw-r--r--   0        0        0       20 2024-05-07 11:55:00.763736 xbotext-0.1.2/xbotext/sofaware.py
+-rw-r--r--   0        0        0      101 2024-05-07 11:55:00.763736 xbotext-0.1.2/xbotext/system.py
+-rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 xbotext-0.1.2/PKG-INFO
```

### Comparing `xbotext-0.1.1/xbotext/sys.py` & `xbotext-0.1.2/xbotext/regedit.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-import winreg
-
-
-def is_show_file_ext():
-    """检查是否显示文件扩展名"""
-    key = winreg.OpenKey(winreg.HKEY_CURRENT_USER, 'Software\\Microsoft\\Windows\\CurrentVersion\\Explorer\\Advanced')
-    value, _ = winreg.QueryValueEx(key, 'HideFileExt')
-    winreg.CloseKey(key)
-    return value == 0
-
-
-def set_show_file_ext():
-    """设置显示文件扩展名"""
-    key = winreg.OpenKey(winreg.HKEY_CURRENT_USER, 'Software\\Microsoft\\Windows\\CurrentVersion\\Explorer\\Advanced', 0, winreg.KEY_WRITE)
-    winreg.SetValueEx(key, 'HideFileExt', 0, winreg.REG_DWORD, 0)
-    winreg.CloseKey(key)
+import winreg
+
+
+def is_show_file_ext():
+    """检查是否显示文件扩展名"""
+    key = winreg.OpenKey(winreg.HKEY_CURRENT_USER, 'Software\\Microsoft\\Windows\\CurrentVersion\\Explorer\\Advanced')
+    value, _ = winreg.QueryValueEx(key, 'HideFileExt')
+    winreg.CloseKey(key)
+    return value == 0
+
+
+def set_show_file_ext():
+    """设置显示文件扩展名"""
+    key = winreg.OpenKey(winreg.HKEY_CURRENT_USER, 'Software\\Microsoft\\Windows\\CurrentVersion\\Explorer\\Advanced', 0, winreg.KEY_WRITE)
+    winreg.SetValueEx(key, 'HideFileExt', 0, winreg.REG_DWORD, 0)
+    winreg.CloseKey(key)
+
+
+
+
```

