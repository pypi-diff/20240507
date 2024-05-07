# Comparing `tmp/google_cloud_utilities-0.7.3.tar.gz` & `tmp/google_cloud_utilities-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_cloud_utilities-0.7.3.tar", last modified: Fri Jan 26 17:58:01 2024, max compression
+gzip compressed data, was "google_cloud_utilities-0.7.4.tar", last modified: Thu Feb 15 15:04:43 2024, max compression
```

## Comparing `google_cloud_utilities-0.7.3.tar` & `google_cloud_utilities-0.7.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 17:58:01.381030 google_cloud_utilities-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-01-26 17:57:48.000000 google_cloud_utilities-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-01-26 17:58:01.381030 google_cloud_utilities-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-26 17:57:48.000000 google_cloud_utilities-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 17:58:01.381030 google_cloud_utilities-0.7.3/google_cloud_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-26 17:57:48.000000 google_cloud_utilities-0.7.3/google_cloud_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18201 2024-01-26 17:57:48.000000 google_cloud_utilities-0.7.3/google_cloud_utilities/gcp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 17:58:01.381030 google_cloud_utilities-0.7.3/google_cloud_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-01-26 17:58:01.000000 google_cloud_utilities-0.7.3/google_cloud_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-01-26 17:58:01.000000 google_cloud_utilities-0.7.3/google_cloud_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 17:58:01.000000 google_cloud_utilities-0.7.3/google_cloud_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-26 17:58:01.000000 google_cloud_utilities-0.7.3/google_cloud_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-26 17:58:01.000000 google_cloud_utilities-0.7.3/google_cloud_utilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-26 17:58:01.381030 google_cloud_utilities-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-01-26 17:57:48.000000 google_cloud_utilities-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 15:04:43.777002 google_cloud_utilities-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-15 15:04:30.000000 google_cloud_utilities-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-02-15 15:04:43.773002 google_cloud_utilities-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-15 15:04:30.000000 google_cloud_utilities-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 15:04:43.773002 google_cloud_utilities-0.7.4/google_cloud_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-15 15:04:30.000000 google_cloud_utilities-0.7.4/google_cloud_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18144 2024-02-15 15:04:30.000000 google_cloud_utilities-0.7.4/google_cloud_utilities/gcp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 15:04:43.773002 google_cloud_utilities-0.7.4/google_cloud_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-02-15 15:04:43.000000 google_cloud_utilities-0.7.4/google_cloud_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-15 15:04:43.000000 google_cloud_utilities-0.7.4/google_cloud_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 15:04:43.000000 google_cloud_utilities-0.7.4/google_cloud_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-15 15:04:43.000000 google_cloud_utilities-0.7.4/google_cloud_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-15 15:04:43.000000 google_cloud_utilities-0.7.4/google_cloud_utilities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 15:04:43.777002 google_cloud_utilities-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-02-15 15:04:30.000000 google_cloud_utilities-0.7.4/setup.py
```

### Comparing `google_cloud_utilities-0.7.3/LICENSE` & `google_cloud_utilities-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `google_cloud_utilities-0.7.3/PKG-INFO` & `google_cloud_utilities-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google_cloud_utilities
-Version: 0.7.3
+Version: 0.7.4
 Summary: A few handy Python functions for interacting with Google Cloud Platform
 Home-page: https://github.com/johnf1004/google_cloud_utilities
 Author: John Foley
 Author-email: johnf1004@yahoo.co.uk
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `google_cloud_utilities-0.7.3/google_cloud_utilities/gcp.py` & `google_cloud_utilities-0.7.4/google_cloud_utilities/gcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from google.cloud import secretmanager
 import pandas as pd
 from dateutil import parser
 import base64
 import json
 from datetime import datetime, timezone
 import subprocess
+import google.oauth2.id_token
+import google.auth.transport.requests
 
 logger = logging.getLogger(__name__)
 
 
 def get_most_recent_date(fs, gcs_path, max_date):
     """
     # Function to get most recent datekey (before max_date) of files in a GCS bucket/folder
@@ -540,14 +542,11 @@
             else:
                 logging.warning("No 'jobConfiguration' field in job")
                 return None, None
         else:
             logging.warning("No 'job' field found in jobCompletedEvent")
             return None, None
 
-def get_gcp_identity_token():
-    # Execute 'gcloud auth print-identity-token' command
-    result = subprocess.run(["gcloud", "auth", "print-identity-token"], capture_output=True, text=True, check=True)
-
-    # Extract and return the identity token
-    identity_token = result.stdout.strip()
-    return identity_token
+def get_gcp_identity_token(audience_url):
+    request = google.auth.transport.requests.Request()
+    id_token = google.oauth2.id_token.fetch_id_token(request, audience_url)
+    return id_token
```

### Comparing `google_cloud_utilities-0.7.3/google_cloud_utilities.egg-info/PKG-INFO` & `google_cloud_utilities-0.7.4/google_cloud_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google_cloud_utilities
-Version: 0.7.3
+Version: 0.7.4
 Summary: A few handy Python functions for interacting with Google Cloud Platform
 Home-page: https://github.com/johnf1004/google_cloud_utilities
 Author: John Foley
 Author-email: johnf1004@yahoo.co.uk
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `google_cloud_utilities-0.7.3/setup.py` & `google_cloud_utilities-0.7.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Package meta-data.
 NAME = 'google_cloud_utilities'
 DESCRIPTION = 'A few handy Python functions for interacting with Google Cloud Platform'
 URL = 'https://github.com/johnf1004/google_cloud_utilities'
 EMAIL = 'johnf1004@yahoo.co.uk'
 AUTHOR = 'John Foley'
 REQUIRES_PYTHON = '>=3.9.7'
-VERSION = '0.7.3'
+VERSION = '0.7.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'google-cloud-bigquery>=3.4.2', 'google-cloud-secret-manager>=2.4.0', 'pandas>=1.5.3',
     'python-dateutil>=2.8.2'
 ]
```

