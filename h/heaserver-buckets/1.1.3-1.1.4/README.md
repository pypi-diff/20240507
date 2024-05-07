# Comparing `tmp/heaserver_buckets-1.1.3.tar.gz` & `tmp/heaserver_buckets-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver_buckets-1.1.3.tar", last modified: Sun May  5 20:32:19 2024, max compression
+gzip compressed data, was "heaserver_buckets-1.1.4.tar", last modified: Tue May  7 20:34:21 2024, max compression
```

## Comparing `heaserver_buckets-1.1.3.tar` & `heaserver_buckets-1.1.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 20:32:19.202571 heaserver_buckets-1.1.3/
--rw-rw-rw-   0        0        0      261 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.3/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.3/.gitignore
--rw-rw-rw-   0        0        0     1515 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.3/Dockerfile
--rw-rw-rw-   0        0        0    11625 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.3/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5302 2024-05-05 20:32:19.200446 heaserver_buckets-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3928 2024-05-05 20:26:22.000000 heaserver_buckets-1.1.3/README.md
--rw-rw-rw-   0        0        0     1737 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.3/RELEASING.md
--rw-rw-rw-   0        0        0      470 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.3/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-05-05 20:32:18.992541 heaserver_buckets-1.1.3/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-05-05 20:32:18.993543 heaserver_buckets-1.1.3/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-05 20:32:19.104812 heaserver_buckets-1.1.3/integrationtests/heaserver/bucketintegrationtest/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.3/integrationtests/heaserver/bucketintegrationtest/__init__.py
--rw-rw-rw-   0        0        0     4817 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.3/integrationtests/heaserver/bucketintegrationtest/test_all.py
--rw-rw-rw-   0        0        0    10927 2024-04-09 21:37:15.000000 heaserver_buckets-1.1.3/integrationtests/heaserver/bucketintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.3/pytest.ini
--rw-rw-rw-   0        0        0      262 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.3/requirements_dev.txt
--rw-rw-rw-   0        0        0     5310 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.3/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-05-05 20:32:19.203707 heaserver_buckets-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1858 2024-05-05 20:31:37.000000 heaserver_buckets-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 20:32:18.995609 heaserver_buckets-1.1.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-05 20:32:18.994542 heaserver_buckets-1.1.3/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-05 20:32:19.108825 heaserver_buckets-1.1.3/src/heaserver/bucket/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.3/src/heaserver/bucket/__init__.py
--rw-rw-rw-   0        0        0    73544 2024-04-03 03:36:32.000000 heaserver_buckets-1.1.3/src/heaserver/bucket/service.py
-drwxrwxrwx   0        0        0        0 2024-05-05 20:32:19.111814 heaserver_buckets-1.1.3/src/heaserver/bucket/wstl/
--rw-rw-rw-   0        0        0    14793 2024-04-09 21:37:15.000000 heaserver_buckets-1.1.3/src/heaserver/bucket/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-05-05 20:32:19.198858 heaserver_buckets-1.1.3/src/heaserver_buckets.egg-info/
--rw-rw-rw-   0        0        0     5302 2024-05-05 20:32:18.000000 heaserver_buckets-1.1.3/src/heaserver_buckets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      829 2024-05-05 20:32:18.000000 heaserver_buckets-1.1.3/src/heaserver_buckets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 20:32:18.000000 heaserver_buckets-1.1.3/src/heaserver_buckets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-05-05 20:32:18.000000 heaserver_buckets-1.1.3/src/heaserver_buckets.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2024-05-05 20:32:18.000000 heaserver_buckets-1.1.3/src/heaserver_buckets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-05 20:32:18.000000 heaserver_buckets-1.1.3/src/heaserver_buckets.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-05 20:32:18.995609 heaserver_buckets-1.1.3/tests/
-drwxrwxrwx   0        0        0        0 2024-05-05 20:32:18.996611 heaserver_buckets-1.1.3/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-05 20:32:19.195453 heaserver_buckets-1.1.3/tests/heaserver/buckettest/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.3/tests/heaserver/buckettest/__init__.py
--rw-rw-rw-   0        0        0     1623 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.3/tests/heaserver/buckettest/test_all.py
--rw-rw-rw-   0        0        0     9173 2024-04-09 21:37:15.000000 heaserver_buckets-1.1.3/tests/heaserver/buckettest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-05-07 20:34:21.447635 heaserver_buckets-1.1.4/
+-rw-rw-rw-   0        0        0      261 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/.gitignore
+-rw-rw-rw-   0        0        0     1515 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     5486 2024-05-07 20:34:21.446243 heaserver_buckets-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4112 2024-05-07 20:27:59.000000 heaserver_buckets-1.1.4/README.md
+-rw-rw-rw-   0        0        0     1737 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/RELEASING.md
+-rw-rw-rw-   0        0        0      470 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-05-07 20:34:21.304543 heaserver_buckets-1.1.4/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-07 20:34:21.304543 heaserver_buckets-1.1.4/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-07 20:34:21.387578 heaserver_buckets-1.1.4/integrationtests/heaserver/bucketintegrationtest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/integrationtests/heaserver/bucketintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0     4817 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/integrationtests/heaserver/bucketintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0    10949 2024-05-07 18:50:12.000000 heaserver_buckets-1.1.4/integrationtests/heaserver/bucketintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/pytest.ini
+-rw-rw-rw-   0        0        0      262 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/requirements_dev.txt
+-rw-rw-rw-   0        0        0     5310 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 20:34:21.447635 heaserver_buckets-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1858 2024-05-07 20:33:25.000000 heaserver_buckets-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 20:34:21.306542 heaserver_buckets-1.1.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 20:34:21.305544 heaserver_buckets-1.1.4/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-07 20:34:21.392028 heaserver_buckets-1.1.4/src/heaserver/bucket/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/src/heaserver/bucket/__init__.py
+-rw-rw-rw-   0        0        0    73812 2024-05-07 18:19:20.000000 heaserver_buckets-1.1.4/src/heaserver/bucket/service.py
+drwxrwxrwx   0        0        0        0 2024-05-07 20:34:21.393598 heaserver_buckets-1.1.4/src/heaserver/bucket/wstl/
+-rw-rw-rw-   0        0        0    14793 2024-04-09 21:37:15.000000 heaserver_buckets-1.1.4/src/heaserver/bucket/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-07 20:34:21.444697 heaserver_buckets-1.1.4/src/heaserver_buckets.egg-info/
+-rw-rw-rw-   0        0        0     5486 2024-05-07 20:34:21.000000 heaserver_buckets-1.1.4/src/heaserver_buckets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2024-05-07 20:34:21.000000 heaserver_buckets-1.1.4/src/heaserver_buckets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 20:34:21.000000 heaserver_buckets-1.1.4/src/heaserver_buckets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-05-07 20:34:21.000000 heaserver_buckets-1.1.4/src/heaserver_buckets.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2024-05-07 20:34:21.000000 heaserver_buckets-1.1.4/src/heaserver_buckets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-07 20:34:21.000000 heaserver_buckets-1.1.4/src/heaserver_buckets.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 20:34:21.307542 heaserver_buckets-1.1.4/tests/
+drwxrwxrwx   0        0        0        0 2024-05-07 20:34:21.307542 heaserver_buckets-1.1.4/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-07 20:34:21.443073 heaserver_buckets-1.1.4/tests/heaserver/buckettest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/tests/heaserver/buckettest/__init__.py
+-rw-rw-rw-   0        0        0     1623 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/tests/heaserver/buckettest/test_all.py
+-rw-rw-rw-   0        0        0     9195 2024-05-07 18:49:58.000000 heaserver_buckets-1.1.4/tests/heaserver/buckettest/testcase.py
```

### Comparing `heaserver_buckets-1.1.3/Dockerfile` & `heaserver_buckets-1.1.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver_buckets-1.1.3/LICENSE` & `heaserver_buckets-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver_buckets-1.1.3/PKG-INFO` & `heaserver_buckets-1.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-buckets
-Version: 1.1.3
+Version: 1.1.4
 Summary: a service for managing buckets and their data within the cloud
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-buckets,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -30,14 +30,18 @@
 
 # HEA Server Buckets Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Buckets Microservice is a service for managing buckets and their data within the cloud.
 
+## Version 1.1.4
+* Grant all users DELETER privileges to buckets so that the webclient permits deletion (the backend will still deny
+users without permissions to delete buckets).
+
 ## Version 1.1.3
 * Fixed potential issue preventing the service from updating temporary credentials.
 
 ## Version 1.1.2
 * Fixed new folder form submission.
 
 ## Version 1.1.1
```

### Comparing `heaserver_buckets-1.1.3/README.md` & `heaserver_buckets-1.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # HEA Server Buckets Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Buckets Microservice is a service for managing buckets and their data within the cloud.
 
+## Version 1.1.4
+* Grant all users DELETER privileges to buckets so that the webclient permits deletion (the backend will still deny
+users without permissions to delete buckets).
+
 ## Version 1.1.3
 * Fixed potential issue preventing the service from updating temporary credentials.
 
 ## Version 1.1.2
 * Fixed new folder form submission.
 
 ## Version 1.1.1
```

### Comparing `heaserver_buckets-1.1.3/RELEASING.md` & `heaserver_buckets-1.1.4/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver_buckets-1.1.3/integrationtests/heaserver/bucketintegrationtest/test_all.py` & `heaserver_buckets-1.1.4/integrationtests/heaserver/bucketintegrationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_buckets-1.1.3/integrationtests/heaserver/bucketintegrationtest/testcase.py` & `heaserver_buckets-1.1.4/integrationtests/heaserver/bucketintegrationtest/testcase.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         'display_name': 'hci-foundation-1',
         'invites': [],
         'modified': None,
         'name': 'hci-foundation-1',
         'owner': AWS_USER,
         'shares': [{
             'invite': None,
-            'permissions': ['EDITOR'],
+            'permissions': ['EDITOR', 'DELETER'],
             'type': 'heaobject.root.ShareImpl',
             'user': 'system|all'
         }],
         'source': 'AWS S3',
         'source_detail': 'AWS S3',
         'type': 'heaobject.bucket.AWSBucket',
         'arn': 'arn:aws:s3::hci-foundation-1',
@@ -60,15 +60,15 @@
             'display_name': 'hci-foundation-2',
             'invites': [],
             'modified': None,
             'name': 'hci-foundation-2',
             'owner': AWS_USER,
             'shares': [{
                 'invite': None,
-                'permissions': ['EDITOR'],
+                'permissions': ['EDITOR', 'DELETER'],
                 'type': 'heaobject.root.ShareImpl',
                 'user': 'system|all'
             }],
             'source': 'AWS S3',
             'source_detail': 'AWS S3',
             'type': 'heaobject.bucket.AWSBucket',
             'arn': 'arn:aws:s3::hci-foundation-2',
```

### Comparing `heaserver_buckets-1.1.3/run-swaggerui.py` & `heaserver_buckets-1.1.4/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver_buckets-1.1.3/setup.py` & `heaserver_buckets-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-buckets',
-    version='1.1.3',
+    version='1.1.4',
     description="a service for managing buckets and their data within the cloud",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
```

### Comparing `heaserver_buckets-1.1.3/src/heaserver/bucket/service.py` & `heaserver_buckets-1.1.4/src/heaserver/bucket/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -748,14 +748,18 @@
                             bucket_item.modified = creation_date
                             bucket_item.created = creation_date
                             bucket_item.actual_object_type_name = bucket_type
                             bucket_item.actual_object_id = bucket_name
                             bucket_item.actual_object_uri = str(bucket_url / bucket_name)
                             bucket_item.source = AWS_S3
                             bucket_item.source_detail = AWS_S3
+                            share = ShareImpl()
+                            share.user = ALL_USERS
+                            share.permissions = [Permission.EDITOR, Permission.DELETER]
+                            bucket_item.shares = [share]
                             yield bucket_item
                     result = [buck.to_dict() for buck in bucket_items()]
                     activity.new_object_uri = f'volumes/{volume_id}/bucketitems/'
                     activity.new_object_type_name = AWSS3BucketItem.get_type_name()
                     activity.new_volume_id = volume_id
                     request.app[HEA_CACHE][cache_key] = result
                     for buck in result:
@@ -1467,15 +1471,15 @@
     b.bucket_id = b.name
     b.source = AWS_S3
     b.source_detail = AWS_S3
     b.arn = f'arn:aws:s3::{b.id}'
     b.owner = AWS_USER
     share = ShareImpl()
     share.user = ALL_USERS
-    share.permissions = [Permission.EDITOR]
+    share.permissions = [Permission.EDITOR, Permission.DELETER]
     b.shares = [share]
 
     if creation_date:
         b.created = creation_date
     elif cached_value := cache.get((sub, volume_id, None, 'items')):
         b.created = next((bucket_['created'] for bucket_ in cached_value if bucket_['name'] == b.name), None)
     else:
```

### Comparing `heaserver_buckets-1.1.3/src/heaserver/bucket/wstl/all.json` & `heaserver_buckets-1.1.4/src/heaserver/bucket/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver_buckets-1.1.3/src/heaserver_buckets.egg-info/PKG-INFO` & `heaserver_buckets-1.1.4/src/heaserver_buckets.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-buckets
-Version: 1.1.3
+Version: 1.1.4
 Summary: a service for managing buckets and their data within the cloud
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-buckets,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -30,14 +30,18 @@
 
 # HEA Server Buckets Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Buckets Microservice is a service for managing buckets and their data within the cloud.
 
+## Version 1.1.4
+* Grant all users DELETER privileges to buckets so that the webclient permits deletion (the backend will still deny
+users without permissions to delete buckets).
+
 ## Version 1.1.3
 * Fixed potential issue preventing the service from updating temporary credentials.
 
 ## Version 1.1.2
 * Fixed new folder form submission.
 
 ## Version 1.1.1
```

### Comparing `heaserver_buckets-1.1.3/src/heaserver_buckets.egg-info/SOURCES.txt` & `heaserver_buckets-1.1.4/src/heaserver_buckets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver_buckets-1.1.3/tests/heaserver/buckettest/test_all.py` & `heaserver_buckets-1.1.4/tests/heaserver/buckettest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_buckets-1.1.3/tests/heaserver/buckettest/testcase.py` & `heaserver_buckets-1.1.4/tests/heaserver/buckettest/testcase.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         'display_name': 'hci-foundation-1',
         'invites': [],
         'modified': None,
         'name': 'hci-foundation-1',
         'owner': AWS_USER,
         'shares': [{
             'invite': None,
-            'permissions': ['EDITOR'],
+            'permissions': ['EDITOR', 'DELETER'],
             'type': 'heaobject.root.ShareImpl',
             'user': 'system|all'
         }],
         'source': 'AWS S3',
         'source_detail': 'AWS S3',
         'type': 'heaobject.bucket.AWSBucket',
         'arn': 'arn:aws:s3::hci-foundation-1',
@@ -54,15 +54,15 @@
             'display_name': 'hci-foundation-2',
             'invites': [],
             'modified': None,
             'name': 'hci-foundation-2',
             'owner': AWS_USER,
             'shares': [{
                 'invite': None,
-                'permissions': ['EDITOR'],
+                'permissions': ['EDITOR', 'DELETER'],
                 'type': 'heaobject.root.ShareImpl',
                 'user': 'system|all'
             }],
             'source': 'AWS S3',
             'source_detail': 'AWS S3',
             'type': 'heaobject.bucket.AWSBucket',
             'arn': 'arn:aws:s3::hci-foundation-2',
```

