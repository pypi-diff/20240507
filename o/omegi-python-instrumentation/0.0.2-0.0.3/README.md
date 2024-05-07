# Comparing `tmp/omegi_python_instrumentation-0.0.2.tar.gz` & `tmp/omegi_python_instrumentation-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omegi_python_instrumentation-0.0.2.tar", last modified: Tue May  7 06:56:05 2024, max compression
+gzip compressed data, was "omegi_python_instrumentation-0.0.3.tar", last modified: Tue May  7 07:04:22 2024, max compression
```

## Comparing `omegi_python_instrumentation-0.0.2.tar` & `omegi_python_instrumentation-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-07 06:56:05.248985 omegi_python_instrumentation-0.0.2/
--rw-r--r--   0 whisenlantern   (501) staff       (20)       13 2024-05-07 06:22:05.000000 omegi_python_instrumentation-0.0.2/LICENSE.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2065 2024-05-07 06:56:05.248780 omegi_python_instrumentation-0.0.2/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)       44 2024-05-07 06:21:19.000000 omegi_python_instrumentation-0.0.2/README.md
--rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi_python_instrumentation-0.0.2/pyproject.toml
--rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-07 06:56:05.249025 omegi_python_instrumentation-0.0.2/setup.cfg
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2167 2024-05-07 06:52:51.000000 omegi_python_instrumentation-0.0.2/setup.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-07 06:56:05.246456 omegi_python_instrumentation-0.0.2/src/
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-07 06:56:05.247656 omegi_python_instrumentation-0.0.2/src/omegi/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2809 2024-05-06 19:38:23.000000 omegi_python_instrumentation-0.0.2/src/omegi/KafkaSpanExporter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1350 2024-05-07 06:42:58.000000 omegi_python_instrumentation-0.0.2/src/omegi/OmegHandler.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2722 2024-05-07 06:42:58.000000 omegi_python_instrumentation-0.0.2/src/omegi/OmegiTracer.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-07 06:14:19.000000 omegi_python_instrumentation-0.0.2/src/omegi/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-07 06:56:05.248455 omegi_python_instrumentation-0.0.2/src/omegi_python_instrumentation.egg-info/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2065 2024-05-07 06:56:05.000000 omegi_python_instrumentation-0.0.2/src/omegi_python_instrumentation.egg-info/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)      427 2024-05-07 06:56:05.000000 omegi_python_instrumentation-0.0.2/src/omegi_python_instrumentation.egg-info/SOURCES.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-07 06:56:05.000000 omegi_python_instrumentation-0.0.2/src/omegi_python_instrumentation.egg-info/dependency_links.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-07 06:56:05.000000 omegi_python_instrumentation-0.0.2/src/omegi_python_instrumentation.egg-info/requires.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-07 06:56:05.000000 omegi_python_instrumentation-0.0.2/src/omegi_python_instrumentation.egg-info/top_level.txt
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-07 07:04:22.569175 omegi_python_instrumentation-0.0.3/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       13 2024-05-07 06:22:05.000000 omegi_python_instrumentation-0.0.3/LICENSE.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2065 2024-05-07 07:04:22.568985 omegi_python_instrumentation-0.0.3/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       44 2024-05-07 06:21:19.000000 omegi_python_instrumentation-0.0.3/README.md
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi_python_instrumentation-0.0.3/pyproject.toml
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-07 07:04:22.569216 omegi_python_instrumentation-0.0.3/setup.cfg
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2167 2024-05-07 07:04:03.000000 omegi_python_instrumentation-0.0.3/setup.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-07 07:04:22.566137 omegi_python_instrumentation-0.0.3/src/
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-07 07:04:22.567793 omegi_python_instrumentation-0.0.3/src/omegi/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2809 2024-05-06 19:38:23.000000 omegi_python_instrumentation-0.0.3/src/omegi/KafkaSpanExporter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1354 2024-05-07 07:03:48.000000 omegi_python_instrumentation-0.0.3/src/omegi/OmegHandler.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2726 2024-05-07 07:03:48.000000 omegi_python_instrumentation-0.0.3/src/omegi/OmegiTracer.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-07 06:14:19.000000 omegi_python_instrumentation-0.0.3/src/omegi/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-07 07:04:22.568683 omegi_python_instrumentation-0.0.3/src/omegi_python_instrumentation.egg-info/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2065 2024-05-07 07:04:22.000000 omegi_python_instrumentation-0.0.3/src/omegi_python_instrumentation.egg-info/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      427 2024-05-07 07:04:22.000000 omegi_python_instrumentation-0.0.3/src/omegi_python_instrumentation.egg-info/SOURCES.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-07 07:04:22.000000 omegi_python_instrumentation-0.0.3/src/omegi_python_instrumentation.egg-info/dependency_links.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-07 07:04:22.000000 omegi_python_instrumentation-0.0.3/src/omegi_python_instrumentation.egg-info/requires.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-07 07:04:22.000000 omegi_python_instrumentation-0.0.3/src/omegi_python_instrumentation.egg-info/top_level.txt
```

### Comparing `omegi_python_instrumentation-0.0.2/PKG-INFO` & `omegi_python_instrumentation-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegi-python-instrumentation
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python Instrumentation for Automatic Error Logging
 Home-page: https://github.com/TeamOmegi/Instrumentation-Python
 Author: Omegi
 Author-email: canon1107@naver.com
 Project-URL: Source Code, https://github.com/TeamOmegi/Instrumentation-Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `omegi_python_instrumentation-0.0.2/setup.py` & `omegi_python_instrumentation-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="omegi-python-instrumentation",
-    version="0.0.2",
+    version="0.0.3",
     author="Omegi",
     author_email="canon1107@naver.com",
     description="Python Instrumentation for Automatic Error Logging",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TeamOmegi/Instrumentation-Python",
     project_urls={
```

### Comparing `omegi_python_instrumentation-0.0.2/src/omegi/KafkaSpanExporter.py` & `omegi_python_instrumentation-0.0.3/src/omegi/KafkaSpanExporter.py`

 * *Files identical despite different names*

### Comparing `omegi_python_instrumentation-0.0.2/src/omegi/OmegHandler.py` & `omegi_python_instrumentation-0.0.3/src/omegi/OmegHandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import traceback
 
 from fastapi import Request
 from opentelemetry import trace
 
-from omegi.OmegiTracer import OmegiTracer
+from src.omegi.OmegiTracer import OmegiTracer
 
 
 def fastapi_handler(omegi_tracer: OmegiTracer):
     async def handler(request: Request, exc: Exception):
         return await __omegi_handler_fastapi__(request, exc, omegi_tracer)
     return handler
```

### Comparing `omegi_python_instrumentation-0.0.2/src/omegi/OmegiTracer.py` & `omegi_python_instrumentation-0.0.3/src/omegi/OmegiTracer.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 import threading
 
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 
-from omegi.KafkaSpanExporter import KafkaSpanExporter
+from src.omegi.KafkaSpanExporter import KafkaSpanExporter
 
 
 class OmegiTracer:
     def __init__(self, service_name, kafka_server, topic, token):
         self.tracer_provider = TracerProvider()
         self.kafka_exporter = KafkaSpanExporter(kafka_server, topic, token)
         self.tracer_provider.add_span_processor(BatchSpanProcessor(self.kafka_exporter))
```

### Comparing `omegi_python_instrumentation-0.0.2/src/omegi_python_instrumentation.egg-info/PKG-INFO` & `omegi_python_instrumentation-0.0.3/src/omegi_python_instrumentation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegi-python-instrumentation
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python Instrumentation for Automatic Error Logging
 Home-page: https://github.com/TeamOmegi/Instrumentation-Python
 Author: Omegi
 Author-email: canon1107@naver.com
 Project-URL: Source Code, https://github.com/TeamOmegi/Instrumentation-Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `omegi_python_instrumentation-0.0.2/src/omegi_python_instrumentation.egg-info/requires.txt` & `omegi_python_instrumentation-0.0.3/src/omegi_python_instrumentation.egg-info/requires.txt`

 * *Files identical despite different names*

