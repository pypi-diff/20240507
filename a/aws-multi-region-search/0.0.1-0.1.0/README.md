# Comparing `tmp/aws-multi-region-search-0.0.1.tar.gz` & `tmp/aws_multi_region_search-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-multi-region-search-0.0.1.tar", last modified: Wed Jun 14 14:56:06 2023, max compression
+gzip compressed data, was "aws_multi_region_search-0.1.0.tar", max compression
```

## Comparing `aws-multi-region-search-0.0.1.tar` & `aws_multi_region_search-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,11 @@
-drwxr-xr-x   0 sky        (501) staff       (20)        0 2023-06-14 14:56:06.651106 aws-multi-region-search-0.0.1/
--rw-r--r--   0 sky        (501) staff       (20)     1048 2023-06-02 15:09:46.000000 aws-multi-region-search-0.0.1/LICENSE
--rw-r--r--   0 sky        (501) staff       (20)      944 2023-06-14 14:56:06.650949 aws-multi-region-search-0.0.1/PKG-INFO
--rw-r--r--   0 sky        (501) staff       (20)      498 2023-06-14 14:43:33.000000 aws-multi-region-search-0.0.1/README.md
-drwxr-xr-x   0 sky        (501) staff       (20)        0 2023-06-14 14:56:06.649366 aws-multi-region-search-0.0.1/aws_multi_region_search.egg-info/
--rw-r--r--   0 sky        (501) staff       (20)      944 2023-06-14 14:56:06.000000 aws-multi-region-search-0.0.1/aws_multi_region_search.egg-info/PKG-INFO
--rw-r--r--   0 sky        (501) staff       (20)      388 2023-06-14 14:56:06.000000 aws-multi-region-search-0.0.1/aws_multi_region_search.egg-info/SOURCES.txt
--rw-r--r--   0 sky        (501) staff       (20)        1 2023-06-14 14:56:06.000000 aws-multi-region-search-0.0.1/aws_multi_region_search.egg-info/dependency_links.txt
--rw-r--r--   0 sky        (501) staff       (20)       43 2023-06-14 14:56:06.000000 aws-multi-region-search-0.0.1/aws_multi_region_search.egg-info/entry_points.txt
--rw-r--r--   0 sky        (501) staff       (20)        5 2023-06-14 14:56:06.000000 aws-multi-region-search-0.0.1/aws_multi_region_search.egg-info/top_level.txt
--rw-r--r--   0 sky        (501) staff       (20)        1 2023-06-14 14:56:06.000000 aws-multi-region-search-0.0.1/aws_multi_region_search.egg-info/zip-safe
-drwxr-xr-x   0 sky        (501) staff       (20)        0 2023-06-14 14:56:06.650663 aws-multi-region-search-0.0.1/awss/
--rw-r--r--   0 sky        (501) staff       (20)       76 2023-06-02 15:06:34.000000 aws-multi-region-search-0.0.1/awss/__init__.py
--rw-r--r--   0 sky        (501) staff       (20)     2346 2023-06-14 14:39:16.000000 aws-multi-region-search-0.0.1/awss/__main__.py
--rw-r--r--   0 sky        (501) staff       (20)     3398 2023-06-14 14:24:06.000000 aws-multi-region-search-0.0.1/awss/ec2.py
--rw-r--r--   0 sky        (501) staff       (20)      710 2023-06-14 14:08:34.000000 aws-multi-region-search-0.0.1/awss/lib.py
--rw-r--r--   0 sky        (501) staff       (20)     1331 2023-06-14 14:28:09.000000 aws-multi-region-search-0.0.1/awss/rds.py
--rw-r--r--   0 sky        (501) staff       (20)     1018 2023-06-14 14:28:09.000000 aws-multi-region-search-0.0.1/awss/sts.py
--rw-r--r--   0 sky        (501) staff       (20)       38 2023-06-14 14:56:06.651158 aws-multi-region-search-0.0.1/setup.cfg
--rw-r--r--   0 sky        (501) staff       (20)     1083 2023-06-14 14:55:38.000000 aws-multi-region-search-0.0.1/setup.py
+-rw-r--r--   0        0        0     1048 2024-05-07 19:35:28.705477 aws_multi_region_search-0.1.0/LICENSE
+-rw-r--r--   0        0        0      498 2024-02-14 15:07:16.232301 aws_multi_region_search-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-07 19:35:54.558650 aws_multi_region_search-0.1.0/awss/__init__.py
+-rw-r--r--   0        0        0     3294 2024-05-07 19:35:54.559240 aws_multi_region_search-0.1.0/awss/__main__.py
+-rw-r--r--   0        0        0     2082 2024-05-07 19:35:54.560081 aws_multi_region_search-0.1.0/awss/acm.py
+-rw-r--r--   0        0        0     3003 2024-05-07 19:35:54.560363 aws_multi_region_search-0.1.0/awss/ec2.py
+-rw-r--r--   0        0        0      787 2024-02-14 15:07:16.233012 aws_multi_region_search-0.1.0/awss/lib.py
+-rw-r--r--   0        0        0     1361 2024-02-14 15:07:16.233129 aws_multi_region_search-0.1.0/awss/rds.py
+-rw-r--r--   0        0        0     1170 2024-02-14 15:07:16.233249 aws_multi_region_search-0.1.0/awss/sts.py
+-rw-r--r--   0        0        0      698 2024-05-07 19:35:54.561120 aws_multi_region_search-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1318 1970-01-01 00:00:00.000000 aws_multi_region_search-0.1.0/PKG-INFO
```

### Comparing `aws-multi-region-search-0.0.1/LICENSE` & `aws_multi_region_search-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-multi-region-search-0.0.1/PKG-INFO` & `aws_multi_region_search-0.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 Metadata-Version: 2.1
 Name: aws-multi-region-search
-Version: 0.0.1
+Version: 0.1.0
 Summary: AWS Multi Region Concurrent Query Tool
 Home-page: https://github.com/skymoore/aws-search
+License: MIT
+Keywords: aws,cloud,multi-region,search,concurrent
 Author: Sky Moore
 Author-email: i@msky.me
-License: MIT
-Keywords: aws,multi-region
+Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: boto3 (>=1.34.99,<2.0.0)
+Requires-Dist: click (>=8.1.7,<9.0.0)
+Project-URL: Repository, https://github.com/skymoore/aws-search
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 ## Multi-Region Multi-Threaded AWS Search Tool
 
 ### Usage Examples:
 
 #### RDS:
 list rds instances in every region
```

### Comparing `aws-multi-region-search-0.0.1/awss/ec2.py` & `aws_multi_region_search-0.1.0/awss/ec2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,103 +1,98 @@
-from time import perf_counter
-from logging import info, error, warning
-from .lib import get_regions, perf_time, multithreaded
+from logging import info
+from .lib import perf_time, multithreaded
 
 
 def get_ami_ids_by_owner(session, region, owner_id, name_filter, print_lock):
     ec2 = session.client("ec2", region_name=region)
     ami_ids = {}
     filter = [
         {
             "Name": "name",
             "Values": [name_filter],
         }
     ]
-    owner_id = [owner_id]
+    owner_id = owner_id
 
     response = ec2.describe_images(
-        Owners=owner_id,
+        Owners=[owner_id],
         Filters=filter,
     )
     for ami in response["Images"]:
         ami_ids[ami["ImageId"]] = ""
 
     while "NextToken" in response:
         response = ec2.describe_images(
-            Owners=owner_id,
+            Owners=[owner_id],
             Filters=filter,
             NextToken=response["NextToken"],
         )
         for ami in response["Images"]:
             ami_ids[ami["ImageId"]] = ""
 
+    len_ami_ids = len(ami_ids.keys())
+
     with print_lock:
-        info(f"{len(ami_ids.keys())} amis owned by {owner_id[0]} in region {region}")
+        info(
+            f"{len_ami_ids} {'ami' if len_ami_ids == 1 else 'amis'} owned by {owner_id} in region {region}"
+        )
     return ami_ids
 
 
 @multithreaded
+def check_instance_for_match(
+    instance, region, instance_ids_by_region, ami_ids, print_lock
+):
+    if instance.image_id in ami_ids:
+        if region not in instance_ids_by_region:
+            instance_ids_by_region[region] = [instance.id]
+        else:
+            instance_ids_by_region[region].append(instance.id)
+
+
+@multithreaded
 def find_instances(
     session, region, print_lock, owner_id, name_filter, instance_ids_by_region
 ):
-    try:
-        ec2_resource = session.resource("ec2", region_name=region)
-        instances = ec2_resource.instances.all()
-        num_instances = len(list(instances))
-
-        if num_instances == 0:
-            with print_lock:
-                info(f"no ec2 instances found in region {region}")
-            return
+    ec2_resource = session.resource("ec2", region_name=region)
+    instances = ec2_resource.instances.all()
+    num_instances = len(list(instances))
+
+    if num_instances == 0:
         with print_lock:
-            info(f"{num_instances} ec2 instances in region {region}")
-        ami_ids = get_ami_ids_by_owner(
-            session, region, owner_id, name_filter, print_lock
-        )
+            info(f"no ec2 instances found in region {region}")
+        return
+    with print_lock:
+        info(f"{num_instances} ec2 instances in region {region}")
 
-        found_instance = False
-        for instance in instances:
-            try:
-                if instance.image_id in ami_ids:
-                    found_instance = True
-                    if region not in instance_ids_by_region:
-                        instance_ids_by_region[region] = [instance.id]
-                    else:
-                        instance_ids_by_region[region].append(instance.id)
-                    with print_lock:
-                        info(
-                            f"matching instance in region {region} with ID: {instance.id}"
-                        )
-            except Exception as e:
-                with print_lock:
-                    error(f"{instance.id}: {e}")
-                continue
-
-        if not found_instance:
-            with print_lock:
-                info(f"no matching instances found in region {region}")
-        else:
-            with print_lock:
-                info(
-                    f"{len(instance_ids_by_region[region])} matching instances found in region {region}"
-                )
+    ami_ids = get_ami_ids_by_owner(session, region, owner_id, name_filter, print_lock)
 
-    except Exception as e:
-        with print_lock:
-            warning(f"{region}: {e}")
+    inputs = [
+        (instance, region, instance_ids_by_region, ami_ids, print_lock)
+        for instance in instances
+    ]
+
+    check_instance_for_match(inputs, 4)
+    len_instance_ids = len(instance_ids_by_region[region])
+    with print_lock:
+        info(
+            f"{len_instance_ids} matching {'instance' if len_instance_ids == 1 else 'instances'} found in region {region}"
+        )
 
 
 @perf_time
-def find_instances_by_ami_owner(session, workers, print_lock, owner_id, name_filter):
-    regions = get_regions(session, "ec2")
+def find_instances_by_ami_owner(
+    session, workers, regions, print_lock, owner_id, name_filter
+):
     info(
         f"searching {len(regions)} aws regions with {workers} workers for ec2 instances running an ami owned by {owner_id} whose name matches {name_filter}..."
     )
     instance_ids_by_region = {}
     inputs = [
         (session, region, print_lock, owner_id, name_filter, instance_ids_by_region)
         for region in regions
     ]
     find_instances(inputs, workers)
+    len_matched_regions = len(instance_ids_by_region.keys())
     info(
-        f"found {len(instance_ids_by_region)} regions with matching instances: {instance_ids_by_region}"
+        f"found {len_matched_regions} {'region' if len_matched_regions == 1 else 'regions'} with match: {instance_ids_by_region}"
     )
```

### Comparing `aws-multi-region-search-0.0.1/awss/lib.py` & `aws_multi_region_search-0.1.0/awss/lib.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from logging import info
 from time import perf_counter
 import concurrent.futures
 
 
-def get_regions(session, service):
-    info("getting regions...")
-    return session.get_available_regions(service)
+def get_all_regions(session):
+    info("getting available regions...")
+    return [
+        region["RegionName"]
+        for region in session.client("ec2").describe_regions()["Regions"]
+    ]
 
 
 def multithreaded(func):
     def wrapper(inputs, workers):
         with concurrent.futures.ThreadPoolExecutor(max_workers=workers) as executor:
             executor.map(lambda params: func(*params), inputs)
```

### Comparing `aws-multi-region-search-0.0.1/awss/rds.py` & `aws_multi_region_search-0.1.0/awss/rds.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from logging import info, warning
-from .lib import get_regions, perf_time, multithreaded
+from .lib import perf_time, multithreaded
 
 
 @multithreaded
 def list_rds(session, region, print_lock):
     try:
         rds = session.client("rds", region_name=region)
         db_names = list()
@@ -16,29 +16,29 @@
         db_names.extend(
             [
                 cluster["DBClusterIdentifier"]
                 for cluster in rds.describe_db_clusters()["DBClusters"]
             ]
         )
 
+        len_db_names = len(db_names)
         with print_lock:
-            if len(db_names) > 0:
+            if len_db_names > 0:
                 info(
-                    f"region: {region}\n\tfound {len(db_names)} databases:\n\t\t"
+                    f"region: {region}\n\tfound {len_db_names} {'database' if len_db_names == 1 else 'databases'}:\n\t\t"
                     + "\n\t\t".join(db_names)
                 )
             else:
                 info(f"no databases found in {region}")
     except Exception as e:
         with print_lock:
             warning(f"in {region}: {e}")
 
 
 @perf_time
-def list_rds_instances(session, workers, print_lock):
-    regions = get_regions(session, "rds")
+def list_rds_instances(session, workers, regions, print_lock):
     info(
         f"searching {len(regions)} aws regions with {workers} workers for rds clusters or instances..."
     )
     inputs = [(session, region, print_lock) for region in regions]
 
     list_rds(inputs, workers)
```

### Comparing `aws-multi-region-search-0.0.1/awss/sts.py` & `aws_multi_region_search-0.1.0/awss/sts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from logging import info, warning
-from .lib import get_regions, perf_time, multithreaded
+from .lib import perf_time, multithreaded
 
 
 @multithreaded
 def check_creds(session, region, print_lock, success, failure):
     try:
         sts = session.client("sts", region_name=region)
         sts.get_caller_identity()
@@ -13,20 +13,25 @@
     except Exception as e:
         failure.append(region)
         with print_lock:
             warning(f"credentials failure in {region}: {e}")
 
 
 @perf_time
-def check_credentials(session, workers, print_lock):
-    regions = get_regions(session, "sts")
+def check_credentials(session, workers, regions, print_lock):
     info(
-        f"checking credentials in {len(regions)} aws regions with {workers} workers..."
+        f"checking credentials in {len(regions)} aws regions with {workers} {'worker' if workers == 1 else 'workers'}..."
     )
     success = []
     failure = []
     inputs = [(session, region, print_lock, success, failure) for region in regions]
 
     check_creds(inputs, workers)
 
-    info(f"credentials ok in {len(success)} regions: {success}")
-    info(f"credentials failure in {len(failure)} regions: {failure}")
+    len_success = len(success)
+    len_failure = len(failure)
+    info(
+        f"credentials ok in {len_success} {'region' if len_success == 1 else 'regions'}: {success}"
+    )
+    info(
+        f"credentials failure in {len_failure} {'region' if len_failure == 1 else 'regions'}: {failure}"
+    )
```

