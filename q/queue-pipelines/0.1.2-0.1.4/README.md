# Comparing `tmp/queue_pipelines-0.1.2.tar.gz` & `tmp/queue_pipelines-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "queue_pipelines-0.1.2.tar", last modified: Sat May  4 15:40:24 2024, max compression
+gzip compressed data, was "queue_pipelines-0.1.4.tar", last modified: Tue May  7 13:59:12 2024, max compression
```

## Comparing `queue_pipelines-0.1.2.tar` & `queue_pipelines-0.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 15:40:24.176299 queue_pipelines-0.1.2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2796 2024-05-04 15:40:24.176299 queue_pipelines-0.1.2/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2178 2024-05-04 15:40:22.000000 queue_pipelines-0.1.2/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      613 2024-05-04 15:40:22.000000 queue_pipelines-0.1.2/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-04 15:40:24.176299 queue_pipelines-0.1.2/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 15:40:24.176299 queue_pipelines-0.1.2/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 15:40:24.176299 queue_pipelines-0.1.2/src/q/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 15:40:24.176299 queue_pipelines-0.1.2/src/q/pipelines/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      123 2024-05-04 13:50:58.000000 queue_pipelines-0.1.2/src/q/pipelines/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      310 2024-05-04 15:33:49.000000 queue_pipelines-0.1.2/src/q/pipelines/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 15:40:24.176299 queue_pipelines-0.1.2/src/q/pipelines/codegen/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 13:50:58.000000 queue_pipelines-0.1.2/src/q/pipelines/codegen/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      190 2024-05-04 13:50:58.000000 queue_pipelines-0.1.2/src/q/pipelines/codegen/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2126 2024-05-04 14:18:33.000000 queue_pipelines-0.1.2/src/q/pipelines/codegen/_local.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      723 2024-05-04 13:50:58.000000 queue_pipelines-0.1.2/src/q/pipelines/codegen/_pipelines.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      581 2024-05-04 13:50:58.000000 queue_pipelines-0.1.2/src/q/pipelines/codegen/_pipelines_init.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2098 2024-05-04 14:49:38.000000 queue_pipelines-0.1.2/src/q/pipelines/codegen/_types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 15:40:24.176299 queue_pipelines-0.1.2/src/q/pipelines/local/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 13:50:58.000000 queue_pipelines-0.1.2/src/q/pipelines/local/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-05-04 13:50:58.000000 queue_pipelines-0.1.2/src/q/pipelines/local/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      846 2024-05-04 15:29:13.000000 queue_pipelines-0.1.2/src/q/pipelines/local/queues.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 15:40:24.176299 queue_pipelines-0.1.2/src/q/pipelines/runners/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 15:33:30.000000 queue_pipelines-0.1.2/src/q/pipelines/runners/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      113 2024-05-04 15:33:43.000000 queue_pipelines-0.1.2/src/q/pipelines/runners/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1447 2024-05-04 15:32:51.000000 queue_pipelines-0.1.2/src/q/pipelines/runners/_connect.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      933 2024-05-04 15:35:47.000000 queue_pipelines-0.1.2/src/q/pipelines/runners/_run.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3779 2024-05-04 13:50:58.000000 queue_pipelines-0.1.2/src/q/pipelines/specs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      484 2024-05-04 14:07:32.000000 queue_pipelines-0.1.2/src/q/pipelines/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 15:40:24.176299 queue_pipelines-0.1.2/src/queue_pipelines.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2796 2024-05-04 15:40:24.000000 queue_pipelines-0.1.2/src/queue_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      809 2024-05-04 15:40:24.000000 queue_pipelines-0.1.2/src/queue_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-04 15:40:24.000000 queue_pipelines-0.1.2/src/queue_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       93 2024-05-04 15:40:24.000000 queue_pipelines-0.1.2/src/queue_pipelines.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        2 2024-05-04 15:40:24.000000 queue_pipelines-0.1.2/src/queue_pipelines.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:59:12.052420 queue_pipelines-0.1.4/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2820 2024-05-07 13:59:12.052420 queue_pipelines-0.1.4/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2178 2024-05-07 13:59:09.000000 queue_pipelines-0.1.4/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      625 2024-05-07 13:59:09.000000 queue_pipelines-0.1.4/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 13:59:12.052420 queue_pipelines-0.1.4/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:59:12.042420 queue_pipelines-0.1.4/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:59:12.042420 queue_pipelines-0.1.4/src/q/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:59:12.042420 queue_pipelines-0.1.4/src/q/pipelines/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      123 2024-05-04 13:50:58.000000 queue_pipelines-0.1.4/src/q/pipelines/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      310 2024-05-04 15:33:49.000000 queue_pipelines-0.1.4/src/q/pipelines/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:59:12.042420 queue_pipelines-0.1.4/src/q/pipelines/codegen/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 13:50:58.000000 queue_pipelines-0.1.4/src/q/pipelines/codegen/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      190 2024-05-04 13:50:58.000000 queue_pipelines-0.1.4/src/q/pipelines/codegen/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2772 2024-05-05 18:09:04.000000 queue_pipelines-0.1.4/src/q/pipelines/codegen/_local.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      723 2024-05-04 13:50:58.000000 queue_pipelines-0.1.4/src/q/pipelines/codegen/_pipelines.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      581 2024-05-04 13:50:58.000000 queue_pipelines-0.1.4/src/q/pipelines/codegen/_pipelines_init.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2098 2024-05-04 14:49:38.000000 queue_pipelines-0.1.4/src/q/pipelines/codegen/_types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:59:12.042420 queue_pipelines-0.1.4/src/q/pipelines/local/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 13:50:58.000000 queue_pipelines-0.1.4/src/q/pipelines/local/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-05-04 13:50:58.000000 queue_pipelines-0.1.4/src/q/pipelines/local/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      846 2024-05-04 15:29:13.000000 queue_pipelines-0.1.4/src/q/pipelines/local/queues.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:59:12.042420 queue_pipelines-0.1.4/src/q/pipelines/runners/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 15:33:30.000000 queue_pipelines-0.1.4/src/q/pipelines/runners/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      113 2024-05-04 15:33:43.000000 queue_pipelines-0.1.4/src/q/pipelines/runners/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1447 2024-05-04 15:32:51.000000 queue_pipelines-0.1.4/src/q/pipelines/runners/_connect.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      933 2024-05-04 18:58:58.000000 queue_pipelines-0.1.4/src/q/pipelines/runners/_run.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3808 2024-05-04 19:25:03.000000 queue_pipelines-0.1.4/src/q/pipelines/specs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      484 2024-05-04 14:07:32.000000 queue_pipelines-0.1.4/src/q/pipelines/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:59:12.042420 queue_pipelines-0.1.4/src/queue_pipelines.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2820 2024-05-07 13:59:12.000000 queue_pipelines-0.1.4/src/queue_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      809 2024-05-07 13:59:12.000000 queue_pipelines-0.1.4/src/queue_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 13:59:12.000000 queue_pipelines-0.1.4/src/queue_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      102 2024-05-07 13:59:12.000000 queue_pipelines-0.1.4/src/queue_pipelines.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        2 2024-05-07 13:59:12.000000 queue_pipelines-0.1.4/src/queue_pipelines.egg-info/top_level.txt
```

### Comparing `queue_pipelines-0.1.2/PKG-INFO` & `queue_pipelines-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: queue-pipelines
-Version: 0.1.2
+Version: 0.1.4
 Summary: Declarative orchestration of asynchronous queue-based tasks
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-api
 Requires-Dist: dslog
 Requires-Dist: prettyprinter
+Requires-Dist: fs-tools
 Provides-Extra: all
 Requires-Dist: queue-kv; extra == "all"
 Requires-Dist: templang; extra == "all"
 Provides-Extra: local
 Requires-Dist: queue-kv; extra == "local"
 Provides-Extra: codegen
 Requires-Dist: templang; extra == "codegen"
```

### Comparing `queue_pipelines-0.1.2/README.md` & `queue_pipelines-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `queue_pipelines-0.1.2/pyproject.toml` & `queue_pipelines-0.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "queue-pipelines"
-version = "0.1.2"
+version = "0.1.4"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Declarative orchestration of asynchronous queue-based tasks"
 dependencies = [
-  "queue-api", "dslog", "prettyprinter"
+  "queue-api", "dslog", "prettyprinter", "fs-tools"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 repo = "https://github.com/marciclabas/pipelines.git"
```

### Comparing `queue_pipelines-0.1.2/src/q/pipelines/codegen/_local.py` & `queue_pipelines-0.1.4/src/q/pipelines/codegen/_local.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # BEGIN
-from typing_extensions import Literal, Any, Unpack
+from typing_extensions import Literal, Any, Unpack, TypedDict, NotRequired
 from dslog import Logger
 from q.api import ReadQueue, WriteQueue
 from q.kv import QueueKV
 import q.pipelines as qp
 AnyT: type = Any # type: ignore
 # UNCOMMENT from MODULE import INPUT, OUTPUT, SPEC_VARIABLE
 # UNCOMMENT from TYPES import Queues, Pipelines
@@ -38,21 +38,44 @@
 
 def run_pipelines(queues: Queues, **pipelines: Unpack[Pipelines]):
   qp.run_pipelines(queues, **pipelines) # type: ignore
 
 def run(
   Qin: ReadQueue[INPUT],
   Qout: WriteQueue[OUTPUT],
-  queues: Queues,
-  connect_logger = Logger.rich().prefix('[CONNECT]'),
+  queues: Queues, *,
+  logger = Logger.rich(),
+  **pipelines: Unpack[Pipelines]
+):
+  ps = qp.run(Qin, Qout, queues, input_task='INPUT_TASK', connect_logger=logger.prefix('[CONNECT]'), **pipelines) # type: ignore
+  for name, p in ps.items():
+    p.start()
+    logger(f'Started process "{name}" at PID = {p.pid}')
+  
+  for name, p in ps.items():
+    p.join()
+    logger(f'Process "{name}" finished')
+
+class Params(TypedDict):
+  queues_path: str
+  protocol: NotRequired[Literal['sqlite', 'fs']]
+  logger: NotRequired[Logger]
+
+def run_local(
+  Qin: ReadQueue[INPUT],
+  Qout: WriteQueue[OUTPUT], *,
+  queues_path: str,
+  protocol: Literal['sqlite', 'fs'] = 'sqlite',
+  logger = Logger.rich(),
   **pipelines: Unpack[Pipelines]
 ):
-  qp.run(Qin, Qout, queues, input_task='INPUT_TASK', connect_logger=connect_logger, **pipelines) # type: ignore
+  Qs = queues(queues_path, protocol=protocol)
+  run(Qin, Qout, Qs, logger=logger, **pipelines)
 
-__all__ = ['input_queue', 'output_queue', 'queues', 'connect', 'run_pipelines', 'run']
+__all__ = ['input_queue', 'output_queue', 'queues', 'connect', 'run_pipelines', 'run', 'run_local', 'Params']
 
 # END
 from templang import parse
 from q.pipelines import Tasks
 
 def local(tasks: Tasks, module: str, types_module: str, spec_variable: str) -> str:
   translations = {
```

### Comparing `queue_pipelines-0.1.2/src/q/pipelines/codegen/_pipelines.py` & `queue_pipelines-0.1.4/src/q/pipelines/codegen/_pipelines.py`

 * *Files identical despite different names*

### Comparing `queue_pipelines-0.1.2/src/q/pipelines/codegen/_pipelines_init.py` & `queue_pipelines-0.1.4/src/q/pipelines/codegen/_pipelines_init.py`

 * *Files identical despite different names*

### Comparing `queue_pipelines-0.1.2/src/q/pipelines/codegen/_types.py` & `queue_pipelines-0.1.4/src/q/pipelines/codegen/_types.py`

 * *Files identical despite different names*

### Comparing `queue_pipelines-0.1.2/src/q/pipelines/local/queues.py` & `queue_pipelines-0.1.4/src/q/pipelines/local/queues.py`

 * *Files identical despite different names*

### Comparing `queue_pipelines-0.1.2/src/q/pipelines/runners/_connect.py` & `queue_pipelines-0.1.4/src/q/pipelines/runners/_connect.py`

 * *Files identical despite different names*

### Comparing `queue_pipelines-0.1.2/src/q/pipelines/runners/_run.py` & `queue_pipelines-0.1.4/src/q/pipelines/runners/_run.py`

 * *Files identical despite different names*

### Comparing `queue_pipelines-0.1.2/src/q/pipelines/specs.py` & `queue_pipelines-0.1.4/src/q/pipelines/specs.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   def __init__(
     self, input_task: Id, Output: type[B],
     tasks: Mapping[Id, Task[A, OutId[Id]]],
   ):
     outkeys = set(x for out in tasks.values() for x in out.outputs) - { 'output' } # type: ignore
     task_keys = set(tasks.keys())
     assert outkeys <= task_keys, f'Invalid output keys: {outkeys - task_keys}'
-    if outkeys != task_keys:
+    if outkeys | { input_task } != task_keys:
       import warnings
       warnings.warn(f'Detected unnreachable tasks: {task_keys - outkeys}')
 
     self.input_task = input_task
     self.Input: type[A] = tasks[input_task].Input
     self.Output = Output
     self.tasks = tasks
@@ -61,17 +61,17 @@
       if r.tag == 'left':
         logger(f'Skipping {task}: {r.value}', level='WARNING')
       else:
         logger(f'Generated {task} pipelines', level='DEBUG')
 
     path = os.path.join(base, '__init__.py')
     source = codegen.pipelines_init(list(self.tasks.keys()), f'..{gen_base}')
-    r = fs.write(path, source)
+    r = fs.write(path, source, replace=False)
     if r.tag == 'left':
-      logger(f'Error writing __init__.py: {r.value}', level='ERROR')
+      logger(f'Skipping __init__.py: {r.value}', level='WARNING')
     else:
       logger(f'Generated __init__.py', level='DEBUG')
 
   def codegen(
     self, __file__: str, variable: str, base: str = 'generated',
     *, logger = Logger.rich().prefix('[CODEGEN]')
   ):
```

### Comparing `queue_pipelines-0.1.2/src/queue_pipelines.egg-info/PKG-INFO` & `queue_pipelines-0.1.4/src/queue_pipelines.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: queue-pipelines
-Version: 0.1.2
+Version: 0.1.4
 Summary: Declarative orchestration of asynchronous queue-based tasks
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-api
 Requires-Dist: dslog
 Requires-Dist: prettyprinter
+Requires-Dist: fs-tools
 Provides-Extra: all
 Requires-Dist: queue-kv; extra == "all"
 Requires-Dist: templang; extra == "all"
 Provides-Extra: local
 Requires-Dist: queue-kv; extra == "local"
 Provides-Extra: codegen
 Requires-Dist: templang; extra == "codegen"
```

### Comparing `queue_pipelines-0.1.2/src/queue_pipelines.egg-info/SOURCES.txt` & `queue_pipelines-0.1.4/src/queue_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

