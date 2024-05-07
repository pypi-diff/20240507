# Comparing `tmp/gmo_fx-0.1.0.tar.gz` & `tmp/gmo_fx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmo_fx-0.1.0.tar", last modified: Tue May  7 10:10:26 2024, max compression
+gzip compressed data, was "gmo_fx-0.1.1.tar", last modified: Tue May  7 13:18:20 2024, max compression
```

## Comparing `gmo_fx-0.1.0.tar` & `gmo_fx-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0 r_noto    (1000) r_noto    (1000)        0 2024-05-07 10:10:26.597654 gmo_fx-0.1.0/
--rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     1067 2024-04-26 12:41:11.000000 gmo_fx-0.1.0/LICENSE
--rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     1086 2024-05-07 10:10:26.593653 gmo_fx-0.1.0/PKG-INFO
--rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)      719 2024-05-07 10:05:52.000000 gmo_fx-0.1.0/README.md
-drwxrwxrwx   0 r_noto    (1000) r_noto    (1000)        0 2024-05-07 10:10:26.474622 gmo_fx-0.1.0/gmo_fx/
--rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)      135 2024-05-06 12:10:47.000000 gmo_fx-0.1.0/gmo_fx/__init__.py
--rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     7751 2024-04-29 11:27:04.000000 gmo_fx-0.1.0/gmo_fx/errors.py
--rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     2114 2024-05-03 13:02:15.000000 gmo_fx-0.1.0/gmo_fx/klines.py
--rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)      566 2024-04-29 11:27:04.000000 gmo_fx-0.1.0/gmo_fx/response.py
--rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     1314 2024-05-03 13:02:15.000000 gmo_fx-0.1.0/gmo_fx/status.py
--rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     1623 2024-05-04 04:15:36.000000 gmo_fx-0.1.0/gmo_fx/symbols.py
--rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     1260 2024-05-03 13:02:15.000000 gmo_fx-0.1.0/gmo_fx/ticker.py
--rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)       59 2024-05-03 13:02:15.000000 gmo_fx-0.1.0/gmo_fx/urls.py
-drwxrwxrwx   0 r_noto    (1000) r_noto    (1000)        0 2024-05-07 10:10:26.585613 gmo_fx-0.1.0/gmo_fx.egg-info/
--rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     1086 2024-05-07 10:10:25.000000 gmo_fx-0.1.0/gmo_fx.egg-info/PKG-INFO
--rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)      427 2024-05-07 10:10:25.000000 gmo_fx-0.1.0/gmo_fx.egg-info/SOURCES.txt
--rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)        1 2024-05-07 10:10:25.000000 gmo_fx-0.1.0/gmo_fx.egg-info/dependency_links.txt
--rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)       17 2024-05-07 10:10:25.000000 gmo_fx-0.1.0/gmo_fx.egg-info/requires.txt
--rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)        7 2024-05-07 10:10:25.000000 gmo_fx-0.1.0/gmo_fx.egg-info/top_level.txt
--rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)       38 2024-05-07 10:10:26.597654 gmo_fx-0.1.0/setup.cfg
--rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)      784 2024-05-07 10:09:47.000000 gmo_fx-0.1.0/setup.py
-drwxrwxrwx   0 r_noto    (1000) r_noto    (1000)        0 2024-05-07 10:10:26.567611 gmo_fx-0.1.0/tests/
--rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     2767 2024-04-29 11:27:04.000000 gmo_fx-0.1.0/tests/test_base_response.py
--rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     6806 2024-05-03 13:02:15.000000 gmo_fx-0.1.0/tests/test_klines.py
--rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     1055 2024-05-01 13:22:22.000000 gmo_fx-0.1.0/tests/test_status.py
--rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     5302 2024-05-04 04:15:36.000000 gmo_fx-0.1.0/tests/test_symbols.py
--rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     4836 2024-05-01 13:22:22.000000 gmo_fx-0.1.0/tests/test_ticker.py
+drwxrwxrwx   0 r_noto    (1000) r_noto    (1000)        0 2024-05-07 13:18:20.296939 gmo_fx-0.1.1/
+-rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     1067 2024-04-26 12:41:11.000000 gmo_fx-0.1.1/LICENSE
+-rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     1086 2024-05-07 13:18:20.292915 gmo_fx-0.1.1/PKG-INFO
+-rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)      719 2024-05-07 10:05:52.000000 gmo_fx-0.1.1/README.md
+drwxrwxrwx   0 r_noto    (1000) r_noto    (1000)        0 2024-05-07 13:18:20.176997 gmo_fx-0.1.1/gmo_fx/
+-rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)      135 2024-05-06 12:10:47.000000 gmo_fx-0.1.1/gmo_fx/__init__.py
+-rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     7751 2024-04-29 11:27:04.000000 gmo_fx-0.1.1/gmo_fx/errors.py
+-rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     2114 2024-05-03 13:02:15.000000 gmo_fx-0.1.1/gmo_fx/klines.py
+-rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)      566 2024-04-29 11:27:04.000000 gmo_fx-0.1.1/gmo_fx/response.py
+-rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     1314 2024-05-03 13:02:15.000000 gmo_fx-0.1.1/gmo_fx/status.py
+-rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     1623 2024-05-04 04:15:36.000000 gmo_fx-0.1.1/gmo_fx/symbols.py
+-rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     1260 2024-05-03 13:02:15.000000 gmo_fx-0.1.1/gmo_fx/ticker.py
+-rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)       59 2024-05-03 13:02:15.000000 gmo_fx-0.1.1/gmo_fx/urls.py
+drwxrwxrwx   0 r_noto    (1000) r_noto    (1000)        0 2024-05-07 13:18:20.286544 gmo_fx-0.1.1/gmo_fx.egg-info/
+-rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     1086 2024-05-07 13:18:19.000000 gmo_fx-0.1.1/gmo_fx.egg-info/PKG-INFO
+-rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)      427 2024-05-07 13:18:19.000000 gmo_fx-0.1.1/gmo_fx.egg-info/SOURCES.txt
+-rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)        1 2024-05-07 13:18:19.000000 gmo_fx-0.1.1/gmo_fx.egg-info/dependency_links.txt
+-rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)       17 2024-05-07 13:18:19.000000 gmo_fx-0.1.1/gmo_fx.egg-info/requires.txt
+-rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)        7 2024-05-07 13:18:19.000000 gmo_fx-0.1.1/gmo_fx.egg-info/top_level.txt
+-rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)       38 2024-05-07 13:18:20.297940 gmo_fx-0.1.1/setup.cfg
+-rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)      784 2024-05-07 10:10:59.000000 gmo_fx-0.1.1/setup.py
+drwxrwxrwx   0 r_noto    (1000) r_noto    (1000)        0 2024-05-07 13:18:20.272732 gmo_fx-0.1.1/tests/
+-rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     2767 2024-04-29 11:27:04.000000 gmo_fx-0.1.1/tests/test_base_response.py
+-rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     6806 2024-05-03 13:02:15.000000 gmo_fx-0.1.1/tests/test_klines.py
+-rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     1055 2024-05-01 13:22:22.000000 gmo_fx-0.1.1/tests/test_status.py
+-rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     5302 2024-05-04 04:15:36.000000 gmo_fx-0.1.1/tests/test_symbols.py
+-rwxrwxrwx   0 r_noto    (1000) r_noto    (1000)     4836 2024-05-01 13:22:22.000000 gmo_fx-0.1.1/tests/test_ticker.py
```

### Comparing `gmo_fx-0.1.0/LICENSE` & `gmo_fx-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gmo_fx-0.1.0/PKG-INFO` & `gmo_fx-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmo_fx
-Version: 0.1.0
+Version: 0.1.1
 Summary: GMO社のFX API用Pythonライブラリ
 Home-page: https://github.com/RikitoNoto/gmo-fx-py
 Download-URL: https://github.com/RikitoNoto/gmo-fx-py
 Author: Rikito Noto
 Author-email: rikitonoto@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `gmo_fx-0.1.0/README.md` & `gmo_fx-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gmo_fx-0.1.0/gmo_fx/errors.py` & `gmo_fx-0.1.1/gmo_fx/errors.py`

 * *Files identical despite different names*

### Comparing `gmo_fx-0.1.0/gmo_fx/klines.py` & `gmo_fx-0.1.1/gmo_fx/klines.py`

 * *Files identical despite different names*

### Comparing `gmo_fx-0.1.0/gmo_fx/response.py` & `gmo_fx-0.1.1/gmo_fx/response.py`

 * *Files identical despite different names*

### Comparing `gmo_fx-0.1.0/gmo_fx/status.py` & `gmo_fx-0.1.1/gmo_fx/status.py`

 * *Files identical despite different names*

### Comparing `gmo_fx-0.1.0/gmo_fx/symbols.py` & `gmo_fx-0.1.1/gmo_fx/symbols.py`

 * *Files identical despite different names*

### Comparing `gmo_fx-0.1.0/gmo_fx/ticker.py` & `gmo_fx-0.1.1/gmo_fx/ticker.py`

 * *Files identical despite different names*

### Comparing `gmo_fx-0.1.0/gmo_fx.egg-info/PKG-INFO` & `gmo_fx-0.1.1/gmo_fx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmo_fx
-Version: 0.1.0
+Version: 0.1.1
 Summary: GMO社のFX API用Pythonライブラリ
 Home-page: https://github.com/RikitoNoto/gmo-fx-py
 Download-URL: https://github.com/RikitoNoto/gmo-fx-py
 Author: Rikito Noto
 Author-email: rikitonoto@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `gmo_fx-0.1.0/setup.py` & `gmo_fx-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 DESCRIPTION = "GMO社のFX API用Pythonライブラリ"
 NAME = "gmo_fx"
 AUTHOR = "Rikito Noto"
 AUTHOR_EMAIL = "rikitonoto@gmail.com"
 URL = "https://github.com/RikitoNoto/gmo-fx-py"
 LICENSE = "MIT"
 DOWNLOAD_URL = "https://github.com/RikitoNoto/gmo-fx-py"
-VERSION = "0.1.0"
+VERSION = "0.1.1"
 INSTALL_REQUIRES = [
     "requests>=2.31.0",
 ]
 PACKAGES = [
     "gmo_fx",
 ]
```

### Comparing `gmo_fx-0.1.0/tests/test_base_response.py` & `gmo_fx-0.1.1/tests/test_base_response.py`

 * *Files identical despite different names*

### Comparing `gmo_fx-0.1.0/tests/test_klines.py` & `gmo_fx-0.1.1/tests/test_klines.py`

 * *Files identical despite different names*

### Comparing `gmo_fx-0.1.0/tests/test_status.py` & `gmo_fx-0.1.1/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `gmo_fx-0.1.0/tests/test_symbols.py` & `gmo_fx-0.1.1/tests/test_symbols.py`

 * *Files identical despite different names*

### Comparing `gmo_fx-0.1.0/tests/test_ticker.py` & `gmo_fx-0.1.1/tests/test_ticker.py`

 * *Files identical despite different names*

