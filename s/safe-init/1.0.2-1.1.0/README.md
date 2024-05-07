# Comparing `tmp/safe_init-1.0.2.tar.gz` & `tmp/safe_init-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe_init-1.0.2.tar", max compression
+gzip compressed data, was "safe_init-1.1.0.tar", max compression
```

## Comparing `safe_init-1.0.2.tar` & `safe_init-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1063 2024-04-12 09:41:11.874812 safe_init-1.0.2/LICENSE
--rw-r--r--   0        0        0    12409 2024-04-12 09:41:11.878812 safe_init-1.0.2/README.md
--rw-r--r--   0        0        0     3205 2024-04-12 09:41:11.890812 safe_init-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      736 2024-04-12 09:41:11.890812 safe_init-1.0.2/safe_init/__init__.py
--rw-r--r--   0        0        0     7429 2024-04-12 09:41:11.890812 safe_init-1.0.2/safe_init/decorator.py
--rw-r--r--   0        0        0     4240 2024-04-12 09:41:11.890812 safe_init-1.0.2/safe_init/dlq.py
--rw-r--r--   0        0        0      751 2024-04-12 09:41:11.890812 safe_init-1.0.2/safe_init/errors.py
--rw-r--r--   0        0        0     5456 2024-04-12 09:41:11.890812 safe_init-1.0.2/safe_init/handler.py
--rw-r--r--   0        0        0        0 2024-04-12 09:41:11.890812 safe_init-1.0.2/safe_init/py.typed
--rw-r--r--   0        0        0     3909 2024-04-12 09:41:11.890812 safe_init-1.0.2/safe_init/safe_logging.py
--rw-r--r--   0        0        0     2551 2024-04-12 09:41:11.890812 safe_init-1.0.2/safe_init/sentry.py
--rw-r--r--   0        0        0     5621 2024-04-12 09:41:11.890812 safe_init-1.0.2/safe_init/slack.py
--rw-r--r--   0        0        0     6334 2024-04-12 09:41:11.890812 safe_init-1.0.2/safe_init/timeout.py
--rw-r--r--   0        0        0     3918 2024-04-12 09:41:11.890812 safe_init-1.0.2/safe_init/tracer.py
--rw-r--r--   0        0        0     3237 2024-04-12 09:41:11.890812 safe_init-1.0.2/safe_init/utils.py
--rw-r--r--   0        0        0    13894 1970-01-01 00:00:00.000000 safe_init-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-07 06:00:23.823182 safe_init-1.1.0/LICENSE
+-rw-r--r--   0        0        0    14385 2024-05-07 06:00:23.823182 safe_init-1.1.0/README.md
+-rw-r--r--   0        0        0     3226 2024-05-07 06:00:23.835182 safe_init-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      736 2024-05-07 06:00:23.835182 safe_init-1.1.0/safe_init/__init__.py
+-rw-r--r--   0        0        0     7429 2024-05-07 06:00:23.835182 safe_init-1.1.0/safe_init/decorator.py
+-rw-r--r--   0        0        0     4240 2024-05-07 06:00:23.835182 safe_init-1.1.0/safe_init/dlq.py
+-rw-r--r--   0        0        0      751 2024-05-07 06:00:23.835182 safe_init-1.1.0/safe_init/errors.py
+-rw-r--r--   0        0        0     5810 2024-05-07 06:00:23.835182 safe_init-1.1.0/safe_init/handler.py
+-rw-r--r--   0        0        0        0 2024-05-07 06:00:23.835182 safe_init-1.1.0/safe_init/py.typed
+-rw-r--r--   0        0        0     3909 2024-05-07 06:00:23.835182 safe_init-1.1.0/safe_init/safe_logging.py
+-rw-r--r--   0        0        0     5832 2024-05-07 06:00:23.839182 safe_init-1.1.0/safe_init/secrets.py
+-rw-r--r--   0        0        0     2551 2024-05-07 06:00:23.839182 safe_init-1.1.0/safe_init/sentry.py
+-rw-r--r--   0        0        0     5621 2024-05-07 06:00:23.839182 safe_init-1.1.0/safe_init/slack.py
+-rw-r--r--   0        0        0     6334 2024-05-07 06:00:23.839182 safe_init-1.1.0/safe_init/timeout.py
+-rw-r--r--   0        0        0     3918 2024-05-07 06:00:23.839182 safe_init-1.1.0/safe_init/tracer.py
+-rw-r--r--   0        0        0     3949 2024-05-07 06:00:23.839182 safe_init-1.1.0/safe_init/utils.py
+-rw-r--r--   0        0        0    15904 1970-01-01 00:00:00.000000 safe_init-1.1.0/PKG-INFO
```

### Comparing `safe_init-1.0.2/LICENSE` & `safe_init-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.2/README.md` & `safe_init-1.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 - **Slack Notifications**: Sends informative Slack notifications with error details, keeping your team informed about any issues in real-time.
 - **Datadog Integration**: Integrates seamlessly with the Datadog Lambda wrapper for enhanced monitoring and metrics collection.
 
 ### Resilience and Reliability
 - **Dead-Letter Queue (DLQ) Support**: Pushes failed events to a dead-letter queue for later processing, ensuring that no events are lost due to errors.
 - **Initialization Checks**: Detects missing Sentry initialization and Lambda init phase timeouts, preventing silent failures and providing early warning signs.
 - **Timeout Notifications**: Sends notifications a configurable number of seconds before the Lambda timeout occurs, giving you a heads-up to investigate and address potential issues.
+- **AWS Secrets Resolution**: Automatically resolves AWS Secrets Manager secrets in environment variables, simplifying secret management and access.
 
 ### Customization and Flexibility
 - **Customizable Logger**: Allows you to use a custom logger instead of the default structlog logger, providing flexibility to integrate with your existing logging setup.
 - **Easy to Use**: Simply set the Lambda handler to `safe_init.handler.handler` and configure the `SAFE_INIT_HANDLER` environment variable to point to your original code handler. No further changes or decorators needed!
 
 ## Installation
 
@@ -78,14 +79,21 @@
 - `SAFE_INIT_NOTIFY_SEC_BEFORE_TIMEOUT` (optional): The number of seconds before the Lambda timeout to send a notification. Defaults to 5 seconds for timeouts < 120s, and 10 seconds for timeouts >= 120s. It's like a friendly tap on the shoulder, reminding you to check on your Lambda before it times out.
 - `SAFE_INIT_TRACER_HOME_PATHS` (optional): A comma-separated list of paths to mark as "home" in function call tracing. Paths containing these strings will be marked with a ⚡ emoji in Slack notifications. Because home is where the heart is, and the ⚡ emoji is just cool!
 - `SAFE_INIT_IGNORE_TIMEOUTS` (optional): Set to `'true'` to disable timeout notifications. For those times when you just don't want to be bothered about timeouts.
 - `SAFE_INIT_NO_SLACK_TIMEOUT_NOTIFICATIONS` (optional): Set to `'true'` to disable Slack notifications for timeouts. Sometimes, you just need a break from all the notifications.
 - `SAFE_INIT_NO_DATADOG_WRAPPER` (optional): Set to `'true'` to disable Datadog integration. If you're not using Datadog, this is the option for you!
 - `SAFE_INIT_AUTO_TRACE_LAMBDAS` (optional): Set to `'true'` to automatically trace all function calls in Lambda handlers. **Warning:** this can significantly increase memory usage and execution time. Use with caution!
 - `SAFE_INIT_LOGGING_USE_CONSOLE_RENDERER` (optional): Set to `'true'` to use the console renderer for logs. For those times when you want your logs to look extra fancy in the console.
+- `SAFE_INIT_RESOLVE_SECRETS` (optional): Set to `true` to resolve AWS Secrets Manager secrets in environment variables. Safe Init will automatically resolve secrets in environment variables with names ending with a configured suffix and save them in environment variables with the original name minus the suffix.
+- `SAFE_INIT_SECRET_ARN_SUFFIX` (optional): The suffix to use for resolving AWS Secrets Manager secrets in environment variables. Defaults to `_SECRET_ARN`. Use this to specify the suffix that marks environment variables as containing secret ARNs.
+- `SAFE_INIT_CACHE_SECRETS` (optional): Set to `true` to cache resolved secrets in Redis. Safe Init will cache resolved secrets in Redis to reduce the number of calls to AWS Secrets Manager.
+- `SAFE_INIT_SECRET_CACHE_REDIS_HOST`, `SAFE_INIT_SECRET_CACHE_REDIS_PORT`, `SAFE_INIT_SECRET_CACHE_REDIS_DB`, `SAFE_INIT_SECRET_CACHE_REDIS_USERNAME`, `SAFE_INIT_SECRET_CACHE_REDIS_PASSWORD` (host&port required if secret caching enabled): Redis connection details for caching resolved secrets. Use these environment variables to specify the Redis host, port, database, and password for caching resolved secrets.
+- `SAFE_INIT_SECRET_CACHE_TTL` (optional): TTL for cached secrets in seconds. Defaults to 1800 seconds (30 minutes). Use this to specify how long resolved secrets should be cached in Redis.
+- `SAFE_INIT_SECRET_CACHE_PREFIX` (optional): Prefix for cached secrets in Redis. Defaults to `safe-init-secret::`. Use this to specify the prefix for keys used to store cached secrets in Redis.
+- `SAFE_INIT_FAIL_ON_SECRET_RESOLUTION_ERROR` (optional): Set to `true` to fail the Lambda initialization if an error occurs during secret resolution. Safe Init will raise an exception if an error occurs during secret resolution, preventing the Lambda function from starting.
 
 With these configuration options, Safe Init provides a flexible and customizable way to enhance your Lambda functions' error handling, logging, and monitoring capabilities. Mix and match the options to suit your needs, and let Safe Init be your loyal companion on your Lambda adventures! 🚀
 
 ## Advanced Usage
 
 ### Custom Logger
```

### Comparing `safe_init-1.0.2/pyproject.toml` & `safe_init-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "safe-init"
-version = "1.0.2"
+version = "1.1.0"
 description = "Safe Init is a Python library that enhances AWS Lambda functions with advanced error handling, logging, monitoring, and resilience features, providing comprehensive observability and reliability for serverless applications."
 license = "MIT"
 authors = ["Maciej Wilczyński <maciej@lupine.software>"]
 repository = "https://github.com/kalepa/safe-init"
 readme = "README.md"
 packages = [{ include = "safe_init" }]
 include = ["safe_init/py.typed"]
@@ -29,14 +29,15 @@
 sentry-sdk = "<2.0.0"
 requests = "^2.31.0"
 awslambdaric = ">=2.0.10"
 boto3 = ">=1.20.0"
 boto3-type-annotations = ">=0.3.1"
 datadog-lambda = "*"
 ddtrace = "*"
+redis = ">=4.0.0,<6"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 mypy = "^1.4.1"
 types-ujson = ">=5.8.0.0"
 types-colorama = ">=0.4.15.11"
 types-urllib3 = ">=1.26.25.13,<2.0.0"
```

### Comparing `safe_init-1.0.2/safe_init/__init__.py` & `safe_init-1.1.0/safe_init/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any
 
-__VERSION__ = "1.0.2"
+__VERSION__ = "1.1.0"
 
 _wrapped_handler = None
 
 
 class LazyHandler:
     @staticmethod
     def _init_handler() -> None:
```

### Comparing `safe_init-1.0.2/safe_init/decorator.py` & `safe_init-1.1.0/safe_init/decorator.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.2/safe_init/dlq.py` & `safe_init-1.1.0/safe_init/dlq.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.2/safe_init/errors.py` & `safe_init-1.1.0/safe_init/errors.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.2/safe_init/handler.py` & `safe_init-1.1.0/safe_init/handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """
 This module provides a function for wrapping a Lambda handler function with error handling and logging.
 """
 
 import hashlib
 import json
 import os
-from collections.abc import Callable
+from collections.abc import Callable, Mapping
 from importlib import import_module
 
 from safe_init.decorator import safe_wrapper
 from safe_init.dlq import SafeInitDummyHandler, context_has_dlq
 from safe_init.errors import (
     SafeInitError,
     SafeInitInitPhaseTimeoutWarning,
     SafeInitMissingSentryWarning,
 )
 from safe_init.safe_logging import log_exception, log_warning
+from safe_init.secrets import context_has_secrets_to_resolve, resolve_secrets
 from safe_init.sentry import sentry_capture
 from safe_init.slack import slack_notify
-from safe_init.utils import get_sentry_sdk
+from safe_init.utils import env, get_sentry_sdk
 
 
 def _init_handler() -> Callable:
     """
     Initializes the Lambda handler function by importing the module and function specified in the SAFE_INIT_HANDLER
     environment variable, and wrapping it with error handling and logging.
 
@@ -35,20 +36,25 @@
     """
     try:
         target_handler = os.getenv("SAFE_INIT_HANDLER", "").strip()
         if not target_handler:
             msg = "SAFE_INIT_HANDLER environment variable is not set"
             raise SafeInitError(msg)  # noqa: TRY301
 
-        _pre_import_hook(target_handler)
-        root_module, handler_name = target_handler.rsplit(".", 1)
-        handler_module = import_module(".".join(root_module.split("/")))
-        _post_import_hook(target_handler)
+        secrets_env: Mapping[str, str | None] = {}
+        if os.getenv("SAFE_INIT_RESOLVE_SECRETS", "false").lower() == "true" and context_has_secrets_to_resolve():
+            secrets_env = resolve_secrets()
+
+        with env(secrets_env):
+            _pre_import_hook(target_handler)
+            root_module, handler_name = target_handler.rsplit(".", 1)
+            handler_module = import_module(".".join(root_module.split("/")))
+            _post_import_hook(target_handler)
 
-        exec_result = safe_wrapper(getattr(handler_module, handler_name))
+            exec_result = safe_wrapper(getattr(handler_module, handler_name))
 
         if not os.getenv("SAFE_INIT_NO_DETECT_UNINITIALIZED_SENTRY") and not get_sentry_sdk().Hub.current.client:
             msg = "Detected missing Sentry initialization"
             slack_notify(
                 msg,
                 SafeInitMissingSentryWarning(msg),
                 handler_name=target_handler,
```

### Comparing `safe_init-1.0.2/safe_init/safe_logging.py` & `safe_init-1.1.0/safe_init/safe_logging.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.2/safe_init/sentry.py` & `safe_init-1.1.0/safe_init/sentry.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.2/safe_init/slack.py` & `safe_init-1.1.0/safe_init/slack.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.2/safe_init/timeout.py` & `safe_init-1.1.0/safe_init/timeout.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.2/safe_init/tracer.py` & `safe_init-1.1.0/safe_init/tracer.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.2/safe_init/utils.py` & `safe_init-1.1.0/safe_init/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import contextlib
 import os
+from collections.abc import Iterator, Mapping
 from typing import Any
 
 from safe_init.tracer import FunctionCall, FunctionCallSummary
 
 _sentry_sdk = None
 
 
@@ -90,7 +92,26 @@
         return "_No function calls were traced_"
     return f"🕵️ *Top {limit} most time-consuming function call{'s' if limit != 1 else ''}:*\n" + "\n".join(
         f"{idx + 1}. `{fnc.function_name}`: *{fnc.total_execution_time:.3f}s*, called"
         f" {fnc.execution_count} time{'s' if fnc.execution_count != 1 else ''} (`{fnc.file_name}`)"
         f" {home_mark(fnc.file_name)}"
         for idx, fnc in enumerate(traces[:limit])
     )
+
+
+@contextlib.contextmanager
+def env(new_vars: Mapping[str, str | None]) -> Iterator:
+    environ = os.environ
+    to_update = {k: v for k, v in new_vars.items() if v is not None}
+    to_remove = [k for k, v in new_vars.items() if v is None]
+
+    stomped = (set(to_update.keys()) | set(to_remove)) & set(environ.keys())
+    update_after = {k: environ[k] for k in stomped}
+    remove_after = frozenset(k for k in to_update if k not in environ)
+
+    try:
+        environ.update(to_update)
+        [environ.pop(k, None) for k in to_remove]
+        yield
+    finally:
+        environ.update(update_after)
+        [environ.pop(k) for k in remove_after]
```

### Comparing `safe_init-1.0.2/PKG-INFO` & `safe_init-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-init
-Version: 1.0.2
+Version: 1.1.0
 Summary: Safe Init is a Python library that enhances AWS Lambda functions with advanced error handling, logging, monitoring, and resilience features, providing comprehensive observability and reliability for serverless applications.
 Home-page: https://github.com/kalepa/safe-init
 License: MIT
 Author: Maciej Wilczyński
 Author-email: maciej@lupine.software
 Requires-Python: >=3.11,<3.12
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,14 +20,15 @@
 Classifier: Topic :: System :: Monitoring
 Classifier: Typing :: Typed
 Requires-Dist: awslambdaric (>=2.0.10)
 Requires-Dist: boto3 (>=1.20.0)
 Requires-Dist: boto3-type-annotations (>=0.3.1)
 Requires-Dist: datadog-lambda
 Requires-Dist: ddtrace
+Requires-Dist: redis (>=4.0.0,<6)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: sentry-sdk (<2.0.0)
 Requires-Dist: structlog (>=24.1.0,<25.0.0)
 Project-URL: Documentation, https://safe-init.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/kalepa/safe-init
 Description-Content-Type: text/markdown
 
@@ -61,14 +62,15 @@
 - **Slack Notifications**: Sends informative Slack notifications with error details, keeping your team informed about any issues in real-time.
 - **Datadog Integration**: Integrates seamlessly with the Datadog Lambda wrapper for enhanced monitoring and metrics collection.
 
 ### Resilience and Reliability
 - **Dead-Letter Queue (DLQ) Support**: Pushes failed events to a dead-letter queue for later processing, ensuring that no events are lost due to errors.
 - **Initialization Checks**: Detects missing Sentry initialization and Lambda init phase timeouts, preventing silent failures and providing early warning signs.
 - **Timeout Notifications**: Sends notifications a configurable number of seconds before the Lambda timeout occurs, giving you a heads-up to investigate and address potential issues.
+- **AWS Secrets Resolution**: Automatically resolves AWS Secrets Manager secrets in environment variables, simplifying secret management and access.
 
 ### Customization and Flexibility
 - **Customizable Logger**: Allows you to use a custom logger instead of the default structlog logger, providing flexibility to integrate with your existing logging setup.
 - **Easy to Use**: Simply set the Lambda handler to `safe_init.handler.handler` and configure the `SAFE_INIT_HANDLER` environment variable to point to your original code handler. No further changes or decorators needed!
 
 ## Installation
 
@@ -111,14 +113,21 @@
 - `SAFE_INIT_NOTIFY_SEC_BEFORE_TIMEOUT` (optional): The number of seconds before the Lambda timeout to send a notification. Defaults to 5 seconds for timeouts < 120s, and 10 seconds for timeouts >= 120s. It's like a friendly tap on the shoulder, reminding you to check on your Lambda before it times out.
 - `SAFE_INIT_TRACER_HOME_PATHS` (optional): A comma-separated list of paths to mark as "home" in function call tracing. Paths containing these strings will be marked with a ⚡ emoji in Slack notifications. Because home is where the heart is, and the ⚡ emoji is just cool!
 - `SAFE_INIT_IGNORE_TIMEOUTS` (optional): Set to `'true'` to disable timeout notifications. For those times when you just don't want to be bothered about timeouts.
 - `SAFE_INIT_NO_SLACK_TIMEOUT_NOTIFICATIONS` (optional): Set to `'true'` to disable Slack notifications for timeouts. Sometimes, you just need a break from all the notifications.
 - `SAFE_INIT_NO_DATADOG_WRAPPER` (optional): Set to `'true'` to disable Datadog integration. If you're not using Datadog, this is the option for you!
 - `SAFE_INIT_AUTO_TRACE_LAMBDAS` (optional): Set to `'true'` to automatically trace all function calls in Lambda handlers. **Warning:** this can significantly increase memory usage and execution time. Use with caution!
 - `SAFE_INIT_LOGGING_USE_CONSOLE_RENDERER` (optional): Set to `'true'` to use the console renderer for logs. For those times when you want your logs to look extra fancy in the console.
+- `SAFE_INIT_RESOLVE_SECRETS` (optional): Set to `true` to resolve AWS Secrets Manager secrets in environment variables. Safe Init will automatically resolve secrets in environment variables with names ending with a configured suffix and save them in environment variables with the original name minus the suffix.
+- `SAFE_INIT_SECRET_ARN_SUFFIX` (optional): The suffix to use for resolving AWS Secrets Manager secrets in environment variables. Defaults to `_SECRET_ARN`. Use this to specify the suffix that marks environment variables as containing secret ARNs.
+- `SAFE_INIT_CACHE_SECRETS` (optional): Set to `true` to cache resolved secrets in Redis. Safe Init will cache resolved secrets in Redis to reduce the number of calls to AWS Secrets Manager.
+- `SAFE_INIT_SECRET_CACHE_REDIS_HOST`, `SAFE_INIT_SECRET_CACHE_REDIS_PORT`, `SAFE_INIT_SECRET_CACHE_REDIS_DB`, `SAFE_INIT_SECRET_CACHE_REDIS_USERNAME`, `SAFE_INIT_SECRET_CACHE_REDIS_PASSWORD` (host&port required if secret caching enabled): Redis connection details for caching resolved secrets. Use these environment variables to specify the Redis host, port, database, and password for caching resolved secrets.
+- `SAFE_INIT_SECRET_CACHE_TTL` (optional): TTL for cached secrets in seconds. Defaults to 1800 seconds (30 minutes). Use this to specify how long resolved secrets should be cached in Redis.
+- `SAFE_INIT_SECRET_CACHE_PREFIX` (optional): Prefix for cached secrets in Redis. Defaults to `safe-init-secret::`. Use this to specify the prefix for keys used to store cached secrets in Redis.
+- `SAFE_INIT_FAIL_ON_SECRET_RESOLUTION_ERROR` (optional): Set to `true` to fail the Lambda initialization if an error occurs during secret resolution. Safe Init will raise an exception if an error occurs during secret resolution, preventing the Lambda function from starting.
 
 With these configuration options, Safe Init provides a flexible and customizable way to enhance your Lambda functions' error handling, logging, and monitoring capabilities. Mix and match the options to suit your needs, and let Safe Init be your loyal companion on your Lambda adventures! 🚀
 
 ## Advanced Usage
 
 ### Custom Logger
```

