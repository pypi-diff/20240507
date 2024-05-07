# Comparing `tmp/asynctaskpool-0.1.2.tar.gz` & `tmp/asynctaskpool-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asynctaskpool-0.1.2.tar", max compression
+gzip compressed data, was "asynctaskpool-0.1.3.tar", max compression
```

## Comparing `asynctaskpool-0.1.2.tar` & `asynctaskpool-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      269 2024-04-17 01:27:05.871060 asynctaskpool-0.1.2/README.md
--rw-r--r--   0        0        0       36 2024-04-17 01:22:02.972148 asynctaskpool-0.1.2/asynctaskpool/__init__.py
--rw-r--r--   0        0        0     1151 2024-04-17 01:22:31.908809 asynctaskpool-0.1.2/asynctaskpool/in_progress_task.py
--rw-r--r--   0        0        0     4434 2024-04-18 02:58:21.795855 asynctaskpool-0.1.2/asynctaskpool/task_pool.py
--rw-r--r--   0        0        0      566 2024-04-18 02:58:42.340541 asynctaskpool-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      911 1970-01-01 00:00:00.000000 asynctaskpool-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      269 2024-04-28 02:44:52.129759 asynctaskpool-0.1.3/README.md
+-rw-r--r--   0        0        0       36 2024-04-28 02:44:52.133759 asynctaskpool-0.1.3/asynctaskpool/__init__.py
+-rw-r--r--   0        0        0      112 2024-04-28 02:44:52.125759 asynctaskpool-0.1.3/asynctaskpool/task_failed_exception.py
+-rw-r--r--   0        0        0     4803 2024-04-28 03:13:06.225490 asynctaskpool-0.1.3/asynctaskpool/taskpool.py
+-rw-r--r--   0        0        0     1568 2024-04-28 02:26:50.979685 asynctaskpool-0.1.3/asynctaskpool/taskpool_task.py
+-rw-r--r--   0        0        0      612 2024-04-28 02:48:45.322715 asynctaskpool-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      916 1970-01-01 00:00:00.000000 asynctaskpool-0.1.3/PKG-INFO
```

### Comparing `asynctaskpool-0.1.2/asynctaskpool/task_pool.py` & `asynctaskpool-0.1.3/asynctaskpool/taskpool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import logging
 from typing import TypeVar, Generic, Any, Coroutine
 
-from .in_progress_task import TaskpoolTask
+from .task_failed_exception import TaskFailedError
+from .taskpool_task import TaskpoolTask
 
 T = TypeVar("T")
 
 
 class AsyncTaskPool(Generic[T]):
     """
     A TaskPool is a utility that receives submitted tasks which have an identity and which should be executed no more
@@ -19,35 +20,42 @@
         self._task_tracker: dict[object, asyncio.Event | T | None] = {}
         self._semaphore = asyncio.Semaphore()
         self._restart_task_if_finished: bool = restart_if_finished
 
     def take_in_precomputed_result_map(self, results: dict[object, T]) -> None:
         self._task_tracker.update(**results)
 
-    async def wait_for_task_to_finish_if_running(self, task_id: str):
-        task_to_wait_for: None | TaskpoolTask = None
-
+    async def wait_for_task_to_finish_if_running(self, task_id: object) -> bool:
         async with self._semaphore:
-            if self._has_task_been_submitted_yet(task_id) and self._is_task_in_progress(task_id):
+            if self._has_task_been_submitted_yet(task_id):
                 task_to_wait_for = self._get_tracked_task(task_id)
 
-        if task_to_wait_for is not None:
-            # Ignore result, we don't need it
-            await task_to_wait_for.wait_and_get_result()
+                if self._has_task_finished(task_to_wait_for):
+                    self._logger.debug("Task %s has already finished, do not need to wait", task_id)
+                    return False
+            else:
+                self._logger.debug("Task %s has not been started", task_id)
+                return False
+
+        self._logger.debug("Waiting for task %s", task_id)
+
+        # Ignore result, we don't need it
+        await task_to_wait_for.wait_and_get_result()
+        return True
 
     async def submit_new_task(self, task_id: object, future: Coroutine) -> T | None:
         # Any async item that we need to await is put into this.
         # Then we await it at the end of the function, so we can use exception-safe 'with' block without holding the semaphore too long.
         async_operation_to_wait_for: Coroutine | None = None
 
         async with self._semaphore:
             if self._has_task_been_submitted_yet(task_id):
                 task = self._get_tracked_task(task_id)
 
-                if not self._is_task_in_progress(task):
+                if self._has_task_finished(task):
                     if not self._restart_task_if_finished:
                         self._logger.debug("Task %s already finished, returning.", task_id)
                         return task
                     else:
                         async_operation_to_wait_for = self._create_and_run_task(task_id, future)
                 else:
                     async_operation_to_wait_for = task.wait_and_get_result()
@@ -59,50 +67,49 @@
 
     def _has_task_been_submitted_yet(self, task_id: object):
         return task_id in self._task_tracker.keys()
 
     def _get_tracked_task(self, task_id: object) -> TaskpoolTask | T | None:
         return self._task_tracker[task_id]
 
-    @staticmethod
-    def _is_task_in_progress(task: Any) -> bool:
-        return isinstance(task, TaskpoolTask)
-
     def _create_and_track_new_unstarted_task(self, task_id: object, future: Coroutine) -> TaskpoolTask:
         self._logger.debug("Creating new task %s.", task_id)
-
         new_in_progress_task = TaskpoolTask(task_id=task_id, future=future)
         self._track_new_task(new_in_progress_task)
         return new_in_progress_task
 
     def _track_new_task(self, task: TaskpoolTask):
         self._task_tracker[task.task_id] = task
 
-    async def _run_task_and_record_result(self, task: TaskpoolTask) -> T:
-        task_result = await task.run_task()
-
-        self._logger.debug("Task %s finished", task.task_id)
-        await self._record_result_of_task_and_mark_finished(task=task, result=task_result)
-
-        return task_result
-
-    async def _record_result_of_task_and_mark_finished(self, task: TaskpoolTask, result: Any):
+    async def _record_result_of_task(self, task: TaskpoolTask, result: Any):
         async with self._semaphore:
-            self._update_tracked_task_with_result(task.task_id, result)
-
-        task.mark_finished()
-
-    def _update_tracked_task_with_result(self, task_id: object, result: Any):
-        self._task_tracker[task_id] = result
+            self._task_tracker[task.task_id] = result
 
     async def _create_and_run_task(self, task_id: object, future: Coroutine):
         new_task = self._create_and_track_new_unstarted_task(task_id=task_id, future=future)
         return await self._run_task_and_record_result(new_task)
 
+    async def _run_task_and_record_result(self, task: TaskpoolTask) -> T:
+        try:
+            task_result = await task.run_task()
+            await self._record_result_of_task(task=task, result=task_result)
+            return task_result
+        except TaskFailedError as e:
+            self._erase_task_due_to_failure(task)
+            raise e
+
+    def _erase_task_due_to_failure(self, task: TaskpoolTask):
+        self._logger.warning("Removing tracking for task %s due to it failing", task.task_id)
+        del self._task_tracker[task.task_id]
+
     def clear_results(self) -> None:
         self._task_tracker.clear()
 
     def get_results_of_all_completed_tasks(self) -> list[T]:
         def exclude_none_and_unfinished_tasks(it):
-            return it is not None and not self._is_task_in_progress(it)
+            return it is not None and self._has_task_finished(it)
 
         return list(filter(exclude_none_and_unfinished_tasks, self._task_tracker.values()))
+
+    @staticmethod
+    def _has_task_finished(task: Any) -> bool:
+        return not isinstance(task, TaskpoolTask)
```

### Comparing `asynctaskpool-0.1.2/pyproject.toml` & `asynctaskpool-0.1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 [tool.poetry]
 name = "asynctaskpool"
-version = "0.1.2"
+version = "0.1.3"
 description = "Provides a task pool for asynchronous tasks to be executed only once."
 authors = ["QCanvas <qcanvas@noreply.codeberg.org>"]
 readme = "README.md"
 repository = "https://codeberg.org/QCanvas/AsyncTaskPool"
 keywords = ["async", "taskpool"]
 classifiers = [
     "Framework :: AsyncIO"
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.10"
+python = "^3.10"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
 pytest-asyncio = "^0.23.6"
+pytest-timeout = "^2.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[pytest]
+timeout = 5
```

### Comparing `asynctaskpool-0.1.2/PKG-INFO` & `asynctaskpool-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: asynctaskpool
-Version: 0.1.2
+Version: 0.1.3
 Summary: Provides a task pool for asynchronous tasks to be executed only once.
 Home-page: https://codeberg.org/QCanvas/AsyncTaskPool
 Keywords: async,taskpool
 Author: QCanvas
 Author-email: qcanvas@noreply.codeberg.org
-Requires-Python: >=3.10
+Requires-Python: >=3.10,<4.0
 Classifier: Framework :: AsyncIO
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://codeberg.org/QCanvas/AsyncTaskPool
 Description-Content-Type: text/markdown
 
 # AsyncTaskPool
 
-This tool provides an asynchronous 'task pool'. Tasks with an identifier can be submitted to it and they will only be executed once -
+This tool provides an asynchronous 'task pool'. Tasks with an identifier can be submitted to it and they will only be
+executed once -
 even when submitted again before the first task has finished.
 The results of these tasks will be cached for next time.
```

