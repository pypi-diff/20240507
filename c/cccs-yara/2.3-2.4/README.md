# Comparing `tmp/cccs-yara-2.3.tar.gz` & `tmp/cccs_yara-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cccs-yara-2.3.tar", last modified: Thu Feb  8 19:42:07 2024, max compression
+gzip compressed data, was "cccs_yara-2.4.tar", last modified: Tue May  7 15:31:22 2024, max compression
```

## Comparing `cccs-yara-2.3.tar` & `cccs_yara-2.4.tar`

### file list

```diff
@@ -1,39 +1,43 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-08 19:42:07.764162 cccs-yara-2.3/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-08 19:42:07.760162 cccs-yara-2.3/.github/
--rw-r--r--   0 vsts      (1001) docker     (127)      143 2024-02-08 19:41:56.000000 cccs-yara-2.3/.github/dependabot.yml
--rw-r--r--   0 vsts      (1001) docker     (127)       33 2024-02-08 19:41:56.000000 cccs-yara-2.3/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-08 19:41:56.000000 cccs-yara-2.3/.gitmodules
--rw-r--r--   0 vsts      (1001) docker     (127)     9638 2024-02-08 19:41:56.000000 cccs-yara-2.3/CCCS_YARA.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     7912 2024-02-08 19:41:56.000000 cccs-yara-2.3/CCCS_YARA_values.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     1401 2024-02-08 19:41:56.000000 cccs-yara-2.3/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)    12345 2024-02-08 19:42:07.764162 cccs-yara-2.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)    11926 2024-02-08 19:41:56.000000 cccs-yara-2.3/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-08 19:42:07.764162 cccs-yara-2.3/cccs_yara.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    12345 2024-02-08 19:42:07.000000 cccs-yara-2.3/cccs_yara.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      784 2024-02-08 19:42:07.000000 cccs-yara-2.3/cccs_yara.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-02-08 19:42:07.000000 cccs-yara-2.3/cccs_yara.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       59 2024-02-08 19:42:07.000000 cccs-yara-2.3/cccs_yara.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      127 2024-02-08 19:42:07.000000 cccs-yara-2.3/cccs_yara.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-02-08 19:42:07.000000 cccs-yara-2.3/cccs_yara.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-08 19:42:07.760162 cccs-yara-2.3/pipelines/
--rw-r--r--   0 vsts      (1001) docker     (127)      785 2024-02-08 19:41:56.000000 cccs-yara-2.3/pipelines/publish.yaml
--rw-r--r--   0 vsts      (1001) docker     (127)      127 2024-02-08 19:41:56.000000 cccs-yara-2.3/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      785 2024-02-08 19:41:56.000000 cccs-yara-2.3/settings.json
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-02-08 19:42:07.764162 cccs-yara-2.3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      688 2024-02-08 19:41:56.000000 cccs-yara-2.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-08 19:42:07.760162 cccs-yara-2.3/templates/
--rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-02-08 19:41:56.000000 cccs-yara-2.3/templates/CCCS_Yara_Template.yara
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-08 19:42:07.764162 cccs-yara-2.3/yara_validator/
--rw-r--r--   0 vsts      (1001) docker     (127)     9638 2024-02-08 19:41:56.000000 cccs-yara-2.3/yara_validator/CCCS_YARA.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     7912 2024-02-08 19:41:56.000000 cccs-yara-2.3/yara_validator/CCCS_YARA_values.yml
--rw-r--r--   0 vsts      (1001) docker     (127)       34 2024-02-08 19:41:56.000000 cccs-yara-2.3/yara_validator/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-08 19:41:56.000000 cccs-yara-2.3/yara_validator/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14526 2024-02-08 19:41:56.000000 cccs-yara-2.3/yara_validator/cli.py
--rw-r--r--   0 vsts      (1001) docker     (127)      556 2024-02-08 19:41:56.000000 cccs-yara-2.3/yara_validator/constants.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-08 19:42:07.764162 cccs-yara-2.3/yara_validator/stix2_patch/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-08 19:41:56.000000 cccs-yara-2.3/yara_validator/stix2_patch/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1167 2024-02-08 19:41:56.000000 cccs-yara-2.3/yara_validator/stix2_patch/filter_casefold.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43443 2024-02-08 19:41:56.000000 cccs-yara-2.3/yara_validator/validator.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-02-08 19:41:56.000000 cccs-yara-2.3/yara_validator/validator_cfg.yml
--rw-r--r--   0 vsts      (1001) docker     (127)    41349 2024-02-08 19:41:56.000000 cccs-yara-2.3/yara_validator/validator_functions.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30243 2024-02-08 19:41:56.000000 cccs-yara-2.3/yara_validator/yara_file_processor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 15:31:22.634491 cccs_yara-2.4/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 15:31:22.630491 cccs_yara-2.4/.github/
+-rw-r--r--   0 vsts      (1001) docker     (127)      143 2024-05-07 15:31:16.000000 cccs_yara-2.4/.github/dependabot.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)       33 2024-05-07 15:31:16.000000 cccs_yara-2.4/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-07 15:31:16.000000 cccs_yara-2.4/.gitmodules
+-rw-r--r--   0 vsts      (1001) docker     (127)     9638 2024-05-07 15:31:16.000000 cccs_yara-2.4/CCCS_YARA.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)     7912 2024-05-07 15:31:16.000000 cccs_yara-2.4/CCCS_YARA_values.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1401 2024-05-07 15:31:16.000000 cccs_yara-2.4/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)    12345 2024-05-07 15:31:22.634491 cccs_yara-2.4/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)    11926 2024-05-07 15:31:16.000000 cccs_yara-2.4/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 15:31:22.630491 cccs_yara-2.4/cccs_yara.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    12345 2024-05-07 15:31:22.000000 cccs_yara-2.4/cccs_yara.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      860 2024-05-07 15:31:22.000000 cccs_yara-2.4/cccs_yara.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-07 15:31:22.000000 cccs_yara-2.4/cccs_yara.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       59 2024-05-07 15:31:22.000000 cccs_yara-2.4/cccs_yara.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      127 2024-05-07 15:31:22.000000 cccs_yara-2.4/cccs_yara.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-05-07 15:31:22.000000 cccs_yara-2.4/cccs_yara.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 15:31:22.630491 cccs_yara-2.4/pipelines/
+-rw-r--r--   0 vsts      (1001) docker     (127)      785 2024-05-07 15:31:16.000000 cccs_yara-2.4/pipelines/publish.yaml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1259 2024-05-07 15:31:16.000000 cccs_yara-2.4/pipelines/test.yaml
+-rw-r--r--   0 vsts      (1001) docker     (127)      127 2024-05-07 15:31:16.000000 cccs_yara-2.4/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      785 2024-05-07 15:31:16.000000 cccs_yara-2.4/settings.json
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-07 15:31:22.634491 cccs_yara-2.4/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      688 2024-05-07 15:31:16.000000 cccs_yara-2.4/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 15:31:22.630491 cccs_yara-2.4/templates/
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-05-07 15:31:16.000000 cccs_yara-2.4/templates/CCCS_Yara_Template.yara
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 15:31:22.630491 cccs_yara-2.4/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)        7 2024-05-07 15:31:16.000000 cccs_yara-2.4/tests/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     1609 2024-05-07 15:31:16.000000 cccs_yara-2.4/tests/test_run_yara_validator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 15:31:22.630491 cccs_yara-2.4/yara_validator/
+-rw-r--r--   0 vsts      (1001) docker     (127)     9638 2024-05-07 15:31:16.000000 cccs_yara-2.4/yara_validator/CCCS_YARA.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)     7912 2024-05-07 15:31:16.000000 cccs_yara-2.4/yara_validator/CCCS_YARA_values.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)       34 2024-05-07 15:31:16.000000 cccs_yara-2.4/yara_validator/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-07 15:31:16.000000 cccs_yara-2.4/yara_validator/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14526 2024-05-07 15:31:16.000000 cccs_yara-2.4/yara_validator/cli.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      556 2024-05-07 15:31:16.000000 cccs_yara-2.4/yara_validator/constants.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 15:31:22.630491 cccs_yara-2.4/yara_validator/stix2_patch/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-07 15:31:16.000000 cccs_yara-2.4/yara_validator/stix2_patch/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1167 2024-05-07 15:31:16.000000 cccs_yara-2.4/yara_validator/stix2_patch/filter_casefold.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43530 2024-05-07 15:31:16.000000 cccs_yara-2.4/yara_validator/validator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-05-07 15:31:16.000000 cccs_yara-2.4/yara_validator/validator_cfg.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)    41350 2024-05-07 15:31:16.000000 cccs_yara-2.4/yara_validator/validator_functions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30243 2024-05-07 15:31:16.000000 cccs_yara-2.4/yara_validator/yara_file_processor.py
```

### Comparing `cccs-yara-2.3/CCCS_YARA.yml` & `cccs_yara-2.4/CCCS_YARA.yml`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.3/CCCS_YARA_values.yml` & `cccs_yara-2.4/CCCS_YARA_values.yml`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.3/LICENSE` & `cccs_yara-2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.3/PKG-INFO` & `cccs_yara-2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cccs-yara
-Version: 2.3
+Version: 2.4
 Summary: A CCCS utility for YARA rule metadata validation
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: clint>=0.5.1
 Requires-Dist: GitPython>=3.1.0
 Requires-Dist: packaging>=19.0
 Requires-Dist: plyara>=2.1.1
```

### Comparing `cccs-yara-2.3/README.md` & `cccs_yara-2.4/README.md`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.3/cccs_yara.egg-info/PKG-INFO` & `cccs_yara-2.4/cccs_yara.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cccs-yara
-Version: 2.3
+Version: 2.4
 Summary: A CCCS utility for YARA rule metadata validation
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: clint>=0.5.1
 Requires-Dist: GitPython>=3.1.0
 Requires-Dist: packaging>=19.0
 Requires-Dist: plyara>=2.1.1
```

### Comparing `cccs-yara-2.3/pipelines/publish.yaml` & `cccs_yara-2.4/pipelines/publish.yaml`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.3/settings.json` & `cccs_yara-2.4/settings.json`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.3/setup.py` & `cccs_yara-2.4/setup.py`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.3/yara_validator/CCCS_YARA.yml` & `cccs_yara-2.4/yara_validator/CCCS_YARA.yml`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.3/yara_validator/CCCS_YARA_values.yml` & `cccs_yara-2.4/yara_validator/CCCS_YARA_values.yml`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.3/yara_validator/cli.py` & `cccs_yara-2.4/yara_validator/cli.py`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.3/yara_validator/constants.py` & `cccs_yara-2.4/yara_validator/constants.py`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.3/yara_validator/stix2_patch/filter_casefold.py` & `cccs_yara-2.4/yara_validator/stix2_patch/filter_casefold.py`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.3/yara_validator/validator.py` & `cccs_yara-2.4/yara_validator/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,29 +135,27 @@
 
     if not check_encoding(yara_file_processor.return_original_rule(),
                           validator_configuration.get(STRING_ENCODING).get(VALUE)):
         file_response = 'Some characters present in file are not:\t{!r}'\
             .format(str(validator_configuration.get(STRING_ENCODING).get(VALUE)))
         yara_file_processor.update_file_error(True, str(yara_file_processor.original_rule_file.name), file_response)
         return yara_file_processor
-    
+
     with open(CONFIG_VALUES_YAML_PATH, 'r', encoding='utf8') as yaml_file:
         scheme = yaml.safe_load(yaml_file)
 
     with open(CONFIG_YAML_PATH, 'r', encoding='utf8') as config_file:
         yara_config = yaml.safe_load(config_file)
 
     validator = YaraValidator(MITRE_STIX_DATA_PATH, CONFIG_YAML_PATH, CONFIG_VALUES_YAML_PATH, yara_config, scheme)
 
     for rule in yara_file_processor.yara_rules:
         try:
+            validator.reset()
             rule.add_rule_return(validator.validation(rule.rule_plyara, rule.rule_string, generate_values))
-            # reset the counter here since we are evaluating 'per rule' 
-            for key, value in validator.required_fields.items():
-                validator.required_fields_index[value.position].count = 0
         except Exception as e:
             raise Exception(
                 f"{rule.rule_plyara.get('rule_name', None)} produced the following exception: {str(e)}. Halting validation..")
 
     return yara_file_processor
 
 
@@ -415,14 +413,21 @@
             self.warning_no_category_type,
             self.warning_no_reference_specified,
             self.warning_common_metadata_errors
         ]
 
     previous_position_values = None
 
+    def reset(self):
+        # Reset back to factory settings for required field validation
+        for value in self.required_fields.values():
+            self.required_fields_index[value.position].count = 0
+            value.found = False
+            value.valid = False
+
     def reindex_metadata_keys(self):
         """
         Reindex the starting index of the positional objects contained in self.required_fields_index. This is so that
             the canonical order is maintained relative to optional and multiple instances of some metadata
         :return: none, it works on the self.required_fields_index and makes changes to that
         """
         previous_position_values = None
@@ -906,8 +911,7 @@
             self.required_fields[cfg_metadata] = self.read_yara_cfg(cfg_metadata, cfg_params,
                                                                     index)  # add a new MetadataAttributes instance
             # replace the name of child metadata with its place holder
             self.handle_child_parent_metadata(cfg_metadata, cfg_params, metadata_in_child_parent_relationship)
         # check if any metadata in child-parent relationship are missing
         self.validate_child_parent_metadata(self.yara_config, metadata_in_child_parent_relationship)
         self.metadata_keys_regex = self.metadata_keys_regex[:-1]
-
```

### Comparing `cccs-yara-2.3/yara_validator/validator_cfg.yml` & `cccs_yara-2.4/yara_validator/validator_cfg.yml`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.3/yara_validator/validator_functions.py` & `cccs_yara-2.4/yara_validator/validator_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,15 +317,15 @@
                 if Helper.validate_date(date):
                     self.required_fields[DATE].attributevalid()
                     update_metadata(date)
                 else:
                     # Date isn't in the expected format, let's see if we can convert it
                     success, formatted_date = convert_date(date)
                     if success and Helper.validate_date(formatted_date):
-                        self.required_fields[DATE].attibutevalid()
+                        self.required_fields[DATE].attributevalid()
                         update_metadata(date, force=True)
                     else:
                         self.required_fields[DATE].attributeinvalid()
             else:
                 rule_date = {DATE: Helper.current_valid_date()}
                 rule_to_date_check[METADATA].insert(metadata_index, rule_date)
                 self.required_fields[DATE].attributevalid()
```

### Comparing `cccs-yara-2.3/yara_validator/yara_file_processor.py` & `cccs_yara-2.4/yara_validator/yara_file_processor.py`

 * *Files identical despite different names*

