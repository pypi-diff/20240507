# Comparing `tmp/yellowbox-0.8.7.tar.gz` & `tmp/yellowbox-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowbox-0.8.7.tar", max compression
+gzip compressed data, was "yellowbox-0.8.8.tar", max compression
```

## Comparing `yellowbox-0.8.7.tar` & `yellowbox-0.8.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1081 2024-03-27 07:55:46.313817 yellowbox-0.8.7/LICENSE
--rw-r--r--   0        0        0     1265 2024-03-27 07:55:46.313817 yellowbox-0.8.7/README.md
--rw-r--r--   0        0        0     5792 2024-03-27 07:55:46.317818 yellowbox-0.8.7/pyproject.toml
--rw-r--r--   0        0        0      772 2024-03-27 07:55:46.317818 yellowbox-0.8.7/yellowbox/__init__.py
--rw-r--r--   0        0        0      236 2024-03-27 07:55:46.317818 yellowbox-0.8.7/yellowbox/_pytest.py
--rw-r--r--   0        0        0       22 2024-03-27 07:55:46.317818 yellowbox-0.8.7/yellowbox/_version.py
--rw-r--r--   0        0        0      546 2024-03-27 07:55:46.317818 yellowbox-0.8.7/yellowbox/clients.py
--rw-r--r--   0        0        0    11812 2024-03-27 07:55:46.317818 yellowbox-0.8.7/yellowbox/containers.py
--rw-r--r--   0        0        0        0 2024-03-27 07:55:46.317818 yellowbox-0.8.7/yellowbox/extras/__init__.py
--rw-r--r--   0        0        0     2602 2024-03-27 07:55:46.317818 yellowbox-0.8.7/yellowbox/extras/aerospike.py
--rw-r--r--   0        0        0     4887 2024-03-27 07:55:46.317818 yellowbox-0.8.7/yellowbox/extras/azure_storage.py
--rw-r--r--   0        0        0     6185 2024-03-27 07:55:46.317818 yellowbox-0.8.7/yellowbox/extras/fake_gcs.py
--rw-r--r--   0        0        0    10016 2024-03-27 07:55:46.317818 yellowbox-0.8.7/yellowbox/extras/http_server.py
--rw-r--r--   0        0        0     5974 2024-03-27 07:55:46.317818 yellowbox-0.8.7/yellowbox/extras/kafka.py
--rw-r--r--   0        0        0    10061 2024-03-27 07:55:46.317818 yellowbox-0.8.7/yellowbox/extras/logstash.py
--rw-r--r--   0        0        0     2558 2024-03-27 07:55:46.317818 yellowbox-0.8.7/yellowbox/extras/mssql.py
--rw-r--r--   0        0        0     3930 2024-03-27 07:55:46.317818 yellowbox-0.8.7/yellowbox/extras/postgresql.py
--rw-r--r--   0        0        0     4773 2024-03-27 07:55:46.317818 yellowbox-0.8.7/yellowbox/extras/rabbit_mq.py
--rw-r--r--   0        0        0     3433 2024-03-27 07:55:46.317818 yellowbox-0.8.7/yellowbox/extras/redis.py
--rw-r--r--   0        0        0     7692 2024-03-27 07:55:46.317818 yellowbox-0.8.7/yellowbox/extras/sql_base.py
--rw-r--r--   0        0        0     5786 2024-03-27 07:55:46.317818 yellowbox-0.8.7/yellowbox/extras/vault.py
--rw-r--r--   0        0        0      813 2024-03-27 07:55:46.317818 yellowbox-0.8.7/yellowbox/extras/webserver/__init__.py
--rw-r--r--   0        0        0     4016 2024-03-27 07:55:46.317818 yellowbox-0.8.7/yellowbox/extras/webserver/class_endpoint.py
--rw-r--r--   0        0        0    14078 2024-03-27 07:55:46.317818 yellowbox-0.8.7/yellowbox/extras/webserver/endpoints.py
--rw-r--r--   0        0        0    19539 2024-03-27 07:55:46.321817 yellowbox-0.8.7/yellowbox/extras/webserver/http_request_capture.py
--rw-r--r--   0        0        0     7772 2024-03-27 07:55:46.321817 yellowbox-0.8.7/yellowbox/extras/webserver/request_capture.py
--rw-r--r--   0        0        0     3812 2024-03-27 07:55:46.321817 yellowbox-0.8.7/yellowbox/extras/webserver/util.py
--rw-r--r--   0        0        0    13041 2024-03-27 07:55:46.321817 yellowbox-0.8.7/yellowbox/extras/webserver/webserver.py
--rw-r--r--   0        0        0    19812 2024-03-27 07:55:46.321817 yellowbox-0.8.7/yellowbox/extras/webserver/ws_request_capture.py
--rw-r--r--   0        0        0    14228 2024-03-27 07:55:46.321817 yellowbox-0.8.7/yellowbox/extras/websocket.py
--rw-r--r--   0        0        0     5768 2024-03-27 07:55:46.321817 yellowbox-0.8.7/yellowbox/image_build.py
--rw-r--r--   0        0        0     3085 2024-03-27 07:55:46.321817 yellowbox-0.8.7/yellowbox/networks.py
--rw-r--r--   0        0        0        0 2024-03-27 07:55:46.321817 yellowbox-0.8.7/yellowbox/py.typed
--rw-r--r--   0        0        0     3543 2024-03-27 07:55:46.321817 yellowbox-0.8.7/yellowbox/retry.py
--rw-r--r--   0        0        0      578 2024-03-27 07:55:46.321817 yellowbox-0.8.7/yellowbox/service.py
--rw-r--r--   0        0        0     7697 2024-03-27 07:55:46.321817 yellowbox-0.8.7/yellowbox/subclasses.py
--rw-r--r--   0        0        0     1975 2024-03-27 07:55:46.321817 yellowbox-0.8.7/yellowbox/utils.py
--rw-r--r--   0        0        0     3960 1970-01-01 00:00:00.000000 yellowbox-0.8.7/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-05-07 13:56:48.951995 yellowbox-0.8.8/LICENSE
+-rw-r--r--   0        0        0     1265 2024-05-07 13:56:48.951995 yellowbox-0.8.8/README.md
+-rw-r--r--   0        0        0     5820 2024-05-07 13:56:48.955995 yellowbox-0.8.8/pyproject.toml
+-rw-r--r--   0        0        0      772 2024-05-07 13:56:48.955995 yellowbox-0.8.8/yellowbox/__init__.py
+-rw-r--r--   0        0        0      236 2024-05-07 13:56:48.955995 yellowbox-0.8.8/yellowbox/_pytest.py
+-rw-r--r--   0        0        0       22 2024-05-07 13:57:21.632235 yellowbox-0.8.8/yellowbox/_version.py
+-rw-r--r--   0        0        0      546 2024-05-07 13:56:48.955995 yellowbox-0.8.8/yellowbox/clients.py
+-rw-r--r--   0        0        0    12140 2024-05-07 13:56:48.955995 yellowbox-0.8.8/yellowbox/containers.py
+-rw-r--r--   0        0        0        0 2024-05-07 13:56:48.955995 yellowbox-0.8.8/yellowbox/extras/__init__.py
+-rw-r--r--   0        0        0     2602 2024-05-07 13:56:48.955995 yellowbox-0.8.8/yellowbox/extras/aerospike.py
+-rw-r--r--   0        0        0     4888 2024-05-07 13:56:48.955995 yellowbox-0.8.8/yellowbox/extras/azure_storage.py
+-rw-r--r--   0        0        0     6185 2024-05-07 13:56:48.955995 yellowbox-0.8.8/yellowbox/extras/fake_gcs.py
+-rw-r--r--   0        0        0    10016 2024-05-07 13:56:48.955995 yellowbox-0.8.8/yellowbox/extras/http_server.py
+-rw-r--r--   0        0        0     5974 2024-05-07 13:56:48.955995 yellowbox-0.8.8/yellowbox/extras/kafka.py
+-rw-r--r--   0        0        0    10061 2024-05-07 13:56:48.959995 yellowbox-0.8.8/yellowbox/extras/logstash.py
+-rw-r--r--   0        0        0     2558 2024-05-07 13:56:48.959995 yellowbox-0.8.8/yellowbox/extras/mssql.py
+-rw-r--r--   0        0        0     3930 2024-05-07 13:56:48.959995 yellowbox-0.8.8/yellowbox/extras/postgresql.py
+-rw-r--r--   0        0        0     4773 2024-05-07 13:56:48.959995 yellowbox-0.8.8/yellowbox/extras/rabbit_mq.py
+-rw-r--r--   0        0        0     3417 2024-05-07 13:56:48.959995 yellowbox-0.8.8/yellowbox/extras/redis.py
+-rw-r--r--   0        0        0     7692 2024-05-07 13:56:48.959995 yellowbox-0.8.8/yellowbox/extras/sql_base.py
+-rw-r--r--   0        0        0     5786 2024-05-07 13:56:48.959995 yellowbox-0.8.8/yellowbox/extras/vault.py
+-rw-r--r--   0        0        0      813 2024-05-07 13:56:48.959995 yellowbox-0.8.8/yellowbox/extras/webserver/__init__.py
+-rw-r--r--   0        0        0     3996 2024-05-07 13:56:48.959995 yellowbox-0.8.8/yellowbox/extras/webserver/class_endpoint.py
+-rw-r--r--   0        0        0    14070 2024-05-07 13:56:48.959995 yellowbox-0.8.8/yellowbox/extras/webserver/endpoints.py
+-rw-r--r--   0        0        0    19483 2024-05-07 13:56:48.959995 yellowbox-0.8.8/yellowbox/extras/webserver/http_request_capture.py
+-rw-r--r--   0        0        0     7772 2024-05-07 13:56:48.959995 yellowbox-0.8.8/yellowbox/extras/webserver/request_capture.py
+-rw-r--r--   0        0        0     3812 2024-05-07 13:56:48.959995 yellowbox-0.8.8/yellowbox/extras/webserver/util.py
+-rw-r--r--   0        0        0    12977 2024-05-07 13:56:48.959995 yellowbox-0.8.8/yellowbox/extras/webserver/webserver.py
+-rw-r--r--   0        0        0    19764 2024-05-07 13:56:48.959995 yellowbox-0.8.8/yellowbox/extras/webserver/ws_request_capture.py
+-rw-r--r--   0        0        0    14198 2024-05-07 13:56:48.959995 yellowbox-0.8.8/yellowbox/extras/websocket.py
+-rw-r--r--   0        0        0     6729 2024-05-07 13:56:48.959995 yellowbox-0.8.8/yellowbox/image_build.py
+-rw-r--r--   0        0        0     3085 2024-05-07 13:56:48.959995 yellowbox-0.8.8/yellowbox/networks.py
+-rw-r--r--   0        0        0        0 2024-05-07 13:56:48.959995 yellowbox-0.8.8/yellowbox/py.typed
+-rw-r--r--   0        0        0     3543 2024-05-07 13:56:48.959995 yellowbox-0.8.8/yellowbox/retry.py
+-rw-r--r--   0        0        0      578 2024-05-07 13:56:48.959995 yellowbox-0.8.8/yellowbox/service.py
+-rw-r--r--   0        0        0     7697 2024-05-07 13:56:48.959995 yellowbox-0.8.8/yellowbox/subclasses.py
+-rw-r--r--   0        0        0     1975 2024-05-07 13:56:48.959995 yellowbox-0.8.8/yellowbox/utils.py
+-rw-r--r--   0        0        0     3910 1970-01-01 00:00:00.000000 yellowbox-0.8.8/PKG-INFO
```

### Comparing `yellowbox-0.8.7/LICENSE` & `yellowbox-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.7/README.md` & `yellowbox-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.7/pyproject.toml` & `yellowbox-0.8.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "yellowbox"
-version = "0.8.7"
+version = "0.8.8"
 description = ""
 authors = ["biocatch ltd"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/biocatchltd/yellowbox"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 docker = ">=4.2.0"
 yaspin = ">=1.0.0"
 requests = "*"
 
 redis = { version = ">=3.3.0", optional = true }
 pika = { version = "*", optional = true }
 # python 3.11 and lower use kafka-python, 3.12 and higher use confluent-kafka
@@ -28,62 +28,62 @@
 psycopg2 = { version = ">=2.8.6", optional = true }
 simple_websocket_server = { version = "*", optional = true }
 websockets = { version = "*", optional = true }
 hvac = { version = "*", optional = true }
 Deprecated = ">=1.2.13"
 SQLAlchemy-Utils = { version = ">=0.38.2", optional = true }
 
-# these dependcies are split due to 3.7 and 3.12 incompatibilities
+# these dependcies are split due to 3.8 and 3.12 incompatibilities
 starlette = [
     { version = ">=0.30", optional = true, python = ">=3.12" },
-    { version = ">=0.9", optional = true, python = ">=3.7" }
+    { version = ">=0.9", optional = true, python = ">=3.8" }
 ]
 uvicorn = [
     { version = ">=0.24", optional = true, python = ">=3.12" },
-    { version = ">=0.13", optional = true, python = ">=3.7" }
+    { version = ">=0.13", optional = true, python = ">=3.8" }
 ]
 pyodbc = [
     { version = ">=5.0.0", optional = true, python = ">=3.12" },
-    { version = ">=4.0.32", optional = true, python = ">=3.7" }
+    { version = ">=4.0.32", optional = true, python = ">=3.8" }
 ]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0.0"
 pytest-cov = "^4.1"
 requests = "^2"
 websocket_client = "*"
-mypy = {version=">=1", python=">=3.8"}
+mypy = {version=">=1"}
 types-requests = "^2.25.0"
 types-redis = "^3.5.4"
 pytest-xdist = "^2.1.0"
 sphinx = {version="^6.1.3", python=">=3.12"}
 furo = {version="*", python=">=3.12"}
 pytest-asyncio = "^0.18.2"
 coverage = "^6.3.2"
 types-Deprecated = "^1.2.7"
 google-cloud-storage = "^2.5.0"
 gcloud-aio-storage = "^8.0.0"
 setuptools = "^67.3.3"
-ruff = {version=">=0.1", python=">=3.8"}
+ruff = {version=">=0.1"}
 typing-extensions = "^4.6.3"
 confluent-kafka = "^2.3.0"
 
 
-# these dependencies are split due to 3.7 and 3.12 incompatibilities
+# these dependencies are split due to 3.8 and 3.12 incompatibilities
 httpx = [
     {version=">=0.25.1", python=">=3.12"},
-    {version=">=0.20", python=">=3.7"}
+    {version=">=0.20", python=">=3.8"}
 ]
 aiohttp = [
     {version=">=3.9", python=">=3.12"},
-    {version="*", python=">=3.7"}
+    {version="*", python=">=3.8"}
 ]
 frozenlist = [
     {version=">1.4", python=">=3.12"},
-    {version="*", python=">=3.7"},
+    {version="*", python=">=3.8"},
 ]
 
 [tool.poetry.extras]
 azure = ["azure-storage-blob", "cffi"]
 kafka = ["kafka-python", "confluent-kafka"]
 postgresql = ["sqlalchemy", "psycopg2", "SQLAlchemy-Utils"]
 mssql = ['sqlalchemy', "SQLAlchemy-Utils"]
@@ -103,14 +103,18 @@
 requires = ["poetry>=1.0.0"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry.plugins.pytest11]
 yellowbox = "yellowbox._pytest"
 
 [tool.ruff]
+line-length = 120
+output-format = "full"
+target-version = "py38"
+[tool.ruff.lint]
 # https://beta.ruff.rs/docs/rules/
 select = ["I", "E", "W", "F", "N", "BLE", "COM", "C4", "ISC", "ICN", "G", "PIE", "T20", "PYI", "Q", "SLF", "SIM",
           "ERA", "PGH", "PLC", "PLE", "PLR", "PLW", "RUF", "PT", "B"]
 # should be included later: UP, ANN, RET?, ARG, TRY, S
 ignore = [
     "ISC001",  # irnored by linter because of formatter
     "COM812",  # trailing comma, handled by black
@@ -128,31 +132,29 @@
     "SIM118",  # Use `key in {}` instead of `key in {}.keys()`
     "SIM112",  # Use capitalized environment variable
     "S311", # use of non-cryptographic random
     "T201",  # print found
     "PT013",  # Found incorrect import of pytest, use simple `import pytest` instead
     "B905", # `zip()` without an explicit `strict=` parameter
 ]
-line-length = 120
-show-source = true
 exclude = [
     "yellowbox/extras/websocket.py",
     "yellowbox/extras/http_server.py",
     "tests/extras/test_websocket.py",
     "tests/extras/test_http_server.py",
     "docs/conf.py",
 ]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 combine-as-imports=true
 
-[tool.ruff.flake8-pytest-style]
+[tool.ruff.lint.flake8-pytest-style]
 raises-require-match-for = []
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/**" = [
     "N802", # Function name should be lowercase
     "N803", # Argument name should be lowercase
     "S105",  # Possible hardcoded password
     "S113",  # Probable use of requests call without timeout
     "PIE804", # Unnecessary `dict` kwargs
     "PT004", # Fixture does not return anything, add leading underscore
```

### Comparing `yellowbox-0.8.7/yellowbox/__init__.py` & `yellowbox-0.8.8/yellowbox/__init__.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.7/yellowbox/clients.py` & `yellowbox-0.8.8/yellowbox/clients.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.7/yellowbox/containers.py` & `yellowbox-0.8.8/yellowbox/containers.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,16 @@
 
     return ports
 
 
 def get_aliases(container: Container, network: Union[str, Network]) -> Sequence[str]:
     if not isinstance(network, str):
         network = network.name
-    return container.attrs["NetworkSettings"]["Networks"][network]["Aliases"]
+    network_attrs = container.attrs["NetworkSettings"]["Networks"][network]
+    return network_attrs.get("Aliases") or network_attrs.get("DNSNames")
 
 
 def short_id(container: Container) -> str:
     """Get the short 12-character id of a container
 
     By default, the short 12-character id is used as a network alias in all
     of the networks connected to the container.
@@ -182,15 +183,15 @@
                     expected_exit_code = (expected_exit_code,)
 
                 if result["StatusCode"] not in expected_exit_code:
                     raise RuntimeError(f"Container {container.id} exited with code {result['StatusCode']}")
             container.remove(force=force, v=True)
 
 
-@lru_cache(maxsize=32)
+@lru_cache(maxsize=128)
 def _get_up_to_date_image(docker_client: DockerClient, image: str) -> Image:
     try:
         local_image = docker_client.images.get(image)
     except ImageNotFound:
         return docker_client.images.pull(image, platform=None)
     else:
         # we check if we should update the local image by checking the remote repo digest
@@ -224,15 +225,21 @@
         Due to inconsistent behaviour of docker's "pull" command across
         platforms, this function will raise an error if no tag is specified
     """
     name, _, tag = image.partition(":")
     if not tag:
         raise ValueError("the image name must contain a tag")
     local_image = _get_up_to_date_image(docker_client, image)
-    return docker_client.containers.create(local_image, *args, **kwargs)
+    # if we pass the image object to `create` it will label the container with a SHA image, we will try to extract the tag
+    # first
+    if local_image.tags:
+        local_image_spec = local_image.tags[0]
+    else:
+        local_image_spec = local_image.id
+    return docker_client.containers.create(local_image_spec, *args, **kwargs)
 
 
 def create_and_pull_with_defaults(*args, _kwargs: Optional[Dict[str, Any]] = None, **default_kwargs):
     if _kwargs:
         kwargs = {**default_kwargs, **_kwargs}
     else:
         kwargs = default_kwargs
@@ -282,21 +289,19 @@
 
     tar_file = tarfile.open(fileobj=temp_file)
     member = tar_file.next()
     return cast("IO[bytes]", tar_file.extractfile(member))
 
 
 @overload
-def upload_file(container: Container, path: Union[str, PathLike[str]], data: bytes) -> None:
-    ...
+def upload_file(container: Container, path: Union[str, PathLike[str]], data: bytes) -> None: ...
 
 
 @overload
-def upload_file(container: Container, path: Union[str, PathLike[str]], *, fileobj: IO[bytes]) -> None:
-    ...
+def upload_file(container: Container, path: Union[str, PathLike[str]], *, fileobj: IO[bytes]) -> None: ...
 
 
 def upload_file(
     container: Container,
     path: Union[str, PathLike[str]],
     data: Optional[bytes] = None,
     fileobj: Optional[IO[bytes]] = None,
```

### Comparing `yellowbox-0.8.7/yellowbox/extras/aerospike.py` & `yellowbox-0.8.8/yellowbox/extras/aerospike.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.7/yellowbox/extras/azure_storage.py` & `yellowbox-0.8.8/yellowbox/extras/azure_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Azure Blob Storage module, for creating container, uploading files to it and downloading files.
 """
+
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional, Sequence, Union
 
 from docker import DockerClient
 from docker.models.networks import Network
```

### Comparing `yellowbox-0.8.7/yellowbox/extras/fake_gcs.py` & `yellowbox-0.8.8/yellowbox/extras/fake_gcs.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.7/yellowbox/extras/http_server.py` & `yellowbox-0.8.8/yellowbox/extras/http_server.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.7/yellowbox/extras/kafka.py` & `yellowbox-0.8.8/yellowbox/extras/kafka.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.7/yellowbox/extras/logstash.py` & `yellowbox-0.8.8/yellowbox/extras/logstash.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.7/yellowbox/extras/mssql.py` & `yellowbox-0.8.8/yellowbox/extras/mssql.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.7/yellowbox/extras/postgresql.py` & `yellowbox-0.8.8/yellowbox/extras/postgresql.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.7/yellowbox/extras/rabbit_mq.py` & `yellowbox-0.8.8/yellowbox/extras/rabbit_mq.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.7/yellowbox/extras/redis.py` & `yellowbox-0.8.8/yellowbox/extras/redis.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,20 +54,18 @@
             raise RuntimeError("Server already started. Cannot set RDB.")
         upload_file(self.container, DEFAULT_RDB_PATH, fileobj=redis_file)
 
     def client_port(self):
         return get_ports(self.container)[REDIS_DEFAULT_PORT]
 
     @overload
-    def client(self, *, client_cls: Callable[..., _T], **kwargs) -> _T:
-        ...
+    def client(self, *, client_cls: Callable[..., _T], **kwargs) -> _T: ...
 
     @overload
-    def client(self, **kwargs) -> Redis:
-        ...
+    def client(self, **kwargs) -> Redis: ...
 
     def client(self, *, client_cls=Redis, **kwargs) -> Any:
         port = self.client_port()
         return client_cls(host=DOCKER_EXPOSE_HOST, port=port, **kwargs)
 
     def start(self, retry_spec: Optional[RetrySpec] = None):
         super().start()
```

### Comparing `yellowbox-0.8.7/yellowbox/extras/sql_base.py` & `yellowbox-0.8.8/yellowbox/extras/sql_base.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.7/yellowbox/extras/vault.py` & `yellowbox-0.8.8/yellowbox/extras/vault.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.7/yellowbox/extras/webserver/__init__.py` & `yellowbox-0.8.8/yellowbox/extras/webserver/__init__.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.7/yellowbox/extras/webserver/class_endpoint.py` & `yellowbox-0.8.8/yellowbox/extras/webserver/class_endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,15 @@
             side_effect = self.side_effect_method.__get__(instance, type(instance))
         else:
             side_effect = self.side_effect_method
         return self.constructor(*self.args, side_effect, **self.kwargs)
 
     if TYPE_CHECKING:
 
-        def __get__(self, instance, owner) -> T:
-            ...
+        def __get__(self, instance, owner) -> T: ...
 
 
 class HTTPEndpointTemplate(EndpointTemplate[MockHTTPEndpoint]):
     """
     A subclass of EndpointTemplate that is used to create an HTTP endpoint.
     """
 
@@ -61,29 +60,27 @@
 def class_http_endpoint(
     methods: METHODS,
     rule_string: str,
     *,
     auto_read_body: bool = True,
     forbid_implicit_head_verb: bool = True,
     name: Optional[str] = None,
-) -> Callable[[Any], HTTPEndpointTemplate]:
-    ...
+) -> Callable[[Any], HTTPEndpointTemplate]: ...
 
 
 @overload
 def class_http_endpoint(
     methods: METHODS,
     rule_string: str,
     side_effect: HTTP_SIDE_EFFECT,
     *,
     auto_read_body: bool = True,
     forbid_implicit_head_verb: bool = True,
     name: Optional[str] = None,
-) -> HTTPEndpointTemplate:
-    ...
+) -> HTTPEndpointTemplate: ...
 
 
 def class_http_endpoint(methods: METHODS, rule_string: str, side_effect: Optional[HTTP_SIDE_EFFECT] = None, **kwargs):
     """
     Creates an HTTP endpoint template. Declare this as a class variable in your webserver subclass to automatically add
      the endpoint to all instances. Can be used as a decorator.
     Args:
```

### Comparing `yellowbox-0.8.7/yellowbox/extras/webserver/endpoints.py` & `yellowbox-0.8.8/yellowbox/extras/webserver/endpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,29 +189,27 @@
 def http_endpoint(
     methods: METHODS,
     rule_string: str,
     *,
     auto_read_body: bool = True,
     forbid_head_verb: bool = True,
     name: Optional[str] = None,
-) -> Callable[[HTTP_SIDE_EFFECT], MockHTTPEndpoint]:
-    ...
+) -> Callable[[HTTP_SIDE_EFFECT], MockHTTPEndpoint]: ...
 
 
 @overload
 def http_endpoint(
     methods: METHODS,
     rule_string: str,
     side_effect: HTTP_SIDE_EFFECT,
     *,
     auto_read_body: bool = True,
     forbid_implicit_head_verb: bool = True,
     name: Optional[str] = None,
-) -> MockHTTPEndpoint:
-    ...
+) -> MockHTTPEndpoint: ...
 
 
 def http_endpoint(
     methods: METHODS,
     rule_string: str,
     side_effect: Optional[HTTP_SIDE_EFFECT] = None,
     *,
```

### Comparing `yellowbox-0.8.7/yellowbox/extras/webserver/http_request_capture.py` & `yellowbox-0.8.8/yellowbox/extras/webserver/http_request_capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 from yellowbox.extras.webserver.util import MismatchReason, reason_is_ne
 
 _missing = object()
 
 
 class BodyValidator(ABC):
     @abstractmethod
-    def validate(self, content: bytes) -> Optional[MismatchReason]:
-        ...
+    def validate(self, content: bytes) -> Optional[MismatchReason]: ...
 
     def repr_map(self) -> Mapping[str, Any]:
         return {"content_predicate": self}
 
 
 @dataclass(frozen=True)
 class BodyValidatorContent(BodyValidator):
@@ -317,16 +316,15 @@
         """
         if not self:
             raise AssertionError("No requests were made")
         if len(self) > 1:
             raise AssertionError("Multiple requests were made:" + "".join(f"\n\t{existing}" for existing in self))
 
     @overload
-    def assert_requested_with(self, expected: ExpectedHTTPRequest):
-        ...
+    def assert_requested_with(self, expected: ExpectedHTTPRequest): ...
 
     @overload
     def assert_requested_with(
         self,
         *,
         headers: Optional[Mapping[str, Collection[str]]] = None,
         headers_submap: Optional[Mapping[str, Collection[str]]] = None,
@@ -339,16 +337,15 @@
         body: Optional[bytes] = None,
         text: Optional[str] = None,
         json: Any = _missing,
         json_submap: Optional[Mapping[str, Any]] = None,
         content_predicate: Optional[
             Union[Callable[[bytes], bool], Tuple[Callable[[bytes], Any], Any], BodyValidator]
         ] = None,
-    ):
-        ...
+    ): ...
 
     def assert_requested_with(self, expected: Optional[ExpectedHTTPRequest] = None, **kwargs):
         """
         Asserts that the latest request recorded matches an expected request
         Args:
             expected: an expected request.
             **kwargs: if an expected request is not provided, then a new expected request is constructed by forwarding
@@ -364,16 +361,15 @@
         if not self:
             raise AssertionError("No requests were made")
         match = expected.matches(self[-1])
         if not match:
             raise AssertionError(str(match))
 
     @overload
-    def assert_requested_once_with(self, expected: ExpectedHTTPRequest):
-        ...
+    def assert_requested_once_with(self, expected: ExpectedHTTPRequest): ...
 
     @overload
     def assert_requested_once_with(
         self,
         *,
         headers: Optional[Mapping[str, Collection[str]]] = None,
         headers_submap: Optional[Mapping[str, Collection[str]]] = None,
@@ -384,16 +380,15 @@
         query_params_submap: Optional[Mapping[str, Collection[str]]] = None,
         method: Optional[str] = None,
         body: Optional[bytes] = None,
         text: Optional[str] = None,
         json: Any = _missing,
         json_submap: Optional[Mapping[str, Any]] = None,
         content_predicate: Optional[Union[Callable[[bytes], bool], Tuple[Callable[[bytes], Any], Any]]] = None,
-    ):
-        ...
+    ): ...
 
     def assert_requested_once_with(self, expected: Optional[ExpectedHTTPRequest] = None, **kwargs):
         """
         Asserts that there is only one request, and that it matches an expected request
         Args:
             expected: an expected request.
             **kwargs: if an expected request is not provided, then a new expected request is constructed by forwarding
@@ -411,16 +406,15 @@
         if len(self) > 1:
             raise AssertionError("Multiple requests were made:" + "".join(f"\n\t{existing}" for existing in self))
         match = expected.matches(self[0])
         if not match:
             raise AssertionError(str(match))
 
     @overload
-    def assert_any_request(self, expected: ExpectedHTTPRequest):
-        ...
+    def assert_any_request(self, expected: ExpectedHTTPRequest): ...
 
     @overload
     def assert_any_request(
         self,
         *,
         headers: Optional[Mapping[str, Collection[str]]] = None,
         headers_submap: Optional[Mapping[str, Collection[str]]] = None,
@@ -433,16 +427,15 @@
         body: Optional[bytes] = None,
         text: Optional[str] = None,
         json: Any = _missing,
         json_submap: Optional[Mapping[str, Any]] = None,
         content_predicate: Optional[
             Union[Callable[[bytes], bool], Tuple[Callable[[bytes], Any], Any], BodyValidator]
         ] = None,
-    ):
-        ...
+    ): ...
 
     def assert_any_request(self, expected: Optional[ExpectedHTTPRequest] = None, **kwargs):
         """
         Asserts that at least one request recorded matches an expected request
         Args:
             expected: an expected request.
             **kwargs: if an expected request is not provided, then a new expected request is constructed by forwarding
```

### Comparing `yellowbox-0.8.7/yellowbox/extras/webserver/request_capture.py` & `yellowbox-0.8.8/yellowbox/extras/webserver/request_capture.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.7/yellowbox/extras/webserver/util.py` & `yellowbox-0.8.8/yellowbox/extras/webserver/util.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.7/yellowbox/extras/webserver/webserver.py` & `yellowbox-0.8.8/yellowbox/extras/webserver/webserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,29 +93,27 @@
             sleep(self._PORT_ACCESS_INTERVAL)
         else:
             raise RuntimeError("timed out when getting binding port")
         self._port = socket.getsockname()[1]
         return self._port
 
     @overload
-    def add_http_endpoint(self, endpoint: MockHTTPEndpoint) -> MockHTTPEndpoint:
-        ...
+    def add_http_endpoint(self, endpoint: MockHTTPEndpoint) -> MockHTTPEndpoint: ...
 
     @overload
     def add_http_endpoint(
         self,
         methods: METHODS,
         rule_string: str,
         side_effect: HTTP_SIDE_EFFECT,
         *,
         auto_read_body: bool = True,
         forbid_implicit_head_verb: bool = True,
         name: Optional[str] = None,
-    ) -> MockHTTPEndpoint:
-        ...
+    ) -> MockHTTPEndpoint: ...
 
     def add_http_endpoint(self, *args, **kwargs) -> MockHTTPEndpoint:
         """
         Add an http endpoint to the server
         Args:
             *args: either a single mock http endpoint, or parameters forwarded to http_endpoint construct one
             **kwargs: forwarded to http_endpoint to construct an endpoint
@@ -155,29 +153,27 @@
             )
             if i is None:
                 raise RuntimeError("endpoint is not found in the server")
             self._app.router.routes.pop(i)
             endpoint.owner = None
 
     @overload
-    def patch_http_endpoint(self, endpoint: MockHTTPEndpoint) -> ContextManager[MockHTTPEndpoint]:
-        ...
+    def patch_http_endpoint(self, endpoint: MockHTTPEndpoint) -> ContextManager[MockHTTPEndpoint]: ...
 
     @overload
     def patch_http_endpoint(
         self,
         methods: METHODS,
         rule_string: str,
         side_effect: HTTP_SIDE_EFFECT,
         *,
         auto_read_body: bool = True,
         forbid_implicit_head_verb: bool = True,
         name: Optional[str] = None,
-    ) -> ContextManager[MockHTTPEndpoint]:
-        ...
+    ) -> ContextManager[MockHTTPEndpoint]: ...
 
     @contextmanager  # type:ignore[misc]
     def patch_http_endpoint(self, *args, **kwargs) -> Iterator[MockHTTPEndpoint]:
         """
         A context manager to add and then remove an http endpoint
         Args:
             *args: forwarded to self.add_http_endpoint
@@ -189,27 +185,25 @@
         ep = self.add_http_endpoint(*args, **kwargs)
         try:
             yield ep
         finally:
             self.remove_http_endpoint(ep)
 
     @overload
-    def add_ws_endpoint(self, endpoint: MockWSEndpoint) -> MockWSEndpoint:
-        ...
+    def add_ws_endpoint(self, endpoint: MockWSEndpoint) -> MockWSEndpoint: ...
 
     @overload
     def add_ws_endpoint(
         self,
         rule_string: str,
         side_effect: WS_SIDE_EFFECT,
         *,
         name: Optional[str] = None,
         allow_abrupt_disconnect: bool = True,
-    ) -> MockWSEndpoint:
-        ...
+    ) -> MockWSEndpoint: ...
 
     def add_ws_endpoint(self, *args, **kwargs):
         """
         Add a websocket endpoint to the server
         Args:
             *args: either a single mock ws endpoint, or parameters forwarded to ws_endpoint construct one
             **kwargs: forwarded to ws_endpoint to construct an endpoint
@@ -251,27 +245,25 @@
             )
             if i is None:
                 raise RuntimeError("endpoint is not found in the server")
             self._app.router.routes.pop(i)
             endpoint.owner = None
 
     @overload
-    def patch_ws_endpoint(self, endpoint: MockWSEndpoint) -> ContextManager[MockWSEndpoint]:
-        ...
+    def patch_ws_endpoint(self, endpoint: MockWSEndpoint) -> ContextManager[MockWSEndpoint]: ...
 
     @overload
     def patch_ws_endpoint(
         self,
         rule_string: str,
         side_effect: WS_SIDE_EFFECT,
         *,
         name: Optional[str] = None,
         allow_abrupt_disconnect: bool = True,
-    ) -> ContextManager[MockWSEndpoint]:
-        ...
+    ) -> ContextManager[MockWSEndpoint]: ...
 
     @contextmanager  # type:ignore[misc]
     def patch_ws_endpoint(self, *args, **kwargs):
         """
         A context manager to add and then remove a ws endpoint
         Args:
             *args: forwarded to self.add_ws_endpoint
```

### Comparing `yellowbox-0.8.7/yellowbox/extras/webserver/ws_request_capture.py` & `yellowbox-0.8.8/yellowbox/extras/webserver/ws_request_capture.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,16 +366,15 @@
         """
         if not self:
             raise AssertionError("No requests were made")
         if len(self) > 1:
             raise AssertionError(f"{len(self)} requests were made")
 
     @overload
-    def assert_requested_with(self, expected: ExpectedWSTranscript):
-        ...
+    def assert_requested_with(self, expected: ExpectedWSTranscript): ...
 
     @overload
     def assert_requested_with(
         self,
         *,
         messages: Sequence[Union[builtins.ellipsis, ExpectedWSMessage]] = (...,),
         headers: Optional[Mapping[bytes, Collection[bytes]]] = None,
@@ -383,16 +382,15 @@
         path: Optional[Union[str, Pattern[str]]] = None,
         path_params: Optional[Mapping[str, Any]] = None,
         path_params_submap: Optional[Mapping[str, Any]] = None,
         query_params: Optional[Mapping[str, Collection[str]]] = None,
         query_params_submap: Optional[Mapping[str, Collection[str]]] = None,
         close: Optional[Tuple[Sender, int]] = None,
         accepted: Optional[bool] = True,
-    ):
-        ...
+    ): ...
 
     def assert_requested_with(self, expected: Optional[ExpectedWSTranscript] = None, **kwargs):
         """
         Asserts that the latest transcript recorded matches an expected transcript
         Args:
             expected: an expected transcript.
             **kwargs: if an expected request is not provided, then a new expected request is constructed by forwarding
@@ -408,16 +406,15 @@
         if not self:
             raise AssertionError("No requests were made")
         match = expected.matches(self[-1])
         if not match:
             raise AssertionError(str(match))
 
     @overload
-    def assert_requested_once_with(self, expected: ExpectedWSTranscript):
-        ...
+    def assert_requested_once_with(self, expected: ExpectedWSTranscript): ...
 
     @overload
     def assert_requested_once_with(
         self,
         *,
         messages: Sequence[Union[builtins.ellipsis, ExpectedWSMessage]] = (...,),
         headers: Optional[Mapping[bytes, Collection[bytes]]] = None,
@@ -425,16 +422,15 @@
         path: Optional[Union[str, Pattern[str]]] = None,
         path_params: Optional[Mapping[str, Any]] = None,
         path_params_submap: Optional[Mapping[str, Any]] = None,
         query_params: Optional[Mapping[str, Collection[str]]] = None,
         query_params_submap: Optional[Mapping[str, Collection[str]]] = None,
         close: Optional[Tuple[Sender, int]] = None,
         accepted: Optional[bool] = True,
-    ):
-        ...
+    ): ...
 
     def assert_requested_once_with(self, expected: Optional[ExpectedWSTranscript] = None, **kwargs):
         """
         Asserts that there is only one transcript, and that it matches an expected transcript
         Args:
             expected: an expected transcript.
             **kwargs: if an expected request is not provided, then a new expected request is constructed by forwarding
@@ -452,16 +448,15 @@
         if len(self) > 1:
             raise AssertionError(f"{len(self)} requests were made")
         match = expected.matches(self[0])
         if not match:
             raise AssertionError(str(match))
 
     @overload
-    def assert_any_request(self, expected: ExpectedWSTranscript):
-        ...
+    def assert_any_request(self, expected: ExpectedWSTranscript): ...
 
     @overload
     def assert_any_request(
         self,
         *,
         messages: Sequence[Union[builtins.ellipsis, ExpectedWSMessage]] = (...,),
         headers: Optional[Mapping[bytes, Collection[bytes]]] = None,
@@ -469,16 +464,15 @@
         path: Optional[Union[str, Pattern[str]]] = None,
         path_params: Optional[Mapping[str, Any]] = None,
         path_params_submap: Optional[Mapping[str, Any]] = None,
         query_params: Optional[Mapping[str, Collection[str]]] = None,
         query_params_submap: Optional[Mapping[str, Collection[str]]] = None,
         close: Optional[Tuple[Sender, int]] = None,
         accepted: Optional[bool] = True,
-    ):
-        ...
+    ): ...
 
     def assert_any_request(self, expected: Optional[ExpectedWSTranscript] = None, **kwargs):
         """
         Asserts that the at least one transcript recorded matches an expected transcript
         Args:
             expected: an expected transcript.
             **kwargs: if an expected request is not provided, then a new expected request is constructed by forwarding
```

### Comparing `yellowbox-0.8.7/yellowbox/extras/websocket.py` & `yellowbox-0.8.8/yellowbox/extras/websocket.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,15 +286,14 @@
         self._thread.join(1)
 
         # Shouldn't actually happen.
         if self._thread.is_alive():
             logger.error("Failed to stop the service gracefully. Timed out.")
 
         self._server.close()
-        return super().stop()
 
     def _get_generator(self, path: str) -> Union[_GEN_FUNCTION_TYPE, None]:
         """Get the IO generator function appropriate to the connected path.
 
         Args:
             path: Websocket path.
```

### Comparing `yellowbox-0.8.7/yellowbox/image_build.py` & `yellowbox-0.8.8/yellowbox/image_build.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 class DockerfileParseError(BuildError):
     pass
 
 
 DockerfileParseException = DockerfileParseError  # legacy alias
 
 
-def _docker_build(docker_client: DockerClient, output: TextIO, **kwargs):
+def _docker_build(docker_client: DockerClient, output: TextIO, **kwargs) -> Optional[str]:
     build_log = docker_client.api.build(**kwargs)
+    id = None
     for msg_b in build_log:
         msgs = str(msg_b, "utf-8").splitlines()
         for msg in msgs:
             try:
                 parse_msg = json.loads(msg)
             except JSONDecodeError as e:
                 raise DockerException("error at build logs") from e
@@ -46,22 +47,28 @@
                     raise BuildError(reason=error_detail, build_log=None)
                 elif error_msg is not None:
                     raise DockerfileParseError(reason=error_msg, build_log=None)
                 elif status is not None and output:
                     print(status, end="", flush=True, file=output)
                 elif aux is not None and output:
                     print(aux, end="", flush=True, file=output)
+                    if "ID" in aux:
+                        # ID, means that the image was created successfully
+                        id = aux["ID"]
                 else:
                     raise DockerException(parse_msg)
+    if id is None:
+        raise BuildError("No ID found in build log")
+    return id
 
 
 @contextmanager
 def build_image(
     docker_client: DockerClient,
-    image_name: str,
+    image_name: Optional[str],
     remove_image: bool = True,
     file: Optional[TextIO] = ...,  # type: ignore[assignment]
     output: Optional[TextIO] = sys.stderr,
     spinner: bool = True,
     **kwargs,
 ):
     """
@@ -81,35 +88,42 @@
             "The `file` parameter is deprecated and will be removed in a future version",
             DeprecationWarning,
             stacklevel=1,
         )
         output = file
 
     # spinner splits into multiple lines in case stream is being printed at the same time
-    if ":" in image_name:
-        image_tag = image_name
+    kwargs = {"rm": True, "forcerm": True, **kwargs}
+    if image_name is None:
+        msg = "Creating anonymous image..."
+        image_tag = None
     else:
-        image_tag = f"{image_name}:test"
+        if ":" in image_name:
+            image_tag = image_name
+        else:
+            image_tag = f"{image_name}:test"
+        msg = f"Creating image {image_tag}..."
+        kwargs["tag"] = image_tag
     yaspin_spinner = _get_spinner(spinner)
-    with yaspin_spinner(f"Creating image {image_tag}..."):
-        kwargs = {"tag": image_tag, "rm": True, "forcerm": True, **kwargs}
-        _docker_build(docker_client, output, **kwargs)
-        yield image_tag
+    with yaspin_spinner(msg):
+        image_id = _docker_build(docker_client, output, **kwargs)
+        image_alias = image_tag if image_tag is not None else image_id
+        yield image_alias
         if remove_image:
             try:
-                docker_client.api.remove_image(image_tag)
+                docker_client.api.remove_image(image_alias)
             except ImageNotFound:
                 # if the image was already deleted
                 pass
 
 
 @asynccontextmanager
 async def async_build_image(
     docker_client: DockerClient,
-    image_name: str,
+    image_name: Optional[str],
     remove_image: bool = True,
     output: Optional[TextIO] = sys.stderr,
     spinner: bool = True,
     **kwargs,
 ):
     """
     Create a docker image (similar to docker build command)
@@ -117,40 +131,51 @@
     Args:
         docker_client: DockerClient to be used to create the image
         image_name: Name of the image to be created. If no tag is provided, the tag "test" will be added.
         remove_image: boolean, whether or not to delete the image at the end, default as True
         file: a file-like object (stream)
     """
     # spinner splits into multiple lines in case stream is being printed at the same time
-    if ":" in image_name:
-        image_tag = image_name
-    else:
-        image_tag = f"{image_name}:test"
     file = StringIO()
     kwargs = {
         "docker_client": docker_client,
         "output": file,
-        "tag": image_tag,
         "rm": True,
         "forcerm": True,
         **kwargs,
     }
+    kwargs = {"rm": True, "forcerm": True, **kwargs}
+    if image_name is None:
+        start_msg = "Creating anonymous image..."
+        fail_msg = "failed building anonymous image"
+        ok_msg = "anonymous image built successfully"
+        image_tag = None
+    else:
+        if ":" in image_name:
+            image_tag = image_name
+        else:
+            image_tag = f"{image_name}:test"
+        start_msg = f".   Creating image {image_tag}..."
+        fail_msg = f"failed building image {image_tag}"
+        ok_msg = f".   image {image_tag} built successfully"
+        kwargs["tag"] = image_tag
     if spinner and output:
-        print(f".   building image {image_tag}...", file=output)
+        print(start_msg, file=output)
     try:
-        await get_event_loop().run_in_executor(None, partial(_docker_build, **kwargs))
+        image_id = await get_event_loop().run_in_executor(None, partial(_docker_build, **kwargs))
     except (DockerException, BuildError, DockerfileParseError) as e:
-        print(f"failed building image {image_tag}", file=sys.stderr)
+        print(fail_msg, file=sys.stderr)
         print(file.getvalue(), file=sys.stderr)
         raise e
-    else:
-        if spinner and output:
-            print(f".   image {image_tag} built successfully", file=output)
-            print(file.getvalue(), file=output)
 
-    yield image_tag
+    if spinner and output:
+        print(ok_msg, file=output)
+        print(file.getvalue(), file=output)
+
+    image_alias = image_id if image_tag is None else image_tag
+    yield image_alias
     if remove_image:
         try:
-            await get_event_loop().run_in_executor(None, docker_client.api.remove_image, image_tag)
+            await get_event_loop().run_in_executor(None, docker_client.api.remove_image, image_alias)
         except ImageNotFound:
             # if the image was already deleted
             pass
```

### Comparing `yellowbox-0.8.7/yellowbox/networks.py` & `yellowbox-0.8.8/yellowbox/networks.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.7/yellowbox/retry.py` & `yellowbox-0.8.8/yellowbox/retry.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.7/yellowbox/service.py` & `yellowbox-0.8.8/yellowbox/service.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.7/yellowbox/subclasses.py` & `yellowbox-0.8.8/yellowbox/subclasses.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.7/yellowbox/utils.py` & `yellowbox-0.8.8/yellowbox/utils.py`

 * *Files identical despite different names*

### Comparing `yellowbox-0.8.7/PKG-INFO` & `yellowbox-0.8.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: yellowbox
-Version: 0.8.7
+Version: 0.8.8
 Summary: 
 Home-page: https://github.com/biocatchltd/yellowbox
 License: MIT
 Author: biocatch ltd
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: aerospike
 Provides-Extra: azure
@@ -33,23 +32,23 @@
 Requires-Dist: cffi (>=1.14.0) ; extra == "azure" or extra == "dev"
 Requires-Dist: confluent-kafka ; (python_version >= "3.12") and (extra == "kafka")
 Requires-Dist: docker (>=4.2.0)
 Requires-Dist: hvac ; extra == "vault" or extra == "dev"
 Requires-Dist: kafka-python ; (python_version < "3.12") and (extra == "kafka" or extra == "dev")
 Requires-Dist: pika ; extra == "rabbit" or extra == "dev"
 Requires-Dist: psycopg2 (>=2.8.6) ; extra == "postgresql" or extra == "dev"
-Requires-Dist: pyodbc (>=4.0.32) ; (python_version >= "3.7") and (extra == "dev")
+Requires-Dist: pyodbc (>=4.0.32) ; (python_version >= "3.8") and (extra == "dev")
 Requires-Dist: pyodbc (>=5.0.0) ; (python_version >= "3.12") and (extra == "dev")
 Requires-Dist: redis (>=3.3.0) ; extra == "redis" or extra == "dev"
 Requires-Dist: requests
 Requires-Dist: simple_websocket_server ; extra == "websocket" or extra == "dev"
 Requires-Dist: sqlalchemy (>=1.3.0) ; extra == "postgresql" or extra == "mssql" or extra == "dev"
 Requires-Dist: starlette (>=0.30) ; (python_version >= "3.12") and (extra == "webserver" or extra == "dev")
-Requires-Dist: starlette (>=0.9) ; (python_version >= "3.7") and (extra == "webserver" or extra == "dev")
-Requires-Dist: uvicorn (>=0.13) ; (python_version >= "3.7") and (extra == "webserver" or extra == "dev")
+Requires-Dist: starlette (>=0.9) ; (python_version >= "3.8") and (extra == "webserver" or extra == "dev")
+Requires-Dist: uvicorn (>=0.13) ; (python_version >= "3.8") and (extra == "webserver" or extra == "dev")
 Requires-Dist: uvicorn (>=0.24) ; (python_version >= "3.12") and (extra == "webserver" or extra == "dev")
 Requires-Dist: websockets ; extra == "webserver" or extra == "dev"
 Requires-Dist: yaspin (>=1.0.0)
 Project-URL: Repository, https://github.com/biocatchltd/yellowbox
 Description-Content-Type: text/markdown
 
 # Yellowbox
```

