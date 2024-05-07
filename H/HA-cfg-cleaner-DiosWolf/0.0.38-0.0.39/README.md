# Comparing `tmp/HA_cfg_cleaner_DiosWolf-0.0.38.tar.gz` & `tmp/ha_cfg_cleaner_dioswolf-0.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HA_cfg_cleaner_DiosWolf-0.0.38.tar", last modified: Fri Apr  5 21:08:26 2024, max compression
+gzip compressed data, was "ha_cfg_cleaner_dioswolf-0.0.39.tar", last modified: Tue May  7 07:16:58 2024, max compression
```

## Comparing `HA_cfg_cleaner_DiosWolf-0.0.38.tar` & `ha_cfg_cleaner_dioswolf-0.0.39.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 21:08:26.838178 HA_cfg_cleaner_DiosWolf-0.0.38/
-drwxrwxrwx   0        0        0        0 2024-04-05 21:08:26.822179 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/
--rw-rw-rw-   0        0        0       24 2024-04-05 21:08:18.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 21:08:26.827180 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/castom_errors/
--rw-rw-rw-   0        0        0      534 2024-04-05 21:04:10.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/castom_errors/castom_errors.py
-drwxrwxrwx   0        0        0        0 2024-04-05 21:08:26.828179 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/configs_HA/
--rw-rw-rw-   0        0        0     3459 2024-03-18 10:54:43.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/configs_HA/config_HA.json
--rw-rw-rw-   0        0        0     4025 2024-03-18 10:27:12.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/configs_HA/config_HA_wind.json
-drwxrwxrwx   0        0        0        0 2024-04-05 21:08:26.829179 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/data_classes_json/
--rw-rw-rw-   0        0        0      593 2024-03-18 09:54:43.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/data_classes_json/args_parse.py
--rw-rw-rw-   0        0        0     1220 2024-04-05 20:37:05.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/data_classes_json/file_config.py
--rw-rw-rw-   0        0        0     1568 2024-03-18 10:34:52.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/data_classes_json/instructions.py
-drwxrwxrwx   0        0        0        0 2024-04-05 21:08:26.834178 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/files_editors/
--rw-rw-rw-   0        0        0     2511 2024-04-05 20:52:56.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/files_editors/addons_editor.py
--rw-rw-rw-   0        0        0     3175 2024-04-05 21:02:15.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/files_editors/automations_editor.py
--rw-rw-rw-   0        0        0     2045 2024-03-05 22:25:38.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/files_editors/editor_restore_state.py
--rw-rw-rw-   0        0        0     3027 2024-04-05 20:36:15.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/files_editors/fileIO_cls.py
--rw-rw-rw-   0        0        0      442 2024-02-26 18:57:11.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/files_editors/file_folder_editor_cls.py
--rw-rw-rw-   0        0        0     2053 2024-04-05 20:37:05.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/files_editors/find_in_files_cls.py
--rw-rw-rw-   0        0        0     3096 2024-03-05 22:12:50.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/files_editors/integrations_cls.py
--rw-rw-rw-   0        0        0     1411 2024-04-05 20:37:26.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/files_editors/script_editor_cls.py
-drwxrwxrwx   0        0        0        0 2024-04-05 21:08:26.834178 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/ha_requests/
--rw-rw-rw-   0        0        0      756 2024-04-05 20:37:05.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/ha_requests/ha_request.py
-drwxrwxrwx   0        0        0        0 2024-04-05 21:08:26.835179 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/instruction_classes/
--rw-rw-rw-   0        0        0    14039 2024-04-05 20:52:56.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/instruction_classes/instruction_executor.py
--rw-rw-rw-   0        0        0     2890 2024-04-05 20:33:37.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/main.py
-drwxrwxrwx   0        0        0        0 2024-04-05 21:08:26.836180 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/parse_classes/
--rw-rw-rw-   0        0        0     1497 2024-04-05 21:08:02.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/parse_classes/arguments_parse.py
--rw-rw-rw-   0        0        0      171 2024-02-23 13:52:30.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/parse_classes/parse_cls.py
-drwxrwxrwx   0        0        0        0 2024-04-05 21:08:26.837179 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf.egg-info/
--rw-rw-rw-   0        0        0      275 2024-04-05 21:08:26.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1417 2024-04-05 21:08:26.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 21:08:26.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-04-05 21:08:26.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       70 2024-04-05 21:08:26.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-04-05 21:08:26.000000 HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-02-27 18:02:40.000000 HA_cfg_cleaner_DiosWolf-0.0.38/LICENSE
--rw-rw-rw-   0        0        0       61 2024-02-27 18:45:02.000000 HA_cfg_cleaner_DiosWolf-0.0.38/MANIFEST.in
--rw-rw-rw-   0        0        0      275 2024-04-05 21:08:26.837179 HA_cfg_cleaner_DiosWolf-0.0.38/PKG-INFO
--rw-rw-rw-   0        0        0       43 2024-02-28 18:51:58.000000 HA_cfg_cleaner_DiosWolf-0.0.38/README.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 21:08:26.838178 HA_cfg_cleaner_DiosWolf-0.0.38/setup.cfg
--rw-rw-rw-   0        0        0      636 2024-03-05 22:25:38.000000 HA_cfg_cleaner_DiosWolf-0.0.38/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:16:58.035553 ha_cfg_cleaner_dioswolf-0.0.39/
+drwxrwxrwx   0        0        0        0 2024-05-07 07:16:57.743007 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/
+-rw-rw-rw-   0        0        0       24 2024-05-07 07:16:42.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:16:57.863039 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/castom_errors/
+-rw-rw-rw-   0        0        0      608 2024-05-07 07:07:31.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/castom_errors/castom_errors.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:16:57.912040 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/configs_HA/
+-rw-rw-rw-   0        0        0     3459 2024-03-18 10:54:43.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/configs_HA/config_HA.json
+-rw-rw-rw-   0        0        0     4025 2024-03-18 10:27:12.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/configs_HA/config_HA_wind.json
+drwxrwxrwx   0        0        0        0 2024-05-07 07:16:57.929039 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/data_classes_json/
+-rw-rw-rw-   0        0        0      593 2024-03-18 09:54:43.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/data_classes_json/args_parse.py
+-rw-rw-rw-   0        0        0     1220 2024-04-05 20:37:05.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/data_classes_json/file_config.py
+-rw-rw-rw-   0        0        0     1568 2024-03-18 10:34:52.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/data_classes_json/instructions.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:16:57.980554 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/files_editors/
+-rw-rw-rw-   0        0        0     2511 2024-04-05 20:52:56.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/files_editors/addons_editor.py
+-rw-rw-rw-   0        0        0     3200 2024-05-07 07:04:30.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/files_editors/automations_editor.py
+-rw-rw-rw-   0        0        0     2045 2024-03-05 22:25:38.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/files_editors/editor_restore_state.py
+-rw-rw-rw-   0        0        0     3027 2024-04-05 20:36:15.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/files_editors/fileIO_cls.py
+-rw-rw-rw-   0        0        0      442 2024-02-26 18:57:11.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/files_editors/file_folder_editor_cls.py
+-rw-rw-rw-   0        0        0     2053 2024-04-05 20:37:05.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/files_editors/find_in_files_cls.py
+-rw-rw-rw-   0        0        0     3096 2024-03-05 22:12:50.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/files_editors/integrations_cls.py
+-rw-rw-rw-   0        0        0     1411 2024-04-05 20:37:26.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/files_editors/script_editor_cls.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:16:57.987555 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/ha_requests/
+-rw-rw-rw-   0        0        0      756 2024-04-05 20:37:05.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/ha_requests/ha_request.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:16:57.992554 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/instruction_classes/
+-rw-rw-rw-   0        0        0    14021 2024-04-05 21:09:49.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/instruction_classes/instruction_executor.py
+-rw-rw-rw-   0        0        0     2890 2024-04-05 20:33:37.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/main.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:16:58.021556 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/parse_classes/
+-rw-rw-rw-   0        0        0     1497 2024-04-05 21:08:02.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/parse_classes/arguments_parse.py
+-rw-rw-rw-   0        0        0      171 2024-02-23 13:52:30.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/parse_classes/parse_cls.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:16:58.031556 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf.egg-info/
+-rw-rw-rw-   0        0        0      275 2024-05-07 07:16:57.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1417 2024-05-07 07:16:57.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 07:16:57.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-05-07 07:16:57.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       70 2024-05-07 07:16:57.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-05-07 07:16:57.000000 ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-02-27 18:02:40.000000 ha_cfg_cleaner_dioswolf-0.0.39/LICENSE
+-rw-rw-rw-   0        0        0       61 2024-02-27 18:45:02.000000 ha_cfg_cleaner_dioswolf-0.0.39/MANIFEST.in
+-rw-rw-rw-   0        0        0      275 2024-05-07 07:16:58.032555 ha_cfg_cleaner_dioswolf-0.0.39/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2024-02-28 18:51:58.000000 ha_cfg_cleaner_dioswolf-0.0.39/README.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 07:16:58.036554 ha_cfg_cleaner_dioswolf-0.0.39/setup.cfg
+-rw-rw-rw-   0        0        0      636 2024-03-05 22:25:38.000000 ha_cfg_cleaner_dioswolf-0.0.39/setup.py
```

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/configs_HA/config_HA.json` & `ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/configs_HA/config_HA.json`

 * *Files identical despite different names*

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/configs_HA/config_HA_wind.json` & `ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/configs_HA/config_HA_wind.json`

 * *Files identical despite different names*

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/data_classes_json/args_parse.py` & `ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/data_classes_json/args_parse.py`

 * *Files identical despite different names*

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/data_classes_json/file_config.py` & `ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/data_classes_json/file_config.py`

 * *Files identical despite different names*

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/data_classes_json/instructions.py` & `ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/data_classes_json/instructions.py`

 * *Files identical despite different names*

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/files_editors/addons_editor.py` & `ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/files_editors/addons_editor.py`

 * *Files identical despite different names*

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/files_editors/automations_editor.py` & `ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/files_editors/automations_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from requests import Response
 
-from HA_cfg_cleaner_DiosWolf.castom_errors.castom_errors import CustomError, RaiseErrors
+from HA_cfg_cleaner_DiosWolf.castom_errors.castom_errors import RaiseErrors
 from HA_cfg_cleaner_DiosWolf.data_classes_json.file_config import (
     Configuration,
     HostInfo,
 )
 from HA_cfg_cleaner_DiosWolf.ha_requests.ha_request import HARequests
 
 
@@ -81,10 +81,10 @@
             + self.host_cfg.port
             + self.host_cfg.automations_off_url
         )
         if automations_entities_ids:
             data = {self.configuration.on_off_field: automations_entities_ids}
             resp = self.ha_request.post_requests(url, data)
 
-            self.error_editor.raise_error(resp.status_code)
+            self.error_editor.raise_error(resp.status_code, self.error_editor.automations_errors)
 
             return resp
```

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/files_editors/editor_restore_state.py` & `ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/files_editors/editor_restore_state.py`

 * *Files identical despite different names*

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/files_editors/fileIO_cls.py` & `ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/files_editors/fileIO_cls.py`

 * *Files identical despite different names*

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/files_editors/find_in_files_cls.py` & `ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/files_editors/find_in_files_cls.py`

 * *Files identical despite different names*

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/files_editors/integrations_cls.py` & `ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/files_editors/integrations_cls.py`

 * *Files identical despite different names*

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/files_editors/script_editor_cls.py` & `ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/files_editors/script_editor_cls.py`

 * *Files identical despite different names*

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/ha_requests/ha_request.py` & `ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/ha_requests/ha_request.py`

 * *Files identical despite different names*

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/instruction_classes/instruction_executor.py` & `ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/instruction_classes/instruction_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 
 from HA_cfg_cleaner_DiosWolf.castom_errors.castom_errors import (
     CustomError,
-    CustomError,
 )
 from HA_cfg_cleaner_DiosWolf.data_classes_json.file_config import ConfigurationFile
 from HA_cfg_cleaner_DiosWolf.data_classes_json.instructions import (
     Instructions,
     ChangeAddonsOptions,
 )
 from HA_cfg_cleaner_DiosWolf.files_editors.addons_editor import AddonsEditor
```

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/main.py` & `ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/main.py`

 * *Files identical despite different names*

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf/parse_classes/arguments_parse.py` & `ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf/parse_classes/arguments_parse.py`

 * *Files identical despite different names*

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.38/HA_cfg_cleaner_DiosWolf.egg-info/SOURCES.txt` & `ha_cfg_cleaner_dioswolf-0.0.39/HA_cfg_cleaner_DiosWolf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.38/LICENSE` & `ha_cfg_cleaner_dioswolf-0.0.39/LICENSE`

 * *Files identical despite different names*

### Comparing `HA_cfg_cleaner_DiosWolf-0.0.38/setup.py` & `ha_cfg_cleaner_dioswolf-0.0.39/setup.py`

 * *Files identical despite different names*

