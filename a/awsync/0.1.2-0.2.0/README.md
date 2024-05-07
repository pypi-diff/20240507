# Comparing `tmp/awsync-0.1.2.tar.gz` & `tmp/awsync-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsync-0.1.2.tar", max compression
+gzip compressed data, was "awsync-0.2.0.tar", max compression
```

## Comparing `awsync-0.1.2.tar` & `awsync-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2024-05-01 04:32:50.769212 awsync-0.1.2/LICENSE
--rw-r--r--   0        0        0     2395 2024-05-01 06:49:57.239651 awsync-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-01 04:07:11.855130 awsync-0.1.2/awsync/__init__.py
--rw-r--r--   0        0        0     1291 2024-05-01 04:07:11.858130 awsync-0.1.2/awsync/__main__.py
--rw-r--r--   0        0        0     7326 2024-05-01 20:57:48.676020 awsync-0.1.2/awsync/client.py
--rw-r--r--   0        0        0        0 2024-05-01 04:07:11.852130 awsync-0.1.2/awsync/models/__init__.py
--rw-r--r--   0        0        0     2275 2024-05-01 19:57:14.549055 awsync-0.1.2/awsync/models/aws.py
--rw-r--r--   0        0        0     1433 2024-05-01 19:56:43.825054 awsync-0.1.2/awsync/models/http.py
--rw-r--r--   0        0        0      283 2024-05-01 19:56:06.559052 awsync-0.1.2/awsync/models/strenum.py
--rw-r--r--   0        0        0     9239 2024-05-01 04:07:11.856130 awsync-0.1.2/awsync/request.py
--rw-r--r--   0        0        0        0 2024-05-01 20:49:43.288001 awsync-0.1.2/py.typed
--rw-r--r--   0        0        0     1071 2024-05-01 20:55:38.356013 awsync-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3365 1970-01-01 00:00:00.000000 awsync-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-01 04:32:50.769212 awsync-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2118 2024-05-07 05:46:47.639367 awsync-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-01 04:07:11.855130 awsync-0.2.0/awsync/__init__.py
+-rw-r--r--   0        0        0      677 2024-05-07 05:46:54.896367 awsync-0.2.0/awsync/__main__.py
+-rw-r--r--   0        0        0     7326 2024-05-07 05:14:49.519264 awsync-0.2.0/awsync/client.py
+-rw-r--r--   0        0        0        0 2024-05-01 04:07:11.852130 awsync-0.2.0/awsync/models/__init__.py
+-rw-r--r--   0        0        0     2573 2024-05-07 05:32:14.863320 awsync-0.2.0/awsync/models/aws.py
+-rw-r--r--   0        0        0     1433 2024-05-01 19:56:43.825054 awsync-0.2.0/awsync/models/http.py
+-rw-r--r--   0        0        0      283 2024-05-01 19:56:06.559052 awsync-0.2.0/awsync/models/strenum.py
+-rw-r--r--   0        0        0        0 2024-05-01 20:49:43.288001 awsync-0.2.0/awsync/py.typed
+-rw-r--r--   0        0        0     9350 2024-05-07 05:35:13.709330 awsync-0.2.0/awsync/request.py
+-rw-r--r--   0        0        0     1071 2024-05-07 05:30:02.627313 awsync-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3088 1970-01-01 00:00:00.000000 awsync-0.2.0/PKG-INFO
```

### Comparing `awsync-0.1.2/LICENSE` & `awsync-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `awsync-0.1.2/README.md` & `awsync-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,49 +6,42 @@
 
 **NOTE: Currently a work in progress!**
 Only a few API methods currently implemented for testing and development.
 
 ## Usage
 
 ```python
+"Module main."
 from asyncio import run
-import os
 from datetime import datetime, UTC
 from httpx import AsyncClient
 
 from awsync.client import Client
 from awsync.models.aws import Region, Credentials
 
 
 async def main() -> int:
     "Main function."
     async with AsyncClient() as httpx_client:
         client = Client(
-            credentials=Credentials(
-                access_key=os.environ["AWS_ACCESS_KEY_ID"],
-                secret_access_key=os.environ["AWS_SECRET_ACCESS_KEY"],
-                session_token=os.environ.get("AWS_SESSION_TOKEN"),
-            ),
+            credentials=Credentials.from_environment(),
             httpx_client=httpx_client,
             utcnow=lambda: datetime.now(UTC),
         )
-
         response = await client.list_stack_resources(
             region=Region.us_east_1, stack_name="Example-Stack-Name"
         )
         print(response)
         return 0
 
 
 if __name__ == "__main__":
     run(main())
 ```
 
-See [awsync/**main**.py](./awsync/__main__.py) for more examples.
-
 ## Local Developer Setup
 
 Requirements:
 
 - [make](https://www.gnu.org/software/make/)
 - [python3](https://www.python.org/)
 - [poetry](https://python-poetry.org/)
@@ -74,11 +67,10 @@
 
 - Logging
 - Test Coverage
 - Automatic Publish CICD
 - Documentation with [mkDocs](https://squidfunk.github.io/mkdocs-material/)
 - Issue template
 - Repository Template variables?
-- Pre-commit hooks?
 - Test Makefile replacements
   - [Poetry run](https://python-poetry.org/docs/cli/#run)
   - [doit](https://pydoit.org/)
```

### Comparing `awsync-0.1.2/awsync/client.py` & `awsync-0.2.0/awsync/client.py`

 * *Files identical despite different names*

### Comparing `awsync-0.1.2/awsync/models/aws.py` & `awsync-0.2.0/awsync/models/aws.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 "AWS type models."
 from awsync.models.strenum import StrEnum
 from dataclasses import dataclass
 from typing import Optional
+import os
 
 
 @dataclass(frozen=True)
 class Credentials:
     "AWS Credentials."
-    access_key: str
+    access_key_id: str
     "The Access Key ID."
     secret_access_key: str
     "The Secret Access Key."
     session_token: Optional[str] = None
     "(Optional) The session security token if using temporary credentials."
 
+    @classmethod
+    def from_environment(cls) -> "Credentials":
+        return cls(
+            access_key_id=os.environ["AWS_ACCESS_KEY_ID"],
+            secret_access_key=os.environ["AWS_SECRET_ACCESS_KEY"],
+            session_token=os.environ.get("AWS_SESSION_TOKEN"),
+        )
+
 
 class Region(StrEnum):
     """
     An AWS Region.
     See: https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-regions-availability-zones.html#concepts-available-regions
     """
```

### Comparing `awsync-0.1.2/awsync/models/http.py` & `awsync-0.2.0/awsync/models/http.py`

 * *Files identical despite different names*

### Comparing `awsync-0.1.2/awsync/request.py` & `awsync-0.2.0/awsync/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,22 @@
 
 def _get_query_string(query: Optional[Dict[str, str]]) -> str:
     "The URI-encoded query string parameters. You URI-encode each name and values individually. You must also sort the parameters in the canonical query string alphabetically by key name. The sorting occurs after encoding. NOTE: Does not include '?' at the start."
     if not query:
         return ""
 
     # quote = UriEncode, sorted = alphabetical sort starting with key
-    return "&".join(sorted([f"{quote(k)}={quote(v)}" for k, v in query.items()]))
+    return "&".join(
+        sorted(
+            [
+                f"{quote(k, safe='-_.~')}={quote(v, safe='-_.~')}"
+                for k, v in query.items()
+            ]
+        )
+    )
 
 
 def _get_canonical_headers(
     host: str,
     credentials: Credentials,
     headers: Dict[str, str],
     iso_8601_timestamp: Timestamp,
@@ -143,15 +150,15 @@
 ) -> Dict[str, str]:
     "Step 4 part 2: Create Authorization header from signature."
     signature = hmac.new(
         signing_key, string_to_sign.encode(), hashlib.sha256
     ).hexdigest()
     authorization_header_value = ",".join(
         [
-            f"AWS4-HMAC-SHA256 Credential={credentials.access_key}/{scope}",
+            f"AWS4-HMAC-SHA256 Credential={credentials.access_key_id}/{scope}",
             f"SignedHeaders={';'.join(sorted([k.lower() for k in canonical_headers.keys()]))}",
             f"Signature={signature}",
         ]
     )
     return {"Authorization": authorization_header_value}
```

### Comparing `awsync-0.1.2/pyproject.toml` & `awsync-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "awsync"
-version = "0.1.2"
+version = "0.2.0"
 description = "An asynchronous, fully-typed AWS API library with a focus on being understandable, reliable, and maintainable."
 license = "Apache-2.0"
 authors = ["JKCT <jkct@visceralfx.com>"]
 readme = "README.md"
 packages = [{include = "awsync"}]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `awsync-0.1.2/PKG-INFO` & `awsync-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsync
-Version: 0.1.2
+Version: 0.2.0
 Summary: An asynchronous, fully-typed AWS API library with a focus on being understandable, reliable, and maintainable.
 Home-page: https://github.com/JKCT/awsync
 License: Apache-2.0
 Keywords: aws,async,boto,request,sdk,typed
 Author: JKCT
 Author-email: jkct@visceralfx.com
 Requires-Python: >=3.8,<4.0
@@ -30,49 +30,42 @@
 
 **NOTE: Currently a work in progress!**
 Only a few API methods currently implemented for testing and development.
 
 ## Usage
 
 ```python
+"Module main."
 from asyncio import run
-import os
 from datetime import datetime, UTC
 from httpx import AsyncClient
 
 from awsync.client import Client
 from awsync.models.aws import Region, Credentials
 
 
 async def main() -> int:
     "Main function."
     async with AsyncClient() as httpx_client:
         client = Client(
-            credentials=Credentials(
-                access_key=os.environ["AWS_ACCESS_KEY_ID"],
-                secret_access_key=os.environ["AWS_SECRET_ACCESS_KEY"],
-                session_token=os.environ.get("AWS_SESSION_TOKEN"),
-            ),
+            credentials=Credentials.from_environment(),
             httpx_client=httpx_client,
             utcnow=lambda: datetime.now(UTC),
         )
-
         response = await client.list_stack_resources(
             region=Region.us_east_1, stack_name="Example-Stack-Name"
         )
         print(response)
         return 0
 
 
 if __name__ == "__main__":
     run(main())
 ```
 
-See [awsync/**main**.py](./awsync/__main__.py) for more examples.
-
 ## Local Developer Setup
 
 Requirements:
 
 - [make](https://www.gnu.org/software/make/)
 - [python3](https://www.python.org/)
 - [poetry](https://python-poetry.org/)
@@ -98,12 +91,11 @@
 
 - Logging
 - Test Coverage
 - Automatic Publish CICD
 - Documentation with [mkDocs](https://squidfunk.github.io/mkdocs-material/)
 - Issue template
 - Repository Template variables?
-- Pre-commit hooks?
 - Test Makefile replacements
   - [Poetry run](https://python-poetry.org/docs/cli/#run)
   - [doit](https://pydoit.org/)
```

