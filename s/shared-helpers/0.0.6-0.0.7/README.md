# Comparing `tmp/shared_helpers-0.0.6.tar.gz` & `tmp/shared_helpers-0.0.7.tar.gz`

## Comparing `shared_helpers-0.0.6.tar` & `shared_helpers-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 shared_helpers-0.0.6/requirements.txt
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 shared_helpers-0.0.6/setup.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 shared_helpers-0.0.6/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.6/src/shared_helpers/__init__.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 shared_helpers-0.0.6/src/shared_helpers/functions.py
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 shared_helpers-0.0.6/src/shared_helpers/main.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 shared_helpers-0.0.6/src/shared_helpers/variables.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.6/src/shared_helpers/lm/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.6/src/shared_helpers/lm/sbbid/__init__.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 shared_helpers-0.0.6/src/shared_helpers/lm/sbbid/sbbid_helper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.6/src/shared_helpers/yandex/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.6/src/shared_helpers/yandex/iam/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.6/src/shared_helpers/yandex/organization/__init__.py
--rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 shared_helpers-0.0.6/src/shared_helpers/yandex/organization/organization_helper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.6/src/shared_helpers/yandex/tracker/__init__.py
--rw-r--r--   0        0        0     9294 2020-02-02 00:00:00.000000 shared_helpers-0.0.6/src/shared_helpers/yandex/tracker/tracker_helper.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 shared_helpers-0.0.6/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.6/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.6/README.md
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 shared_helpers-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 shared_helpers-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/requirements.txt
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/setup.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/__init__.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/functions.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/main.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/variables.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/lm/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/lm/sbbid/__init__.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/lm/sbbid/sbbid_helper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/yandex/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/yandex/iam/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/yandex/organization/__init__.py
+-rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/yandex/organization/organization_helper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/yandex/tracker/__init__.py
+-rw-r--r--   0        0        0     9294 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/yandex/tracker/tracker_helper.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/README.md
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/PKG-INFO
```

### Comparing `shared_helpers-0.0.6/src/shared_helpers/functions.py` & `shared_helpers-0.0.7/src/shared_helpers/functions.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import calendar
 import requests
-from datetime import date
-from datetime import datetime
 import json
 import time
 import jwt
 import os
-
+from datetime import date
+from datetime import datetime
 from urllib3.util import Retry
 from requests.adapters import HTTPAdapter
+
 import shared_helpers.variables as variables
 
 req = requests.Session()
 retries = Retry(total=5,
                 backoff_factor=2,
                 status_forcelist=[429, 500, 502, 503, 504])
```

### Comparing `shared_helpers-0.0.6/src/shared_helpers/main.py` & `shared_helpers-0.0.7/src/shared_helpers/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import shared_helpers.variables as variables
-from yandex.organization.organization_helper import CloudHelper
-from yandex.tracker.tracker_helper import TrackerHelper
-from lm.sbbid.sbbid_helper import SbbIdHelper
-from functions import TokenHelper
+from shared_helpers.yandex.organization.organization_helper import CloudHelper
+from shared_helpers.yandex.tracker.tracker_helper import TrackerHelper
+from shared_helpers.lm.sbbid.sbbid_helper import SbbIdHelper
+from shared_helpers.functions import TokenHelper
 
 token_helper = TokenHelper()
 
 def fetch_current_iam_token() -> str:
     """Fetch a valid IAM token or return None."""
     token = None
     if (
```

### Comparing `shared_helpers-0.0.6/src/shared_helpers/lm/sbbid/sbbid_helper.py` & `shared_helpers-0.0.7/src/shared_helpers/lm/sbbid/sbbid_helper.py`

 * *Files identical despite different names*

### Comparing `shared_helpers-0.0.6/src/shared_helpers/yandex/organization/organization_helper.py` & `shared_helpers-0.0.7/src/shared_helpers/yandex/organization/organization_helper.py`

 * *Files identical despite different names*

### Comparing `shared_helpers-0.0.6/src/shared_helpers/yandex/tracker/tracker_helper.py` & `shared_helpers-0.0.7/src/shared_helpers/yandex/tracker/tracker_helper.py`

 * *Files identical despite different names*

### Comparing `shared_helpers-0.0.6/.gitignore` & `shared_helpers-0.0.7/.gitignore`

 * *Files identical despite different names*

