# Comparing `tmp/datamaker-sdk-0.6.tar.gz` & `tmp/datamaker_sdk-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamaker-sdk-0.6.tar", last modified: Wed Oct 18 02:10:31 2023, max compression
+gzip compressed data, was "datamaker_sdk-0.9.tar", last modified: Tue May  7 04:38:36 2024, max compression
```

## Comparing `datamaker-sdk-0.6.tar` & `datamaker_sdk-0.9.tar`

### file list

```diff
@@ -1,41 +1,37 @@
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-10-18 02:10:31.324357 datamaker-sdk-0.6/
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-10-18 02:10:31.316357 datamaker-sdk-0.6/.github/
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-10-18 02:10:31.320357 datamaker-sdk-0.6/.github/workflows/
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      233 2023-08-03 00:15:32.000000 datamaker-sdk-0.6/.github/workflows/lint.yml
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1131 2023-08-03 00:15:32.000000 datamaker-sdk-0.6/.github/workflows/python-publish.yml
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      221 2023-06-15 08:58:52.000000 datamaker-sdk-0.6/.gitignore
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      276 2023-08-03 00:15:32.000000 datamaker-sdk-0.6/.pre-commit-config.yaml
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1101 2023-06-15 08:58:52.000000 datamaker-sdk-0.6/LICENSE
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1051 2023-10-18 02:10:31.324357 datamaker-sdk-0.6/PKG-INFO
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)        0 2023-06-15 08:58:52.000000 datamaker-sdk-0.6/README.md
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-10-18 02:10:31.320357 datamaker-sdk-0.6/datamaker/
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)        0 2023-06-15 08:58:52.000000 datamaker-sdk-0.6/datamaker/__init__.py
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-10-18 02:10:31.320357 datamaker-sdk-0.6/datamaker/client/
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     3599 2023-08-03 00:15:32.000000 datamaker-sdk-0.6/datamaker/client/__init__.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      405 2023-06-15 08:58:52.000000 datamaker-sdk-0.6/datamaker/client/exceptions.py
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-10-18 02:10:31.320357 datamaker-sdk-0.6/datamaker/client/mixins/
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)        0 2023-06-15 08:58:52.000000 datamaker-sdk-0.6/datamaker/client/mixins/__init__.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1042 2023-08-03 00:15:32.000000 datamaker-sdk-0.6/datamaker/client/mixins/annotation.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     4167 2023-10-18 02:10:23.000000 datamaker-sdk-0.6/datamaker/client/mixins/dataset.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      242 2023-08-03 00:15:32.000000 datamaker-sdk-0.6/datamaker/client/mixins/hitl.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      846 2023-10-18 02:10:23.000000 datamaker-sdk-0.6/datamaker/client/mixins/integration.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      938 2023-08-03 00:15:32.000000 datamaker-sdk-0.6/datamaker/client/mixins/ml.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      445 2023-08-03 00:15:32.000000 datamaker-sdk-0.6/datamaker/client/utils.py
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-10-18 02:10:31.320357 datamaker-sdk-0.6/datamaker/plugins/
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1049 2023-06-15 08:58:52.000000 datamaker-sdk-0.6/datamaker/plugins/__init__.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1676 2023-06-15 08:58:52.000000 datamaker-sdk-0.6/datamaker/plugins/exports.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1946 2023-09-05 00:30:04.000000 datamaker-sdk-0.6/datamaker/plugins/imports.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     7035 2023-08-03 00:15:32.000000 datamaker-sdk-0.6/datamaker/plugins/neural_networks.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      455 2023-06-15 08:58:52.000000 datamaker-sdk-0.6/datamaker/plugins/preprocessors.py
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-10-18 02:10:31.320357 datamaker-sdk-0.6/datamaker/utils/
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)        0 2023-06-15 08:58:52.000000 datamaker-sdk-0.6/datamaker/utils/__init__.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     2000 2023-08-03 00:15:32.000000 datamaker-sdk-0.6/datamaker/utils/file.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1434 2023-08-03 00:15:32.000000 datamaker-sdk-0.6/datamaker/utils/logger.py
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-10-18 02:10:31.324357 datamaker-sdk-0.6/datamaker_sdk.egg-info/
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1051 2023-10-18 02:10:31.000000 datamaker-sdk-0.6/datamaker_sdk.egg-info/PKG-INFO
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      881 2023-10-18 02:10:31.000000 datamaker-sdk-0.6/datamaker_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)        1 2023-10-18 02:10:31.000000 datamaker-sdk-0.6/datamaker_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      106 2023-10-18 02:10:31.000000 datamaker-sdk-0.6/datamaker_sdk.egg-info/requires.txt
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)       10 2023-10-18 02:10:31.000000 datamaker-sdk-0.6/datamaker_sdk.egg-info/top_level.txt
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      341 2023-08-03 00:15:32.000000 datamaker-sdk-0.6/pyproject.toml
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1004 2023-10-18 02:10:31.324357 datamaker-sdk-0.6/setup.cfg
+drwxr-xr-x   0 yueunjeong   (501) staff       (20)        0 2024-05-07 04:38:36.175701 datamaker_sdk-0.9/
+-rw-r--r--   0 yueunjeong   (501) staff       (20)     1101 2024-04-03 08:07:59.000000 datamaker_sdk-0.9/LICENSE
+-rw-r--r--   0 yueunjeong   (501) staff       (20)     1051 2024-05-07 04:38:36.175635 datamaker_sdk-0.9/PKG-INFO
+-rw-r--r--   0 yueunjeong   (501) staff       (20)        0 2024-04-03 08:07:59.000000 datamaker_sdk-0.9/README.md
+drwxr-xr-x   0 yueunjeong   (501) staff       (20)        0 2024-05-07 04:38:36.169096 datamaker_sdk-0.9/datamaker/
+-rw-r--r--   0 yueunjeong   (501) staff       (20)        0 2024-04-03 08:07:59.000000 datamaker_sdk-0.9/datamaker/__init__.py
+drwxr-xr-x   0 yueunjeong   (501) staff       (20)        0 2024-05-07 04:38:36.170836 datamaker_sdk-0.9/datamaker/client/
+-rw-r--r--   0 yueunjeong   (501) staff       (20)     3599 2024-04-03 08:07:59.000000 datamaker_sdk-0.9/datamaker/client/__init__.py
+-rw-r--r--   0 yueunjeong   (501) staff       (20)      405 2024-04-03 08:07:59.000000 datamaker_sdk-0.9/datamaker/client/exceptions.py
+drwxr-xr-x   0 yueunjeong   (501) staff       (20)        0 2024-05-07 04:38:36.172705 datamaker_sdk-0.9/datamaker/client/mixins/
+-rw-r--r--   0 yueunjeong   (501) staff       (20)        0 2024-04-03 08:07:59.000000 datamaker_sdk-0.9/datamaker/client/mixins/__init__.py
+-rw-r--r--   0 yueunjeong   (501) staff       (20)     1042 2024-04-15 05:46:39.000000 datamaker_sdk-0.9/datamaker/client/mixins/annotation.py
+-rw-r--r--   0 yueunjeong   (501) staff       (20)     4097 2024-04-03 08:08:13.000000 datamaker_sdk-0.9/datamaker/client/mixins/dataset.py
+-rw-r--r--   0 yueunjeong   (501) staff       (20)      398 2024-05-03 04:02:10.000000 datamaker_sdk-0.9/datamaker/client/mixins/hitl.py
+-rw-r--r--   0 yueunjeong   (501) staff       (20)      846 2024-04-03 08:07:59.000000 datamaker_sdk-0.9/datamaker/client/mixins/integration.py
+-rw-r--r--   0 yueunjeong   (501) staff       (20)      938 2024-04-03 08:07:59.000000 datamaker_sdk-0.9/datamaker/client/mixins/ml.py
+-rw-r--r--   0 yueunjeong   (501) staff       (20)      445 2024-04-03 08:07:59.000000 datamaker_sdk-0.9/datamaker/client/utils.py
+drwxr-xr-x   0 yueunjeong   (501) staff       (20)        0 2024-05-07 04:38:36.173922 datamaker_sdk-0.9/datamaker/plugins/
+-rw-r--r--   0 yueunjeong   (501) staff       (20)     1154 2024-04-15 05:47:15.000000 datamaker_sdk-0.9/datamaker/plugins/__init__.py
+-rw-r--r--   0 yueunjeong   (501) staff       (20)     1676 2024-04-03 08:07:59.000000 datamaker_sdk-0.9/datamaker/plugins/exports.py
+-rw-r--r--   0 yueunjeong   (501) staff       (20)     1946 2024-04-03 08:17:08.000000 datamaker_sdk-0.9/datamaker/plugins/imports.py
+-rw-r--r--   0 yueunjeong   (501) staff       (20)     6989 2024-04-03 08:07:59.000000 datamaker_sdk-0.9/datamaker/plugins/neural_networks.py
+-rw-r--r--   0 yueunjeong   (501) staff       (20)      455 2024-04-03 08:07:59.000000 datamaker_sdk-0.9/datamaker/plugins/preprocessors.py
+drwxr-xr-x   0 yueunjeong   (501) staff       (20)        0 2024-05-07 04:38:36.174515 datamaker_sdk-0.9/datamaker/utils/
+-rw-r--r--   0 yueunjeong   (501) staff       (20)        0 2024-04-03 08:07:59.000000 datamaker_sdk-0.9/datamaker/utils/__init__.py
+-rw-r--r--   0 yueunjeong   (501) staff       (20)     2126 2024-04-03 08:08:13.000000 datamaker_sdk-0.9/datamaker/utils/file.py
+-rw-r--r--   0 yueunjeong   (501) staff       (20)     1434 2024-04-03 08:07:59.000000 datamaker_sdk-0.9/datamaker/utils/logger.py
+-rw-r--r--   0 yueunjeong   (501) staff       (20)      214 2024-04-03 08:08:13.000000 datamaker_sdk-0.9/datamaker/utils/string.py
+drwxr-xr-x   0 yueunjeong   (501) staff       (20)        0 2024-05-07 04:38:36.175344 datamaker_sdk-0.9/datamaker_sdk.egg-info/
+-rw-r--r--   0 yueunjeong   (501) staff       (20)     1051 2024-05-07 04:38:36.000000 datamaker_sdk-0.9/datamaker_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 yueunjeong   (501) staff       (20)      817 2024-05-07 04:38:36.000000 datamaker_sdk-0.9/datamaker_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 yueunjeong   (501) staff       (20)        1 2024-05-07 04:38:36.000000 datamaker_sdk-0.9/datamaker_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 yueunjeong   (501) staff       (20)      106 2024-05-07 04:38:36.000000 datamaker_sdk-0.9/datamaker_sdk.egg-info/requires.txt
+-rw-r--r--   0 yueunjeong   (501) staff       (20)       10 2024-05-07 04:38:36.000000 datamaker_sdk-0.9/datamaker_sdk.egg-info/top_level.txt
+-rw-r--r--   0 yueunjeong   (501) staff       (20)      439 2024-04-23 04:06:04.000000 datamaker_sdk-0.9/pyproject.toml
+-rw-r--r--   0 yueunjeong   (501) staff       (20)     1004 2024-05-07 04:38:36.175984 datamaker_sdk-0.9/setup.cfg
+-rw-r--r--   0 yueunjeong   (501) staff       (20)       38 2024-05-07 04:26:28.000000 datamaker_sdk-0.9/setup.py
```

### Comparing `datamaker-sdk-0.6/LICENSE` & `datamaker_sdk-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.6/PKG-INFO` & `datamaker_sdk-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamaker-sdk
-Version: 0.6
+Version: 0.9
 Summary: datamaker sdk
 Home-page: https://www.datamaker.io
 Author: datamaker
 Author-email: developer@datamaker.io
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datamaker-sdk-0.6/datamaker/client/__init__.py` & `datamaker_sdk-0.9/datamaker/client/__init__.py`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.6/datamaker/client/mixins/annotation.py` & `datamaker_sdk-0.9/datamaker/client/mixins/annotation.py`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.6/datamaker/client/mixins/dataset.py` & `datamaker_sdk-0.9/datamaker/client/mixins/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,21 +68,19 @@
                     batch_sequential.append(data_sequential)
 
             data_units = self.create_data_units(batch)
 
             if batch_sequential:
                 for data, data_unit in zip(batch_sequential, data_units):
                     for name, files in data.items():
-                        self.create_data_unit_files(
-                            {
-                                'data_unit': data_unit['id'],
-                                'name': name,
-                                'files': files,
-                            }
-                        )
+                        self.create_data_unit_files({
+                            'data_unit': data_unit['id'],
+                            'name': name,
+                            'files': files,
+                        })
 
             if project_id:
                 labels_data = []
                 for data, data_unit in zip(batch, data_units):
                     label_data = {
                         'project': project_id,
                         'data_unit': data_unit['id'],
```

### Comparing `datamaker-sdk-0.6/datamaker/client/mixins/integration.py` & `datamaker_sdk-0.9/datamaker/client/mixins/integration.py`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.6/datamaker/client/mixins/ml.py` & `datamaker_sdk-0.9/datamaker/client/mixins/ml.py`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.6/datamaker/plugins/__init__.py` & `datamaker_sdk-0.9/datamaker/plugins/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from datamaker.utils.logger import Logger
 
 
 class BasePlugin:
     base_path = None
     logger = None
     progress_prefix = ''
+    input_schema = None
 
     def __init__(self, logger=None, progress_prefix=None):
         self.base_path = Path(config.TEMP_ROOT) / 'service_executions' / generate()
         if progress_prefix:
             self.progress_prefix = progress_prefix
 
         if logger:
@@ -31,7 +32,11 @@
         self.logger.log(action, data)
 
     def log_message(self, message):
         self.logger.log('message', {'content': message})
 
     def end_log(self):
         self.log_message(_('작업이 완료되었습니다.'))
+
+    @classmethod
+    def get_input_schema(cls):
+        return cls.input_schema
```

### Comparing `datamaker-sdk-0.6/datamaker/plugins/exports.py` & `datamaker_sdk-0.9/datamaker/plugins/exports.py`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.6/datamaker/plugins/imports.py` & `datamaker_sdk-0.9/datamaker/plugins/imports.py`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.6/datamaker/plugins/neural_networks.py` & `datamaker_sdk-0.9/datamaker/plugins/neural_networks.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,21 +117,19 @@
         except KeyError:
             classification = None
 
         for category, dataset in input_dataset.items():
             configuration = copy.deepcopy(
                 self.input_dataset_conversion['configuration']
             )
-            configuration.update(
-                {
-                    'name': category,
-                    'classification': classification,
-                    'export_root': str(self.get_model_base_path()),
-                }
-            )
+            configuration.update({
+                'name': category,
+                'classification': classification,
+                'export_root': str(self.get_model_base_path()),
+            })
             export_plugin = self.export_plugin_class(
                 dataset,
                 len(dataset),
                 configuration,
                 logger=self.logger,
                 progress_prefix=category,
             )
```

### Comparing `datamaker-sdk-0.6/datamaker/utils/file.py` & `datamaker_sdk-0.9/datamaker/utils/file.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 from functools import reduce
 from pathlib import Path
 
 import requests
 from constance import config
 from django.core.files import File
 from django.core.files.temp import NamedTemporaryFile
+from datamaker.utils.string import remove_query_string
 
 
 def download_file(url, path_download, name=None, coerce=None):
+    url_parsed = Path(remove_query_string(url))
     if name:
-        name += Path(url).suffix
+        name += url_parsed.suffix
     else:
-        name = Path(url).name
+        name = url_parsed.name
 
     media_url = os.path.join(config.BACKEND_HOST, 'media/')
 
     if config.MEDIA_ROOT and url.startswith(media_url):
         path = Path(config.MEDIA_ROOT) / url.replace(media_url, '')
     else:
         path = path_download / name
@@ -57,14 +59,14 @@
 
 
 def get_file_from_url(url):
     r = requests.get(url, allow_redirects=True)
     file = NamedTemporaryFile(delete=True)
     file.write(r.content)
     file.flush()
-    return File(file, name=Path(url).name)
+    return File(file, name=Path(remove_query_string(url)).name)
 
 
 def json_default(value):
     if isinstance(value, Path):
         return str(value)
     raise TypeError
```

### Comparing `datamaker-sdk-0.6/datamaker/utils/logger.py` & `datamaker_sdk-0.9/datamaker/utils/logger.py`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.6/datamaker_sdk.egg-info/PKG-INFO` & `datamaker_sdk-0.9/datamaker_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamaker-sdk
-Version: 0.6
+Version: 0.9
 Summary: datamaker sdk
 Home-page: https://www.datamaker.io
 Author: datamaker
 Author-email: developer@datamaker.io
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datamaker-sdk-0.6/datamaker_sdk.egg-info/SOURCES.txt` & `datamaker_sdk-0.9/datamaker_sdk.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-.gitignore
-.pre-commit-config.yaml
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
-.github/workflows/lint.yml
-.github/workflows/python-publish.yml
+setup.py
 datamaker/__init__.py
 datamaker/client/__init__.py
 datamaker/client/exceptions.py
 datamaker/client/utils.py
 datamaker/client/mixins/__init__.py
 datamaker/client/mixins/annotation.py
 datamaker/client/mixins/dataset.py
@@ -20,12 +17,13 @@
 datamaker/plugins/exports.py
 datamaker/plugins/imports.py
 datamaker/plugins/neural_networks.py
 datamaker/plugins/preprocessors.py
 datamaker/utils/__init__.py
 datamaker/utils/file.py
 datamaker/utils/logger.py
+datamaker/utils/string.py
 datamaker_sdk.egg-info/PKG-INFO
 datamaker_sdk.egg-info/SOURCES.txt
 datamaker_sdk.egg-info/dependency_links.txt
 datamaker_sdk.egg-info/requires.txt
 datamaker_sdk.egg-info/top_level.txt
```

### Comparing `datamaker-sdk-0.6/setup.cfg` & `datamaker_sdk-0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = datamaker-sdk
-version = 0.6
+version = 0.9
 description = datamaker sdk
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.datamaker.io
 author = datamaker
 author_email = developer@datamaker.io
 license = MIT
```

