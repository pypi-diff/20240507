# Comparing `tmp/python_statemachine-2.1.2.tar.gz` & `tmp/python_statemachine-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_statemachine-2.1.2.tar", max compression
+gzip compressed data, was "python_statemachine-2.2.0.tar", max compression
```

## Comparing `python_statemachine-2.1.2.tar` & `python_statemachine-2.2.0.tar`

### file list

```diff
@@ -1,30 +1,28 @@
--rw-r--r--   0        0        0     1074 2023-01-12 02:09:26.102515 python_statemachine-2.1.2/LICENSE
--rw-r--r--   0        0        0    10511 2023-08-03 11:07:28.388948 python_statemachine-2.1.2/README.md
--rw-r--r--   0        0        0     4157 2023-10-06 15:46:31.622910 python_statemachine-2.1.2/pyproject.toml
--rw-r--r--   0        0        0      192 2023-10-06 15:46:31.622910 python_statemachine-2.1.2/statemachine/__init__.py
--rw-r--r--   0        0        0     8265 2023-10-06 15:46:11.682909 python_statemachine-2.1.2/statemachine/callbacks.py
--rw-r--r--   0        0        0        0 2023-01-12 02:09:26.112515 python_statemachine-2.1.2/statemachine/contrib/__init__.py
--rw-r--r--   0        0        0     6748 2023-03-05 22:27:00.883303 python_statemachine-2.1.2/statemachine/contrib/diagram.py
--rw-r--r--   0        0        0     3598 2023-10-06 15:46:11.682909 python_statemachine-2.1.2/statemachine/dispatcher.py
--rw-r--r--   0        0        0     2106 2023-03-13 01:49:09.127086 python_statemachine-2.1.2/statemachine/event.py
--rw-r--r--   0        0        0     2257 2023-03-13 01:45:45.507089 python_statemachine-2.1.2/statemachine/event_data.py
--rw-r--r--   0        0        0      731 2023-03-05 22:27:00.883303 python_statemachine-2.1.2/statemachine/events.py
--rw-r--r--   0        0        0      952 2023-03-13 01:45:45.507089 python_statemachine-2.1.2/statemachine/exceptions.py
--rw-r--r--   0        0        0     5779 2023-08-03 11:07:28.388948 python_statemachine-2.1.2/statemachine/factory.py
--rw-r--r--   0        0        0      359 2023-01-12 02:09:26.112515 python_statemachine-2.1.2/statemachine/graph.py
--rw-r--r--   0        0        0      362 2023-03-05 22:27:00.883303 python_statemachine-2.1.2/statemachine/i18n.py
--rw-r--r--   0        0        0      452 2023-06-12 01:10:29.514642 python_statemachine-2.1.2/statemachine/locale/en/LC_MESSAGES/statemachine.mo
--rw-r--r--   0        0        0     1685 2023-06-12 01:17:52.284641 python_statemachine-2.1.2/statemachine/locale/en/LC_MESSAGES/statemachine.po
--rw-r--r--   0        0        0     1914 2023-06-12 01:10:29.514642 python_statemachine-2.1.2/statemachine/locale/pt_BR/LC_MESSAGES/statemachine.mo
--rw-r--r--   0        0        0     2375 2023-06-12 01:17:52.284641 python_statemachine-2.1.2/statemachine/locale/pt_BR/LC_MESSAGES/statemachine.po
--rw-r--r--   0        0        0     1055 2023-03-13 01:45:45.507089 python_statemachine-2.1.2/statemachine/mixins.py
--rw-r--r--   0        0        0      211 2023-06-12 01:16:16.764636 python_statemachine-2.1.2/statemachine/model.py
--rw-r--r--   0        0        0      959 2023-06-12 01:16:16.764636 python_statemachine-2.1.2/statemachine/registry.py
--rw-r--r--   0        0        0     7463 2023-10-06 15:46:11.682909 python_statemachine-2.1.2/statemachine/signature.py
--rw-r--r--   0        0        0     8175 2023-10-06 15:46:11.682909 python_statemachine-2.1.2/statemachine/state.py
--rw-r--r--   0        0        0    11998 2023-10-06 15:46:11.682909 python_statemachine-2.1.2/statemachine/statemachine.py
--rw-r--r--   0        0        0     4151 2023-06-12 01:16:16.764636 python_statemachine-2.1.2/statemachine/states.py
--rw-r--r--   0        0        0     4833 2023-10-06 15:46:11.692909 python_statemachine-2.1.2/statemachine/transition.py
--rw-r--r--   0        0        0     5949 2023-06-12 01:16:16.764636 python_statemachine-2.1.2/statemachine/transition_list.py
--rw-r--r--   0        0        0      317 2023-10-06 15:46:11.692909 python_statemachine-2.1.2/statemachine/utils.py
--rw-r--r--   0        0        0    11454 1970-01-01 00:00:00.000000 python_statemachine-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-07 00:25:17.694061 python_statemachine-2.2.0/LICENSE
+-rw-r--r--   0        0        0    10511 2024-05-07 00:25:17.694061 python_statemachine-2.2.0/README.md
+-rw-r--r--   0        0        0     4340 2024-05-07 00:25:17.698061 python_statemachine-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      192 2024-05-07 00:25:17.698061 python_statemachine-2.2.0/statemachine/__init__.py
+-rw-r--r--   0        0        0     8704 2024-05-07 00:25:17.698061 python_statemachine-2.2.0/statemachine/callbacks.py
+-rw-r--r--   0        0        0        0 2024-05-07 00:25:17.698061 python_statemachine-2.2.0/statemachine/contrib/__init__.py
+-rw-r--r--   0        0        0     7004 2024-05-07 00:25:17.698061 python_statemachine-2.2.0/statemachine/contrib/diagram.py
+-rw-r--r--   0        0        0     4924 2024-05-07 00:25:17.698061 python_statemachine-2.2.0/statemachine/dispatcher.py
+-rw-r--r--   0        0        0     2106 2024-05-07 00:25:17.698061 python_statemachine-2.2.0/statemachine/event.py
+-rw-r--r--   0        0        0     2257 2024-05-07 00:25:17.698061 python_statemachine-2.2.0/statemachine/event_data.py
+-rw-r--r--   0        0        0      731 2024-05-07 00:25:17.698061 python_statemachine-2.2.0/statemachine/events.py
+-rw-r--r--   0        0        0      952 2024-05-07 00:25:17.698061 python_statemachine-2.2.0/statemachine/exceptions.py
+-rw-r--r--   0        0        0     8015 2024-05-07 00:25:17.698061 python_statemachine-2.2.0/statemachine/factory.py
+-rw-r--r--   0        0        0      487 2024-05-07 00:25:17.698061 python_statemachine-2.2.0/statemachine/graph.py
+-rw-r--r--   0        0        0      362 2024-05-07 00:25:17.698061 python_statemachine-2.2.0/statemachine/i18n.py
+-rw-r--r--   0        0        0     1685 2024-05-07 00:25:17.698061 python_statemachine-2.2.0/statemachine/locale/en/LC_MESSAGES/statemachine.po
+-rw-r--r--   0        0        0     2375 2024-05-07 00:25:17.698061 python_statemachine-2.2.0/statemachine/locale/pt_BR/LC_MESSAGES/statemachine.po
+-rw-r--r--   0        0        0     1017 2024-05-07 00:25:17.698061 python_statemachine-2.2.0/statemachine/mixins.py
+-rw-r--r--   0        0        0      211 2024-05-07 00:25:17.698061 python_statemachine-2.2.0/statemachine/model.py
+-rw-r--r--   0        0        0      959 2024-05-07 00:25:17.698061 python_statemachine-2.2.0/statemachine/registry.py
+-rw-r--r--   0        0        0     7507 2024-05-07 00:25:17.698061 python_statemachine-2.2.0/statemachine/signature.py
+-rw-r--r--   0        0        0     8315 2024-05-07 00:25:17.698061 python_statemachine-2.2.0/statemachine/state.py
+-rw-r--r--   0        0        0    11659 2024-05-07 00:25:17.702061 python_statemachine-2.2.0/statemachine/statemachine.py
+-rw-r--r--   0        0        0     4203 2024-05-07 00:25:17.702061 python_statemachine-2.2.0/statemachine/states.py
+-rw-r--r--   0        0        0     5388 2024-05-07 00:25:17.702061 python_statemachine-2.2.0/statemachine/transition.py
+-rw-r--r--   0        0        0     5949 2024-05-07 00:25:17.702061 python_statemachine-2.2.0/statemachine/transition_list.py
+-rw-r--r--   0        0        0      458 2024-05-07 00:25:17.702061 python_statemachine-2.2.0/statemachine/utils.py
+-rw-r--r--   0        0        0    11454 1970-01-01 00:00:00.000000 python_statemachine-2.2.0/PKG-INFO
```

### Comparing `python_statemachine-2.1.2/LICENSE` & `python_statemachine-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.2/README.md` & `python_statemachine-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.2/pyproject.toml` & `python_statemachine-2.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-statemachine"
-version = "2.1.2"
+version = "2.2.0"
 description = "Python Finite State Machines made easy."
 authors = ["Fernando Macedo <fgmacedo@gmail.com>"]
 maintainers = [
     "Fernando Macedo <fgmacedo@gmail.com>",
 ]
 license = "MIT license"
 readme = "README.md"
@@ -30,37 +30,35 @@
     "Topic :: Software Development :: Libraries"
 ]
 
 [tool.poetry.extras]
 diagrams = ["pydot"]
 
 [tool.poetry.dependencies]
-python = ">=3.7, <3.13"
+python = ">=3.9, <3.13"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.0"
-pytest-cov = "^4.0.0"
-pytest-sugar = "^0.9.6"
-pydot = "^1.4.2"
-ruff = "^0.0.257"
-pre-commit = "^2.21.0"
-mypy = "^0.991"
-black = "^22.12.0"
-pdbpp = "^0.10.3"
+pytest = "^8.1.1"
+pytest-cov = "^5.0.0"
+pytest-sugar = "^1.0.0"
+pydot = "^2.0.0"
+ruff = "^0.3.7"
+pre-commit = "^3.7.0"
+mypy = "^1.9.0"
 pytest-mock = "^3.10.0"
 pytest-profiling = "^1.7.0"
 pytest-benchmark = "^4.0.0"
 
 [tool.poetry.group.docs.dependencies]
-Sphinx = "4.5.0"
-sphinx-rtd-theme = "1.1.1"
-myst-parser = "^0.18.1"
-sphinx-gallery = "^0.11.1"
-pillow = "^9.4.0"
-sphinx-autobuild = "^2021.3.14"
+Sphinx = "7.2.6"
+sphinx-rtd-theme = "2.0.0"
+myst-parser = "^2.0.0"
+sphinx-gallery = "^0.15.0"
+pillow = "^10.3.0"
+sphinx-autobuild = "^2024.4.16"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = "--ignore=docs/conf.py --ignore=docs/auto_examples/ --ignore=docs/_build/ --ignore=tests/examples/ --cov --cov-config .coveragerc --doctest-glob='*.md' --doctest-modules --doctest-continue-on-failure --benchmark-autosave"
@@ -87,32 +85,16 @@
     "W503",
 ]
 max-line-length = 99
 
 [tool.ruff]
 src = ["statemachine"]
 
-# Enable Pyflakes and pycodestyle rules.
-select = [
-    "E", # pycodestyle errors
-    "W", # pycodestyle warnings
-    "F", # pyflakes
-    "I", # isort
-    "UP", # pyupgrade
-    "C",  # flake8-comprehensions
-    "B",  # flake8-bugbear
-    "PT", # flake8-pytest-style
-]
-ignore = [
-    "UP006", # `use-pep585-annotation` Requires Python3.9+
-    "UP035", # `use-pep585-annotation` Requires Python3.9+
-    "UP038", # `use-pep585-annotation` Requires Python3.9+
-]
-
 line-length = 99
+target-version = "py312"
 
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".direnv",
     ".eggs",
     ".git",
     ".mypy_cache",
@@ -127,27 +109,49 @@
     "build",
     "dist",
     "node_modules",
     "auto_examples",
     "venv",
 ]
 
+[tool.ruff.lint]
+
+# Enable Pyflakes and pycodestyle rules.
+select = [
+    "E", # pycodestyle errors
+    "W", # pycodestyle warnings
+    "F", # pyflakes
+    "I", # isort
+    "UP", # pyupgrade
+    "C",  # flake8-comprehensions
+    "B",  # flake8-bugbear
+    "PT", # flake8-pytest-style
+]
+ignore = [
+    "UP006", # `use-pep585-annotation` Requires Python3.9+
+    "UP035", # `use-pep585-annotation` Requires Python3.9+
+    "UP038", # `use-pep585-annotation` Requires Python3.9+
+]
+
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
-# Assume Python 3.11.
-target-version = "py311"
+[tool.ruff.lint.per-file-ignores]
+# Ignore `E402` (import violations) in all `__init__.py` files, and in `path/to/file.py`.
+"__init__.py" = ["E402"]
+"path/to/file.py" = ["E402"]
+"tests/examples/**.py" = ["B018"]
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 6
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 force-single-line = true
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 # Use Google-style docstrings.
 convention = "google"
 
 [tool.coverage.run]
 branch = true
 relative_files = true
 data_file = ".coverage"
```

### Comparing `python_statemachine-2.1.2/statemachine/callbacks.py` & `python_statemachine-2.2.0/statemachine/callbacks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,123 +1,155 @@
+from bisect import insort
 from collections import defaultdict
 from collections import deque
+from enum import IntEnum
 from typing import Callable
 from typing import Dict
+from typing import Generator
 from typing import List
 
 from .exceptions import AttrNotFound
 from .i18n import _
 from .utils import ensure_iterable
 
 
+class CallbackPriority(IntEnum):
+    GENERIC = 0
+    INLINE = 10
+    DECORATOR = 20
+    NAMING = 30
+    AFTER = 40
+
+
+def allways_true(*args, **kwargs):
+    return True
+
+
 class CallbackWrapper:
     def __init__(
         self,
         callback: Callable,
         condition: Callable,
+        meta: "CallbackMeta",
         unique_key: str,
-        expected_value: "bool | None" = None,
     ) -> None:
         self._callback = callback
         self.condition = condition
+        self.meta = meta
         self.unique_key = unique_key
-        self.expected_value = expected_value
 
     def __repr__(self):
         return f"{type(self).__name__}({self.unique_key})"
 
+    def __str__(self):
+        return str(self.meta)
+
+    def __lt__(self, other):
+        return self.meta.priority < other.meta.priority
+
     def __call__(self, *args, **kwargs):
-        result = self._callback(*args, **kwargs)
-        if self.expected_value is not None:
-            return bool(result) == self.expected_value
-        return result
+        return self._callback(*args, **kwargs)
 
 
 class CallbackMeta:
     """A thin wrapper that register info about actions and guards.
 
     At first, `func` can be a string or a callable, and even if it's already
     a callable, his signature can mismatch.
 
     After instantiation, `.setup(resolver)` must be called before any real
     call is performed, to allow the proper callback resolution.
     """
 
-    def __init__(self, func, suppress_errors=False, cond=None, expected_value=None):
+    def __init__(
+        self,
+        func,
+        suppress_errors=False,
+        cond=None,
+        priority: CallbackPriority = CallbackPriority.NAMING,
+        expected_value=None,
+    ):
         self.func = func
         self.suppress_errors = suppress_errors
-        self.cond = CallbackMetaList().add(cond)
+        self.cond = cond
         self.expected_value = expected_value
+        self.priority = priority
 
     def __repr__(self):
-        return f"{type(self).__name__}({self.func!r})"
+        return f"{type(self).__name__}({self.func!r}, suppress_errors={self.suppress_errors!r})"
 
     def __str__(self):
         return getattr(self.func, "__name__", self.func)
 
     def __eq__(self, other):
         return self.func == other.func
 
     def __hash__(self):
         return id(self)
 
     def _update_func(self, func):
         self.func = func
 
-    def build(self, resolver) -> "CallbackWrapper | None":
+    def _wrap_callable(self, func, _expected_value):
+        return func
+
+    def build(self, resolver) -> Generator["CallbackWrapper", None, None]:
         """
         Resolves the `func` into a usable callable.
 
         Args:
             resolver (callable): A method responsible to build and return a valid callable that
                 can receive arbitrary parameters like `*args, **kwargs`.
         """
-        callback = resolver(self.func)
-        if not callback.is_empty:
-            conditions = CallbacksExecutor()
-            conditions.add(self.cond, resolver)
-
-            return CallbackWrapper(
-                callback=callback,
-                condition=conditions.all,
+        for callback in resolver(self.func):
+            condition = next(resolver(self.cond)) if self.cond is not None else allways_true
+            yield CallbackWrapper(
+                callback=self._wrap_callable(callback, self.expected_value),
+                condition=condition,
+                meta=self,
                 unique_key=callback.unique_key,
-                expected_value=self.expected_value,
             )
 
-        if not self.suppress_errors:
-            raise AttrNotFound(
-                _("Did not found name '{}' from model or statemachine").format(
-                    self.func
-                )
-            )
-        return None
-
 
 class BoolCallbackMeta(CallbackMeta):
     """A thin wrapper that register info about actions and guards.
 
     At first, `func` can be a string or a callable, and even if it's already
     a callable, his signature can mismatch.
 
     After instantiation, `.setup(resolver)` must be called before any real
     call is performed, to allow the proper callback resolution.
     """
 
-    def __init__(self, func, suppress_errors=False, cond=None, expected_value=True):
-        self.func = func
-        self.suppress_errors = suppress_errors
-        self.cond = CallbackMetaList().add(cond)
-        self.expected_value = expected_value
+    def __init__(
+        self,
+        func,
+        suppress_errors=False,
+        cond=None,
+        priority: CallbackPriority = CallbackPriority.NAMING,
+        expected_value=True,
+    ):
+        super().__init__(
+            func, suppress_errors, cond, priority=priority, expected_value=expected_value
+        )
 
     def __str__(self):
         name = super().__str__()
         return name if self.expected_value else f"!{name}"
 
+    def _wrap_callable(self, func, expected_value):
+        def bool_wrapper(*args, **kwargs):
+            return bool(func(*args, **kwargs)) == expected_value
+
+        return bool_wrapper
+
 
 class CallbackMetaList:
+    """List of `CallbackMeta` instances"""
+
     def __init__(self, factory=CallbackMeta):
         self.items: List[CallbackMeta] = []
         self.factory = factory
 
     def __repr__(self):
         return f"{type(self).__name__}({self.items!r}, factory={self.factory!r})"
 
@@ -153,108 +185,101 @@
         func._callbacks_to_update.add(callback._update_func)
         func._is_event = is_event
         func._transitions = transitions
 
         return func
 
     def __call__(self, callback):
+        """Allows usage of the callback list as a decorator."""
         return self._add_unbounded_callback(callback)
 
     def __iter__(self):
         return iter(self.items)
 
     def clear(self):
         self.items = []
 
-    def _add(self, func, registry=None, prepend=False, **kwargs):
+    def _add(self, func, **kwargs):
         meta = self.factory(func, **kwargs)
-        if registry is not None and not registry(self, meta, prepend=prepend):
-            return
 
         if meta in self.items:
             return
 
-        if prepend:
-            self.items.insert(0, meta)
-        else:
-            self.items.append(meta)
+        self.items.append(meta)
         return meta
 
     def add(self, callbacks, **kwargs):
         if callbacks is None:
             return self
 
         unprepared = ensure_iterable(callbacks)
         for func in unprepared:
             self._add(func, **kwargs)
 
         return self
 
 
 class CallbacksExecutor:
+    """A list of callbacks that can be executed in order."""
+
     def __init__(self):
         self.items: List[CallbackWrapper] = deque()
         self.items_already_seen = set()
 
     def __iter__(self):
         return iter(self.items)
 
     def __repr__(self):
         return f"{type(self).__name__}({self.items!r})"
 
-    def add_one(
-        self, callback_info: CallbackMeta, resolver: Callable, prepend: bool = False
-    ) -> "CallbackWrapper | None":
-        callback = callback_info.build(resolver)
-        if callback is None:
-            return None
-
-        if callback.unique_key in self.items_already_seen:
-            return None
-
-        self.items_already_seen.add(callback.unique_key)
-        if prepend:
-            self.items.insert(0, callback)
-        else:
-            self.items.append(callback)
-        return callback
+    def __str__(self):
+        return ", ".join(str(c) for c in self)
+
+    def _add(self, callback_meta: CallbackMeta, resolver: Callable):
+        for callback in callback_meta.build(resolver):
+            if callback.unique_key in self.items_already_seen:
+                continue
+
+            self.items_already_seen.add(callback.unique_key)
+            insort(self.items, callback)
 
     def add(self, items: CallbackMetaList, resolver: Callable):
         """Validate configurations"""
         for item in items:
-            self.add_one(item, resolver)
+            self._add(item, resolver)
         return self
 
     def call(self, *args, **kwargs):
         return [
-            callback(*args, **kwargs)
-            for callback in self
-            if callback.condition(*args, **kwargs)
+            callback(*args, **kwargs) for callback in self if callback.condition(*args, **kwargs)
         ]
 
     def all(self, *args, **kwargs):
         return all(condition(*args, **kwargs) for condition in self)
 
 
 class CallbacksRegistry:
     def __init__(self) -> None:
-        self._registry: Dict[CallbackMetaList, CallbacksExecutor] = defaultdict(
-            CallbacksExecutor
-        )
+        self._registry: Dict[CallbackMetaList, CallbacksExecutor] = defaultdict(CallbacksExecutor)
 
-    def register(self, callbacks: CallbackMetaList, resolver):
-        executor_list = self[callbacks]
-        executor_list.add(callbacks, resolver)
+    def register(self, meta_list: CallbackMetaList, resolver):
+        executor_list = self[meta_list]
+        executor_list.add(meta_list, resolver)
         return executor_list
 
-    def __getitem__(self, callbacks: CallbackMetaList) -> CallbacksExecutor:
-        return self._registry[callbacks]
+    def clear(self):
+        self._registry.clear()
+
+    def __getitem__(self, meta_list: CallbackMetaList) -> CallbacksExecutor:
+        return self._registry[meta_list]
 
-    def build_register_function_for_resolver(self, resolver):
-        def register(
-            meta_list: CallbackMetaList,
-            meta: CallbackMeta,
-            prepend: bool = False,
-        ):
-            return self[meta_list].add_one(meta, resolver, prepend=prepend)
+    def check(self, meta_list: CallbackMetaList):
+        executor = self[meta_list]
+        for meta in meta_list:
+            if meta.suppress_errors:
+                continue
 
-        return register
+            if any(callback for callback in executor if callback.meta == meta):
+                continue
+            raise AttrNotFound(
+                _("Did not found name '{}' from model or statemachine").format(meta.func)
+            )
```

### Comparing `python_statemachine-2.1.2/statemachine/contrib/diagram.py` & `python_statemachine-2.2.0/statemachine/contrib/diagram.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,29 +62,43 @@
             self.machine.initial_state.id,
             label="",
             color="blue",
             fontname=self.font_name,
             fontsize=self.transition_font_size,
         )
 
+    def _actions_getter(self):
+        if isinstance(self.machine, StateMachine):
+
+            def getter(x):
+                return self.machine._callbacks(x)
+        else:
+
+            def getter(x):
+                return x
+
+        return getter
+
     def _state_actions(self, state):
-        entry = ", ".join([str(action) for action in state.enter])
-        exit = ", ".join([str(action) for action in state.exit])
+        getter = self._actions_getter()
+
+        entry = str(getter(state.enter))
+        exit_ = str(getter(state.exit))
         internal = ", ".join(
-            f"{transition.event} / {transition.on!s}"
+            f"{transition.event} / {str(getter(transition.on))}"
             for transition in state.transitions
             if transition.internal
         )
 
         if entry:
             entry = f"entry / {entry}"
-        if exit:
-            exit = f"exit / {exit}"
+        if exit_:
+            exit_ = f"exit / {exit_}"
 
-        actions = "\n".join(x for x in [entry, exit, internal] if x)
+        actions = "\n".join(x for x in [entry, exit_, internal] if x)
 
         if actions:
             actions = f"\n{actions}"
 
         return actions
 
     def _state_as_node(self, state):
```

### Comparing `python_statemachine-2.1.2/statemachine/dispatcher.py` & `python_statemachine-2.2.0/statemachine/dispatcher.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from collections import namedtuple
 from operator import attrgetter
 from typing import Any
+from typing import Generator
 
 from .signature import SignatureAdapter
 
 
 class ObjectConfig(namedtuple("ObjectConfig", "obj skip_attrs resolver_id")):
     """Configuration for objects passed to resolver_factory.
 
@@ -14,25 +15,18 @@
     """
 
     @classmethod
     def from_obj(cls, obj, skip_attrs=None):
         if isinstance(obj, ObjectConfig):
             return obj
         else:
-            return cls(obj, set(skip_attrs) if skip_attrs else set(), str(id(obj)))
-
-    def getattr(self, attr):
-        if attr in self.skip_attrs:
-            return
-        return getattr(self.obj, attr, None)
+            return cls(obj, skip_attrs or set(), str(id(obj)))
 
 
 class WrapSearchResult:
-    is_empty = False
-
     def __init__(self, attribute, resolver_id) -> None:
         self.attribute = attribute
         self.resolver_id = resolver_id
         self._cache = None
         self.unique_key = f"{attribute}@{resolver_id}"
 
     def __repr__(self):
@@ -44,18 +38,14 @@
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         if self._cache is None:
             self._cache = self.wrap()
         assert self._cache
         return self._cache(*args, **kwds)
 
 
-class EmptyWrapSearchResult(WrapSearchResult):
-    is_empty = True
-
-
 class CallableSearchResult(WrapSearchResult):
     def __init__(self, attribute, a_callable, resolver_id) -> None:
         self.a_callable = a_callable
         super().__init__(attribute, resolver_id)
 
     def wrap(self):
         return SignatureAdapter.wrap(self.a_callable)
@@ -89,36 +79,78 @@
         def wrapper(*args, **kwargs):
             kwargs.pop("machine", None)
             return self.func(*args, **kwargs)
 
         return wrapper
 
 
-def search_callable(attr, *configs) -> WrapSearchResult:
-    if callable(attr) or isinstance(attr, property):
-        return CallableSearchResult(attr, attr, None)
-
-    for config in configs:
-        func = config.getattr(attr)
-        if func is not None:
-            if not callable(func):
-                return AttributeCallableSearchResult(
-                    attr, config.obj, config.resolver_id
-                )
+def _search_callable_attr_is_property(
+    attr, configs: tuple[ObjectConfig]
+) -> "WrapSearchResult | None":
+    # if the attr is a property, we'll try to find the object that has the
+    # property on the configs
+    attr_name = attr.fget.__name__
+    for obj, _skip_attrs, resolver_id in configs:
+        func = getattr(type(obj), attr_name, None)
+        if func is not None and func is attr:
+            return AttributeCallableSearchResult(attr_name, obj, resolver_id)
+    return None
+
+
+def _search_callable_attr_is_callable(attr, configs: tuple[ObjectConfig]) -> WrapSearchResult:
+    # if the attr is an unbounded method, we'll try to find the bounded method
+    # on the configs
+    if not hasattr(attr, "__self__"):
+        for obj, _skip_attrs, resolver_id in configs:
+            func = getattr(obj, attr.__name__, None)
+            if func is not None and func.__func__ is attr:
+                return CallableSearchResult(attr.__name__, func, resolver_id)
+
+    return CallableSearchResult(attr, attr, None)
+
+
+def _search_callable_in_configs(
+    attr, configs: tuple[ObjectConfig]
+) -> Generator[WrapSearchResult, None, None]:
+    for obj, skip_attrs, resolver_id in configs:
+        if attr in skip_attrs:
+            continue
+
+        if not hasattr(obj, attr):
+            continue
+
+        func = getattr(obj, attr)
+        if not callable(func):
+            yield AttributeCallableSearchResult(attr, obj, resolver_id)
+
+        if getattr(func, "_is_sm_event", False):
+            yield EventSearchResult(attr, func, resolver_id)
+
+        yield CallableSearchResult(attr, func, resolver_id)
+
+
+def search_callable(attr, configs: tuple) -> Generator[WrapSearchResult, None, None]:  # noqa: C901
+    if isinstance(attr, property):
+        result = _search_callable_attr_is_property(attr, configs)
+        if result is not None:
+            yield result
+        return
+
+    if callable(attr):
+        yield _search_callable_attr_is_callable(attr, configs)
+        return
 
-            if getattr(func, "_is_sm_event", False):
-                return EventSearchResult(attr, func, config.resolver_id)
+    yield from _search_callable_in_configs(attr, configs)
 
-            return CallableSearchResult(attr, func, config.resolver_id)
 
-    return EmptyWrapSearchResult(attr, None)
-
-
-def resolver_factory(*objects):
+def resolver_factory(objects: tuple[ObjectConfig]):
     """Factory that returns a configured resolver."""
 
-    objects = [ObjectConfig.from_obj(obj) for obj in objects]
-
-    def wrapper(attr):
-        return search_callable(attr, *objects)
+    def wrapper(attr) -> Generator[WrapSearchResult, None, None]:
+        yield from search_callable(attr, objects)
 
     return wrapper
+
+
+def resolver_factory_from_objects(*objects: tuple[Any]):
+    configs = tuple(ObjectConfig.from_obj(o) for o in objects)
+    return resolver_factory(configs)
```

### Comparing `python_statemachine-2.1.2/statemachine/event.py` & `python_statemachine-2.2.0/statemachine/event.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.2/statemachine/event_data.py` & `python_statemachine-2.2.0/statemachine/event_data.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.2/statemachine/events.py` & `python_statemachine-2.2.0/statemachine/events.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.2/statemachine/exceptions.py` & `python_statemachine-2.2.0/statemachine/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.2/statemachine/locale/en/LC_MESSAGES/statemachine.po` & `python_statemachine-2.2.0/statemachine/locale/en/LC_MESSAGES/statemachine.po`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.2/statemachine/locale/pt_BR/LC_MESSAGES/statemachine.po` & `python_statemachine-2.2.0/statemachine/locale/pt_BR/LC_MESSAGES/statemachine.po`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.2/statemachine/mixins.py` & `python_statemachine-2.2.0/statemachine/mixins.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,17 +16,15 @@
     state_machine_attr = "statemachine"  # type: str
     """Name of the model's attribute that will hold the machine instance."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         if not self.state_machine_name:
             raise ValueError(
-                _("{!r} is not a valid state machine name.").format(
-                    self.state_machine_name
-                )
+                _("{!r} is not a valid state machine name.").format(self.state_machine_name)
             )
         machine_cls = registry.get_machine_cls(self.state_machine_name)
         setattr(
             self,
             self.state_machine_attr,
             machine_cls(self, state_field=self.state_field_name),
         )
```

### Comparing `python_statemachine-2.1.2/statemachine/registry.py` & `python_statemachine-2.2.0/statemachine/registry.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.2/statemachine/signature.py` & `python_statemachine-2.2.0/statemachine/signature.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 from inspect import Signature
 from types import MethodType
 from typing import Any
 
 
 def _make_key(method):
     method = method.func if isinstance(method, partial) else method
+    method = method.fget if isinstance(method, property) else method
     if isinstance(method, MethodType):
         return hash(
             (
                 method.__qualname__,
                 method.__self__.__class__.__name__,
                 method.__code__.co_varnames,
             )
         )
     else:
         return hash((method.__qualname__, method.__code__.co_varnames))
 
 
 def signature_cache(user_function):
-
     cache = {}
     cache_get = cache.get
 
     def cached_function(cls, method):
         key = _make_key(method)
         sig = cache_get(key)
         if sig is None:
@@ -109,16 +109,15 @@
                                 "but was passed as a keyword"
                             )
                             msg = msg.format(arg=param.name)
                             raise TypeError(msg) from None
                         parameters_ex = (param,)
                         break
                     elif (
-                        param.kind == Parameter.VAR_KEYWORD
-                        or param.default is not Parameter.empty
+                        param.kind == Parameter.VAR_KEYWORD or param.default is not Parameter.empty
                     ):
                         # That's fine too - we have a default value for this
                         # parameter.  So, lets start parsing `kwargs`, starting
                         # with the current parameter
                         parameters_ex = (param,)
                         break
                     else:
```

### Comparing `python_statemachine-2.1.2/statemachine/state.py` & `python_statemachine-2.2.0/statemachine/state.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Dict
 from weakref import ref
 
 from .callbacks import CallbackMetaList
+from .callbacks import CallbackPriority
 from .exceptions import StateMachineError
 from .i18n import _
 from .transition import Transition
 from .transition_list import TransitionList
 
 if TYPE_CHECKING:
     from .statemachine import StateMachine
@@ -103,61 +104,59 @@
     ):
         self.name = name
         self.value = value
         self._initial = initial
         self._final = final
         self._id: str = ""
         self.transitions = TransitionList()
-        self.enter = CallbackMetaList().add(enter)
-        self.exit = CallbackMetaList().add(exit)
+        self.enter = CallbackMetaList().add(enter, priority=CallbackPriority.INLINE)
+        self.exit = CallbackMetaList().add(exit, priority=CallbackPriority.INLINE)
 
     def __eq__(self, other):
-        return (
-            isinstance(other, State) and self.name == other.name and self.id == other.id
-        )
+        return isinstance(other, State) and self.name == other.name and self.id == other.id
 
     def __hash__(self):
         return hash(repr(self))
 
-    def _setup(self, register):
+    def _setup(self):
+        self.enter.add("on_enter_state", priority=CallbackPriority.GENERIC, suppress_errors=True)
+        self.enter.add(
+            f"on_enter_{self.id}", priority=CallbackPriority.NAMING, suppress_errors=True
+        )
+        self.exit.add("on_exit_state", priority=CallbackPriority.GENERIC, suppress_errors=True)
+        self.exit.add(f"on_exit_{self.id}", priority=CallbackPriority.NAMING, suppress_errors=True)
+
+    def _add_observer(self, register):
         register(self.enter)
         register(self.exit)
-        return self
 
-    def _add_observer(self, registry):
-        self.enter.add(
-            "on_enter_state", registry=registry, prepend=True, suppress_errors=True
-        )
-        self.enter.add(f"on_enter_{self.id}", registry=registry, suppress_errors=True)
-        self.exit.add(
-            "on_exit_state", registry=registry, prepend=True, suppress_errors=True
-        )
-        self.exit.add(f"on_exit_{self.id}", registry=registry, suppress_errors=True)
+    def _check_callbacks(self, check):
+        check(self.enter)
+        check(self.exit)
 
     def __repr__(self):
         return (
             f"{type(self).__name__}({self.name!r}, id={self.id!r}, value={self.value!r}, "
             f"initial={self.initial!r}, final={self.final!r})"
         )
 
+    def __str__(self):
+        return self.name
+
     def __get__(self, machine, owner):
         if machine is None:
             return self
         return self.for_instance(machine=machine, cache=machine._states_for_instance)
 
     def __set__(self, instance, value):
         raise StateMachineError(
-            _("State overriding is not allowed. Trying to add '{}' to {}").format(
-                value, self.id
-            )
+            _("State overriding is not allowed. Trying to add '{}' to {}").format(value, self.id)
         )
 
-    def for_instance(
-        self, machine: "StateMachine", cache: Dict["State", "State"]
-    ) -> "State":
+    def for_instance(self, machine: "StateMachine", cache: Dict["State", "State"]) -> "State":
         if self not in cache:
             cache[self] = InstanceState(self, machine)
 
         return cache[self]
 
     @property
     def id(self) -> str:
@@ -167,17 +166,15 @@
         self._id = id
         if self.value is None:
             self.value = id
         if not self.name:
             self.name = self._id.replace("_", " ").capitalize()
 
     def _to_(self, *states: "State", **kwargs):
-        transitions = TransitionList(
-            Transition(self, state, **kwargs) for state in states
-        )
+        transitions = TransitionList(Transition(self, state, **kwargs) for state in states)
         self.transitions.add_transitions(transitions)
         return transitions
 
     def _from_(self, *states: "State", **kwargs):
         transitions = TransitionList()
         for origin in states:
             transition = Transition(origin, self, **kwargs)
```

### Comparing `python_statemachine-2.1.2/statemachine/statemachine.py` & `python_statemachine-2.2.0/statemachine/statemachine.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from collections import deque
+from copy import deepcopy
 from functools import partial
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Dict
 
+from statemachine.graph import iterate_states_and_transitions
+
+from .callbacks import CallbackMetaList
+from .callbacks import CallbacksExecutor
 from .callbacks import CallbacksRegistry
 from .dispatcher import ObjectConfig
 from .dispatcher import resolver_factory
 from .event import Event
 from .event_data import EventData
 from .event_data import TriggerData
 from .exceptions import InvalidDefinition
@@ -69,136 +74,112 @@
         self.start_value = start_value
         self.allow_event_without_transition = allow_event_without_transition
         self.__rtc = rtc
         self.__processing: bool = False
         self._external_queue: deque = deque()
         self._callbacks_registry = CallbacksRegistry()
         self._states_for_instance: Dict["State", "State"] = {}
+        self._observers: Dict[Any, Any] = {}
 
-        assert hasattr(self, "_abstract")
         if self._abstract:
             raise InvalidDefinition(_("There are no states or transitions."))
 
-        initial_transition = Transition(
-            None, self._get_initial_state(), event="__initial__"
-        )
-        self._setup(initial_transition)
-        self._activate_initial_state(initial_transition)
+        self._register_callbacks()
+        self._activate_initial_state()
+
+    def __init_subclass__(cls, strict_states: bool = False):
+        cls._strict_states = strict_states
+        super().__init_subclass__()
 
     if TYPE_CHECKING:
         """Makes mypy happy with dynamic created attributes"""
 
-        def __getattr__(self, attribute: str) -> Any:
-            ...
+        def __getattr__(self, attribute: str) -> Any: ...
 
     def __repr__(self):
         current_state_id = self.current_state.id if self.current_state_value else None
         return (
             f"{type(self).__name__}(model={self.model!r}, state_field={self.state_field!r}, "
             f"current_state={current_state_id!r})"
         )
 
+    def __deepcopy__(self, memo):
+        deepcopy_method = self.__deepcopy__
+        self.__deepcopy__ = None
+        try:
+            cp = deepcopy(self, memo)
+        finally:
+            self.__deepcopy__ = deepcopy_method
+            cp.__deepcopy__ = deepcopy_method
+        cp._callbacks_registry.clear()
+        cp._register_callbacks()
+        cp.add_observer(*cp._observers.keys())
+        return cp
+
     def _get_initial_state(self):
-        current_state_value = (
-            self.start_value if self.start_value else self.initial_state.value
-        )
+        current_state_value = self.start_value if self.start_value else self.initial_state.value
         try:
             return self.states_map[current_state_value]
         except KeyError as err:
             raise InvalidStateValue(current_state_value) from err
 
-    def _activate_initial_state(self, initial_transition):
+    def _activate_initial_state(self):
         if self.current_state_value is None:
             # send an one-time event `__initial__` to enter the current state.
             # current_state = self.current_state
+            initial_transition = Transition(None, self._get_initial_state(), event="__initial__")
             initial_transition.before.clear()
             initial_transition.on.clear()
             initial_transition.after.clear()
 
             event_data = EventData(
                 trigger_data=TriggerData(
                     machine=self,
                     event=initial_transition.event,
                 ),
                 transition=initial_transition,
             )
             self._activate(event_data)
 
-    def _get_protected_attrs(self):
-        return {
-            "_abstract",
-            "model",
-            "state_field",
-            "start_value",
-            "initial_state",
-            "final_states",
-            "states",
-            "_events",
-            "states_map",
-            "send",
-        } | {s.id for s in self.states}
-
-    def _visit_states_and_transitions(self, visitor):
-        for state in self.states:
-            visitor(state)
-            for transition in state.transitions:
-                visitor(transition)
-
-    def _setup(self, initial_transition: Transition):
-        """
-        Args:
-            initial_transition: A special :ref:`transition` that triggers the enter on the
-                `initial` :ref:`State`.
-        """
-        machine = ObjectConfig.from_obj(self, skip_attrs=self._get_protected_attrs())
-        model = ObjectConfig.from_obj(self.model, skip_attrs={self.state_field})
-        default_resolver = resolver_factory(machine, model)
-
-        register = partial(self._callbacks_registry.register, resolver=default_resolver)
-
-        observer_visitor = self._build_observers_visitor(machine, model)
-
-        def setup_visitor(visited):
-            visited._setup(register)
-            observer_visitor(visited)
-
-        self._visit_states_and_transitions(setup_visitor)
-
-        initial_transition._setup(register)
-
-    def _build_observers_visitor(self, *observers):
-        registry_callbacks = [
+    def _register_callbacks(self):
+        self._add_observer(
             (
-                self._callbacks_registry.build_register_function_for_resolver(
-                    resolver_factory(observer)
-                )
+                ObjectConfig.from_obj(self, skip_attrs=self._protected_attrs),
+                ObjectConfig.from_obj(self.model, skip_attrs={self.state_field}),
             )
-            for observer in observers
-        ]
+        )
 
-        def _add_observer_for_resolver(visited):
-            for register in registry_callbacks:
-                visited._add_observer(register)
+        check_callbacks = self._callbacks_registry.check
+        for visited in iterate_states_and_transitions(self.states):
+            try:
+                visited._check_callbacks(check_callbacks)
+            except Exception as err:
+                raise InvalidDefinition(
+                    f"Error on {visited!s} when resolving callbacks: {err}"
+                ) from err
+
+    def _add_observer(self, observers):
+        register = partial(self._callbacks_registry.register, resolver=resolver_factory(observers))
+        for visited in iterate_states_and_transitions(self.states):
+            visited._add_observer(register)
 
-        return _add_observer_for_resolver
+        return self
 
     def add_observer(self, *observers):
         """Add an observer.
 
         Observers are a way to generically add behavior to a :ref:`StateMachine` without changing
         its internal implementation.
 
         .. seealso::
 
             :ref:`observers`.
         """
-
-        visitor = self._build_observers_visitor(*observers)
-        self._visit_states_and_transitions(visitor)
-        return self
+        self._observers.update({o: None for o in observers})
+        return self._add_observer(tuple(ObjectConfig.from_obj(o) for o in observers))
 
     def _repr_html_(self):
         return f'<div class="statemachine">{self._repr_svg_()}</div>'
 
     def _repr_svg_(self):
         return self._graph().create_svg().decode()
 
@@ -244,18 +225,15 @@
     @property
     def events(self):
         return self.__class__.events
 
     @property
     def allowed_events(self):
         """List of the current allowed events."""
-        return [
-            getattr(self, event)
-            for event in self.current_state.transitions.unique_events
-        ]
+        return [getattr(self, event) for event in self.current_state.transitions.unique_events]
 
     def _process(self, trigger):
         """Process event triggers.
 
         The simplest implementation is the non-RTC (synchronous),
         where the trigger will be run immediately and the result collected as the return.
 
@@ -313,36 +291,30 @@
         return first_result if first_result is not sentinel else None
 
     def _activate(self, event_data: EventData):
         transition = event_data.transition
         source = event_data.state
         target = transition.target
 
-        result = self._callbacks_registry[transition.before].call(
+        result = self._callbacks(transition.before).call(
             *event_data.args, **event_data.extended_kwargs
         )
         if source is not None and not transition.internal:
-            self._callbacks_registry[source.exit].call(
-                *event_data.args, **event_data.extended_kwargs
-            )
+            self._callbacks(source.exit).call(*event_data.args, **event_data.extended_kwargs)
 
-        result += self._callbacks_registry[transition.on].call(
+        result += self._callbacks(transition.on).call(
             *event_data.args, **event_data.extended_kwargs
         )
 
         self.current_state = target
         event_data.state = target
 
         if not transition.internal:
-            self._callbacks_registry[target.enter].call(
-                *event_data.args, **event_data.extended_kwargs
-            )
-        self._callbacks_registry[transition.after].call(
-            *event_data.args, **event_data.extended_kwargs
-        )
+            self._callbacks(target.enter).call(*event_data.args, **event_data.extended_kwargs)
+        self._callbacks(transition.after).call(*event_data.args, **event_data.extended_kwargs)
 
         if len(result) == 0:
             result = None
         elif len(result) == 1:
             result = result[0]
 
         return result
@@ -353,7 +325,10 @@
         .. seealso::
 
             See: :ref:`triggering events`.
 
         """
         event = Event(event)
         return event.trigger(self, *args, **kwargs)
+
+    def _callbacks(self, meta_list: CallbackMetaList) -> CallbacksExecutor:
+        return self._callbacks_registry[meta_list]
```

### Comparing `python_statemachine-2.1.2/statemachine/states.py` & `python_statemachine-2.2.0/statemachine/states.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,29 +11,31 @@
 class States:
     """
     A class representing a collection of :ref:`State` objects.
 
     Helps creating :ref:`StateMachine`'s :ref:`state` definitions from other
     sources, like an ``Enum`` class, using :meth:`States.from_enum`.
 
+    >>> states_def = [('open', {'initial': True}), ('closed', {'final': True})]
+
     >>> from statemachine import StateMachine
     >>> class SM(StateMachine):
     ...
     ...     states = States({
-    ...         name: State(initial=idx == 0) for idx, name in enumerate(["initial", "final"])
+    ...         name: State(**params) for name, params in states_def
     ...     })
     ...
-    ...     finish = states.initial.to(states.final)
+    ...     close = states.open.to(states.closed)
 
     And states can be used as usual.
 
     >>> sm = SM()
-    >>> sm.send("finish")
+    >>> sm.send("close")
     >>> sm.current_state.id
-    'final'
+    'closed'
 
     """
 
     def __init__(self, states: "Dict[str, State] | None" = None) -> None:
         """
         Initializes a new instance of the States class.
```

### Comparing `python_statemachine-2.1.2/statemachine/transition.py` & `python_statemachine-2.2.0/statemachine/transition.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import TYPE_CHECKING
 
 from .callbacks import BoolCallbackMeta
 from .callbacks import CallbackMetaList
+from .callbacks import CallbackPriority
 from .event import same_event_cond_builder
 from .events import Events
 from .exceptions import InvalidDefinition
 
 if TYPE_CHECKING:
     from .event_data import EventData
 
@@ -44,82 +45,90 @@
         validators=None,
         cond=None,
         unless=None,
         on=None,
         before=None,
         after=None,
     ):
-
         self.source = source
         self.target = target
         self.internal = internal
 
         if internal and source is not target:
             raise InvalidDefinition("Internal transitions should be self-transitions.")
 
         self._events = Events().add(event)
-        self.validators = CallbackMetaList().add(validators)
-        self.before = CallbackMetaList().add(before)
-        self.on = CallbackMetaList().add(on)
-        self.after = CallbackMetaList().add(after)
+        self.validators = CallbackMetaList().add(validators, priority=CallbackPriority.INLINE)
+        self.before = CallbackMetaList().add(before, priority=CallbackPriority.INLINE)
+        self.on = CallbackMetaList().add(on, priority=CallbackPriority.INLINE)
+        self.after = CallbackMetaList().add(after, priority=CallbackPriority.INLINE)
         self.cond = (
             CallbackMetaList(factory=BoolCallbackMeta)
-            .add(cond)
-            .add(unless, expected_value=False)
+            .add(cond, priority=CallbackPriority.INLINE)
+            .add(unless, priority=CallbackPriority.INLINE, expected_value=False)
         )
 
     def __repr__(self):
         return (
             f"{type(self).__name__}({self.source!r}, {self.target!r}, event={self.event!r}, "
             f"internal={self.internal!r})"
         )
 
-    def _setup(self, register):
-        register(self.validators)
-        register(self.cond)
-        register(self.before)
-        register(self.on)
-        register(self.after)
+    def __str__(self):
+        return f"transition {self.event!s} from {self.source!s} to {self.target!s}"
 
-    def _add_observer(self, registry):
+    def _setup(self):
         before = self.before.add
         on = self.on.add
         after = self.after.add
-        before(
-            "before_transition", registry=registry, suppress_errors=True, prepend=True
-        )
-        on("on_transition", registry=registry, suppress_errors=True, prepend=True)
+
+        before("before_transition", priority=CallbackPriority.GENERIC, suppress_errors=True)
+        on("on_transition", priority=CallbackPriority.GENERIC, suppress_errors=True)
 
         for event in self._events:
             same_event_cond = same_event_cond_builder(event)
             before(
                 f"before_{event}",
-                registry=registry,
+                priority=CallbackPriority.NAMING,
                 suppress_errors=True,
                 cond=same_event_cond,
             )
             on(
                 f"on_{event}",
-                registry=registry,
+                priority=CallbackPriority.NAMING,
                 suppress_errors=True,
                 cond=same_event_cond,
             )
             after(
                 f"after_{event}",
-                registry=registry,
+                priority=CallbackPriority.NAMING,
                 suppress_errors=True,
                 cond=same_event_cond,
             )
 
         after(
             "after_transition",
-            registry=registry,
+            priority=CallbackPriority.AFTER,
             suppress_errors=True,
         )
 
+    def _add_observer(self, register):
+        register(self.validators)
+        register(self.cond)
+        register(self.before)
+        register(self.on)
+        register(self.after)
+
+    def _check_callbacks(self, check):
+        check(self.validators)
+        check(self.cond)
+        check(self.before)
+        check(self.on)
+        check(self.after)
+
     def match(self, event):
         return self._events.match(event)
 
     @property
     def event(self):
         return str(self._events)
```

### Comparing `python_statemachine-2.1.2/statemachine/transition_list.py` & `python_statemachine-2.2.0/statemachine/transition_list.py`

 * *Files identical despite different names*

### Comparing `python_statemachine-2.1.2/PKG-INFO` & `python_statemachine-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: python-statemachine
-Version: 2.1.2
+Version: 2.2.0
 Summary: Python Finite State Machines made easy.
 Home-page: https://github.com/fgmacedo/python-statemachine
 License: MIT
 Author: Fernando Macedo
 Author-email: fgmacedo@gmail.com
 Maintainer: Fernando Macedo
 Maintainer-email: fgmacedo@gmail.com
-Requires-Python: >=3.7,<3.13
+Requires-Python: >=3.9,<3.13
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: diagrams
 Description-Content-Type: text/markdown
 
 # Python StateMachine
 
 [![pypi](https://img.shields.io/pypi/v/python-statemachine.svg)](https://pypi.python.org/pypi/python-statemachine)
```

