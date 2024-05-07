# Comparing `tmp/sqlpile-0.2.2.tar.gz` & `tmp/sqlpile-0.3.0.tar.gz`

## Comparing `sqlpile-0.2.2.tar` & `sqlpile-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 sqlpile-0.2.2/.python-version
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 sqlpile-0.2.2/requirements-dev.lock
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 sqlpile-0.2.2/requirements.lock
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sqlpile-0.2.2/.vscode/settings.json
--rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 sqlpile-0.2.2/docs/CODE_STYLE.md
--rw-r--r--   0        0        0  2731400 2020-02-02 00:00:00.000000 sqlpile-0.2.2/docs/imgs/good-oop.png
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 sqlpile-0.2.2/src/sqlpile/__init__.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 sqlpile-0.2.2/src/sqlpile/abcs.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 sqlpile-0.2.2/src/sqlpile/config.py
--rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 sqlpile-0.2.2/src/sqlpile/core.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 sqlpile-0.2.2/src/sqlpile/database.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 sqlpile-0.2.2/src/sqlpile/main.py
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 sqlpile-0.2.2/src/sqlpile/utils.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 sqlpile-0.2.2/.gitignore
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 sqlpile-0.2.2/README.md
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 sqlpile-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 sqlpile-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 sqlpile-0.3.0/.python-version
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 sqlpile-0.3.0/requirements-dev.lock
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 sqlpile-0.3.0/requirements.lock
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sqlpile-0.3.0/.vscode/settings.json
+-rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 sqlpile-0.3.0/docs/CODE_STYLE.md
+-rw-r--r--   0        0        0  2731400 2020-02-02 00:00:00.000000 sqlpile-0.3.0/docs/imgs/good-oop.png
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 sqlpile-0.3.0/src/sqlpile/__init__.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 sqlpile-0.3.0/src/sqlpile/abcs.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 sqlpile-0.3.0/src/sqlpile/config.py
+-rw-r--r--   0        0        0    18034 2020-02-02 00:00:00.000000 sqlpile-0.3.0/src/sqlpile/core.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 sqlpile-0.3.0/src/sqlpile/database.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 sqlpile-0.3.0/src/sqlpile/main.py
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 sqlpile-0.3.0/src/sqlpile/utils.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 sqlpile-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 sqlpile-0.3.0/README.md
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 sqlpile-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 sqlpile-0.3.0/PKG-INFO
```

### Comparing `sqlpile-0.2.2/requirements-dev.lock` & `sqlpile-0.3.0/requirements.lock`

 * *Files 25% similar despite different names*

```diff
@@ -10,118 +10,213 @@
 -e file:.
 aiosqlite==0.20.0
     # via sqlpile
 annotated-types==0.6.0
     # via pydantic
 anyio==4.3.0
     # via asyncer
+    # via httpx
 asttokens==2.4.1
     # via devtools
 asyncer==0.0.7
     # via sqlpile
 attrs==23.2.0
     # via lancedb
 cachetools==5.3.3
     # via lancedb
 certifi==2024.2.2
+    # via httpcore
+    # via httpx
     # via requests
 charset-normalizer==3.3.2
     # via requests
+click==8.1.7
+    # via typer
 cloudpickle==3.0.0
     # via sqlpile
+construct==2.10.68
+    # via construct-typing
+construct-typing==0.5.6
+    # via solana
 cytoolz==0.12.3
     # via sqlpile
 decorator==5.1.1
     # via retry
 deprecation==2.1.0
     # via lancedb
+    # via postgrest
 devtools==0.12.2
     # via sqlpile
 diskcache==5.6.3
     # via sqlpile
+    # via supamodel
+dnspython==2.6.1
+    # via email-validator
 duckdb==0.10.2
     # via duckdb-engine
     # via sqlpile
 duckdb-engine==0.12.0
     # via sqlpile
+email-validator==2.1.1
+    # via pydantic
 executing==2.0.1
     # via devtools
+gotrue==2.4.2
+    # via supabase
+h11==0.14.0
+    # via httpcore
+httpcore==1.0.5
+    # via httpx
+httpx==0.27.0
+    # via gotrue
+    # via postgrest
+    # via solana
+    # via storage3
+    # via supabase
+    # via supafunc
 idna==3.7
     # via anyio
+    # via email-validator
+    # via httpx
     # via requests
+inflector==3.1.1
+    # via supamodel
+jsonalias==0.1.1
+    # via solders
 lancedb==0.6.11
     # via sqlpile
 loguru==0.7.2
     # via sqlpile
+    # via supamodel
 lz4==4.3.3
     # via sqlpile
 markdown-it-py==3.0.0
     # via rich
 mdurl==0.1.2
     # via markdown-it-py
 numpy==1.26.4
+    # via pandas
     # via pyarrow
     # via pylance
+    # via scipy
+    # via supamodel
+orjson==3.10.3
+    # via supamodel
 overrides==7.7.0
     # via lancedb
 packaging==24.0
     # via deprecation
     # via duckdb-engine
-pathspec==0.12.1
-    # via ssort
+pandas==2.2.2
+    # via supamodel
+pendulum==3.0.0
+    # via supamodel
+postgrest==0.16.4
+    # via supabase
 psycopg==3.1.18
     # via sqlpile
 psycopg-binary==3.1.18
     # via psycopg
 py==1.11.0
     # via retry
 pyarrow==15.0.0
     # via pylance
 pydantic==2.7.1
+    # via gotrue
     # via lancedb
+    # via postgrest
     # via pydantic-settings
+    # via supamodel
 pydantic-core==2.18.2
     # via pydantic
 pydantic-settings==2.2.1
     # via sqlpile
+    # via supamodel
 pygments==2.17.2
     # via devtools
     # via rich
 pylance==0.10.12
     # via lancedb
 pyrsistent==0.20.0
     # via sqlpile
+python-dateutil==2.9.0.post0
+    # via pandas
+    # via pendulum
+    # via realtime
+    # via storage3
+    # via time-machine
 python-dotenv==1.0.1
     # via pydantic-settings
+pytz==2024.1
+    # via pandas
 ratelimiter==1.2.0.post0
     # via lancedb
+realtime==1.0.4
+    # via supabase
 requests==2.31.0
     # via lancedb
 retry==0.9.2
     # via lancedb
 rich==13.7.1
     # via sqlpile
+    # via supamodel
+    # via typer
+scipy==1.13.0
+    # via supamodel
 semver==3.0.2
     # via lancedb
+shellingham==1.5.4
+    # via typer
 six==1.16.0
     # via asttokens
+    # via python-dateutil
 sniffio==1.3.1
     # via anyio
+    # via httpx
+solana==0.33.0
+    # via supamodel
+solders==0.21.0
+    # via solana
+    # via supamodel
 sqlalchemy==2.0.29
     # via duckdb-engine
     # via sqlpile
-ssort==0.13.0
+storage3==0.7.4
+    # via supabase
+strenum==0.4.15
+    # via postgrest
+supabase==2.4.5
+    # via supamodel
+supafunc==0.4.5
+    # via supabase
+supamodel==0.5.8
+    # via sqlpile
+time-machine==2.14.1
+    # via pendulum
 toolz==0.12.1
     # via cytoolz
     # via sqlpile
 tqdm==4.66.2
     # via lancedb
+typer==0.12.3
+    # via supamodel
 typing-extensions==4.11.0
     # via aiosqlite
     # via psycopg
     # via pydantic
     # via pydantic-core
+    # via realtime
+    # via solana
+    # via solders
     # via sqlalchemy
+    # via storage3
+    # via typer
+tzdata==2024.1
+    # via pandas
+    # via pendulum
 urllib3==2.2.1
     # via requests
+websockets==11.0.3
+    # via realtime
+    # via solana
 xxhash==3.4.1
     # via sqlpile
```

### Comparing `sqlpile-0.2.2/docs/CODE_STYLE.md` & `sqlpile-0.3.0/docs/CODE_STYLE.md`

 * *Files identical despite different names*

### Comparing `sqlpile-0.2.2/docs/imgs/good-oop.png` & `sqlpile-0.3.0/docs/imgs/good-oop.png`

 * *Files identical despite different names*

### Comparing `sqlpile-0.2.2/src/sqlpile/abcs.py` & `sqlpile-0.3.0/src/sqlpile/abcs.py`

 * *Files identical despite different names*

### Comparing `sqlpile-0.2.2/src/sqlpile/config.py` & `sqlpile-0.3.0/src/sqlpile/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 
 class ApplicationSettings(BaseSettings):
     model_config: ConfigDict = SettingsConfigDict(
         arbitrary_types_allowed=True,
         case_sensitive=False,
         env_file=(".env", ".env.dev"),
+        extra="ignore",
     )
     app_name: str = "sqlpile"
     database_name: str = "default"
     memory_database_type: str = "sqlite"
     local_database_type: str = "duckdb"
     app_data_dir: Path = Field(
         default_factory=lambda: Path.home() / ".app_data" / "sqlpile" / "databases"
```

### Comparing `sqlpile-0.2.2/src/sqlpile/core.py` & `sqlpile-0.3.0/src/sqlpile/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import time
 import uuid
 from contextlib import contextmanager
 from typing import Any
 
 from sqlalchemy import Sequence, create_engine
 from sqlalchemy.orm import Session, sessionmaker
+from supabase import Client
 
 from sqlpile.abcs import BaseCache
 from sqlpile.database import Base, CacheEntry
 from sqlpile.utils import (
     SerializerCompressor,
     create_hash_key,
     deserialize_value,
@@ -375,14 +376,125 @@
         :param key: key for item
         :return: True if key is found, else False
 
         """
         return self.contains(key, retry)
 
 
+class SupabaseCache:
+    def __init__(self, supa_client: Client):
+        self.supabase: Client = supa_client
+
+    def get_serial_key(self, key) -> bytes:
+        return create_hash_key(key)
+
+    def get_serial_value(self, value) -> bytes:
+        return get_serialize_value(value)
+
+    def get_deserial_value(self, compressed_value) -> Any:
+        return deserialize_value(compressed_value)
+
+    def set(self, key, value, expire=None, tag=None):
+        now = time.time()
+        expire_time = None if expire is None else now + expire
+        serialized_key = self.get_serial_key(key)
+        compressed_value = self.get_serial_value(value)
+
+        data = {
+            "key": serialized_key,
+            "raw": 1,
+            "store_time": now,
+            "expire_time": expire_time,
+            "access_time": now,
+            "access_count": 0,
+            "tag": tag,
+            "value": compressed_value,
+        }
+
+        response = self.supabase.table("cache_entries").upsert(data).execute()
+        if response.status_code != 200:
+            raise Exception(f"Failed to set cache entry: {response.text}")
+
+        return True
+
+    def get(self, key, default=None, expire_time=False, tag=False):
+        serialized_key = self.get_serial_key(key)
+
+        response = (
+            self.supabase.table("cache_entries")
+            .select("*")
+            .eq("key", serialized_key)
+            .execute()
+        )
+
+        if response.status_code != 200:
+            raise Exception(f"Failed to get cache entry: {response.text}")
+
+        data = response.data
+        if not data or (
+            data[0]["expire_time"] is not None and data[0]["expire_time"] < time.time()
+        ):
+            return default
+
+        compressed_value = data[0]["value"]
+        value = self.get_deserial_value(compressed_value)
+
+        update_data = {
+            "access_time": time.time(),
+            "access_count": data[0]["access_count"] + 1,
+        }
+        self.supabase.table("cache_entries").update(update_data).eq(
+            "key", serialized_key
+        ).execute()
+
+        if expire_time and tag:
+            return value, data[0]["expire_time"], data[0]["tag"]
+        elif expire_time:
+            return value, data[0]["expire_time"]
+        elif tag:
+            return value, data[0]["tag"]
+        else:
+            return value
+
+    def delete(self, key):
+        serialized_key = self.get_serial_key(key)
+
+        response = (
+            self.supabase.table("cache_entries")
+            .delete()
+            .eq("key", serialized_key)
+            .execute()
+        )
+
+        if response.status_code != 200:
+            raise Exception(f"Failed to delete cache entry: {response.text}")
+
+        if not response.data:
+            raise KeyError(key)
+
+        return True
+
+    # Implement other methods like pop, incr, decr, push, etc.
+
+    def contains(self, key):
+        serialized_key = self.get_serial_key(key)
+
+        response = (
+            self.supabase.table("cache_entries")
+            .select("*")
+            .eq("key", serialized_key)
+            .execute()
+        )
+
+        if response.status_code != 200:
+            raise Exception(f"Failed to check cache entry: {response.text}")
+
+        return bool(response.data)
+
+
 class MultiLayerCache(BaseCache):
     def __init__(self, remote_cache: BaseCache, local_cache: BaseCache):
         self.localz = remote_cache
         # We could add a middle one too
         self.remote = local_cache
         self.init_executor()
```

### Comparing `sqlpile-0.2.2/src/sqlpile/database.py` & `sqlpile-0.3.0/src/sqlpile/database.py`

 * *Files identical despite different names*

### Comparing `sqlpile-0.2.2/src/sqlpile/main.py` & `sqlpile-0.3.0/src/sqlpile/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import functools
 import time
 
 from loguru import logger
 from rich import print
+from supamodel import supabase_client
 from toolz import curry
 
 from sqlpile.abcs import BaseCache
 from sqlpile.config import settings as config
-from sqlpile.core import MultiLayerCache, SQLCache
+from sqlpile.core import MultiLayerCache, SQLCache, SupabaseCache
 
 
 def dogpile(cache_instance: BaseCache):
     def decorator(func):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             raw_key = (func.__name__, args, tuple(sorted(kwargs.items())))
@@ -25,15 +26,15 @@
 
         return wrapper
 
     return decorator
 
 
 def get_layered_cache():
-    remote = SQLCache(config.remote_db_uri)
+    remote = SupabaseCache(supabase_client)
     local = SQLCache(config.local_db_uri)
     cache = MultiLayerCache(local, remote)
     return cache
 
 
 # Create curry function of dogpile
 cache = get_layered_cache()
```

### Comparing `sqlpile-0.2.2/src/sqlpile/utils.py` & `sqlpile-0.3.0/src/sqlpile/utils.py`

 * *Files identical despite different names*

### Comparing `sqlpile-0.2.2/README.md` & `sqlpile-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sqlpile-0.2.2/pyproject.toml` & `sqlpile-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sqlpile"
-version = "0.2.2"
+version = "0.3.0"
 description = "Add your description here"
 authors = [{ name = "Kevin Hill", email = "kivo360@gmail.com" }]
 dependencies = [
     "sqlalchemy>=2.0.29",
     "psycopg[binary]>=3.1.18",
     "cloudpickle>=3.0.0",
     "lz4>=4.3.3",
@@ -18,14 +18,15 @@
     "duckdb-engine>=0.12.0",
     "pyrsistent>=0.20.0",
     "diskcache>=5.6.3",
     "asyncer>=0.0.7",
     "aiosqlite>=0.20.0",
     "cytoolz>=0.12.3",
     "toolz>=0.12.1",
+    "supamodel>=0.5.8",
 ]
 readme = "README.md"
 requires-python = ">= 3.8"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

### Comparing `sqlpile-0.2.2/PKG-INFO` & `sqlpile-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sqlpile
-Version: 0.2.2
+Version: 0.3.0
 Summary: Add your description here
 Author-email: Kevin Hill <kivo360@gmail.com>
 Requires-Python: >=3.8
 Requires-Dist: aiosqlite>=0.20.0
 Requires-Dist: asyncer>=0.0.7
 Requires-Dist: cloudpickle>=3.0.0
 Requires-Dist: cytoolz>=0.12.3
@@ -16,14 +16,15 @@
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: lz4>=4.3.3
 Requires-Dist: psycopg[binary]>=3.1.18
 Requires-Dist: pydantic-settings>=2.2.1
 Requires-Dist: pyrsistent>=0.20.0
 Requires-Dist: rich>=13.7.1
 Requires-Dist: sqlalchemy>=2.0.29
+Requires-Dist: supamodel>=0.5.8
 Requires-Dist: toolz>=0.12.1
 Requires-Dist: xxhash>=3.4.1
 Description-Content-Type: text/markdown
 
 # SQLPile - SQL-Based Multi-Layered Caching (Arrow + SQLite + Postgres)
 
 Full-featured multi-layered distributed cache using SQL databases. Why build a cache on top of a database? Largely because SQL has similar interfaces across many different databases, and it's easy to scale out. This project is a work in progress, and is not yet ready for production use.
```

