# Comparing `tmp/aepp-0.3.4.post1.tar.gz` & `tmp/aepp-0.3.4.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aepp-0.3.4.post1.tar", last modified: Tue Apr  2 10:50:42 2024, max compression
+gzip compressed data, was "aepp-0.3.4.post2.tar", last modified: Tue May  7 13:42:31 2024, max compression
```

## Comparing `aepp-0.3.4.post1.tar` & `aepp-0.3.4.post2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 10:50:42.118875 aepp-0.3.4.post1/
--rw-rw-rw-   0        0        0    10337 2023-05-10 18:38:24.000000 aepp-0.3.4.post1/LICENSE
--rw-rw-rw-   0        0        0       16 2023-05-10 18:38:24.000000 aepp-0.3.4.post1/MANIFEST.in
--rw-rw-rw-   0        0        0     4274 2024-04-02 10:50:42.118875 aepp-0.3.4.post1/PKG-INFO
--rw-rw-rw-   0        0        0     3457 2024-03-18 13:57:44.000000 aepp-0.3.4.post1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 10:50:42.053016 aepp-0.3.4.post1/aepp/
--rw-rw-rw-   0        0        0     5224 2023-05-10 18:04:54.000000 aepp-0.3.4.post1/aepp/__init__.py
--rw-rw-rw-   0        0        0       25 2024-03-25 07:12:28.000000 aepp-0.3.4.post1/aepp/__version__.py
--rw-rw-rw-   0        0        0    17426 2024-02-21 09:35:17.000000 aepp-0.3.4.post1/aepp/accesscontrol.py
--rw-rw-rw-   0        0        0    58818 2024-03-18 13:57:44.000000 aepp-0.3.4.post1/aepp/catalog.py
--rw-rw-rw-   0        0        0     2579 2024-03-18 13:57:44.000000 aepp-0.3.4.post1/aepp/config.py
--rw-rw-rw-   0        0        0    17655 2024-02-21 09:35:17.000000 aepp-0.3.4.post1/aepp/configs.py
--rw-rw-rw-   0        0        0    30251 2024-03-20 09:24:20.000000 aepp-0.3.4.post1/aepp/connector.py
--rw-rw-rw-   0        0        0    42510 2024-02-21 09:35:17.000000 aepp-0.3.4.post1/aepp/customerprofile.py
--rw-rw-rw-   0        0        0    14252 2023-11-02 07:50:23.000000 aepp-0.3.4.post1/aepp/dataaccess.py
--rw-rw-rw-   0        0        0    27357 2023-11-02 07:50:23.000000 aepp-0.3.4.post1/aepp/dataprep.py
--rw-rw-rw-   0        0        0     8778 2023-11-02 07:50:23.000000 aepp-0.3.4.post1/aepp/datasets.py
--rw-rw-rw-   0        0        0    24348 2023-11-02 07:50:23.000000 aepp-0.3.4.post1/aepp/destination.py
--rw-rw-rw-   0        0        0     5378 2023-11-02 07:50:23.000000 aepp-0.3.4.post1/aepp/destinationinstanceservice.py
--rw-rw-rw-   0        0        0    18629 2023-09-28 14:47:02.000000 aepp-0.3.4.post1/aepp/exportDatasetToDataLandingZone.py
--rw-rw-rw-   0        0        0    76765 2023-12-04 09:42:32.000000 aepp-0.3.4.post1/aepp/flowservice.py
--rw-rw-rw-   0        0        0    13075 2024-03-18 13:57:44.000000 aepp-0.3.4.post1/aepp/hygiene.py
--rw-rw-rw-   0        0        0    20080 2024-02-21 09:35:17.000000 aepp-0.3.4.post1/aepp/identity.py
--rw-rw-rw-   0        0        0    21460 2024-03-25 07:12:28.000000 aepp-0.3.4.post1/aepp/ingestion.py
--rw-rw-rw-   0        0        0     9951 2023-11-02 07:50:23.000000 aepp-0.3.4.post1/aepp/observability.py
--rw-rw-rw-   0        0        0    24930 2023-11-02 07:50:23.000000 aepp-0.3.4.post1/aepp/policy.py
--rw-rw-rw-   0        0        0     8794 2023-11-02 07:50:23.000000 aepp-0.3.4.post1/aepp/privacyservice.py
--rw-rw-rw-   0        0        0    52507 2023-11-02 07:50:24.000000 aepp-0.3.4.post1/aepp/queryservice.py
--rw-rw-rw-   0        0        0    21063 2023-11-02 07:50:24.000000 aepp-0.3.4.post1/aepp/sandboxes.py
--rw-rw-rw-   0        0        0   215461 2024-03-01 18:04:45.000000 aepp-0.3.4.post1/aepp/schema.py
--rw-rw-rw-   0        0        0    42269 2024-03-25 07:12:28.000000 aepp-0.3.4.post1/aepp/segmentation.py
--rw-rw-rw-   0        0        0     7761 2023-10-23 08:56:18.000000 aepp-0.3.4.post1/aepp/sensei.py
--rw-rw-rw-   0        0        0     1200 2023-10-23 08:56:14.000000 aepp-0.3.4.post1/aepp/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:50:42.118875 aepp-0.3.4.post1/aepp.egg-info/
--rw-rw-rw-   0        0        0     4274 2024-04-02 10:50:41.000000 aepp-0.3.4.post1/aepp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      928 2024-04-02 10:50:41.000000 aepp-0.3.4.post1/aepp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 10:50:41.000000 aepp-0.3.4.post1/aepp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-02 10:50:41.000000 aepp-0.3.4.post1/aepp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-02 10:50:41.000000 aepp-0.3.4.post1/aepp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 10:50:42.118875 aepp-0.3.4.post1/setup.cfg
--rw-rw-rw-   0        0        0     2206 2023-11-23 12:55:39.000000 aepp-0.3.4.post1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:50:42.113944 aepp-0.3.4.post1/tests/
--rw-rw-rw-   0        0        0      623 2023-05-10 18:04:54.000000 aepp-0.3.4.post1/tests/__init__.py
--rw-rw-rw-   0        0        0     2246 2023-05-10 18:04:54.000000 aepp-0.3.4.post1/tests/catalog_test.py
--rw-rw-rw-   0        0        0     1238 2023-05-10 18:04:54.000000 aepp-0.3.4.post1/tests/dataaccess_test.py
--rw-rw-rw-   0        0        0     1093 2023-05-10 18:04:54.000000 aepp-0.3.4.post1/tests/datasets_test.py
--rw-rw-rw-   0        0        0     2105 2023-05-23 14:25:29.000000 aepp-0.3.4.post1/tests/destinationinstanceservice_test.py
--rw-rw-rw-   0        0        0     7684 2023-09-28 14:47:02.000000 aepp-0.3.4.post1/tests/exportDatasetToDatalandingZone_test.py
--rw-rw-rw-   0        0        0     4208 2023-05-10 18:04:54.000000 aepp-0.3.4.post1/tests/flowservice_test.py
--rw-rw-rw-   0        0        0     2774 2023-05-10 18:04:54.000000 aepp-0.3.4.post1/tests/schema_test.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:42:31.142091 aepp-0.3.4.post2/
+-rw-rw-rw-   0        0        0    10337 2023-05-10 18:38:24.000000 aepp-0.3.4.post2/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-05-10 18:38:24.000000 aepp-0.3.4.post2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4274 2024-05-07 13:42:31.126465 aepp-0.3.4.post2/PKG-INFO
+-rw-rw-rw-   0        0        0     3457 2024-03-18 13:57:44.000000 aepp-0.3.4.post2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 13:42:31.073678 aepp-0.3.4.post2/aepp/
+-rw-rw-rw-   0        0        0     5224 2023-05-10 18:04:54.000000 aepp-0.3.4.post2/aepp/__init__.py
+-rw-rw-rw-   0        0        0       25 2024-05-07 13:39:17.000000 aepp-0.3.4.post2/aepp/__version__.py
+-rw-rw-rw-   0        0        0    17426 2024-02-21 09:35:17.000000 aepp-0.3.4.post2/aepp/accesscontrol.py
+-rw-rw-rw-   0        0        0    58818 2024-03-18 13:57:44.000000 aepp-0.3.4.post2/aepp/catalog.py
+-rw-rw-rw-   0        0        0     2579 2024-03-18 13:57:44.000000 aepp-0.3.4.post2/aepp/config.py
+-rw-rw-rw-   0        0        0    17655 2024-02-21 09:35:17.000000 aepp-0.3.4.post2/aepp/configs.py
+-rw-rw-rw-   0        0        0    30327 2024-04-26 09:38:20.000000 aepp-0.3.4.post2/aepp/connector.py
+-rw-rw-rw-   0        0        0    42510 2024-02-21 09:35:17.000000 aepp-0.3.4.post2/aepp/customerprofile.py
+-rw-rw-rw-   0        0        0    14252 2023-11-02 07:50:23.000000 aepp-0.3.4.post2/aepp/dataaccess.py
+-rw-rw-rw-   0        0        0    27357 2023-11-02 07:50:23.000000 aepp-0.3.4.post2/aepp/dataprep.py
+-rw-rw-rw-   0        0        0     8778 2023-11-02 07:50:23.000000 aepp-0.3.4.post2/aepp/datasets.py
+-rw-rw-rw-   0        0        0    24348 2023-11-02 07:50:23.000000 aepp-0.3.4.post2/aepp/destination.py
+-rw-rw-rw-   0        0        0     5378 2023-11-02 07:50:23.000000 aepp-0.3.4.post2/aepp/destinationinstanceservice.py
+-rw-rw-rw-   0        0        0    18629 2023-09-28 14:47:02.000000 aepp-0.3.4.post2/aepp/exportDatasetToDataLandingZone.py
+-rw-rw-rw-   0        0        0    76727 2024-05-07 13:37:57.000000 aepp-0.3.4.post2/aepp/flowservice.py
+-rw-rw-rw-   0        0        0    13075 2024-03-18 13:57:44.000000 aepp-0.3.4.post2/aepp/hygiene.py
+-rw-rw-rw-   0        0        0    20080 2024-02-21 09:35:17.000000 aepp-0.3.4.post2/aepp/identity.py
+-rw-rw-rw-   0        0        0    21460 2024-03-25 07:12:28.000000 aepp-0.3.4.post2/aepp/ingestion.py
+-rw-rw-rw-   0        0        0     9951 2023-11-02 07:50:23.000000 aepp-0.3.4.post2/aepp/observability.py
+-rw-rw-rw-   0        0        0    24930 2023-11-02 07:50:23.000000 aepp-0.3.4.post2/aepp/policy.py
+-rw-rw-rw-   0        0        0     8794 2023-11-02 07:50:23.000000 aepp-0.3.4.post2/aepp/privacyservice.py
+-rw-rw-rw-   0        0        0    52507 2023-11-02 07:50:24.000000 aepp-0.3.4.post2/aepp/queryservice.py
+-rw-rw-rw-   0        0        0    21063 2024-04-11 15:08:07.000000 aepp-0.3.4.post2/aepp/sandboxes.py
+-rw-rw-rw-   0        0        0   215461 2024-04-22 12:03:10.000000 aepp-0.3.4.post2/aepp/schema.py
+-rw-rw-rw-   0        0        0    42377 2024-04-02 14:45:01.000000 aepp-0.3.4.post2/aepp/segmentation.py
+-rw-rw-rw-   0        0        0     7761 2023-10-23 08:56:18.000000 aepp-0.3.4.post2/aepp/sensei.py
+-rw-rw-rw-   0        0        0     1200 2023-10-23 08:56:14.000000 aepp-0.3.4.post2/aepp/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:42:31.126465 aepp-0.3.4.post2/aepp.egg-info/
+-rw-rw-rw-   0        0        0     4274 2024-05-07 13:42:30.000000 aepp-0.3.4.post2/aepp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      928 2024-05-07 13:42:30.000000 aepp-0.3.4.post2/aepp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 13:42:30.000000 aepp-0.3.4.post2/aepp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-07 13:42:30.000000 aepp-0.3.4.post2/aepp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-07 13:42:30.000000 aepp-0.3.4.post2/aepp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 13:42:31.142091 aepp-0.3.4.post2/setup.cfg
+-rw-rw-rw-   0        0        0     2206 2023-11-23 12:55:39.000000 aepp-0.3.4.post2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:42:31.126465 aepp-0.3.4.post2/tests/
+-rw-rw-rw-   0        0        0      623 2023-05-10 18:04:54.000000 aepp-0.3.4.post2/tests/__init__.py
+-rw-rw-rw-   0        0        0     2246 2023-05-10 18:04:54.000000 aepp-0.3.4.post2/tests/catalog_test.py
+-rw-rw-rw-   0        0        0     1238 2023-05-10 18:04:54.000000 aepp-0.3.4.post2/tests/dataaccess_test.py
+-rw-rw-rw-   0        0        0     1093 2023-05-10 18:04:54.000000 aepp-0.3.4.post2/tests/datasets_test.py
+-rw-rw-rw-   0        0        0     2105 2023-05-23 14:25:29.000000 aepp-0.3.4.post2/tests/destinationinstanceservice_test.py
+-rw-rw-rw-   0        0        0     7684 2023-09-28 14:47:02.000000 aepp-0.3.4.post2/tests/exportDatasetToDatalandingZone_test.py
+-rw-rw-rw-   0        0        0     4208 2023-05-10 18:04:54.000000 aepp-0.3.4.post2/tests/flowservice_test.py
+-rw-rw-rw-   0        0        0     2774 2023-05-10 18:04:54.000000 aepp-0.3.4.post2/tests/schema_test.py
```

### Comparing `aepp-0.3.4.post1/LICENSE` & `aepp-0.3.4.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/PKG-INFO` & `aepp-0.3.4.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aepp
-Version: 0.3.4.post1
+Version: 0.3.4.post2
 Summary: Package to manage AEP API endpoint and some helper functions
 Home-page: https://github.com/adobe/aepp
 Author: Julien Piccini
 Author-email: piccini.julien@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `aepp-0.3.4.post1/README.md` & `aepp-0.3.4.post2/README.md`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/aepp/__init__.py` & `aepp-0.3.4.post2/aepp/__init__.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/aepp/accesscontrol.py` & `aepp-0.3.4.post2/aepp/accesscontrol.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/aepp/catalog.py` & `aepp-0.3.4.post2/aepp/catalog.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/aepp/config.py` & `aepp-0.3.4.post2/aepp/config.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/aepp/configs.py` & `aepp-0.3.4.post2/aepp/configs.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/aepp/connector.py` & `aepp-0.3.4.post2/aepp/connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,14 +116,15 @@
             self.config["date_limit"] = (
                 time.time() + token_info.expiry / timeScale - 500
             )
             self.header.update({"Authorization": f"Bearer {self.token}"})
         else:
             self.token = self.config["token"]
             self.header.update({"Authorization": f"Bearer {self.token}"})
+            self.header.update({"x-sandbox-name": self.config['sandbox']})
             self.connectionType = self.config['connectionType']
         # x-sandbox-id is required when using non-user token, but forbidden for user token
         if self.connectionType == 'oauthV1' and "x-sandbox-id" not in self.header:
             self.update_sandbox_id(self.config["sandbox"])
 
     def _find_path(self, path: str) -> Optional[Path]:
         """Checks if the file denoted by the specified `path` exists and returns the Path object
```

### Comparing `aepp-0.3.4.post1/aepp/customerprofile.py` & `aepp-0.3.4.post2/aepp/customerprofile.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/aepp/dataaccess.py` & `aepp-0.3.4.post2/aepp/dataaccess.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/aepp/dataprep.py` & `aepp-0.3.4.post2/aepp/dataprep.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/aepp/datasets.py` & `aepp-0.3.4.post2/aepp/datasets.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/aepp/destination.py` & `aepp-0.3.4.post2/aepp/destination.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/aepp/destinationinstanceservice.py` & `aepp-0.3.4.post2/aepp/destinationinstanceservice.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/aepp/exportDatasetToDataLandingZone.py` & `aepp-0.3.4.post2/aepp/exportDatasetToDataLandingZone.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/aepp/flowservice.py` & `aepp-0.3.4.post2/aepp/flowservice.py`

 * *Files 0% similar despite different names*

```diff
@@ -1656,16 +1656,16 @@
                 myIndex=index
                 operation['mappingId'] = mappingId
                 operation['mappingVersion'] = myVersion
         if myIndex is not None:
             patchOperation = [{'op': 'replace',
             'path': f'/transformations/{myIndex}',
             'value': {'name': 'Mapping',
-            'params': {'mappingId': operation['params']['mappingId'],
-            'mappingVersion': operation['params']['mappingVersion']}}}
+            'params': {'mappingId': operation['mappingId'],
+            'mappingVersion': operation['mappingVersion']}}}
             ]
         else:
             raise Exception('Could not find a mapping transformation in the flow')
-        res = self.updateFlow(self.id,self.etag,patchOperation)
+        res = self.updateFlow(patchOperation)
         self.flowData = res
         self.__setAttributes__(res)
         return res
```

### Comparing `aepp-0.3.4.post1/aepp/hygiene.py` & `aepp-0.3.4.post2/aepp/hygiene.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/aepp/identity.py` & `aepp-0.3.4.post2/aepp/identity.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/aepp/ingestion.py` & `aepp-0.3.4.post2/aepp/ingestion.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/aepp/observability.py` & `aepp-0.3.4.post2/aepp/observability.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/aepp/policy.py` & `aepp-0.3.4.post2/aepp/policy.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/aepp/privacyservice.py` & `aepp-0.3.4.post2/aepp/privacyservice.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/aepp/queryservice.py` & `aepp-0.3.4.post2/aepp/queryservice.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/aepp/sandboxes.py` & `aepp-0.3.4.post2/aepp/sandboxes.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     It comes from the sandbox API:
     https://www.adobe.io/apis/experienceplatform/home/api-reference.html#!acpdr/swagger-specs/sandbox-api.yaml
     """
 
     ## logging capability
     loggingEnabled = False
     logger = None
-    ARTIFACS_Type = ["REGISTRY_SCHEMA","MAPPING_SET","CATALOG_DATASET","JOURNEY","PROFILE_SEGMENT"]
+    ARTIFACS_TYPE = ["REGISTRY_SCHEMA","MAPPING_SET","CATALOG_DATASET","JOURNEY","PROFILE_SEGMENT"]
 
     def __init__(
         self,
         config: Union[dict,ConnectObject] = aepp.config.config_object,
         header: dict = aepp.config.header,
         loggingObject: dict = None,
         **kwargs,
@@ -273,15 +273,15 @@
             name : REQUIRED : Name of the package.
             description : OPTIONAL : Description of the package
             fullPackage : OPTIONAL : If you want to copy the whole sandbox. (default False)
             artefacts : OPTIONAL : If you set fullPackage to False, then you need to provide a dictionary of items with their type.
                 example : 
                 {"27115daa-c92b-4f17-a077-d65ffeb0c525":"PROFILE_SEGMENT",
                 "d8d8ed6d-696a-40bd-b4fe-ca053ec94e29" : "JOURNEY"}
-                For more types, refers to ARTIFACS_Type 
+                For more types, refers to ARTIFACS_TYPE 
             expiry : OPTIONAL : The expiry of that package in days (default 90 days)
         """
         if self.loggingEnabled:
             self.logger.debug(f"Starting createPackage")
         delta90days = datetime.timedelta(days=expiry)
         now = datetime.datetime.now()
         now90days = now + delta90days
@@ -405,15 +405,15 @@
         Arguments:
             packageId : REQUIRED : The package ID to be imported
             targetSandbox : REQUIRED : The Target sandbox to be used
             alternatives : OPTIONAL : A dictionary, a map, of artifacts existing in your package that already exists in the targeted sandboxes.
                 example of alternative dictionary: 
                     {"artifactIdInPackage": {
                         "id": "targetSandboxArtifactId"
-                        "type" : "REGISTRY_SCHEMA" (refer to ARTIFACS_Type for more types)
+                        "type" : "REGISTRY_SCHEMA" (refer to ARTIFACS_TYPE for more types)
                         }
                     }
         """
         if packageId is None:
             raise ValueError("Requires a package ID to be specified")
         if targetSandbox is None:
             raise ValueError("Requires a target sandbox to be specified")
```

### Comparing `aepp-0.3.4.post1/aepp/schema.py` & `aepp-0.3.4.post2/aepp/schema.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/aepp/segmentation.py` & `aepp-0.3.4.post2/aepp/segmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -932,14 +932,15 @@
 
     def extractPaths(self,audience:Union[dict,str]=None,recursive:bool=False)->list:
         """
         BETA
         Extract the schema paths present in the segment or audience definition.
         Argument:
             audience : REQUIRED : Audience or segment definition.
+            recursive : OPTIONAL : If you want to check the path used in the audience used in the audience
         """
         if audience is None:
             raise ValueError("require an audience or segment definition")
         if type(audience) == str:
             audience = self.getAudience(audience)
         formatt = audience.get('expression',{}).get('format')
         if formatt == 'pql/text':
```

### Comparing `aepp-0.3.4.post1/aepp/sensei.py` & `aepp-0.3.4.post2/aepp/sensei.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/aepp/utils.py` & `aepp-0.3.4.post2/aepp/utils.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/aepp.egg-info/PKG-INFO` & `aepp-0.3.4.post2/aepp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aepp
-Version: 0.3.4.post1
+Version: 0.3.4.post2
 Summary: Package to manage AEP API endpoint and some helper functions
 Home-page: https://github.com/adobe/aepp
 Author: Julien Piccini
 Author-email: piccini.julien@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `aepp-0.3.4.post1/aepp.egg-info/SOURCES.txt` & `aepp-0.3.4.post2/aepp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/setup.py` & `aepp-0.3.4.post2/setup.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/tests/__init__.py` & `aepp-0.3.4.post2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/tests/catalog_test.py` & `aepp-0.3.4.post2/tests/catalog_test.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/tests/dataaccess_test.py` & `aepp-0.3.4.post2/tests/dataaccess_test.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/tests/datasets_test.py` & `aepp-0.3.4.post2/tests/datasets_test.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/tests/destinationinstanceservice_test.py` & `aepp-0.3.4.post2/tests/destinationinstanceservice_test.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/tests/exportDatasetToDatalandingZone_test.py` & `aepp-0.3.4.post2/tests/exportDatasetToDatalandingZone_test.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/tests/flowservice_test.py` & `aepp-0.3.4.post2/tests/flowservice_test.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4.post1/tests/schema_test.py` & `aepp-0.3.4.post2/tests/schema_test.py`

 * *Files identical despite different names*

