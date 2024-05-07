# Comparing `tmp/3dfin-0.3.3.tar.gz` & `tmp/3dfin-0.4.0a0.tar.gz`

## Comparing `3dfin-0.3.3.tar` & `3dfin-0.4.0a0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    78160 2020-02-02 00:00:00.000000 3dfin-0.3.3/3dfin_logo.png
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 3dfin-0.3.3/CONTRIBUTING.md
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 3dfin-0.3.3/src/three_d_fin/3DFinconfig.ini
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 3dfin-0.3.3/src/three_d_fin/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 3dfin-0.3.3/src/three_d_fin/__init__.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 3dfin-0.3.3/src/three_d_fin/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 3dfin-0.3.3/src/three_d_fin/cloudcompare/__init__.py
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 3dfin-0.3.3/src/three_d_fin/cloudcompare/plugin.py
--rw-r--r--   0        0        0    12667 2020-02-02 00:00:00.000000 3dfin-0.3.3/src/three_d_fin/cloudcompare/plugin_processing.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 3dfin-0.3.3/src/three_d_fin/cloudcompare/plugin_progress.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 3dfin-0.3.3/src/three_d_fin/cloudcompare/assets/3dfin_color_scale.xml
--rw-r--r--   0        0        0    14597 2020-02-02 00:00:00.000000 3dfin-0.3.3/src/three_d_fin/cloudcompare/assets/3dfin_logo_plugin.png
--rw-r--r--   0        0        0  4119707 2020-02-02 00:00:00.000000 3dfin-0.3.3/src/three_d_fin/documentation/documentation.pdf
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 3dfin-0.3.3/src/three_d_fin/gui/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 3dfin-0.3.3/src/three_d_fin/gui/__init__.py
--rw-r--r--   0        0        0    21639 2020-02-02 00:00:00.000000 3dfin-0.3.3/src/three_d_fin/gui/application.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 3dfin-0.3.3/src/three_d_fin/gui/expert_dlg.py
--rw-r--r--   0        0        0  1861465 2020-02-02 00:00:00.000000 3dfin-0.3.3/src/three_d_fin/gui/gui_ressources.py
--rw-r--r--   0        0        0   258590 2020-02-02 00:00:00.000000 3dfin-0.3.3/src/three_d_fin/gui/main_window.py
--rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 3dfin-0.3.3/src/three_d_fin/processing/__init__.py
--rw-r--r--   0        0        0    28372 2020-02-02 00:00:00.000000 3dfin-0.3.3/src/three_d_fin/processing/abstract_processing.py
--rw-r--r--   0        0        0    21219 2020-02-02 00:00:00.000000 3dfin-0.3.3/src/three_d_fin/processing/configuration.py
--rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 3dfin-0.3.3/src/three_d_fin/processing/io.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 3dfin-0.3.3/src/three_d_fin/processing/progress.py
--rw-r--r--   0        0        0     7903 2020-02-02 00:00:00.000000 3dfin-0.3.3/src/three_d_fin/processing/standalone_processing.py
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 3dfin-0.3.3/tests/lowerlimitchange.ini
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 3dfin-0.3.3/tests/test_configuration.py
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 3dfin-0.3.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 3dfin-0.3.3/LICENSE
--rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 3dfin-0.3.3/README.md
--rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 3dfin-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 3dfin-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    78160 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/3dfin_logo.png
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/src/three_d_fin/3DFinconfig.ini
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/src/three_d_fin/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/src/three_d_fin/__init__.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/src/three_d_fin/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/src/three_d_fin/cloudcompare/__init__.py
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/src/three_d_fin/cloudcompare/plugin.py
+-rw-r--r--   0        0        0    12667 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/src/three_d_fin/cloudcompare/plugin_processing.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/src/three_d_fin/cloudcompare/plugin_progress.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/src/three_d_fin/cloudcompare/assets/3dfin_color_scale.xml
+-rw-r--r--   0        0        0    14597 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/src/three_d_fin/cloudcompare/assets/3dfin_logo_plugin.png
+-rw-r--r--   0        0        0  4119707 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/src/three_d_fin/documentation/documentation.pdf
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/src/three_d_fin/gui/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/src/three_d_fin/gui/__init__.py
+-rw-r--r--   0        0        0    21639 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/src/three_d_fin/gui/application.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/src/three_d_fin/gui/expert_dlg.py
+-rw-r--r--   0        0        0  1861465 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/src/three_d_fin/gui/gui_ressources.py
+-rw-r--r--   0        0        0   258590 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/src/three_d_fin/gui/main_window.py
+-rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/src/three_d_fin/processing/__init__.py
+-rw-r--r--   0        0        0    28372 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/src/three_d_fin/processing/abstract_processing.py
+-rw-r--r--   0        0        0    21219 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/src/three_d_fin/processing/configuration.py
+-rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/src/three_d_fin/processing/io.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/src/three_d_fin/processing/progress.py
+-rw-r--r--   0        0        0     7903 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/src/three_d_fin/processing/standalone_processing.py
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/tests/lowerlimitchange.ini
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/tests/test_configuration.py
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/LICENSE
+-rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/README.md
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/pyproject.toml
+-rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 3dfin-0.4.0a0/PKG-INFO
```

### Comparing `3dfin-0.3.3/3dfin_logo.png` & `3dfin-0.4.0a0/3dfin_logo.png`

 * *Files identical despite different names*

### Comparing `3dfin-0.3.3/CONTRIBUTING.md` & `3dfin-0.4.0a0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `3dfin-0.3.3/src/three_d_fin/3DFinconfig.ini` & `3dfin-0.4.0a0/src/three_d_fin/3DFinconfig.ini`

 * *Files identical despite different names*

### Comparing `3dfin-0.3.3/src/three_d_fin/__about__.py` & `3dfin-0.4.0a0/src/three_d_fin/__about__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.3.3"
+__version__ = "0.4.0a0"
 
 # Copyright infos
 __copyright_info_1__ = (
     "3DFin: Forest Inventory Copyright (C) 2023 Carlos Cabo & Diego Laino."
 )
 __copyright_info_2__ = (
     "This program comes with ABSOLUTELY NO WARRANTY. This is a free "
```

### Comparing `3dfin-0.3.3/src/three_d_fin/cloudcompare/plugin.py` & `3dfin-0.4.0a0/src/three_d_fin/cloudcompare/plugin.py`

 * *Files identical despite different names*

### Comparing `3dfin-0.3.3/src/three_d_fin/cloudcompare/plugin_processing.py` & `3dfin-0.4.0a0/src/three_d_fin/cloudcompare/plugin_processing.py`

 * *Files identical despite different names*

### Comparing `3dfin-0.3.3/src/three_d_fin/cloudcompare/plugin_progress.py` & `3dfin-0.4.0a0/src/three_d_fin/cloudcompare/plugin_progress.py`

 * *Files identical despite different names*

### Comparing `3dfin-0.3.3/src/three_d_fin/cloudcompare/assets/3dfin_color_scale.xml` & `3dfin-0.4.0a0/src/three_d_fin/cloudcompare/assets/3dfin_color_scale.xml`

 * *Files identical despite different names*

### Comparing `3dfin-0.3.3/src/three_d_fin/cloudcompare/assets/3dfin_logo_plugin.png` & `3dfin-0.4.0a0/src/three_d_fin/cloudcompare/assets/3dfin_logo_plugin.png`

 * *Files identical despite different names*

### Comparing `3dfin-0.3.3/src/three_d_fin/documentation/documentation.pdf` & `3dfin-0.4.0a0/src/three_d_fin/documentation/documentation.pdf`

 * *Files identical despite different names*

### Comparing `3dfin-0.3.3/src/three_d_fin/gui/application.py` & `3dfin-0.4.0a0/src/three_d_fin/gui/application.py`

 * *Files identical despite different names*

### Comparing `3dfin-0.3.3/src/three_d_fin/gui/expert_dlg.py` & `3dfin-0.4.0a0/src/three_d_fin/gui/expert_dlg.py`

 * *Files identical despite different names*

### Comparing `3dfin-0.3.3/src/three_d_fin/gui/gui_ressources.py` & `3dfin-0.4.0a0/src/three_d_fin/gui/gui_ressources.py`

 * *Files 0% similar despite different names*

```diff
@@ -28272,57 +28272,57 @@
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x02\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x16\x00\x00\x00\x03\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x12\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
-\x00\x00\x01\x8e\x43\x24\x55\x51\
+\x00\x00\x01\x8f\x53\x46\xb5\x56\
 \x00\x00\x00\x38\x00\x00\x00\x00\x00\x01\x00\x00\x08\xbd\
-\x00\x00\x01\x8e\x43\x24\x55\x51\
+\x00\x00\x01\x8f\x53\x46\xb5\x56\
 \x00\x00\x00\x52\x00\x00\x00\x00\x00\x01\x00\x00\xe1\x11\
-\x00\x00\x01\x8e\x43\x24\x55\x4d\
+\x00\x00\x01\x8f\x53\x46\xb5\x52\
 \x00\x00\x00\x74\x00\x00\x00\x00\x00\x01\x00\x01\x27\x74\
-\x00\x00\x01\x8e\x43\x24\x55\x51\
+\x00\x00\x01\x8f\x53\x46\xb5\x56\
 \x00\x00\x00\x9e\x00\x00\x00\x00\x00\x01\x00\x01\xd3\x3c\
-\x00\x00\x01\x8e\x43\x24\x55\x51\
+\x00\x00\x01\x8f\x53\x46\xb5\x56\
 \x00\x00\x00\xc2\x00\x00\x00\x00\x00\x01\x00\x02\x01\xeb\
-\x00\x00\x01\x8e\x43\x24\x55\x51\
+\x00\x00\x01\x8f\x53\x46\xb5\x56\
 \x00\x00\x00\xe8\x00\x00\x00\x00\x00\x01\x00\x02\x2c\xeb\
-\x00\x00\x01\x8e\x43\x24\x55\x51\
+\x00\x00\x01\x8f\x53\x46\xb5\x56\
 \x00\x00\x01\x04\x00\x00\x00\x00\x00\x01\x00\x02\xd3\x10\
-\x00\x00\x01\x8e\x43\x24\x55\x4d\
+\x00\x00\x01\x8f\x53\x46\xb5\x52\
 \x00\x00\x01\x30\x00\x00\x00\x00\x00\x01\x00\x02\xda\xec\
-\x00\x00\x01\x8e\x43\x24\x55\x51\
+\x00\x00\x01\x8f\x53\x46\xb5\x52\
 \x00\x00\x01\x30\x00\x00\x00\x00\x00\x01\x00\x03\x19\x2e\
-\x00\x00\x01\x8e\x43\x24\x55\x51\
+\x00\x00\x01\x8f\x53\x46\xb5\x52\
 \x00\x00\x01\x54\x00\x00\x00\x00\x00\x01\x00\x03\x57\x70\
-\x00\x00\x01\x8e\x43\x24\x55\x4d\
+\x00\x00\x01\x8f\x53\x46\xb5\x52\
 \x00\x00\x01\x80\x00\x00\x00\x00\x00\x01\x00\x03\x64\x53\
-\x00\x00\x01\x8e\x43\x24\x55\x4d\
+\x00\x00\x01\x8f\x53\x46\xb5\x52\
 \x00\x00\x01\xa4\x00\x00\x00\x00\x00\x01\x00\x03\xb2\xbe\
-\x00\x00\x01\x8e\x43\x24\x55\x51\
+\x00\x00\x01\x8f\x53\x46\xb5\x56\
 \x00\x00\x01\xd0\x00\x00\x00\x00\x00\x01\x00\x05\x53\xc6\
-\x00\x00\x01\x8e\x43\x24\x55\x51\
+\x00\x00\x01\x8f\x53\x46\xb5\x56\
 \x00\x00\x01\xf0\x00\x00\x00\x00\x00\x01\x00\x05\x56\xcf\
-\x00\x00\x01\x8e\x43\x24\x55\x4d\
+\x00\x00\x01\x8f\x53\x46\xb5\x52\
 \x00\x00\x02\x12\x00\x00\x00\x00\x00\x01\x00\x05\x60\x05\
-\x00\x00\x01\x8e\x43\x24\x55\x51\
+\x00\x00\x01\x8f\x53\x46\xb5\x56\
 \x00\x00\x02\x36\x00\x00\x00\x00\x00\x01\x00\x05\x6b\x31\
-\x00\x00\x01\x8e\x43\x24\x55\x51\
+\x00\x00\x01\x8f\x53\x46\xb5\x56\
 \x00\x00\x02\x5e\x00\x00\x00\x00\x00\x01\x00\x05\x99\x11\
-\x00\x00\x01\x8e\x43\x24\x55\x51\
+\x00\x00\x01\x8f\x53\x46\xb5\x56\
 \x00\x00\x02\x88\x00\x00\x00\x00\x00\x01\x00\x05\xe0\x0a\
-\x00\x00\x01\x8e\x43\x24\x55\x51\
+\x00\x00\x01\x8f\x53\x46\xb5\x56\
 \x00\x00\x02\xb6\x00\x00\x00\x00\x00\x01\x00\x06\x8a\xb5\
-\x00\x00\x01\x8e\x43\x24\x55\x4d\
+\x00\x00\x01\x8f\x53\x46\xb5\x52\
 \x00\x00\x02\xe0\x00\x00\x00\x00\x00\x01\x00\x06\xc9\xd8\
-\x00\x00\x01\x8e\x43\x24\x55\x4d\
+\x00\x00\x01\x8f\x53\x46\xb5\x52\
 \x00\x00\x03\x04\x00\x00\x00\x00\x00\x01\x00\x06\xd3\x22\
-\x00\x00\x01\x8e\x43\x24\x55\x4d\
+\x00\x00\x01\x8f\x53\x46\xb5\x52\
 "
 
 qt_version = [int(v) for v in QtCore.qVersion().split('.')]
 if qt_version < [5, 8, 0]:
     rcc_version = 1
     qt_resource_struct = qt_resource_struct_v1
 else:
```

### Comparing `3dfin-0.3.3/src/three_d_fin/gui/main_window.py` & `3dfin-0.4.0a0/src/three_d_fin/gui/main_window.py`

 * *Files identical despite different names*

### Comparing `3dfin-0.3.3/src/three_d_fin/processing/__init__.py` & `3dfin-0.4.0a0/src/three_d_fin/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `3dfin-0.3.3/src/three_d_fin/processing/abstract_processing.py` & `3dfin-0.4.0a0/src/three_d_fin/processing/abstract_processing.py`

 * *Files identical despite different names*

### Comparing `3dfin-0.3.3/src/three_d_fin/processing/configuration.py` & `3dfin-0.4.0a0/src/three_d_fin/processing/configuration.py`

 * *Files identical despite different names*

### Comparing `3dfin-0.3.3/src/three_d_fin/processing/io.py` & `3dfin-0.4.0a0/src/three_d_fin/processing/io.py`

 * *Files identical despite different names*

### Comparing `3dfin-0.3.3/src/three_d_fin/processing/progress.py` & `3dfin-0.4.0a0/src/three_d_fin/processing/progress.py`

 * *Files identical despite different names*

### Comparing `3dfin-0.3.3/src/three_d_fin/processing/standalone_processing.py` & `3dfin-0.4.0a0/src/three_d_fin/processing/standalone_processing.py`

 * *Files identical despite different names*

### Comparing `3dfin-0.3.3/tests/lowerlimitchange.ini` & `3dfin-0.4.0a0/tests/lowerlimitchange.ini`

 * *Files identical despite different names*

### Comparing `3dfin-0.3.3/tests/test_configuration.py` & `3dfin-0.4.0a0/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `3dfin-0.3.3/.gitignore` & `3dfin-0.4.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `3dfin-0.3.3/LICENSE` & `3dfin-0.4.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `3dfin-0.3.3/README.md` & `3dfin-0.4.0a0/README.md`

 * *Files identical despite different names*

### Comparing `3dfin-0.3.3/pyproject.toml` & `3dfin-0.4.0a0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "pyqt5~=5.15"]
 build-backend = "hatchling.build"
 
 [project]
 name = "3DFin"
 description = "Automatic dendrometry and forest inventory for terrestrial point clouds, application package"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = "GPL-3.0-or-later"
 keywords = ["lidar", "forestry", "tls"]
 authors = [
   { name = "Carlos Cabo", email = "carloscabo@uniovi.es" },
   { name = "Diego Laino", email = "diegolainor@gmail.com" },
 ]
 classifiers = [
@@ -23,20 +23,20 @@
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Topic :: Scientific/Engineering",
   "Topic :: Scientific/Engineering :: GIS",
   "Intended Audience :: Science/Research",
 ]
 dependencies = [
-  "lazrs~=0.5.0",
-  "pandas~=2.0.0",
-  "XlsxWriter~=3.1.0",
-  "dendromatics~=0.4.2",
-  "pydantic~=1.10.7",
-  "PyQT5~=5.15"
+  "lazrs~=0.6.0",
+  "pandas~=2.2.0",
+  "XlsxWriter~=3.2.0",
+  "dendromatics~=0.5.0a0",
+  "pydantic~=1.10.15",
+  "pyqt5~=5.15"
 ]
 dynamic = ["version"]
 
 # Entry point for CloudCompare plugin
 [project.entry-points."cloudcompare.plugins"]
 3DFin = "three_d_fin.cloudcompare.plugin:ThreeDFinCC"
 
@@ -70,80 +70,76 @@
   "pyuic5 {args} qt-files/src/main_window.ui -o src/three_d_fin/gui/main_window.py --import-from=three_d_fin.gui --resource-suffix=", 
   "pyuic5 {args} qt-files/src/expert_dlg.ui -o src/three_d_fin/gui/expert_dlg.py --import-from=three_d_fin.gui --resource-suffix="
 ]
 qt-ressource = "pyrcc5 {args} qt-files/src/gui_ressources.qrc -o src/three_d_fin/gui/gui_ressources.py"
 qt-all = ["qt-moc", "qt-ressource"]
 
 [tool.hatch.build.targets.sdist.hooks.custom]
-dependencies = ["PyQT5~=5.15"]
 path = "scripts/qt_build_hook.py"
 src_folder = "qt-files/src"
 dest_folder = "src/three_d_fin/gui"
 import_from = "three_d_fin.gui" # TODO: it could be infered from dest_folder
 
 # PyInstaller builder
 [tool.hatch.build.targets.custom]
 require-runtime-dependencies = true
 dependencies = ["pyinstaller"]
 path = "scripts/pyinstaller_builder.py"
 
 # We need to duplicate this for pyinstaller custom target
 # it is not very DRY. The best would be to depends on sdist target
 [tool.hatch.build.targets.custom.hooks.custom] 
-dependencies = ["PyQT5~=5.15"]
 path = "scripts/qt_build_hook.py"
 src_folder = "qt-files/src"
 dest_folder = "src/three_d_fin/gui"
 import_from = "three_d_fin.gui" # TODO: it could be infered from dest_folder
 
 [[tool.hatch.envs.test.matrix]]
-python = ["38", "39", "310", "311", "312"]
+python = ["39", "310", "311", "312"]
 
 [tool.coverage.run]
 branch = true
 parallel = true
 omit = ["src/three_d_fin/__about__.py"]
 
 [tool.coverage.report]
 exclude_lines = ["no cov", "if __name__ == .__main__.:", "if TYPE_CHECKING:"]
 
 [tool.hatch.envs.lint]
 detached = true
-dependencies = ["ruff>=0.0.261", "black>=23.3.0", "mypy>=1.2.0"]
+dependencies = ["mypy>=1.2.0"]
 
 [tool.hatch.envs.lint.scripts]
 # static analysis with ruff
 check-type = "mypy --install-types --non-interactive {args:src/three_d_fin tests}"
-check-static = "ruff check {args:.}"
-check-format = "black --check --diff --color {args:.}"
-fix-static = "ruff --fix {args:.}"
-fix-format = "black {args:.}"
+check-static = "hatch fmt -l --check"
+check-format = "hatch fmt -f --check"
+fix-static = "hatch fmt -l"
+fix-format = "hatch fmt -f"
 check-all = ["check-static", "check-format"]
 fix-all = ["fix-static", "fix-format", "check-all"]
 
 [tool.ruff]
-select = ["E", "W", "YTT", "PTH", "NPY", "RET", "PYI", "Q", "F", "B", "I", "D"]
-target-version = "py310"
 line-length = 88
+target-version = "py310"
+
+[tool.ruff.lint]
+select = ["I001","E", "W", "YTT", "PTH", "NPY", "RET", "PYI", "Q", "F", "B", "I", "D"]
 # TODO: for now we ignore "Line too long error (E501)" 
 # because our comments are too longs
-# Black will take care of the line lenght in code anyway
+# code formatting will take care of the line length in code anyway
 ignore = [
   "E501",
   # Ignore docstring in public package and module
   "D100",
   "D104",
   # Blank line before class
   "D203",
   # multiline summary second line
   "D213",
 ]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["three_d_fin"]
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
-
-[tool.black]
-line-length = 88
-target-version = ["py310"]
```

### Comparing `3dfin-0.3.3/PKG-INFO` & `3dfin-0.4.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: 3DFin
-Version: 0.3.3
+Version: 0.4.0a0
 Summary: Automatic dendrometry and forest inventory for terrestrial point clouds, application package
 Project-URL: Documentation, https://github.com/3DFin/3DFin#README.md
 Project-URL: Issues, https://github.com/3DFin/3DFin/issues
 Project-URL: Source, https://github.com/3DFin/3DFin
 Author-email: Carlos Cabo <carloscabo@uniovi.es>, Diego Laino <diegolainor@gmail.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
@@ -16,21 +16,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: GIS
-Requires-Python: >=3.8
-Requires-Dist: dendromatics~=0.4.2
-Requires-Dist: lazrs~=0.5.0
-Requires-Dist: pandas~=2.0.0
-Requires-Dist: pydantic~=1.10.7
+Requires-Python: >=3.9
+Requires-Dist: dendromatics~=0.5.0a0
+Requires-Dist: lazrs~=0.6.0
+Requires-Dist: pandas~=2.2.0
+Requires-Dist: pydantic~=1.10.15
 Requires-Dist: pyqt5~=5.15
-Requires-Dist: xlsxwriter~=3.1.0
+Requires-Dist: xlsxwriter~=3.2.0
 Description-Content-Type: text/markdown
 
 
 <img width="892" alt="3dfin_logo" src="https://user-images.githubusercontent.com/68945855/233049674-8d2c96a7-8abc-4a7c-8e83-4a329ba6dd0c.png">
 
 Welcome to 3DFin: 3D Forest inventory's official repository!
```

