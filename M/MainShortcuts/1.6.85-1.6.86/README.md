# Comparing `tmp/mainshortcuts-1.6.85.tar.gz` & `tmp/mainshortcuts-1.6.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mainshortcuts-1.6.85.tar", max compression
+gzip compressed data, was "mainshortcuts-1.6.86.tar", max compression
```

## Comparing `mainshortcuts-1.6.85.tar` & `mainshortcuts-1.6.86.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rwxr-xr-x   0        0        0     2788 2024-03-02 06:10:12.000000 mainshortcuts-1.6.85/README.md
--rwxr-xr-x   0        0        0      696 2024-05-07 03:14:38.000000 mainshortcuts-1.6.85/pyproject.toml
--rwxr-xr-x   0        0        0     5623 2024-05-07 03:13:52.000000 mainshortcuts-1.6.85/src/MainShortcuts/MainCore.py
--rwxr-xr-x   0        0        0      937 2024-05-07 03:14:32.000000 mainshortcuts-1.6.85/src/MainShortcuts/__init__.py
--rwxr-xr-x   0        0        0      465 2024-04-28 11:33:14.000000 mainshortcuts-1.6.85/src/MainShortcuts/addon.py
--rwxr-xr-x   0        0        0     4960 2024-05-06 14:36:10.000000 mainshortcuts-1.6.85/src/MainShortcuts/cfg.py
--rwxr-xr-x   0        0        0     1003 2024-05-01 01:56:58.000000 mainshortcuts-1.6.85/src/MainShortcuts/dict.py
--rwxr-xr-x   0        0        0     1472 2024-04-28 11:59:24.000000 mainshortcuts-1.6.85/src/MainShortcuts/dictplus.py
--rwxr-xr-x   0        0        0     3345 2024-04-28 12:07:16.000000 mainshortcuts-1.6.85/src/MainShortcuts/dir.py
--rwxr-xr-x   0        0        0     2923 2024-04-28 12:09:32.000000 mainshortcuts-1.6.85/src/MainShortcuts/file.py
--rwxr-xr-x   0        0        0     5925 2024-04-28 12:17:10.000000 mainshortcuts-1.6.85/src/MainShortcuts/fileobj.py
--rwxr-xr-x   0        0        0     2672 2024-05-07 03:14:39.000000 mainshortcuts-1.6.85/src/MainShortcuts/imports.py
--rwxr-xr-x   0        0        0     3603 2024-04-28 12:27:24.000000 mainshortcuts-1.6.85/src/MainShortcuts/json.py
--rwxr-xr-x   0        0        0     2174 2024-04-28 12:29:34.000000 mainshortcuts-1.6.85/src/MainShortcuts/list.py
--rwxr-xr-x   0        0        0     1040 2024-03-21 02:56:48.000000 mainshortcuts-1.6.85/src/MainShortcuts/main.py
--rwxr-xr-x   0        0        0       86 2024-01-17 08:34:46.000000 mainshortcuts-1.6.85/src/MainShortcuts/os.py
--rwxr-xr-x   0        0        0     6265 2024-04-28 12:35:16.000000 mainshortcuts-1.6.85/src/MainShortcuts/path.py
--rwxr-xr-x   0        0        0      789 2024-04-28 12:36:52.000000 mainshortcuts-1.6.85/src/MainShortcuts/proc.py
--rwxr-xr-x   0        0        0     1428 2024-03-27 04:45:04.000000 mainshortcuts-1.6.85/src/MainShortcuts/script.py
--rwxr-xr-x   0        0        0      983 2024-04-28 12:40:04.000000 mainshortcuts-1.6.85/src/MainShortcuts/str.py
--rwxr-xr-x   0        0        0    14818 2024-04-28 12:41:38.000000 mainshortcuts-1.6.85/src/MainShortcuts/values.py
--rwxr-xr-x   0        0        0     1194 2024-04-26 04:58:06.000000 mainshortcuts-1.6.85/src/MainShortcuts/win.py
--rw-r--r--   0        0        0     3510 1970-01-01 00:00:00.000000 mainshortcuts-1.6.85/PKG-INFO
+-rwxr-xr-x   0        0        0     2788 2024-03-02 06:10:12.000000 mainshortcuts-1.6.86/README.md
+-rwxr-xr-x   0        0        0      696 2024-05-07 03:20:06.000000 mainshortcuts-1.6.86/pyproject.toml
+-rwxr-xr-x   0        0        0     5677 2024-05-07 03:19:44.000000 mainshortcuts-1.6.86/src/MainShortcuts/MainCore.py
+-rwxr-xr-x   0        0        0      937 2024-05-07 03:20:00.000000 mainshortcuts-1.6.86/src/MainShortcuts/__init__.py
+-rwxr-xr-x   0        0        0      465 2024-04-28 11:33:14.000000 mainshortcuts-1.6.86/src/MainShortcuts/addon.py
+-rwxr-xr-x   0        0        0     4960 2024-05-06 14:36:10.000000 mainshortcuts-1.6.86/src/MainShortcuts/cfg.py
+-rwxr-xr-x   0        0        0     1003 2024-05-01 01:56:58.000000 mainshortcuts-1.6.86/src/MainShortcuts/dict.py
+-rwxr-xr-x   0        0        0     1472 2024-04-28 11:59:24.000000 mainshortcuts-1.6.86/src/MainShortcuts/dictplus.py
+-rwxr-xr-x   0        0        0     3345 2024-04-28 12:07:16.000000 mainshortcuts-1.6.86/src/MainShortcuts/dir.py
+-rwxr-xr-x   0        0        0     2923 2024-04-28 12:09:32.000000 mainshortcuts-1.6.86/src/MainShortcuts/file.py
+-rwxr-xr-x   0        0        0     5925 2024-04-28 12:17:10.000000 mainshortcuts-1.6.86/src/MainShortcuts/fileobj.py
+-rwxr-xr-x   0        0        0     2672 2024-05-07 03:20:07.000000 mainshortcuts-1.6.86/src/MainShortcuts/imports.py
+-rwxr-xr-x   0        0        0     3603 2024-04-28 12:27:24.000000 mainshortcuts-1.6.86/src/MainShortcuts/json.py
+-rwxr-xr-x   0        0        0     2174 2024-04-28 12:29:34.000000 mainshortcuts-1.6.86/src/MainShortcuts/list.py
+-rwxr-xr-x   0        0        0     1040 2024-03-21 02:56:48.000000 mainshortcuts-1.6.86/src/MainShortcuts/main.py
+-rwxr-xr-x   0        0        0       86 2024-01-17 08:34:46.000000 mainshortcuts-1.6.86/src/MainShortcuts/os.py
+-rwxr-xr-x   0        0        0     6265 2024-04-28 12:35:16.000000 mainshortcuts-1.6.86/src/MainShortcuts/path.py
+-rwxr-xr-x   0        0        0      789 2024-04-28 12:36:52.000000 mainshortcuts-1.6.86/src/MainShortcuts/proc.py
+-rwxr-xr-x   0        0        0     1428 2024-03-27 04:45:04.000000 mainshortcuts-1.6.86/src/MainShortcuts/script.py
+-rwxr-xr-x   0        0        0      983 2024-04-28 12:40:04.000000 mainshortcuts-1.6.86/src/MainShortcuts/str.py
+-rwxr-xr-x   0        0        0    14818 2024-04-28 12:41:38.000000 mainshortcuts-1.6.86/src/MainShortcuts/values.py
+-rwxr-xr-x   0        0        0     1194 2024-04-26 04:58:06.000000 mainshortcuts-1.6.86/src/MainShortcuts/win.py
+-rw-r--r--   0        0        0     3510 1970-01-01 00:00:00.000000 mainshortcuts-1.6.86/PKG-INFO
```

### Comparing `mainshortcuts-1.6.85/README.md` & `mainshortcuts-1.6.86/README.md`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.85/pyproject.toml` & `mainshortcuts-1.6.86/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.poetry]
-version = "1.6.85"
+version = "1.6.86"
 name = "MainShortcuts"
 description = "Simplifying Python Built-in Commands"
 authors = [ "MainPlay TG <xbox.roman6666666666@gmail.com>",]
 readme = "README.md"
 repository = "https://github.com/MainPlay-TG/MainShortcuts.py"
 packages = [
     { include = "MainShortcuts", from = "src" },
```

### Comparing `mainshortcuts-1.6.85/src/MainShortcuts/MainCore.py` & `mainshortcuts-1.6.86/src/MainShortcuts/MainCore.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
       pass
     self.exception=traceback.format_exc # Получить traceback в виде текста
     self.pid=os.getpid() # PID программы
     self.run=__name__=="__main__" # Запущена программа или её импортируют?
     self.embed=dictplus()
     self.embed.lines=[
       "from MainShortcuts.MainCore import *",
+      "from MainShortcuts.MainCore import _MainCore",
       "mcore=_MainCore(__name__=__name__,__file__=__file__)",
       "cprint,cformat=mcore.cprint,mcore.cformat",
       "globals=dictplus()",
       'cfg=ms.cfg(mcore.execdir+"/cfg.json")',
       "cfg.default={}",
       "cfg.dload()",
       ]
```

### Comparing `mainshortcuts-1.6.85/src/MainShortcuts/__init__.py` & `mainshortcuts-1.6.86/src/MainShortcuts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """MainShortcuts - \u043D\u0435\u0431\u043E\u043B\u044C\u0448\u0430\u044F \u0431\u0438\u0431\u043B\u0438\u043E\u0442\u0435\u043A\u0430 \u0434\u043B\u044F \u0443\u043F\u0440\u043E\u0449\u0435\u043D\u0438\u044F \u043D\u0430\u043F\u0438\u0441\u0430\u043D\u0438\u044F \u043A\u043E\u0434\u0430
 \u0420\u0430\u0437\u0440\u0430\u0431\u043E\u0442\u0447\u0438\u043A: MainPlay TG
 https://t.me/MainPlay_InfoCh"""
 
-__version_tuple__=(1,6,85)
+__version_tuple__=(1,6,86)
 __depends__={
   "required":[
     "json",
     "os",
     "platform",
     "shutil",
     "subprocess",
```

### Comparing `mainshortcuts-1.6.85/src/MainShortcuts/cfg.py` & `mainshortcuts-1.6.86/src/MainShortcuts/cfg.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.85/src/MainShortcuts/dict.py` & `mainshortcuts-1.6.86/src/MainShortcuts/dict.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.85/src/MainShortcuts/dictplus.py` & `mainshortcuts-1.6.86/src/MainShortcuts/dictplus.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.85/src/MainShortcuts/dir.py` & `mainshortcuts-1.6.86/src/MainShortcuts/dir.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.85/src/MainShortcuts/file.py` & `mainshortcuts-1.6.86/src/MainShortcuts/file.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.85/src/MainShortcuts/fileobj.py` & `mainshortcuts-1.6.86/src/MainShortcuts/fileobj.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.85/src/MainShortcuts/imports.py` & `mainshortcuts-1.6.86/src/MainShortcuts/imports.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.85/src/MainShortcuts/json.py` & `mainshortcuts-1.6.86/src/MainShortcuts/json.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.85/src/MainShortcuts/list.py` & `mainshortcuts-1.6.86/src/MainShortcuts/list.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.85/src/MainShortcuts/main.py` & `mainshortcuts-1.6.86/src/MainShortcuts/main.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.85/src/MainShortcuts/path.py` & `mainshortcuts-1.6.86/src/MainShortcuts/path.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.85/src/MainShortcuts/proc.py` & `mainshortcuts-1.6.86/src/MainShortcuts/proc.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.85/src/MainShortcuts/script.py` & `mainshortcuts-1.6.86/src/MainShortcuts/script.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.85/src/MainShortcuts/str.py` & `mainshortcuts-1.6.86/src/MainShortcuts/str.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.85/src/MainShortcuts/values.py` & `mainshortcuts-1.6.86/src/MainShortcuts/values.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.85/src/MainShortcuts/win.py` & `mainshortcuts-1.6.86/src/MainShortcuts/win.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.85/PKG-INFO` & `mainshortcuts-1.6.86/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MainShortcuts
-Version: 1.6.85
+Version: 1.6.86
 Summary: Simplifying Python Built-in Commands
 Home-page: https://github.com/MainPlay-TG/MainShortcuts.py
 Author: MainPlay TG
 Author-email: xbox.roman6666666666@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

