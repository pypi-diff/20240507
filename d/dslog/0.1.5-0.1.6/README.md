# Comparing `tmp/dslog-0.1.5.tar.gz` & `tmp/dslog-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dslog-0.1.5.tar", last modified: Sat May  4 07:20:56 2024, max compression
+gzip compressed data, was "dslog-0.1.6.tar", last modified: Tue May  7 08:02:55 2024, max compression
```

## Comparing `dslog-0.1.5.tar` & `dslog-0.1.6.tar`

### file list

```diff
@@ -1,28 +1,34 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 07:20:56.424342 dslog-0.1.5/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1096 2024-05-04 07:20:56.424342 dslog-0.1.5/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      716 2024-05-04 07:20:53.000000 dslog-0.1.5/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      514 2024-05-04 07:20:53.000000 dslog-0.1.5/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-04 07:20:56.424342 dslog-0.1.5/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 07:20:56.404342 dslog-0.1.5/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 07:20:56.404342 dslog-0.1.5/src/dslog/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      476 2024-05-04 07:20:39.000000 dslog-0.1.5/src/dslog/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 07:20:56.414342 dslog-0.1.5/src/dslog/formatters/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-02 07:46:22.000000 dslog-0.1.5/src/dslog/formatters/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      108 2024-05-02 07:46:22.000000 dslog-0.1.5/src/dslog/formatters/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      437 2024-05-02 07:46:22.000000 dslog-0.1.5/src/dslog/formatters/formatters.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2081 2024-05-02 07:51:07.000000 dslog-0.1.5/src/dslog/logger.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 07:20:56.414342 dslog-0.1.5/src/dslog/loggers/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-02 07:46:22.000000 dslog-0.1.5/src/dslog/loggers/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       75 2024-05-02 07:46:22.000000 dslog-0.1.5/src/dslog/loggers/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      502 2024-05-02 07:46:22.000000 dslog-0.1.5/src/dslog/loggers/_file.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       99 2024-05-02 07:46:22.000000 dslog-0.1.5/src/dslog/loggers/_rich.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      641 2024-05-04 07:20:24.000000 dslog-0.1.5/src/dslog/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 07:20:56.424342 dslog-0.1.5/src/dslog/util/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-02 07:46:22.000000 dslog-0.1.5/src/dslog/util/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1018 2024-05-02 07:46:22.000000 dslog-0.1.5/src/dslog/util/uvicorn.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 07:20:56.424342 dslog-0.1.5/src/dslog.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1096 2024-05-04 07:20:56.000000 dslog-0.1.5/src/dslog.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      519 2024-05-04 07:20:56.000000 dslog-0.1.5/src/dslog.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-04 07:20:56.000000 dslog-0.1.5/src/dslog.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       25 2024-05-04 07:20:56.000000 dslog-0.1.5/src/dslog.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        6 2024-05-04 07:20:56.000000 dslog-0.1.5/src/dslog.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 08:02:55.683247 dslog-0.1.6/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2049 2024-05-07 08:02:55.683247 dslog-0.1.6/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1541 2024-05-07 08:02:53.000000 dslog-0.1.6/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      554 2024-05-07 08:02:53.000000 dslog-0.1.6/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 08:02:55.683247 dslog-0.1.6/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 08:02:55.673247 dslog-0.1.6/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 08:02:55.673247 dslog-0.1.6/src/dslog/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      505 2024-05-07 07:13:39.000000 dslog-0.1.6/src/dslog/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      193 2024-05-07 07:36:40.000000 dslog-0.1.6/src/dslog/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 08:02:55.673247 dslog-0.1.6/src/dslog/formatters/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-02 07:46:22.000000 dslog-0.1.6/src/dslog/formatters/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       84 2024-05-07 07:50:28.000000 dslog-0.1.6/src/dslog/formatters/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      685 2024-05-07 07:50:21.000000 dslog-0.1.6/src/dslog/formatters/formatters.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2386 2024-05-07 07:51:43.000000 dslog-0.1.6/src/dslog/logger.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 08:02:55.683247 dslog-0.1.6/src/dslog/loggers/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-02 07:46:22.000000 dslog-0.1.6/src/dslog/loggers/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       75 2024-05-02 07:46:22.000000 dslog-0.1.6/src/dslog/loggers/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      477 2024-05-07 06:47:46.000000 dslog-0.1.6/src/dslog/loggers/_file.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      241 2024-05-07 07:43:26.000000 dslog-0.1.6/src/dslog/loggers/_rich.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      585 2024-05-07 07:46:06.000000 dslog-0.1.6/src/dslog/stdlib.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      827 2024-05-07 06:54:14.000000 dslog-0.1.6/src/dslog/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 08:02:55.683247 dslog-0.1.6/src/dslog/uvicorn/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-07 07:39:35.000000 dslog-0.1.6/src/dslog/uvicorn/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      350 2024-05-07 07:41:23.000000 dslog-0.1.6/src/dslog/uvicorn/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1018 2024-05-02 07:46:22.000000 dslog-0.1.6/src/dslog/uvicorn/config.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      200 2024-05-07 07:41:10.000000 dslog-0.1.6/src/dslog/uvicorn/format.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1858 2024-05-07 07:57:45.000000 dslog-0.1.6/src/dslog/uvicorn/setup.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      539 2024-05-07 07:23:03.000000 dslog-0.1.6/src/dslog/uvicorn/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 08:02:55.683247 dslog-0.1.6/src/dslog.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2049 2024-05-07 08:02:55.000000 dslog-0.1.6/src/dslog.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      680 2024-05-07 08:02:55.000000 dslog-0.1.6/src/dslog.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 08:02:55.000000 dslog-0.1.6/src/dslog.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       59 2024-05-07 08:02:55.000000 dslog-0.1.6/src/dslog.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        6 2024-05-07 08:02:55.000000 dslog-0.1.6/src/dslog.egg-info/top_level.txt
```

### Comparing `dslog-0.1.5/pyproject.toml` & `dslog-0.1.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dslog"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Dead-simple logging: what python's logging should've been"
 dependencies = [
   "lazy-loader"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 repo = "https://github.com/marciclabas/dslog.git"
 
 [project.optional-dependencies]
+uvicorn = ["uvicorn"]
 rich = ["rich"]
+click = ["click"]
```

### Comparing `dslog-0.1.5/src/dslog/logger.py` & `dslog-0.1.6/src/dslog/logger.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,59 @@
-from email.policy import default
-from typing import Literal, Protocol
+from typing import Literal, Protocol, Generic, TypeVarTuple
 from dataclasses import dataclass
 from abc import ABC, abstractmethod
 from .types import Level, Handler, Formatter, value
 from . import loggers, formatters
 
-class LogFn(Protocol):
-  def __call__(self, *objs, level: Level = 'INFO'):
+Objs = TypeVarTuple('Objs')
+
+class LogFn(Protocol, Generic[*Objs]):
+  def __call__(self, *objs: *Objs, level: Level = 'INFO'):
     ...
 
-class Logger(ABC, LogFn):
+class Logger(ABC, LogFn[*Objs], Generic[*Objs]):
   @abstractmethod
-  def __call__(self, *objs, level: Level = 'INFO'):
+  def __call__(self, *objs: *Objs, level: Level = 'INFO'):
     ...
 
   @classmethod
   def of(cls, handler: Handler) -> 'Logger':
     return LoggerOf(handler)
 
   @classmethod
-  def rich(cls) -> 'Logger':
+  def click(cls) -> 'Logger[*Objs]':
+    """`print` logger formatted with `click`"""
+    return Logger.of(print).format(formatters.click) 
+
+  @classmethod
+  def rich(cls) -> 'Logger[*Objs]':
     """Nicely formatted rich logger (use `loggers.rich` aka `Logger.of(rich.print)` for a non-formatted version)"""
-    return loggers.rich().format(formatters.rich_formatter)
+    return loggers.rich().format(formatters.rich) 
   
   @classmethod
-  def file(cls, filepath: str, *, mode: Literal['w', 'a'] = 'a') -> 'Logger':
+  def file(cls, filepath: str, *, mode: Literal['w', 'a'] = 'a') -> 'Logger[*Objs]':
     """Default formatted file logger (use `loggers.file` for a non-formatted version)"""
-    return loggers.file(filepath, mode=mode).format(formatters.default_formatter)
+    return loggers.file(filepath, mode=mode).format(formatters.default)
   
   @classmethod
-  def empty(cls) -> 'Logger':
-    """A logger that doesn't do anything"""
+  def empty(cls) -> 'Logger[*Objs]':
+    """*Objs logger that doesn't do anything"""
     return LoggerOf(lambda *_, **_kw: None)
 
   def limit(self, min_level: Level) -> 'Logger':
     return Limited(min_level, self)
   
-  def format(self, format: Formatter) -> 'Logger':
+  def format(self, format: Formatter[*Objs]) -> 'Logger[*Objs]':
     return Formatted(format, self)
   
-  def prefix(self, prefix: str) -> 'Logger':
-    return self.format(lambda *objs, **_: (prefix, *objs))
+  def prefix(self, prefix: str) -> 'Logger[*Objs]':
+    return self.format(lambda *objs, **_: (prefix, *objs)) # type: ignore
   
-  def postfix(self, postfix: str) -> 'Logger':
-    return self.format(lambda *objs, **_: (*objs, postfix))
+  def postfix(self, postfix: str) -> 'Logger[*Objs]':
+    return self.format(lambda *objs, **_: (*objs, postfix)) # type: ignore
   
 @dataclass
 class LoggerOf(Logger):
   handler: Handler
   def __call__(self, *objs, **_):
     self.handler(*objs)
 
@@ -57,14 +63,14 @@
   logger: Logger
 
   def __call__(self, *objs, level: Level = 'INFO'):
     if value(level) >= value(self.min_level):
       self.logger(*objs, level=level)
 
 @dataclass
-class Formatted(Logger):
-  formatter: Formatter
+class Formatted(Logger[*Objs]):
+  formatter: Formatter[*Objs]
   logger: Logger
 
   def __call__(self, *objs, level: Level = 'INFO'):
     formatted_objs = self.formatter(*objs, level=level)
     self.logger(*formatted_objs, level=level)
```

### Comparing `dslog-0.1.5/src/dslog/util/uvicorn.py` & `dslog-0.1.6/src/dslog/uvicorn/config.py`

 * *Files identical despite different names*

### Comparing `dslog-0.1.5/src/dslog.egg-info/SOURCES.txt` & `dslog-0.1.6/src/dslog.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 README.md
 pyproject.toml
 src/dslog/__init__.py
+src/dslog/__init__.pyi
 src/dslog/logger.py
+src/dslog/stdlib.py
 src/dslog/types.py
 src/dslog.egg-info/PKG-INFO
 src/dslog.egg-info/SOURCES.txt
 src/dslog.egg-info/dependency_links.txt
 src/dslog.egg-info/requires.txt
 src/dslog.egg-info/top_level.txt
 src/dslog/formatters/__init__.py
 src/dslog/formatters/__init__.pyi
 src/dslog/formatters/formatters.py
 src/dslog/loggers/__init__.py
 src/dslog/loggers/__init__.pyi
 src/dslog/loggers/_file.py
 src/dslog/loggers/_rich.py
-src/dslog/util/__init__.py
-src/dslog/util/uvicorn.py
+src/dslog/uvicorn/__init__.py
+src/dslog/uvicorn/__init__.pyi
+src/dslog/uvicorn/config.py
+src/dslog/uvicorn/format.py
+src/dslog/uvicorn/setup.py
+src/dslog/uvicorn/types.py
```

