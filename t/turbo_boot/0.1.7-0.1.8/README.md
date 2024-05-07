# Comparing `tmp/turbo_boot-0.1.7.tar.gz` & `tmp/turbo_boot-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbo_boot-0.1.7.tar", max compression
+gzip compressed data, was "turbo_boot-0.1.8.tar", max compression
```

## Comparing `turbo_boot-0.1.7.tar` & `turbo_boot-0.1.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2024-03-15 09:20:57.704789 turbo_boot-0.1.7/README.md
--rw-r--r--   0        0        0      425 2024-05-07 06:25:46.764582 turbo_boot-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-18 03:35:51.274526 turbo_boot-0.1.7/turbo_boot/__init__.py
--rw-r--r--   0        0        0     1706 2024-05-07 06:23:11.945862 turbo_boot-0.1.7/turbo_boot/config_loader.py
--rw-r--r--   0        0        0     2853 2024-05-07 06:21:30.227121 turbo_boot-0.1.7/turbo_boot/http_methods.py
--rw-r--r--   0        0        0     3846 2024-05-07 06:23:07.051859 turbo_boot-0.1.7/turbo_boot/logging.py
--rw-r--r--   0        0        0      140 2024-05-07 06:21:41.486201 turbo_boot-0.1.7/turbo_boot/logging_level.py
--rw-r--r--   0        0        0     2236 2024-05-07 06:22:08.082211 turbo_boot-0.1.7/turbo_boot/rest_controller.py
--rw-r--r--   0        0        0      353 2024-05-07 06:22:16.285522 turbo_boot-0.1.7/turbo_boot/singleton_meta.py
--rw-r--r--   0        0        0     2788 2024-05-07 06:23:54.976754 turbo_boot-0.1.7/turbo_boot/turbo_boot.py
--rw-r--r--   0        0        0      511 1970-01-01 00:00:00.000000 turbo_boot-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-15 09:20:57.704789 turbo_boot-0.1.8/README.md
+-rw-r--r--   0        0        0      425 2024-05-07 06:45:46.861469 turbo_boot-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-18 03:35:51.274526 turbo_boot-0.1.8/turbo_boot/__init__.py
+-rw-r--r--   0        0        0     1669 2024-05-07 06:43:43.303120 turbo_boot-0.1.8/turbo_boot/config_loader.py
+-rw-r--r--   0        0        0     2853 2024-05-07 06:21:30.227121 turbo_boot-0.1.8/turbo_boot/http_methods.py
+-rw-r--r--   0        0        0     3802 2024-05-07 06:43:59.614955 turbo_boot-0.1.8/turbo_boot/logging.py
+-rw-r--r--   0        0        0      140 2024-05-07 06:21:41.486201 turbo_boot-0.1.8/turbo_boot/logging_level.py
+-rw-r--r--   0        0        0     2236 2024-05-07 06:22:08.082211 turbo_boot-0.1.8/turbo_boot/rest_controller.py
+-rw-r--r--   0        0        0      353 2024-05-07 06:22:16.285522 turbo_boot-0.1.8/turbo_boot/singleton_meta.py
+-rw-r--r--   0        0        0     2788 2024-05-07 06:23:54.976754 turbo_boot-0.1.8/turbo_boot/turbo_boot.py
+-rw-r--r--   0        0        0      511 1970-01-01 00:00:00.000000 turbo_boot-0.1.8/PKG-INFO
```

### Comparing `turbo_boot-0.1.7/turbo_boot/config_loader.py` & `turbo_boot-0.1.8/turbo_boot/config_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,10 +39,8 @@
 
     def __substitute_env_variables(self, value):
         if isinstance(value, str):
             parts = value.split(":$")
             if len(parts) == 2 and parts[1].startswith("{") and parts[1].endswith("}"):
                 env_var = parts[1][2:-1]
                 return os.environ.get(env_var, parts[0])
-        return value
-
-application_config = ConfigLoader()
+        return value
```

### Comparing `turbo_boot-0.1.7/turbo_boot/http_methods.py` & `turbo_boot-0.1.8/turbo_boot/http_methods.py`

 * *Files identical despite different names*

### Comparing `turbo_boot-0.1.7/turbo_boot/logging.py` & `turbo_boot-0.1.8/turbo_boot/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,9 +70,7 @@
         self.__logger.debug(log_msg)
     
     def error(self, log_msg):
         self.__logger.error(log_msg)
     
     def critical(self, log_msg):
         self.__logger.critical(log_msg)
-        
-logger = Logger(application_config)
```

### Comparing `turbo_boot-0.1.7/turbo_boot/rest_controller.py` & `turbo_boot-0.1.8/turbo_boot/rest_controller.py`

 * *Files identical despite different names*

### Comparing `turbo_boot-0.1.7/turbo_boot/turbo_boot.py` & `turbo_boot-0.1.8/turbo_boot/turbo_boot.py`

 * *Files identical despite different names*

