# Comparing `tmp/turbo_boot-0.1.6.tar.gz` & `tmp/turbo_boot-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbo_boot-0.1.6.tar", max compression
+gzip compressed data, was "turbo_boot-0.1.7.tar", max compression
```

## Comparing `turbo_boot-0.1.6.tar` & `turbo_boot-0.1.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2024-03-15 09:20:57.704789 turbo_boot-0.1.6/README.md
--rw-r--r--   0        0        0      425 2024-03-18 07:53:37.990378 turbo_boot-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-18 03:35:51.274526 turbo_boot-0.1.6/turbo_boot/__init__.py
--rw-r--r--   0        0        0     1282 2024-03-18 07:52:00.279590 turbo_boot-0.1.6/turbo_boot/config_loader.py
--rw-r--r--   0        0        0     3004 2024-03-17 07:31:27.602699 turbo_boot-0.1.6/turbo_boot/http_methods.py
--rw-r--r--   0        0        0     3413 2024-03-18 07:51:38.262471 turbo_boot-0.1.6/turbo_boot/logging.py
--rw-r--r--   0        0        0      138 2024-03-17 12:11:00.548805 turbo_boot-0.1.6/turbo_boot/logging_level.py
--rw-r--r--   0        0        0     2221 2024-03-17 09:48:12.675397 turbo_boot-0.1.6/turbo_boot/rest_controller.py
--rw-r--r--   0        0        0      351 2024-03-18 03:40:26.627582 turbo_boot-0.1.6/turbo_boot/singleton_meta.py
--rw-r--r--   0        0        0     3503 2024-03-18 07:52:59.369883 turbo_boot-0.1.6/turbo_boot/turbo_boot.py
--rw-r--r--   0        0        0      511 1970-01-01 00:00:00.000000 turbo_boot-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-15 09:20:57.704789 turbo_boot-0.1.7/README.md
+-rw-r--r--   0        0        0      425 2024-05-07 06:25:46.764582 turbo_boot-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-18 03:35:51.274526 turbo_boot-0.1.7/turbo_boot/__init__.py
+-rw-r--r--   0        0        0     1706 2024-05-07 06:23:11.945862 turbo_boot-0.1.7/turbo_boot/config_loader.py
+-rw-r--r--   0        0        0     2853 2024-05-07 06:21:30.227121 turbo_boot-0.1.7/turbo_boot/http_methods.py
+-rw-r--r--   0        0        0     3846 2024-05-07 06:23:07.051859 turbo_boot-0.1.7/turbo_boot/logging.py
+-rw-r--r--   0        0        0      140 2024-05-07 06:21:41.486201 turbo_boot-0.1.7/turbo_boot/logging_level.py
+-rw-r--r--   0        0        0     2236 2024-05-07 06:22:08.082211 turbo_boot-0.1.7/turbo_boot/rest_controller.py
+-rw-r--r--   0        0        0      353 2024-05-07 06:22:16.285522 turbo_boot-0.1.7/turbo_boot/singleton_meta.py
+-rw-r--r--   0        0        0     2788 2024-05-07 06:23:54.976754 turbo_boot-0.1.7/turbo_boot/turbo_boot.py
+-rw-r--r--   0        0        0      511 1970-01-01 00:00:00.000000 turbo_boot-0.1.7/PKG-INFO
```

### Comparing `turbo_boot-0.1.6/turbo_boot/http_methods.py` & `turbo_boot-0.1.7/turbo_boot/http_methods.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,114 +1,122 @@
 from functools import wraps
 
+
 def validate_path(path: str):
     if path is None or len(path.strip()) < 1:
         raise ValueError("Path cannot be None or empty")
 
     if path is not None:
-        if not path.startswith('/'):
+        if not path.startswith("/"):
             raise ValueError("Path must start with '/'")
 
+
 def GetMapping(path: str, **kwargs):
     validate_path(path=path)
-            
-    def decorator(func):        
+
+    def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
 
         wrapper.__metadata__ = {"method_name": "GET", "path": path, **kwargs}
         return wrapper
 
     return decorator
 
+
 def PostMapping(path: str, **kwargs):
     validate_path(path=path)
-            
-    def decorator(func):        
+
+    def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
 
         wrapper.__metadata__ = {"method_name": "POST", "path": path, **kwargs}
         return wrapper
 
     return decorator
 
+
 def PutMapping(path: str, **kwargs):
     validate_path(path=path)
-            
-    def decorator(func):        
+
+    def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
 
         wrapper.__metadata__ = {"method_name": "PUT", "path": path, **kwargs}
         return wrapper
 
     return decorator
 
 
 def DeleteMapping(path: str, **kwargs):
     validate_path(path=path)
-            
-    def decorator(func):        
+
+    def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
 
         wrapper.__metadata__ = {"method_name": "DELETE", "path": path, **kwargs}
         return wrapper
 
     return decorator
 
+
 def OptionsMapping(path: str, **kwargs):
     validate_path(path=path)
-            
-    def decorator(func):        
+
+    def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
 
         wrapper.__metadata__ = {"method_name": "OPTIONS", "path": path, **kwargs}
         return wrapper
 
     return decorator
 
+
 def HeadMapping(path: str, **kwargs):
     validate_path(path=path)
-            
-    def decorator(func):        
+
+    def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
 
         wrapper.__metadata__ = {"method_name": "HEAD", "path": path, **kwargs}
         return wrapper
 
     return decorator
 
+
 def PatchMapping(path: str, **kwargs):
     validate_path(path=path)
-            
-    def decorator(func):        
+
+    def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
 
         wrapper.__metadata__ = {"method_name": "PATCH", "path": path, **kwargs}
         return wrapper
 
     return decorator
 
+
 def TraceMapping(path: str, **kwargs):
     validate_path(path=path)
-            
-    def decorator(func):        
+
+    def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
 
         wrapper.__metadata__ = {"method_name": "TRACE", "path": path, **kwargs}
         return wrapper
 
-    return decorator
+    return decorator
```

### Comparing `turbo_boot-0.1.6/turbo_boot/logging.py` & `turbo_boot-0.1.7/turbo_boot/logging.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from turbo_boot.singleton_meta import SingletonMeta
-from turbo_boot.config_loader import ConfigLoader
+from turbo_boot.config_loader import application_config, ConfigLoader
 import logging
 from logging.handlers import RotatingFileHandler
 from turbo_boot.logging_level import LoggingLevel
 import sys
 import os
 
 def get_boolean(val: str) -> bool:
@@ -54,8 +54,25 @@
     def __setup_console_handler(self):
         if (get_boolean(self.__config_loader.get_config("turbo-boot.logging.console-handler.enabled")) or True):
             logger = self.__logger
             logger.stdout_handler = logging.StreamHandler(sys.stdout)
             
             logger.stdout_handler.setLevel(LoggingLevel[str(self.__config_loader.get_config("turbo-boot.logging.console-handler.level") or self.__global_log_level).upper()].value)
             logger.stdout_handler.setFormatter(logging.Formatter((self.__config_loader.get_config("turbo-boot.logging.console-handler.format") or self.__global_log_format)))
-            logger.addHandler(logger.stdout_handler)
+            logger.addHandler(logger.stdout_handler)
+
+    def info(self, log_msg):
+        self.__logger.info(log_msg)
+    
+    def warning(self, log_msg):
+        self.__logger.warning(log_msg)
+        
+    def debug(self, log_msg):
+        self.__logger.debug(log_msg)
+    
+    def error(self, log_msg):
+        self.__logger.error(log_msg)
+    
+    def critical(self, log_msg):
+        self.__logger.critical(log_msg)
+        
+logger = Logger(application_config)
```

### Comparing `turbo_boot-0.1.6/turbo_boot/rest_controller.py` & `turbo_boot-0.1.7/turbo_boot/rest_controller.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 import inspect
 from typing import Dict, Optional, Type
-from urllib.parse import urljoin
 
 from fastapi import APIRouter
 
-Any = object()
 
 class RestController:
-    def __init__(self, prefix: Optional[str] = None, dependencies: Optional[Dict[str, Any]] = None):
+    def __init__(self, prefix: Optional[str] = None, dependencies: Optional[Dict] = None):
         self.prefix = prefix
         if prefix is not None:
-            if prefix == '/':
+            if prefix == "/":
                 raise ValueError("Prefix cannot be '/'")
-            if not prefix.startswith('/'):
+            if not prefix.startswith("/"):
                 raise ValueError("Prefix must start with '/'")
         self.dependencies = dependencies
-        
+
     def __call__(self, cls: Type) -> Type:
         setattr(cls, "__rest_controller__", True)
-        
+
         router = APIRouter()
         setattr(cls, "__api_router__", router)
-        
+
         instance = cls(**(self.dependencies or {}))
-        
+
         for attr_name in dir(cls):
             attr_value = getattr(instance, attr_name)
             if callable(attr_value) and not attr_name.startswith("__"):
                 if hasattr(attr_value, "__metadata__"):
-                    arguments_to_remove = ['self', 'path', 'methods', 'endpoint']
+                    arguments_to_remove = ["self", "path", "methods", "endpoint"]
                     argument_list = list(inspect.signature(APIRouter.add_api_route).parameters.keys())
                     filtered_arguments = [arg for arg in argument_list if arg not in arguments_to_remove]
                     parameters = {}
                     parameters["methods"] = [attr_value.__metadata__.get("method_name")]
                     if self.prefix is not None:
-                        m_prefix = self.prefix.rstrip('/') 
-                        m_path = attr_value.__metadata__["path"].rstrip('/') 
-                        parameters["path"] = urljoin(m_prefix, m_path)
+                        m_prefix = self.prefix.rstrip("/")
+                        m_path = attr_value.__metadata__["path"].rstrip("/")
+                        m_path = m_path.lstrip("/")
+                        if len(m_path) > 0:
+                            parameters["path"] = m_prefix + "/" + m_path
+                        else:
+                            parameters["path"] = m_prefix
                     else:
                         parameters["path"] = attr_value.__metadata__["path"]
-                    
+
                     parameters["endpoint"] = attr_value
-                    
+
                     for argument in filtered_arguments:
                         if argument in attr_value.__metadata__:
                             parameters[argument] = attr_value.__metadata__[argument]
-                    
+
                     router.add_api_route(**parameters)
-                    
-        return cls
+
+        return cls
```

