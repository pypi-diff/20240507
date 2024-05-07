# Comparing `tmp/django_environment_config-0.1.1.tar.gz` & `tmp/django_environment_config-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_environment_config-0.1.1.tar", max compression
+gzip compressed data, was "django_environment_config-0.1.2.tar", max compression
```

## Comparing `django_environment_config-0.1.1.tar` & `django_environment_config-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2889 2024-05-07 06:54:48.025603 django_environment_config-0.1.1/LICENSE
--rw-r--r--   0        0        0     3152 2024-05-07 06:54:48.025603 django_environment_config-0.1.1/README.md
--rw-r--r--   0        0        0       64 2024-05-07 06:54:48.025603 django_environment_config-0.1.1/env_config/__init__.py
--rw-r--r--   0        0        0     4558 2024-05-07 06:54:48.025603 django_environment_config-0.1.1/env_config/base.py
--rw-r--r--   0        0        0      364 2024-05-07 06:54:48.025603 django_environment_config-0.1.1/env_config/constants.py
--rw-r--r--   0        0        0     1058 2024-05-07 06:54:48.029603 django_environment_config-0.1.1/env_config/errors.py
--rw-r--r--   0        0        0        0 2024-05-07 06:54:48.029603 django_environment_config-0.1.1/env_config/py.typed
--rw-r--r--   0        0        0     1210 2024-05-07 06:54:48.029603 django_environment_config-0.1.1/env_config/typing.py
--rw-r--r--   0        0        0    13191 2024-05-07 06:54:48.029603 django_environment_config-0.1.1/env_config/values.py
--rw-r--r--   0        0        0        0 2024-05-07 06:54:48.029603 django_environment_config-0.1.1/env_config_pytest_plugin/__init__.py
--rw-r--r--   0        0        0      792 2024-05-07 06:54:48.029603 django_environment_config-0.1.1/env_config_pytest_plugin/hooks.py
--rw-r--r--   0        0        0     8728 2024-05-07 06:54:48.029603 django_environment_config-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4644 1970-01-01 00:00:00.000000 django_environment_config-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2889 2024-05-07 07:17:58.989233 django_environment_config-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3152 2024-05-07 07:17:58.989233 django_environment_config-0.1.2/README.md
+-rw-r--r--   0        0        0       64 2024-05-07 07:17:58.993233 django_environment_config-0.1.2/env_config/__init__.py
+-rw-r--r--   0        0        0     4558 2024-05-07 07:17:58.993233 django_environment_config-0.1.2/env_config/base.py
+-rw-r--r--   0        0        0      364 2024-05-07 07:17:58.993233 django_environment_config-0.1.2/env_config/constants.py
+-rw-r--r--   0        0        0     1058 2024-05-07 07:17:58.993233 django_environment_config-0.1.2/env_config/errors.py
+-rw-r--r--   0        0        0        0 2024-05-07 07:17:58.993233 django_environment_config-0.1.2/env_config/py.typed
+-rw-r--r--   0        0        0     1210 2024-05-07 07:17:58.993233 django_environment_config-0.1.2/env_config/typing.py
+-rw-r--r--   0        0        0    13294 2024-05-07 07:17:58.993233 django_environment_config-0.1.2/env_config/values.py
+-rw-r--r--   0        0        0        0 2024-05-07 07:17:58.993233 django_environment_config-0.1.2/env_config_pytest_plugin/__init__.py
+-rw-r--r--   0        0        0      792 2024-05-07 07:17:58.993233 django_environment_config-0.1.2/env_config_pytest_plugin/hooks.py
+-rw-r--r--   0        0        0     8728 2024-05-07 07:17:58.993233 django_environment_config-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4644 1970-01-01 00:00:00.000000 django_environment_config-0.1.2/PKG-INFO
```

### Comparing `django_environment_config-0.1.1/LICENSE` & `django_environment_config-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.1.1/README.md` & `django_environment_config-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.1.1/env_config/base.py` & `django_environment_config-0.1.2/env_config/base.py`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.1.1/env_config/errors.py` & `django_environment_config-0.1.2/env_config/errors.py`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.1.1/env_config/typing.py` & `django_environment_config-0.1.2/env_config/typing.py`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.1.1/env_config/values.py` & `django_environment_config-0.1.2/env_config/values.py`

 * *Files 1% similar despite different names*

```diff
@@ -399,21 +399,23 @@
 
     def __init__(
         self,
         child: Value[T] | None = None,
         *,
         default: T | None,
         env_name: str | None | Undefined = Undefined,
+        check_limit: int | None = None,
     ) -> None:
         self.child = child or StringValue()
         self.env: type[Environment] | None = None
+        self.check_limit = check_limit
         super().__init__(default=default, env_name=env_name)
 
     def get_for_environment(self, env: type[Environment]) -> None:
-        for parent in env.mro()[1:]:
+        for parent in env.mro()[slice(1, self.check_limit)]:
             value: Any = getattr(parent, self.name, Undefined)
             if value is not Undefined:
                 return self.convert(value)
         return self.convert(self.default)
 
     def convert(self, value: str | T) -> T:
         return self.child.convert(value)
```

### Comparing `django_environment_config-0.1.1/env_config_pytest_plugin/hooks.py` & `django_environment_config-0.1.2/env_config_pytest_plugin/hooks.py`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.1.1/pyproject.toml` & `django_environment_config-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-environment-config"
-version = "0.1.1"
+version = "0.1.2"
 description = "Configure django settings for multiple environments."
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "env_config" },
     { include = "env_config_pytest_plugin" },
```

### Comparing `django_environment_config-0.1.1/PKG-INFO` & `django_environment_config-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-environment-config
-Version: 0.1.1
+Version: 0.1.2
 Summary: Configure django settings for multiple environments.
 Home-page: https://mrthearman.github.io/django-environment-config
 License: MIT
 Keywords: django,configuration,settings,environment,env,config
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.10,<4
```

