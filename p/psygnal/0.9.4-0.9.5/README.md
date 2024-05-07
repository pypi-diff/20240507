# Comparing `tmp/psygnal-0.9.4.tar.gz` & `tmp/psygnal-0.9.5.tar.gz`

## Comparing `psygnal-0.9.4.tar` & `psygnal-0.9.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0    27389 2020-02-02 00:00:00.000000 psygnal-0.9.4/CHANGELOG.md
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/__init__.py
--rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/_dataclass_utils.py
--rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/_evented_decorator.py
--rw-r--r--   0        0        0    19995 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/_evented_model_v1.py
--rw-r--r--   0        0        0    19098 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/_evented_model_v2.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/_exceptions.py
--rw-r--r--   0        0        0     9108 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/_group.py
--rw-r--r--   0        0        0    16852 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/_group_descriptor.py
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/_queue.py
--rw-r--r--   0        0        0    51104 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/_signal.py
--rw-r--r--   0        0        0     8328 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/_throttler.py
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/_throttler.pyi
--rw-r--r--   0        0        0    17372 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/_weak_callback.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/py.typed
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/qt.py
--rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/_pyinstaller_util/__init__.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/_pyinstaller_util/_pyinstaller_hook.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/_pyinstaller_util/hook-psygnal.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/containers/__init__.py
--rw-r--r--   0        0        0     5746 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/containers/_evented_dict.py
--rw-r--r--   0        0        0    15427 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/containers/_evented_list.py
--rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/containers/_evented_proxy.py
--rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/containers/_evented_set.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/containers/_selectable_evented_list.py
--rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 psygnal-0.9.4/src/psygnal/containers/_selection.py
--rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 psygnal-0.9.4/tests/test_bench.py
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 psygnal-0.9.4/tests/test_dataclass_utils.py
--rw-r--r--   0        0        0     5661 2020-02-02 00:00:00.000000 psygnal-0.9.4/tests/test_evented_decorator.py
--rw-r--r--   0        0        0    21427 2020-02-02 00:00:00.000000 psygnal-0.9.4/tests/test_evented_model.py
--rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 psygnal-0.9.4/tests/test_group.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 psygnal-0.9.4/tests/test_group_descriptor.py
--rw-r--r--   0        0        0    26724 2020-02-02 00:00:00.000000 psygnal-0.9.4/tests/test_psygnal.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 psygnal-0.9.4/tests/test_pyinstaller_hook.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 psygnal-0.9.4/tests/test_qt_compat.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 psygnal-0.9.4/tests/test_throttler.py
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 psygnal-0.9.4/tests/test_utils.py
--rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 psygnal-0.9.4/tests/test_weak_callable.py
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 psygnal-0.9.4/tests/containers/test_evented_dict.py
--rw-r--r--   0        0        0    11859 2020-02-02 00:00:00.000000 psygnal-0.9.4/tests/containers/test_evented_list.py
--rw-r--r--   0        0        0     5089 2020-02-02 00:00:00.000000 psygnal-0.9.4/tests/containers/test_evented_proxy.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 psygnal-0.9.4/tests/containers/test_evented_set.py
--rw-r--r--   0        0        0     4453 2020-02-02 00:00:00.000000 psygnal-0.9.4/tests/containers/test_selectable_evented_list.py
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 psygnal-0.9.4/tests/containers/test_selection.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 psygnal-0.9.4/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 psygnal-0.9.4/LICENSE
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 psygnal-0.9.4/README.md
--rw-r--r--   0        0        0     6089 2020-02-02 00:00:00.000000 psygnal-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     6832 2020-02-02 00:00:00.000000 psygnal-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0    28375 2020-02-02 00:00:00.000000 psygnal-0.9.5/CHANGELOG.md
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/__init__.py
+-rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/_dataclass_utils.py
+-rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/_evented_decorator.py
+-rw-r--r--   0        0        0    19995 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/_evented_model_v1.py
+-rw-r--r--   0        0        0    19098 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/_evented_model_v2.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/_exceptions.py
+-rw-r--r--   0        0        0     9108 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/_group.py
+-rw-r--r--   0        0        0    16939 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/_group_descriptor.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/_queue.py
+-rw-r--r--   0        0        0    51096 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/_signal.py
+-rw-r--r--   0        0        0     8328 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/_throttler.py
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/_throttler.pyi
+-rw-r--r--   0        0        0    19781 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/_weak_callback.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/py.typed
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/qt.py
+-rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/_pyinstaller_util/__init__.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/_pyinstaller_util/_pyinstaller_hook.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/_pyinstaller_util/hook-psygnal.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/containers/__init__.py
+-rw-r--r--   0        0        0     5746 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/containers/_evented_dict.py
+-rw-r--r--   0        0        0    15427 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/containers/_evented_list.py
+-rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/containers/_evented_proxy.py
+-rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/containers/_evented_set.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/containers/_selectable_evented_list.py
+-rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 psygnal-0.9.5/src/psygnal/containers/_selection.py
+-rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 psygnal-0.9.5/tests/test_bench.py
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 psygnal-0.9.5/tests/test_dataclass_utils.py
+-rw-r--r--   0        0        0     5661 2020-02-02 00:00:00.000000 psygnal-0.9.5/tests/test_evented_decorator.py
+-rw-r--r--   0        0        0    21427 2020-02-02 00:00:00.000000 psygnal-0.9.5/tests/test_evented_model.py
+-rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 psygnal-0.9.5/tests/test_group.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 psygnal-0.9.5/tests/test_group_descriptor.py
+-rw-r--r--   0        0        0    26724 2020-02-02 00:00:00.000000 psygnal-0.9.5/tests/test_psygnal.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 psygnal-0.9.5/tests/test_pyinstaller_hook.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 psygnal-0.9.5/tests/test_qt_compat.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 psygnal-0.9.5/tests/test_throttler.py
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 psygnal-0.9.5/tests/test_utils.py
+-rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 psygnal-0.9.5/tests/test_weak_callable.py
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 psygnal-0.9.5/tests/containers/test_evented_dict.py
+-rw-r--r--   0        0        0    11859 2020-02-02 00:00:00.000000 psygnal-0.9.5/tests/containers/test_evented_list.py
+-rw-r--r--   0        0        0     5089 2020-02-02 00:00:00.000000 psygnal-0.9.5/tests/containers/test_evented_proxy.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 psygnal-0.9.5/tests/containers/test_evented_set.py
+-rw-r--r--   0        0        0     4453 2020-02-02 00:00:00.000000 psygnal-0.9.5/tests/containers/test_selectable_evented_list.py
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 psygnal-0.9.5/tests/containers/test_selection.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 psygnal-0.9.5/.gitignore
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 psygnal-0.9.5/LICENSE
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 psygnal-0.9.5/README.md
+-rw-r--r--   0        0        0     6089 2020-02-02 00:00:00.000000 psygnal-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     6884 2020-02-02 00:00:00.000000 psygnal-0.9.5/PKG-INFO
```

### Comparing `psygnal-0.9.4/CHANGELOG.md` & `psygnal-0.9.5/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 # Changelog
 
+## [v0.9.5](https://github.com/pyapp-kit/psygnal/tree/v0.9.5) (2023-11-13)
+
+[Full Changelog](https://github.com/pyapp-kit/psygnal/compare/v0.9.4...v0.9.5)
+
+**Implemented enhancements:**
+
+- feat: better repr for WeakCallback objects [\#236](https://github.com/pyapp-kit/psygnal/pull/236) ([tlambert03](https://github.com/tlambert03))
+
+**Merged pull requests:**
+
+- fix: fix py37 build [\#243](https://github.com/pyapp-kit/psygnal/pull/243) ([tlambert03](https://github.com/tlambert03))
+- ci\(dependabot\): bump pypa/cibuildwheel from 2.16.1 to 2.16.2 [\#240](https://github.com/pyapp-kit/psygnal/pull/240) ([dependabot[bot]](https://github.com/apps/dependabot))
+- ci\(dependabot\): bump pypa/cibuildwheel from 2.15.0 to 2.16.1 [\#238](https://github.com/pyapp-kit/psygnal/pull/238) ([dependabot[bot]](https://github.com/apps/dependabot))
+- refactor: make EmitLoop error message clearer [\#232](https://github.com/pyapp-kit/psygnal/pull/232) ([tlambert03](https://github.com/tlambert03))
+
 ## [v0.9.4](https://github.com/pyapp-kit/psygnal/tree/v0.9.4) (2023-09-19)
 
 [Full Changelog](https://github.com/pyapp-kit/psygnal/compare/v0.9.3...v0.9.4)
 
 **Implemented enhancements:**
 
 - perf: don't compare before/after values in evented dataclass/model when no signals connected [\#235](https://github.com/pyapp-kit/psygnal/pull/235) ([tlambert03](https://github.com/tlambert03))
```

### Comparing `psygnal-0.9.4/src/psygnal/__init__.py` & `psygnal-0.9.5/src/psygnal/__init__.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/src/psygnal/_dataclass_utils.py` & `psygnal-0.9.5/src/psygnal/_dataclass_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
     if is_pydantic_model(cls):
         if hasattr(cls, "model_fields"):
             for field_name, p_field in cls.model_fields.items():
                 if not p_field.frozen or not exclude_frozen:
                     yield field_name, p_field.annotation
         else:
             for p_field in cls.__fields__.values():  # type: ignore [attr-defined]
-                if p_field.field_info.allow_mutation or not exclude_frozen:  # type: ignore  # noqa
+                if p_field.field_info.allow_mutation or not exclude_frozen:  # type: ignore
                     yield p_field.name, p_field.outer_type_  # type: ignore
         return
 
     attrs_fields = getattr(cls, "__attrs_attrs__", None)
     if attrs_fields is not None:
         for a_field in attrs_fields:
             yield a_field.name, a_field.type
```

### Comparing `psygnal-0.9.4/src/psygnal/_evented_decorator.py` & `psygnal-0.9.5/src/psygnal/_evented_decorator.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/src/psygnal/_evented_model_v1.py` & `psygnal-0.9.5/src/psygnal/_evented_model_v1.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/src/psygnal/_evented_model_v2.py` & `psygnal-0.9.5/src/psygnal/_evented_model_v2.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/src/psygnal/_group.py` & `psygnal-0.9.5/src/psygnal/_group.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/src/psygnal/_group_descriptor.py` & `psygnal-0.9.5/src/psygnal/_group_descriptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -419,16 +419,18 @@
             # __get__ logic in the future, but if it fails, no big deal.
             if self._name and self._cache_on_instance:
                 with contextlib.suppress(Exception):
                     setattr(instance, self._name, self._instance_map[obj_id])
 
             # clean up the cache when the instance is deleted
             with contextlib.suppress(TypeError):
-                # mypy says too many attributes for weakref.finalize, but it's wrong.
-                weakref.finalize(instance, self._instance_map.pop, obj_id, None)  # type: ignore [call-arg]  # noqa
+                # on 3.7 this is type error, above it's not... but mypy yells about
+                # type ignore on 3.8+, so we do this funny business instead.
+                args = (instance, self._instance_map.pop, obj_id, None)
+                weakref.finalize(*args)  # type: ignore
 
         return self._instance_map[obj_id]
 
     def _create_group(self, owner: type) -> type[SignalGroup]:
         Group = self._signal_group or _build_dataclass_signal_group(owner, self._eqop)
         if self._warn_on_no_fields and not Group._signals_:
             warnings.warn(
```

### Comparing `psygnal-0.9.4/src/psygnal/_queue.py` & `psygnal-0.9.5/src/psygnal/_queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,8 +91,8 @@
     queue = QueuedCallback._GLOBAL_QUEUE[_thread]
 
     while not queue.empty():
         cb, args = queue.get()
         try:
             cb(args)
         except Exception as e:  # pragma: no cover
-            raise EmitLoopError(slot_repr=repr(cb), args=args, exc=e) from e
+            raise EmitLoopError(cb=cb, args=args, exc=e) from e
```

### Comparing `psygnal-0.9.4/src/psygnal/_signal.py` & `psygnal-0.9.5/src/psygnal/_signal.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 
 from mypy_extensions import mypyc_attr
 from typing_extensions import get_args, get_origin
 
 from ._exceptions import EmitLoopError
 from ._queue import QueuedCallback
 from ._weak_callback import (
+    StrongFunction,
     WeakCallback,
-    _StrongFunction,
-    _WeakSetattr,
-    _WeakSetitem,
+    WeakSetattr,
+    WeakSetitem,
     weak_callback,
 )
 
 if TYPE_CHECKING:
     from typing_extensions import Literal
 
     from ._group import EmissionInfo
@@ -593,15 +593,15 @@
                 stacklevel=2,
             )
             obj = obj()
         if not hasattr(obj, attr):
             raise AttributeError(f"Object {obj} has no attribute {attr!r}")
 
         with self._lock:
-            caller = _WeakSetattr(
+            caller = WeakSetattr(
                 obj,
                 attr,
                 max_args=maxargs,
                 finalize=self._try_discard,
                 on_ref_error=on_ref_error,
             )
             self._slots.append(caller)
@@ -626,15 +626,15 @@
         Raises
         ------
         ValueError
             If `missing_ok` is `True` and no attribute setter is connected.
         """
         # sourcery skip: merge-nested-ifs, use-next
         with self._lock:
-            cb = _WeakSetattr(obj, attr, on_ref_error="ignore")
+            cb = WeakSetattr(obj, attr, on_ref_error="ignore")
             self._try_discard(cb, missing_ok)
 
     def connect_setitem(
         self,
         obj: weakref.ref | object,
         key: str,
         maxargs: int | None = None,
@@ -697,15 +697,15 @@
                 stacklevel=2,
             )
             obj = obj()
         if not hasattr(obj, "__setitem__"):
             raise TypeError(f"Object {obj} does not support __setitem__")
 
         with self._lock:
-            caller = _WeakSetitem(
+            caller = WeakSetitem(
                 obj,  # type: ignore
                 key,
                 max_args=maxargs,
                 finalize=self._try_discard,
                 on_ref_error=on_ref_error,
             )
             self._slots.append(caller)
@@ -734,15 +734,15 @@
             If `missing_ok` is `True` and no item setter is connected.
         """
         if not hasattr(obj, "__setitem__"):
             raise TypeError(f"Object {obj} does not support __setitem__")
 
         # sourcery skip: merge-nested-ifs, use-next
         with self._lock:
-            caller = _WeakSetitem(obj, key, on_ref_error="ignore")
+            caller = WeakSetitem(obj, key, on_ref_error="ignore")
             self._try_discard(caller, missing_ok)
 
     def _check_nargs(
         self, slot: Callable, spec: Signature
     ) -> tuple[Signature | None, int | None, bool]:
         """Make sure slot is compatible with signature.
 
@@ -986,15 +986,15 @@
         with self._lock:
             with Signal._emitting(self):
                 for caller in self._slots:
                     try:
                         caller.cb(args)
                     except Exception as e:
                         raise EmitLoopError(
-                            slot_repr=repr(caller), args=args, exc=e
+                            cb=caller, args=args, exc=e, signal=self
                         ) from e
 
         return None
 
     def block(self, exclude: Iterable[str | SignalInstance] = ()) -> None:
         """Block this signal from emitting.
 
@@ -1120,15 +1120,15 @@
             "_is_paused",
             "_args_queue",
             "_check_nargs_on_connect",
             "_check_types_on_connect",
         )
         dd = {slot: getattr(self, slot) for slot in attrs}
         dd["_instance"] = self._instance()
-        dd["_slots"] = [x for x in self._slots if isinstance(x, _StrongFunction)]
+        dd["_slots"] = [x for x in self._slots if isinstance(x, StrongFunction)]
         if len(self._slots) > len(dd["_slots"]):
             warnings.warn(
                 "Pickling a SignalInstance does not copy connected weakly referenced "
                 "slots.",
                 stacklevel=2,
             )
```

### Comparing `psygnal-0.9.4/src/psygnal/_throttler.py` & `psygnal-0.9.5/src/psygnal/_throttler.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/src/psygnal/_throttler.pyi` & `psygnal-0.9.5/src/psygnal/_throttler.pyi`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/src/psygnal/_weak_callback.py` & `psygnal-0.9.5/src/psygnal/_weak_callback.py`

 * *Files 16% similar despite different names*

```diff
@@ -108,46 +108,46 @@
     if isinstance(cb, partial):
         args = cb.args + args
         kwargs = cb.keywords
         cb = cb.func
 
     if isinstance(cb, FunctionType):
         return (
-            _StrongFunction(cb, max_args, args, kwargs)
+            StrongFunction(cb, max_args, args, kwargs)
             if strong_func
-            else _WeakFunction(cb, max_args, args, kwargs, finalize, on_ref_error)
+            else WeakFunction(cb, max_args, args, kwargs, finalize, on_ref_error)
         )
 
     if isinstance(cb, MethodType):
         if getattr(cb, "__name__", None) == "__setitem__":
             try:
                 key = args[0]
             except IndexError as e:  # pragma: no cover
                 raise TypeError(
                     "WeakCallback.__setitem__ requires a key argument"
                 ) from e
             obj = cast("SupportsSetitem", cb.__self__)
-            return _WeakSetitem(obj, key, max_args, finalize, on_ref_error)
-        return _WeakMethod(cb, max_args, args, kwargs, finalize, on_ref_error)
+            return WeakSetitem(obj, key, max_args, finalize, on_ref_error)
+        return WeakMethod(cb, max_args, args, kwargs, finalize, on_ref_error)
 
     if isinstance(cb, (MethodWrapperType, BuiltinMethodType)):
         if kwargs:  # pragma: no cover
             raise NotImplementedError(
                 "MethodWrapperTypes do not support keyword arguments"
             )
 
         if cb is setattr:
             try:
                 obj, attr = args[:2]
             except IndexError as e:  # pragma: no cover
                 raise TypeError(
                     "setattr requires two arguments, an object and an attribute name."
                 ) from e
-            return _WeakSetattr(obj, attr, max_args, finalize, on_ref_error)
-        return _WeakBuiltin(cb, max_args, args, finalize, on_ref_error)
+            return WeakSetattr(obj, attr, max_args, finalize, on_ref_error)
+        return WeakBuiltin(cb, max_args, args, finalize, on_ref_error)
 
     if _is_toolz_curry(cb):
         cb_partial = getattr(cb, "_partial", None)
         if cb_partial is None:  # pragma: no cover
             raise TypeError(
                 "toolz.curry object found without a '_partial' attribute. This "
                 "version of toolz is not supported. Please open an issue at psygnal."
@@ -157,15 +157,15 @@
             *args,
             max_args=max_args,
             finalize=finalize,
             on_ref_error=on_ref_error,
         )
 
     if callable(cb):
-        return _WeakFunction(cb, max_args, args, kwargs, finalize, on_ref_error)
+        return WeakFunction(cb, max_args, args, kwargs, finalize, on_ref_error)
 
     raise TypeError(f"unsupported type {type(cb)}")  # pragma: no cover
 
 
 class WeakCallback(Generic[_R]):
     """Abstract Base Class for weakly-referenced callbacks.
 
@@ -184,14 +184,17 @@
     def __init__(
         self,
         obj: Any,
         max_args: int | None = None,
         on_ref_error: RefErrorChoice = "warn",
     ) -> None:
         self._key: str = WeakCallback.object_key(obj)
+        self._obj_module: str = getattr(obj, "__module__", None) or ""
+        self._obj_qualname: str = getattr(obj, "__qualname__", "")
+        self._object_repr: str = WeakCallback.object_repr(obj)
         self._max_args: int | None = max_args
         self._alive: bool = True
         self._on_ref_error: RefErrorChoice = on_ref_error
 
     def cb(self, args: tuple[Any, ...] = ()) -> None:
         """Call the callback with `args`. Args will be spread when calling the func."""
         raise NotImplementedError()
@@ -232,14 +235,17 @@
                 )
 
             def _strong_ref() -> _T:
                 return obj
 
             return _strong_ref
 
+    def slot_repr(self) -> str:
+        return f"{self._obj_module}.{self._obj_qualname}"
+
     @staticmethod
     def object_key(obj: Any) -> str:
         """Return a unique key for an object.
 
         This includes information about the object's type, module, and id. It has
         considerations for bound methods (which would otherwise have a different id
         for each instance).
@@ -254,28 +260,50 @@
             obj_name = f"{type_name}.{method_name}"
         else:
             obj_id = id(obj)
             module = getattr(obj, "__module__", None) or ""
             obj_name = getattr(obj, "__name__", None) or ""
         return f"{module}:{obj_name}@{hex(obj_id)}"
 
+    @staticmethod
+    def object_repr(obj: Any) -> str:
+        """Return a human-readable repr for obj."""
+        module = getattr(obj, "__module__", "")
+        if hasattr(obj, "__self__"):
+            # bound method ... don't take the id of the bound method itself.
+            owner_cls = type(obj.__self__)
+            module = getattr(owner_cls, "__module__", None) or ""
+            method_name = getattr(obj, "__name__", None) or ""
+            if module == "builtins":
+                return method_name
+            type_qname = getattr(owner_cls, "__qualname__", "")
+            return f"{module}.{type_qname}.{method_name}"
+        elif getattr(obj, "__qualname__", ""):
+            return f"{module}.{obj.__qualname__}"
+        elif getattr(type(obj), "__qualname__", ""):
+            return f"{module}.{type(obj).__qualname__}"
+        return repr(obj)
+
+    def __repr__(self) -> str:
+        return f"<{self.__class__.__name__} on {self._object_repr}>"
+
 
 def _kill_and_finalize(
     wcb: WeakCallback, finalize: Callable[[WeakCallback], Any]
 ) -> Callable[[weakref.ReferenceType], None]:
     def _cb(_: weakref.ReferenceType) -> None:
         if wcb._alive:
             wcb._alive = False
             finalize(wcb)
 
     return _cb
 
 
 @mypyc_attr(serializable=True)
-class _StrongFunction(WeakCallback):
+class StrongFunction(WeakCallback):
     """Wrapper around a strong function reference."""
 
     def __init__(
         self,
         obj: Callable,
         max_args: int | None = None,
         args: tuple[Any, ...] = (),
@@ -283,14 +311,17 @@
         on_ref_error: RefErrorChoice = "warn",
     ) -> None:
         super().__init__(obj, max_args, on_ref_error)
         self._f = obj
         self._args = args
         self._kwargs = kwargs or {}
 
+        if args:
+            self._object_repr = f"{self._object_repr}{(*args,)!r}".replace(")", " ...)")
+
     def cb(self, args: tuple[Any, ...] = ()) -> None:
         if self._max_args is not None:
             args = args[: self._max_args]
         self._f(*self._args, *args, **self._kwargs)
 
     def dereference(self) -> Callable:
         if self._args or self._kwargs:
@@ -302,15 +333,15 @@
         return {k: getattr(self, k) for k in atr}
 
     def __setstate__(self, state: dict) -> None:
         for k, v in state.items():
             setattr(self, k, v)
 
 
-class _WeakFunction(WeakCallback):
+class WeakFunction(WeakCallback):
     """Wrapper around a weak function reference."""
 
     def __init__(
         self,
         obj: Callable,
         max_args: int | None = None,
         args: tuple[Any, ...] = (),
@@ -319,14 +350,17 @@
         on_ref_error: RefErrorChoice = "warn",
     ) -> None:
         super().__init__(obj, max_args, on_ref_error)
         self._f = self._try_ref(obj, finalize)
         self._args = args
         self._kwargs = kwargs or {}
 
+        if args:
+            self._object_repr = f"{self._object_repr}{(*args,)!r}".replace(")", " ...)")
+
     def cb(self, args: tuple[Any, ...] = ()) -> None:
         f = self._f()
         if f is None:
             raise ReferenceError("weakly-referenced object no longer exists")
         if self._max_args is not None:
             args = args[: self._max_args]
         f(*self._args, *args, **self._kwargs)
@@ -336,15 +370,15 @@
         if f is None:
             return None
         if self._args or self._kwargs:
             return partial(f, *self._args, **self._kwargs)
         return f
 
 
-class _WeakMethod(WeakCallback):
+class WeakMethod(WeakCallback):
     """Wrapper around a method bound to a weakly-referenced object.
 
     Bound methods have a `__self__` attribute that holds a strong reference to the
     object they are bound to and a `__func__` attribute that holds a reference
     to the function that implements the method (on the class level)
 
     When `cb` is called here, it dereferences the two, and calls:
@@ -356,19 +390,26 @@
         obj: MethodType,
         max_args: int | None = None,
         args: tuple[Any, ...] = (),
         kwargs: dict[str, Any] | None = None,
         finalize: Callable | None = None,
         on_ref_error: RefErrorChoice = "warn",
     ) -> None:
-        super().__init__(obj.__self__, max_args, on_ref_error)
+        super().__init__(obj, max_args, on_ref_error)
         self._obj_ref = self._try_ref(obj.__self__, finalize)
         self._func_ref = self._try_ref(obj.__func__, finalize)
         self._args = args
         self._kwargs = kwargs or {}
+        if args:
+            self._object_repr = f"{self._object_repr}{(*args,)!r}".replace(")", " ...)")
+
+    def slot_repr(self) -> str:
+        obj = self._obj_ref()
+        func_name = getattr(self._func_ref(), "__name__", "<method>")
+        return f"{self._obj_module}.{obj.__class__.__qualname__}.{func_name}"
 
     def cb(self, args: tuple[Any, ...] = ()) -> None:
         obj = self._obj_ref()
         func = self._func_ref()
         if obj is None or func is None:
             raise ReferenceError("weakly-referenced object no longer exists")
 
@@ -383,15 +424,15 @@
             return None
         method = func.__get__(obj)
         if self._args or self._kwargs:
             return partial(method, *self._args, **self._kwargs)
         return method
 
 
-class _WeakBuiltin(WeakCallback):
+class WeakBuiltin(WeakCallback):
     """Wrapper around a c-based method on a weakly-referenced object.
 
     Builtin/extension methods do have a `__self__` attribute (the object to which they
     are bound), but don't have a __func__ attribute, so we need to store the name of the
     method and look it up on the object when the callback is called.
 
     When `cb` is called here, it dereferences the object, and calls:
@@ -406,43 +447,54 @@
         finalize: Callable | None = None,
         on_ref_error: RefErrorChoice = "warn",
     ) -> None:
         super().__init__(obj, max_args, on_ref_error)
         self._obj_ref = self._try_ref(obj.__self__, finalize)
         self._func_name = obj.__name__
         self._args = args
+        if args:
+            self._object_repr = f"{self._object_repr}{(*args,)!r}".replace(")", " ...)")
+
+    def slot_repr(self) -> str:
+        obj = self._obj_ref()
+        return f"{obj.__class__.__qualname__}.{self._func_name}"
 
     def cb(self, args: tuple[Any, ...] = ()) -> None:
         func = getattr(self._obj_ref(), self._func_name, None)
         if func is None:
             raise ReferenceError("weakly-referenced object no longer exists")
         if self._max_args is None:
             func(*self._args, *args)
         else:
             func(*self._args, *args[: self._max_args])
 
     def dereference(self) -> MethodWrapperType | BuiltinMethodType | None:
         return getattr(self._obj_ref(), self._func_name, None)
 
 
-class _WeakSetattr(WeakCallback):
+class WeakSetattr(WeakCallback):
     """Caller to set an attribute on a weakly-referenced object."""
 
     def __init__(
         self,
         obj: object,
         attr: str,
         max_args: int | None = None,
         finalize: Callable | None = None,
         on_ref_error: RefErrorChoice = "warn",
     ) -> None:
         super().__init__(obj, max_args, on_ref_error)
         self._key += f".__setattr__({attr!r})"
         self._obj_ref = self._try_ref(obj, finalize)
         self._attr = attr
+        self._object_repr += f".__setattr__({attr!r}, ...)"
+
+    def slot_repr(self) -> str:
+        obj = self._obj_ref()
+        return f"setattr({obj.__class__.__qualname__}, {self._attr!r}, ...)"
 
     def cb(self, args: tuple[Any, ...] = ()) -> None:
         obj = self._obj_ref()
         if obj is None:
             raise ReferenceError("weakly-referenced object no longer exists")
         if self._max_args is not None:
             args = args[: self._max_args]
@@ -454,29 +506,34 @@
 
 
 class SupportsSetitem(Protocol):
     def __setitem__(self, key: Any, value: Any) -> None:
         ...
 
 
-class _WeakSetitem(WeakCallback):
+class WeakSetitem(WeakCallback):
     """Caller to call __setitem__ on a weakly-referenced object."""
 
     def __init__(
         self,
         obj: SupportsSetitem,
         key: Any,
         max_args: int | None = None,
         finalize: Callable | None = None,
         on_ref_error: RefErrorChoice = "warn",
     ) -> None:
         super().__init__(obj, max_args, on_ref_error)
         self._key += f".__setitem__({key!r})"
         self._obj_ref = self._try_ref(obj, finalize)
         self._itemkey = key
+        self._object_repr += f".__setitem__({key!r}, ...)"
+
+    def slot_repr(self) -> str:
+        obj = self._obj_ref()
+        return f"{obj.__class__.__qualname__}.__setitem__({self._itemkey!r}, ...)"
 
     def cb(self, args: tuple[Any, ...] = ()) -> None:
         obj = self._obj_ref()
         if obj is None:
             raise ReferenceError("weakly-referenced object no longer exists")
         if self._max_args is not None:
             args = args[: self._max_args]
```

### Comparing `psygnal-0.9.4/src/psygnal/qt.py` & `psygnal-0.9.5/src/psygnal/qt.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/src/psygnal/utils.py` & `psygnal-0.9.5/src/psygnal/utils.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/src/psygnal/_pyinstaller_util/hook-psygnal.py` & `psygnal-0.9.5/src/psygnal/_pyinstaller_util/hook-psygnal.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/src/psygnal/containers/__init__.py` & `psygnal-0.9.5/src/psygnal/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/src/psygnal/containers/_evented_dict.py` & `psygnal-0.9.5/src/psygnal/containers/_evented_dict.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/src/psygnal/containers/_evented_list.py` & `psygnal-0.9.5/src/psygnal/containers/_evented_list.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/src/psygnal/containers/_evented_proxy.py` & `psygnal-0.9.5/src/psygnal/containers/_evented_proxy.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/src/psygnal/containers/_evented_set.py` & `psygnal-0.9.5/src/psygnal/containers/_evented_set.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/src/psygnal/containers/_selectable_evented_list.py` & `psygnal-0.9.5/src/psygnal/containers/_selectable_evented_list.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/src/psygnal/containers/_selection.py` & `psygnal-0.9.5/src/psygnal/containers/_selection.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/tests/test_bench.py` & `psygnal-0.9.5/tests/test_bench.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/tests/test_dataclass_utils.py` & `psygnal-0.9.5/tests/test_dataclass_utils.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/tests/test_evented_decorator.py` & `psygnal-0.9.5/tests/test_evented_decorator.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/tests/test_evented_model.py` & `psygnal-0.9.5/tests/test_evented_model.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/tests/test_group.py` & `psygnal-0.9.5/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/tests/test_group_descriptor.py` & `psygnal-0.9.5/tests/test_group_descriptor.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/tests/test_psygnal.py` & `psygnal-0.9.5/tests/test_psygnal.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/tests/test_pyinstaller_hook.py` & `psygnal-0.9.5/tests/test_pyinstaller_hook.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/tests/test_qt_compat.py` & `psygnal-0.9.5/tests/test_qt_compat.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/tests/test_throttler.py` & `psygnal-0.9.5/tests/test_throttler.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/tests/test_utils.py` & `psygnal-0.9.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/tests/test_weak_callable.py` & `psygnal-0.9.5/tests/test_weak_callable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import gc
 from functools import partial
+from typing import Any
 from unittest.mock import Mock
 from weakref import ref
 
 import pytest
 import toolz
 
 from psygnal._weak_callback import WeakCallback, weak_callback
@@ -174,18 +175,42 @@
     dp = cb.dereference()
 
     assert dp.func is p.func
     assert dp.args == p.args
     assert dp.keywords == p.keywords
 
 
-def test_queued_callbacks():
+def test_queued_callbacks() -> None:
     from psygnal._queue import QueuedCallback
 
     def func(x):
         return x
 
     cb = weak_callback(func)
     qcb = QueuedCallback(cb, thread="current")
 
     assert qcb.dereference() is func
     assert qcb(1) == 1
+
+
+def test_cb_raises() -> None:
+    from psygnal import EmitLoopError
+
+    m = str(EmitLoopError(weak_callback(print), (1,), RuntimeError("test")))
+    assert "an error occurred in callback 'module.print'" in m
+    m = str(EmitLoopError(print, (1,), RuntimeError("test")))
+    assert " an error occurred in callback 'print'" in m
+
+    class T:
+        x = 1
+
+        def __setitem__(self, *_: Any) -> Any:
+            pass
+
+    t = T()
+    cb = weak_callback(setattr, t, "x")
+    m = str(EmitLoopError(cb, (2,), RuntimeError("test")))
+    assert 'an error occurred in callback "setattr' in m
+
+    cb = weak_callback(t.__setitem__, "x")
+    m = str(EmitLoopError(cb, (2,), RuntimeError("test")))
+    assert ".T.__setitem__" in m
```

### Comparing `psygnal-0.9.4/tests/containers/test_evented_dict.py` & `psygnal-0.9.5/tests/containers/test_evented_dict.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/tests/containers/test_evented_list.py` & `psygnal-0.9.5/tests/containers/test_evented_list.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/tests/containers/test_evented_proxy.py` & `psygnal-0.9.5/tests/containers/test_evented_proxy.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/tests/containers/test_evented_set.py` & `psygnal-0.9.5/tests/containers/test_evented_set.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/tests/containers/test_selectable_evented_list.py` & `psygnal-0.9.5/tests/containers/test_selectable_evented_list.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/tests/containers/test_selection.py` & `psygnal-0.9.5/tests/containers/test_selection.py`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/.gitignore` & `psygnal-0.9.5/.gitignore`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/LICENSE` & `psygnal-0.9.5/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-
-BSD License
-
 Copyright (c) 2021, Talley Lambert
-All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `psygnal-0.9.4/README.md` & `psygnal-0.9.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # psygnal
 
 [![License](https://img.shields.io/pypi/l/psygnal.svg?color=green)](https://github.com/pyapp-kit/psygnal/raw/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/psygnal.svg?color=green)](https://pypi.org/project/psygnal)
-![Conda](https://img.shields.io/conda/v/conda-forge/psygnal)
+[![Conda](https://img.shields.io/conda/v/conda-forge/psygnal)](https://github.com/conda-forge/psygnal-feedstock)
 [![Python Version](https://img.shields.io/pypi/pyversions/psygnal.svg?color=green)](https://python.org)
 [![CI](https://github.com/pyapp-kit/psygnal/actions/workflows/test.yml/badge.svg)](https://github.com/pyapp-kit/psygnal/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/pyapp-kit/psygnal/branch/main/graph/badge.svg?token=qGnz9GXpEb)](https://codecov.io/gh/pyapp-kit/psygnal)
 [![Documentation Status](https://readthedocs.org/projects/psygnal/badge/?version=latest)](https://psygnal.readthedocs.io/en/latest/?badge=latest)
 [![Benchmarks](https://img.shields.io/badge/⏱-codspeed-%23FF7B53)](https://codspeed.io/pyapp-kit/psygnal)
 
 Psygnal (pronounced "signal") is a pure python implementation of the [observer
```

### Comparing `psygnal-0.9.4/pyproject.toml` & `psygnal-0.9.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `psygnal-0.9.4/PKG-INFO` & `psygnal-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psygnal
-Version: 0.9.4
+Version: 0.9.5
 Summary: Fast python callback/event system modeled after Qt Signals
 Project-URL: homepage, https://github.com/pyapp-kit/psygnal
 Project-URL: repository, https://github.com/pyapp-kit/psygnal
 Project-URL: documentation, https://psygnal.readthedocs.io
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
@@ -70,15 +70,15 @@
 Requires-Dist: qtpy; extra == 'testqt'
 Description-Content-Type: text/markdown
 
 # psygnal
 
 [![License](https://img.shields.io/pypi/l/psygnal.svg?color=green)](https://github.com/pyapp-kit/psygnal/raw/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/psygnal.svg?color=green)](https://pypi.org/project/psygnal)
-![Conda](https://img.shields.io/conda/v/conda-forge/psygnal)
+[![Conda](https://img.shields.io/conda/v/conda-forge/psygnal)](https://github.com/conda-forge/psygnal-feedstock)
 [![Python Version](https://img.shields.io/pypi/pyversions/psygnal.svg?color=green)](https://python.org)
 [![CI](https://github.com/pyapp-kit/psygnal/actions/workflows/test.yml/badge.svg)](https://github.com/pyapp-kit/psygnal/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/pyapp-kit/psygnal/branch/main/graph/badge.svg?token=qGnz9GXpEb)](https://codecov.io/gh/pyapp-kit/psygnal)
 [![Documentation Status](https://readthedocs.org/projects/psygnal/badge/?version=latest)](https://psygnal.readthedocs.io/en/latest/?badge=latest)
 [![Benchmarks](https://img.shields.io/badge/⏱-codspeed-%23FF7B53)](https://codspeed.io/pyapp-kit/psygnal)
 
 Psygnal (pronounced "signal") is a pure python implementation of the [observer
```

