# Comparing `tmp/temporal_kan-0.1.1.tar.gz` & `tmp/temporal_kan-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temporal_kan-0.1.1.tar", max compression
+gzip compressed data, was "temporal_kan-0.1.2.tar", max compression
```

## Comparing `temporal_kan-0.1.1.tar` & `temporal_kan-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      489 2024-05-07 12:34:24.615303 temporal_kan-0.1.1/README.md
--rw-r--r--   0        0        0      411 2024-05-07 14:02:23.161227 temporal_kan-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      613 2024-05-07 13:15:31.231940 temporal_kan-0.1.1/temporal_kan/__init__.py
--rw-r--r--   0        0        0     6021 2024-05-07 13:56:07.437067 temporal_kan-0.1.1/temporal_kan/glstm.py
--rw-r--r--   0        0        0     3757 2024-05-07 13:56:12.573077 temporal_kan-0.1.1/temporal_kan/gr.py
--rw-r--r--   0        0        0     4165 2024-05-07 13:56:18.197088 temporal_kan-0.1.1/temporal_kan/sltsm.py
--rw-r--r--   0        0        0      132 2024-05-07 13:02:40.269087 temporal_kan-0.1.1/temporal_kan/spline.py
--rw-r--r--   0        0        0     3424 2024-05-07 13:56:26.321103 temporal_kan-0.1.1/temporal_kan/sr.py
--rw-r--r--   0        0        0      922 1970-01-01 00:00:00.000000 temporal_kan-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1417 2024-05-07 14:08:23.794098 temporal_kan-0.1.2/README.md
+-rw-r--r--   0        0        0      411 2024-05-07 14:12:36.556411 temporal_kan-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      641 2024-05-07 14:11:58.520102 temporal_kan-0.1.2/temporal_kan/__init__.py
+-rw-r--r--   0        0        0     6021 2024-05-07 13:56:07.437067 temporal_kan-0.1.2/temporal_kan/glstm.py
+-rw-r--r--   0        0        0     3757 2024-05-07 13:56:12.573077 temporal_kan-0.1.2/temporal_kan/gr.py
+-rw-r--r--   0        0        0     1264 2024-05-07 14:12:04.212149 temporal_kan-0.1.2/temporal_kan/kan.py
+-rw-r--r--   0        0        0     4165 2024-05-07 13:56:18.197088 temporal_kan-0.1.2/temporal_kan/sltsm.py
+-rw-r--r--   0        0        0      132 2024-05-07 13:02:40.269087 temporal_kan-0.1.2/temporal_kan/spline.py
+-rw-r--r--   0        0        0     3424 2024-05-07 13:56:26.321103 temporal_kan-0.1.2/temporal_kan/sr.py
+-rw-r--r--   0        0        0     1850 1970-01-01 00:00:00.000000 temporal_kan-0.1.2/PKG-INFO
```

### Comparing `temporal_kan-0.1.1/temporal_kan/__init__.py` & `temporal_kan-0.1.2/temporal_kan/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from temporal_kan.spline import power_spline
 from temporal_kan.sr import SRKAN
 from temporal_kan.gr import GRKAN
 from temporal_kan.sltsm import SLSTM_KAN
 from temporal_kan.glstm import GLSTM_KAN
+from temporal_kan.kan import KAN
 
 
-def TemporalKanModel(model_type: str = 'SRKAN', *args, **kwargs):
+def TemporalKan(model_type: str = 'SRKAN', *args, **kwargs):
     if model_type == 'SRKAN':
         return SRKAN(*args, **kwargs)
     elif model_type == 'GRKAN':
         return GRKAN(*args, **kwargs)
     elif model_type == 'SLSTM_KAN':
         return SLSTM_KAN(*args, **kwargs)
     elif model_type == 'GLSTM_KAN':
```

### Comparing `temporal_kan-0.1.1/temporal_kan/glstm.py` & `temporal_kan-0.1.2/temporal_kan/glstm.py`

 * *Files identical despite different names*

### Comparing `temporal_kan-0.1.1/temporal_kan/gr.py` & `temporal_kan-0.1.2/temporal_kan/gr.py`

 * *Files identical despite different names*

### Comparing `temporal_kan-0.1.1/temporal_kan/sltsm.py` & `temporal_kan-0.1.2/temporal_kan/sltsm.py`

 * *Files identical despite different names*

### Comparing `temporal_kan-0.1.1/temporal_kan/sr.py` & `temporal_kan-0.1.2/temporal_kan/sr.py`

 * *Files identical despite different names*

