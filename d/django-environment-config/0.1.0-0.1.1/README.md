# Comparing `tmp/django_environment_config-0.1.0.tar.gz` & `tmp/django_environment_config-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_environment_config-0.1.0.tar", max compression
+gzip compressed data, was "django_environment_config-0.1.1.tar", max compression
```

## Comparing `django_environment_config-0.1.0.tar` & `django_environment_config-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2889 2024-05-01 15:47:36.879834 django_environment_config-0.1.0/LICENSE
--rw-r--r--   0        0        0     3152 2024-05-01 15:47:36.879834 django_environment_config-0.1.0/README.md
--rw-r--r--   0        0        0       64 2024-05-01 15:47:36.879834 django_environment_config-0.1.0/env_config/__init__.py
--rw-r--r--   0        0        0     4558 2024-05-01 15:47:36.879834 django_environment_config-0.1.0/env_config/base.py
--rw-r--r--   0        0        0      364 2024-05-01 15:47:36.879834 django_environment_config-0.1.0/env_config/constants.py
--rw-r--r--   0        0        0     1058 2024-05-01 15:47:36.879834 django_environment_config-0.1.0/env_config/errors.py
--rw-r--r--   0        0        0        0 2024-05-01 15:47:36.879834 django_environment_config-0.1.0/env_config/py.typed
--rw-r--r--   0        0        0     1210 2024-05-01 15:47:36.879834 django_environment_config-0.1.0/env_config/typing.py
--rw-r--r--   0        0        0    12049 2024-05-01 15:47:36.879834 django_environment_config-0.1.0/env_config/values.py
--rw-r--r--   0        0        0        0 2024-05-01 15:47:36.879834 django_environment_config-0.1.0/env_config_pytest_plugin/__init__.py
--rw-r--r--   0        0        0      792 2024-05-01 15:47:36.879834 django_environment_config-0.1.0/env_config_pytest_plugin/hooks.py
--rw-r--r--   0        0        0     8728 2024-05-01 15:47:36.879834 django_environment_config-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4644 1970-01-01 00:00:00.000000 django_environment_config-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2889 2024-05-07 06:54:48.025603 django_environment_config-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3152 2024-05-07 06:54:48.025603 django_environment_config-0.1.1/README.md
+-rw-r--r--   0        0        0       64 2024-05-07 06:54:48.025603 django_environment_config-0.1.1/env_config/__init__.py
+-rw-r--r--   0        0        0     4558 2024-05-07 06:54:48.025603 django_environment_config-0.1.1/env_config/base.py
+-rw-r--r--   0        0        0      364 2024-05-07 06:54:48.025603 django_environment_config-0.1.1/env_config/constants.py
+-rw-r--r--   0        0        0     1058 2024-05-07 06:54:48.029603 django_environment_config-0.1.1/env_config/errors.py
+-rw-r--r--   0        0        0        0 2024-05-07 06:54:48.029603 django_environment_config-0.1.1/env_config/py.typed
+-rw-r--r--   0        0        0     1210 2024-05-07 06:54:48.029603 django_environment_config-0.1.1/env_config/typing.py
+-rw-r--r--   0        0        0    13191 2024-05-07 06:54:48.029603 django_environment_config-0.1.1/env_config/values.py
+-rw-r--r--   0        0        0        0 2024-05-07 06:54:48.029603 django_environment_config-0.1.1/env_config_pytest_plugin/__init__.py
+-rw-r--r--   0        0        0      792 2024-05-07 06:54:48.029603 django_environment_config-0.1.1/env_config_pytest_plugin/hooks.py
+-rw-r--r--   0        0        0     8728 2024-05-07 06:54:48.029603 django_environment_config-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4644 1970-01-01 00:00:00.000000 django_environment_config-0.1.1/PKG-INFO
```

### Comparing `django_environment_config-0.1.0/LICENSE` & `django_environment_config-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.1.0/README.md` & `django_environment_config-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.1.0/env_config/base.py` & `django_environment_config-0.1.1/env_config/base.py`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.1.0/env_config/errors.py` & `django_environment_config-0.1.1/env_config/errors.py`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.1.0/env_config/typing.py` & `django_environment_config-0.1.1/env_config/typing.py`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.1.0/env_config/values.py` & `django_environment_config-0.1.1/env_config/values.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,15 +162,15 @@
 
 class SequenceValue(Value, ABC, Generic[T]):
     def __init__(
         self,
         child: Value[T] | None = None,
         *,
         default: Sequence[T] | None = Undefined,
-        env_name: str | Undefined = Undefined,
+        env_name: str | None | Undefined = Undefined,
         delimiter: str = ",",
     ) -> None:
         self.child = child or StringValue()
         self.delimiter = delimiter
         super().__init__(default=default, env_name=env_name)
 
     def iterate(self, value: str | Sequence[Any]) -> Generator[T, None, None]:
@@ -205,15 +205,15 @@
 
 class MappingValue(Value, ABC, Generic[T]):
     def __init__(  # noqa: PLR0913
         self,
         child: Value[T] | None = None,
         *,
         default: Mapping[str, T] | None = Undefined,
-        env_name: str | Undefined = Undefined,
+        env_name: str | None | Undefined = Undefined,
         kv_delimiter: str = "=",
         item_delimiter: str = ";",
     ) -> None:
         self.child = child or StringValue()
         self.kv_delimiter = kv_delimiter
         self.item_delimiter = item_delimiter
         super().__init__(default=default, env_name=env_name)
@@ -286,41 +286,47 @@
     """Parses env variables into a string value, and validates that it matches the given regex."""
 
     def __init__(
         self,
         *,
         regex: str,
         default: str | None = Undefined,
-        env_name: str | Undefined = Undefined,
+        env_name: str | None | Undefined = Undefined,
     ) -> None:
         self.regex = regex
         super().__init__(default=default, env_name=env_name)
 
     def convert(self, value: str) -> str:
         from django.core.validators import RegexValidator
 
         RegexValidator(regex=self.regex)(value)
         return value
 
 
 class PathValue(StringValue):
     """Parses env variable into a string value, and can optionally validate that the path exists."""
 
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         *,
         default: str | None = Undefined,
-        env_name: str | Undefined = Undefined,
+        env_name: str | None | Undefined = Undefined,
         check_exists: bool = True,
+        create_if_missing: bool = False,
+        mode: int = 0o777,
     ) -> None:
         self.check_exists = check_exists
+        self.create_if_missing = create_if_missing
+        self.mode = mode
         super().__init__(default=default, env_name=env_name)
 
     def convert(self, value: str) -> str:
         path = Path(value).absolute()
+        if self.create_if_missing:
+            path.mkdir(mode=self.mode, parents=True, exist_ok=True)
         if self.check_exists and not path.exists():
             msg = f"Path '{path}' does not exist"
             raise ValueError(msg)
 
         return str(path)
 
 
@@ -382,7 +388,32 @@
                 "(e.g., `pip install django-environment-config[cache]`) "
                 "to use the CacheURLValue."
             )
             raise MissingExtraDependencyError(msg) from error
 
         config = parse(value)
         return {self.cache_alias: config}
+
+
+class ParentValue(Value[T]):
+    """Parses value from the parent environment, or the default value if parent doesn't have the value."""
+
+    def __init__(
+        self,
+        child: Value[T] | None = None,
+        *,
+        default: T | None,
+        env_name: str | None | Undefined = Undefined,
+    ) -> None:
+        self.child = child or StringValue()
+        self.env: type[Environment] | None = None
+        super().__init__(default=default, env_name=env_name)
+
+    def get_for_environment(self, env: type[Environment]) -> None:
+        for parent in env.mro()[1:]:
+            value: Any = getattr(parent, self.name, Undefined)
+            if value is not Undefined:
+                return self.convert(value)
+        return self.convert(self.default)
+
+    def convert(self, value: str | T) -> T:
+        return self.child.convert(value)
```

### Comparing `django_environment_config-0.1.0/env_config_pytest_plugin/hooks.py` & `django_environment_config-0.1.1/env_config_pytest_plugin/hooks.py`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.1.0/pyproject.toml` & `django_environment_config-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-environment-config"
-version = "0.1.0"
+version = "0.1.1"
 description = "Configure django settings for multiple environments."
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "env_config" },
     { include = "env_config_pytest_plugin" },
@@ -52,28 +52,28 @@
 python-dotenv = ">=1.0.1"
 typing-extensions = { version = ">=4.11.0", python = "<3.12" }
 dj-database-url = { version = "^2.1.0", optional = true }
 django-cache-url = { version = "^3.4.5", optional = true }
 
 [tool.poetry.group.test.dependencies]
 pytest = "8.2.0"
-coverage = "7.5.0"
+coverage = "7.5.1"
 pytest-django = "4.8.0"
 pre-commit = "3.7.0"
 tox = "4.15.0"
 tox-gh-actions = "3.2.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.6.0"
 pymdown-extensions = "10.8.1"
 mkdocs-mermaid2-plugin = "1.1.1"
 
 [tool.poetry.group.lint.dependencies]
 mypy = "1.10.0"
-django-stubs = "4.2.7"
+django-stubs = "5.0.0"
 
 [tool.poetry.extras]
 db = ["dj-database-url"]
 cache = ["django-cache-url"]
 
 [tool.poetry.plugins.pytest11]
 django_environment_config = "env_config_pytest_plugin.hooks"
```

### Comparing `django_environment_config-0.1.0/PKG-INFO` & `django_environment_config-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-environment-config
-Version: 0.1.0
+Version: 0.1.1
 Summary: Configure django settings for multiple environments.
 Home-page: https://mrthearman.github.io/django-environment-config
 License: MIT
 Keywords: django,configuration,settings,environment,env,config
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.10,<4
```

