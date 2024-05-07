# Comparing `tmp/msgpack-1.0.7.tar.gz` & `tmp/msgpack-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgpack-1.0.7.tar", last modified: Thu Sep 28 13:20:26 2023, max compression
+gzip compressed data, was "msgpack-1.0.8.tar", last modified: Sat Mar  2 01:19:03 2024, max compression
```

## Comparing `msgpack-1.0.7.tar` & `msgpack-1.0.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-09-28 13:20:26.697617 msgpack-1.0.7/
--rw-r--r--   0 inada-n    (502) staff       (20)      614 2014-02-12 16:44:57.000000 msgpack-1.0.7/COPYING
--rw-r--r--   0 inada-n    (502) staff       (20)      125 2019-12-12 09:21:06.000000 msgpack-1.0.7/MANIFEST.in
--rw-r--r--   0 inada-n    (502) staff       (20)     9074 2023-09-28 13:20:26.697386 msgpack-1.0.7/PKG-INFO
--rw-r--r--   0 inada-n    (502) staff       (20)     7737 2023-09-13 22:16:50.000000 msgpack-1.0.7/README.md
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-09-28 13:20:26.694246 msgpack-1.0.7/msgpack/
--rw-r--r--   0 inada-n    (502) staff       (20)     1077 2023-09-28 13:20:17.000000 msgpack-1.0.7/msgpack/__init__.py
--rw-r--r--   0 inada-n    (502) staff       (20)  1024996 2023-09-28 13:20:26.000000 msgpack-1.0.7/msgpack/_cmsgpack.cpp
--rw-r--r--   0 inada-n    (502) staff       (20)      335 2019-12-12 09:11:24.000000 msgpack-1.0.7/msgpack/_cmsgpack.pyx
--rw-r--r--   0 inada-n    (502) staff       (20)    14607 2023-09-05 10:30:14.000000 msgpack-1.0.7/msgpack/_packer.pyx
--rw-r--r--   0 inada-n    (502) staff       (20)    18888 2023-09-05 10:30:14.000000 msgpack-1.0.7/msgpack/_unpacker.pyx
--rw-r--r--   0 inada-n    (502) staff       (20)      220 2019-12-03 06:50:41.000000 msgpack-1.0.7/msgpack/buff_converter.h
--rw-r--r--   0 inada-n    (502) staff       (20)     1081 2019-01-25 10:46:58.000000 msgpack-1.0.7/msgpack/exceptions.py
--rw-r--r--   0 inada-n    (502) staff       (20)     5629 2023-09-05 10:30:14.000000 msgpack-1.0.7/msgpack/ext.py
--rw-r--r--   0 inada-n    (502) staff       (20)    33175 2023-09-05 10:30:14.000000 msgpack-1.0.7/msgpack/fallback.py
--rw-r--r--   0 inada-n    (502) staff       (20)     2072 2023-09-28 06:34:12.000000 msgpack-1.0.7/msgpack/pack.h
--rw-r--r--   0 inada-n    (502) staff       (20)    21775 2022-05-23 05:55:10.000000 msgpack-1.0.7/msgpack/pack_template.h
--rw-r--r--   0 inada-n    (502) staff       (20)     6452 2023-03-08 13:19:00.000000 msgpack-1.0.7/msgpack/sysdep.h
--rw-r--r--   0 inada-n    (502) staff       (20)    10976 2021-11-16 05:48:37.000000 msgpack-1.0.7/msgpack/unpack.h
--rw-r--r--   0 inada-n    (502) staff       (20)     2366 2014-02-12 16:44:57.000000 msgpack-1.0.7/msgpack/unpack_define.h
--rw-r--r--   0 inada-n    (502) staff       (20)    14846 2022-05-23 05:55:10.000000 msgpack-1.0.7/msgpack/unpack_template.h
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-09-28 13:20:26.694788 msgpack-1.0.7/msgpack.egg-info/
--rw-r--r--   0 inada-n    (502) staff       (20)     9074 2023-09-28 13:20:26.000000 msgpack-1.0.7/msgpack.egg-info/PKG-INFO
--rw-r--r--   0 inada-n    (502) staff       (20)      840 2023-09-28 13:20:26.000000 msgpack-1.0.7/msgpack.egg-info/SOURCES.txt
--rw-r--r--   0 inada-n    (502) staff       (20)        1 2023-09-28 13:20:26.000000 msgpack-1.0.7/msgpack.egg-info/dependency_links.txt
--rw-r--r--   0 inada-n    (502) staff       (20)        8 2023-09-28 13:20:26.000000 msgpack-1.0.7/msgpack.egg-info/top_level.txt
--rw-r--r--   0 inada-n    (502) staff       (20)     1832 2023-09-13 20:09:22.000000 msgpack-1.0.7/pyproject.toml
--rw-r--r--   0 inada-n    (502) staff       (20)       38 2023-09-28 13:20:26.697657 msgpack-1.0.7/setup.cfg
--rw-r--r--   0 inada-n    (502) staff       (20)     1737 2023-09-28 06:34:12.000000 msgpack-1.0.7/setup.py
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-09-28 13:20:26.697129 msgpack-1.0.7/test/
--rw-r--r--   0 inada-n    (502) staff       (20)      730 2023-09-05 10:30:14.000000 msgpack-1.0.7/test/test_buffer.py
--rw-r--r--   0 inada-n    (502) staff       (20)     2953 2023-07-20 17:41:11.000000 msgpack-1.0.7/test/test_case.py
--rw-r--r--   0 inada-n    (502) staff       (20)     1699 2023-07-20 17:41:11.000000 msgpack-1.0.7/test/test_except.py
--rw-r--r--   0 inada-n    (502) staff       (20)     2618 2023-07-20 17:41:11.000000 msgpack-1.0.7/test/test_extension.py
--rw-r--r--   0 inada-n    (502) staff       (20)     2303 2023-07-20 17:41:11.000000 msgpack-1.0.7/test/test_format.py
--rw-r--r--   0 inada-n    (502) staff       (20)     3823 2023-07-20 17:41:11.000000 msgpack-1.0.7/test/test_limits.py
--rw-r--r--   0 inada-n    (502) staff       (20)     2771 2023-09-05 10:30:14.000000 msgpack-1.0.7/test/test_memoryview.py
--rw-r--r--   0 inada-n    (502) staff       (20)     2718 2023-07-20 17:41:11.000000 msgpack-1.0.7/test/test_newspec.py
--rw-r--r--   0 inada-n    (502) staff       (20)     2102 2023-09-05 10:30:14.000000 msgpack-1.0.7/test/test_obj.py
--rw-r--r--   0 inada-n    (502) staff       (20)     4318 2023-09-05 10:30:14.000000 msgpack-1.0.7/test/test_pack.py
--rw-r--r--   0 inada-n    (502) staff       (20)     1856 2019-12-12 09:11:24.000000 msgpack-1.0.7/test/test_read_size.py
--rw-r--r--   0 inada-n    (502) staff       (20)     1141 2023-09-05 10:30:14.000000 msgpack-1.0.7/test/test_seq.py
--rw-r--r--   0 inada-n    (502) staff       (20)     4119 2023-07-20 17:41:11.000000 msgpack-1.0.7/test/test_sequnpack.py
--rw-r--r--   0 inada-n    (502) staff       (20)     1727 2023-07-20 17:41:11.000000 msgpack-1.0.7/test/test_stricttype.py
--rw-r--r--   0 inada-n    (502) staff       (20)      392 2023-09-05 10:30:14.000000 msgpack-1.0.7/test/test_subtype.py
--rw-r--r--   0 inada-n    (502) staff       (20)     4992 2023-09-05 10:30:14.000000 msgpack-1.0.7/test/test_timestamp.py
--rw-r--r--   0 inada-n    (502) staff       (20)     2496 2023-07-20 17:41:11.000000 msgpack-1.0.7/test/test_unpack.py
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2024-03-02 01:19:03.808492 msgpack-1.0.8/
+-rw-r--r--   0 inada-n    (502) staff       (20)      614 2014-02-12 16:44:57.000000 msgpack-1.0.8/COPYING
+-rw-r--r--   0 inada-n    (502) staff       (20)      125 2023-12-20 05:12:51.000000 msgpack-1.0.8/MANIFEST.in
+-rw-r--r--   0 inada-n    (502) staff       (20)     9074 2024-03-02 01:19:03.808167 msgpack-1.0.8/PKG-INFO
+-rw-r--r--   0 inada-n    (502) staff       (20)     7737 2023-09-13 22:16:50.000000 msgpack-1.0.8/README.md
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2024-03-02 01:19:03.800618 msgpack-1.0.8/msgpack/
+-rw-r--r--   0 inada-n    (502) staff       (20)     1077 2024-03-02 01:18:40.000000 msgpack-1.0.8/msgpack/__init__.py
+-rw-r--r--   0 inada-n    (502) staff       (20)  1021863 2024-03-02 01:19:03.000000 msgpack-1.0.8/msgpack/_cmsgpack.cpp
+-rw-r--r--   0 inada-n    (502) staff       (20)      335 2019-12-12 09:11:24.000000 msgpack-1.0.8/msgpack/_cmsgpack.pyx
+-rw-r--r--   0 inada-n    (502) staff       (20)    14607 2023-09-05 10:30:14.000000 msgpack-1.0.8/msgpack/_packer.pyx
+-rw-r--r--   0 inada-n    (502) staff       (20)    18888 2023-09-05 10:30:14.000000 msgpack-1.0.8/msgpack/_unpacker.pyx
+-rw-r--r--   0 inada-n    (502) staff       (20)      220 2019-12-03 06:50:41.000000 msgpack-1.0.8/msgpack/buff_converter.h
+-rw-r--r--   0 inada-n    (502) staff       (20)     1081 2019-01-25 10:46:58.000000 msgpack-1.0.8/msgpack/exceptions.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     5629 2023-09-05 10:30:14.000000 msgpack-1.0.8/msgpack/ext.py
+-rw-r--r--   0 inada-n    (502) staff       (20)    33175 2023-09-05 10:30:14.000000 msgpack-1.0.8/msgpack/fallback.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     2072 2023-09-28 06:34:12.000000 msgpack-1.0.8/msgpack/pack.h
+-rw-r--r--   0 inada-n    (502) staff       (20)    21775 2022-05-23 05:55:10.000000 msgpack-1.0.8/msgpack/pack_template.h
+-rw-r--r--   0 inada-n    (502) staff       (20)     6452 2023-03-08 13:19:00.000000 msgpack-1.0.8/msgpack/sysdep.h
+-rw-r--r--   0 inada-n    (502) staff       (20)    10976 2021-11-16 05:48:37.000000 msgpack-1.0.8/msgpack/unpack.h
+-rw-r--r--   0 inada-n    (502) staff       (20)     2366 2014-02-12 16:44:57.000000 msgpack-1.0.8/msgpack/unpack_define.h
+-rw-r--r--   0 inada-n    (502) staff       (20)    14846 2022-05-23 05:55:10.000000 msgpack-1.0.8/msgpack/unpack_template.h
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2024-03-02 01:19:03.807696 msgpack-1.0.8/msgpack.egg-info/
+-rw-r--r--   0 inada-n    (502) staff       (20)     9074 2024-03-02 01:19:03.000000 msgpack-1.0.8/msgpack.egg-info/PKG-INFO
+-rw-r--r--   0 inada-n    (502) staff       (20)      840 2024-03-02 01:19:03.000000 msgpack-1.0.8/msgpack.egg-info/SOURCES.txt
+-rw-r--r--   0 inada-n    (502) staff       (20)        1 2024-03-02 01:19:03.000000 msgpack-1.0.8/msgpack.egg-info/dependency_links.txt
+-rw-r--r--   0 inada-n    (502) staff       (20)        8 2024-03-02 01:19:03.000000 msgpack-1.0.8/msgpack.egg-info/top_level.txt
+-rw-r--r--   0 inada-n    (502) staff       (20)     1923 2024-03-02 01:18:40.000000 msgpack-1.0.8/pyproject.toml
+-rw-r--r--   0 inada-n    (502) staff       (20)       38 2024-03-02 01:19:03.808714 msgpack-1.0.8/setup.cfg
+-rw-r--r--   0 inada-n    (502) staff       (20)     1737 2023-09-28 06:34:12.000000 msgpack-1.0.8/setup.py
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2024-03-02 01:19:03.807038 msgpack-1.0.8/test/
+-rw-r--r--   0 inada-n    (502) staff       (20)      730 2023-09-05 10:30:14.000000 msgpack-1.0.8/test/test_buffer.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     2953 2023-07-20 17:41:11.000000 msgpack-1.0.8/test/test_case.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     1699 2023-07-20 17:41:11.000000 msgpack-1.0.8/test/test_except.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     2618 2023-07-20 17:41:11.000000 msgpack-1.0.8/test/test_extension.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     2303 2023-07-20 17:41:11.000000 msgpack-1.0.8/test/test_format.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     3823 2023-07-20 17:41:11.000000 msgpack-1.0.8/test/test_limits.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     2771 2023-09-05 10:30:14.000000 msgpack-1.0.8/test/test_memoryview.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     2718 2023-07-20 17:41:11.000000 msgpack-1.0.8/test/test_newspec.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     2102 2023-09-05 10:30:14.000000 msgpack-1.0.8/test/test_obj.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     4318 2023-09-05 10:30:14.000000 msgpack-1.0.8/test/test_pack.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     1856 2019-12-12 09:11:24.000000 msgpack-1.0.8/test/test_read_size.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     1141 2023-09-05 10:30:14.000000 msgpack-1.0.8/test/test_seq.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     4119 2023-07-20 17:41:11.000000 msgpack-1.0.8/test/test_sequnpack.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     1727 2023-07-20 17:41:11.000000 msgpack-1.0.8/test/test_stricttype.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      392 2023-09-05 10:30:14.000000 msgpack-1.0.8/test/test_subtype.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     4992 2023-09-05 10:30:14.000000 msgpack-1.0.8/test/test_timestamp.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     2496 2023-07-20 17:41:11.000000 msgpack-1.0.8/test/test_unpack.py
```

### Comparing `msgpack-1.0.7/COPYING` & `msgpack-1.0.8/COPYING`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/PKG-INFO` & `msgpack-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgpack
-Version: 1.0.7
+Version: 1.0.8
 Summary: MessagePack serializer
 Author-email: Inada Naoki <songofacandy@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://msgpack.org/
 Project-URL: Documentation, https://msgpack-python.readthedocs.io/
 Project-URL: Repository, https://github.com/msgpack/msgpack-python/
 Project-URL: Tracker, https://github.com/msgpack/msgpack-python/issues
```

### Comparing `msgpack-1.0.7/README.md` & `msgpack-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/msgpack/__init__.py` & `msgpack-1.0.8/msgpack/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .exceptions import *
 from .ext import ExtType, Timestamp
 
 import os
 
 
-version = (1, 0, 7)
-__version__ = "1.0.7"
+version = (1, 0, 8)
+__version__ = "1.0.8"
 
 
 if os.environ.get("MSGPACK_PUREPYTHON"):
     from .fallback import Packer, unpackb, Unpacker
 else:
     try:
         from ._cmsgpack import Packer, unpackb, Unpacker
```

### Comparing `msgpack-1.0.7/msgpack/_cmsgpack.cpp` & `msgpack-1.0.8/msgpack/_cmsgpack.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.2 */
+/* Generated by Cython 3.0.8 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
   #ifndef Py_LIMITED_API
     #if CYTHON_LIMITED_API+0 > 0x03030000
@@ -32,23 +32,23 @@
     #endif
     
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#if CYTHON_LIMITED_API
+#if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_2" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030002F0
+#define CYTHON_HEX_VERSION 0x030008F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -254,15 +254,15 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
-#elif defined(PY_NOGIL)
+#elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
@@ -597,25 +597,28 @@
 #if CYTHON_COMPILING_IN_LIMITED_API
     static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *exception_table = NULL;
         PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
-        PyObject *version_info; // borrowed
+        #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
+        PyObject *version_info;
         PyObject *py_minor_version = NULL;
+        #endif
         long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
-        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        minor_version = 11;
         #else
         if (!(version_info = PySys_GetObject("version_info"))) goto end;
         if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
         minor_version = PyLong_AsLong(py_minor_version);
+        Py_DECREF(py_minor_version);
         if (minor_version == -1 && PyErr_Occurred()) goto end;
         #endif
         if (!(types_module = PyImport_ImportModule("types"))) goto end;
         if (!(code_type = PyObject_GetAttrString(types_module, "CodeType"))) goto end;
         if (minor_version <= 7) {
             (void)p;
             result = PyObject_CallFunction(code_type, "iiiiiOOOOOOiOO", a, k, l, s, f, code,
@@ -628,15 +631,14 @@
             result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOOiOO", a,p, k, l, s, f, code,
                           c, n, v, fn, name, name, fline, lnos, exception_table, fv, cell);
         }
     end:
         Py_XDECREF(code_type);
         Py_XDECREF(exception_table);
         Py_XDECREF(types_module);
-        Py_XDECREF(py_minor_version);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
         return result;
     }
     #ifndef CO_OPTIMIZED
     #define CO_OPTIMIZED 0x0001
@@ -661,15 +663,15 @@
     #endif
 #elif PY_VERSION_HEX >= 0x030B0000
   static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
     PyCodeObject *result;
-    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
     if (!empty_bytes) return NULL;
     result =
       #if PY_VERSION_HEX >= 0x030C0000
         PyUnstable_Code_NewWithPosOnlyArgs
       #else
         PyCode_NewWithPosOnlyArgs
       #endif
@@ -772,14 +774,39 @@
                                             size_t nargsf, PyObject *kwnames);
   #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  ((size_t)1 << (8 * sizeof(size_t) - 1))
   #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(((size_t)(n)) & ~__Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET))
 #else
   #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  0
   #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(n))
 #endif
+#if PY_MAJOR_VERSION >= 0x030900B1
+#define __Pyx_PyCFunction_CheckExact(func)  PyCFunction_CheckExact(func)
+#else
+#define __Pyx_PyCFunction_CheckExact(func)  PyCFunction_Check(func)
+#endif
+#define __Pyx_CyOrPyCFunction_Check(func)  PyCFunction_Check(func)
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_CyOrPyCFunction_GET_FUNCTION(func)  (((PyCFunctionObject*)(func))->m_ml->ml_meth)
+#elif !CYTHON_COMPILING_IN_LIMITED_API
+#define __Pyx_CyOrPyCFunction_GET_FUNCTION(func)  PyCFunction_GET_FUNCTION(func)
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_CyOrPyCFunction_GET_FLAGS(func)  (((PyCFunctionObject*)(func))->m_ml->ml_flags)
+static CYTHON_INLINE PyObject* __Pyx_CyOrPyCFunction_GET_SELF(PyObject *func) {
+    return (__Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_STATIC) ? NULL : ((PyCFunctionObject*)func)->m_self;
+}
+#endif
+static CYTHON_INLINE int __Pyx__IsSameCFunction(PyObject *func, void *cfunc) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+    return PyCFunction_Check(func) && PyCFunction_GetFunction(func) == (PyCFunction) cfunc;
+#else
+    return PyCFunction_Check(func) && PyCFunction_GET_FUNCTION(func) == (PyCFunction) cfunc;
+#endif
+}
+#define __Pyx_IsSameCFunction(func, cfunc)   __Pyx__IsSameCFunction(func, cfunc)
 #if __PYX_LIMITED_VERSION_HEX < 0x030900B1
   #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  ((void)m, PyType_FromSpecWithBases(s, b))
   typedef PyObject *(*__Pyx_PyCMethod)(PyObject *, PyTypeObject *, PyObject *const *, size_t, PyObject *);
 #else
   #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  PyType_FromModuleAndSpec(m, s, b)
   #define __Pyx_PyCMethod  PyCMethod
 #endif
@@ -798,14 +825,16 @@
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_PyThreadState_Current PyThreadState_Get()
 #elif !CYTHON_FAST_THREAD_STATE
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
+#elif PY_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyThreadState_Current PyThreadState_GetUnchecked()
 #elif PY_VERSION_HEX >= 0x03060000
   #define __Pyx_PyThreadState_Current _PyThreadState_UncheckedGet()
 #elif PY_VERSION_HEX >= 0x03000000
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #else
   #define __Pyx_PyThreadState_Current _PyThreadState_Current
 #endif
@@ -873,27 +902,27 @@
     #else
         static CYTHON_INLINE int PyGILState_Check(void) {
             PyThreadState * tstate = _PyThreadState_Current;
             return tstate && (tstate == PyGILState_GetThisThreadState());
         }
     #endif
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030d0000 || defined(_PyDict_NewPresized)
 #define __Pyx_PyDict_NewPresized(n)  ((n <= 8) ? PyDict_New() : _PyDict_NewPresized(n))
 #else
 #define __Pyx_PyDict_NewPresized(n)  PyDict_New()
 #endif
 #if PY_MAJOR_VERSION >= 3 || CYTHON_FUTURE_DIVISION
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_TrueDivide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceTrueDivide(x,y)
 #else
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_Divide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceDivide(x,y)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && PY_VERSION_HEX < 0x030d0000 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStrWithError(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStr(PyObject *dict, PyObject *name) {
     PyObject *res = __Pyx_PyDict_GetItemStrWithError(dict, name);
     if (res == NULL) PyErr_Clear();
     return res;
 }
 #elif PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
@@ -929,15 +958,15 @@
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyObject_GenericSetAttr((PyObject*)tp, k, v)
 #else
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyDict_SetItem(tp->tp_dict, k, v)
 #endif
 #if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
-    PyTypeObject *type = Py_TYPE(obj);\
+    PyTypeObject *type = Py_TYPE((PyObject*)obj);\
     assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
     PyObject_GC_Del(obj);\
     Py_DECREF(type);\
 }
 #else
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
 #endif
@@ -1073,14 +1102,23 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
+#if PY_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
+#else
+  static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
+      PyObject *module = PyImport_AddModule(name);
+      Py_XINCREF(module);
+      return module;
+  }
+#endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
   #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
   #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
@@ -1226,14 +1264,15 @@
             #define PyDateTime_TIME_GET_TZINFO(o)                 ((((PyDateTime_Time*)o)->hastzinfo) ? ((PyDateTime_Time*)o)->tzinfo : Py_None)
         #endif
         #ifndef PyDateTime_DATE_GET_TZINFO
             #define PyDateTime_DATE_GET_TZINFO(o)                 ((((PyDateTime_DateTime*)o)->hastzinfo) ? ((PyDateTime_DateTime*)o)->tzinfo : Py_None)
         #endif
     #endif
     
+#include <stddef.h>
 #include "pythread.h"
 #include "pack.h"
 #include "buff_converter.h"
 #include <stdlib.h>
 #include <limits.h>
 #include <stdint.h>
 #include "unpack.h"
@@ -1281,17 +1320,18 @@
 #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define __Pyx_sst_abs(value) llabs(value)
 #elif defined (__GNUC__)
     #define __Pyx_sst_abs(value) __builtin_llabs(value)
 #else
     #define __Pyx_sst_abs(value) ((value<0) ? -value : value)
 #endif
+static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s);
 static CYTHON_INLINE const char* __Pyx_PyObject_AsString(PyObject*);
 static CYTHON_INLINE const char* __Pyx_PyObject_AsStringAndSize(PyObject*, Py_ssize_t* length);
-#define __Pyx_PyByteArray_FromString(s) PyByteArray_FromStringAndSize((const char*)s, strlen((const char*)s))
+static CYTHON_INLINE PyObject* __Pyx_PyByteArray_FromString(const char*);
 #define __Pyx_PyByteArray_FromStringAndSize(s, l) PyByteArray_FromStringAndSize((const char*)s, l)
 #define __Pyx_PyBytes_FromString        PyBytes_FromString
 #define __Pyx_PyBytes_FromStringAndSize PyBytes_FromStringAndSize
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char*);
 #if PY_MAJOR_VERSION < 3
     #define __Pyx_PyStr_FromString        __Pyx_PyBytes_FromString
     #define __Pyx_PyStr_FromStringAndSize __Pyx_PyBytes_FromStringAndSize
@@ -1378,15 +1418,15 @@
     #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
-  #else  // Py < 3.12
+  #else
   #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
   #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
   #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
   #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
   #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
@@ -1399,14 +1439,15 @@
   #if PY_VERSION_HEX >= 0x030C00A5
   #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->long_value.ob_digit)
   #else
   #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->ob_digit)
   #endif
 #endif
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
+#include <string.h>
 static int __Pyx_sys_getdefaultencoding_not_ascii;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     PyObject* ascii_chars_u = NULL;
     PyObject* ascii_chars_b = NULL;
     const char* default_encoding_c;
@@ -1449,14 +1490,15 @@
 }
 #endif
 #if __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT && PY_MAJOR_VERSION >= 3
 #define __Pyx_PyUnicode_FromStringAndSize(c_str, size) PyUnicode_DecodeUTF8(c_str, size, NULL)
 #else
 #define __Pyx_PyUnicode_FromStringAndSize(c_str, size) PyUnicode_Decode(c_str, size, __PYX_DEFAULT_STRING_ENCODING, NULL)
 #if __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT
+#include <string.h>
 static char* __PYX_DEFAULT_STRING_ENCODING;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     char* default_encoding_c;
     sys = PyImport_ImportModule("sys");
     if (!sys) goto bad;
@@ -1506,14 +1548,19 @@
   "<stringsource>",
   "msgpack/_cmsgpack.pyx",
   "type.pxd",
   "bool.pxd",
   "complex.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
+/* ForceInitThreads.proto */
+#ifndef __PYX_FORCE_INIT_THREADS
+  #define __PYX_FORCE_INIT_THREADS 0
+#endif
+
 /* #### Code section: numeric_typedefs ### */
 /* #### Code section: complex_type_declarations ### */
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_obj_7msgpack_9_cmsgpack_Packer;
 struct __pyx_obj_7msgpack_9_cmsgpack_Unpacker;
@@ -1888,29 +1935,34 @@
 #else
     #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
 #endif
 #if CYTHON_AVOID_BORROWED_REFS
     #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
     #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
 #else
-    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
-    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
+    #define __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
     #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+    CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
+  #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
-    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
-    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
+  #endif
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
+                                                   to have the same reference counting */
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
     #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
@@ -2172,30 +2224,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_2
-#define __PYX_HAVE_RT_ImportType_proto_3_0_2
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_8
+#define __PYX_HAVE_RT_ImportType_proto_3_0_8
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_2(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_2(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_2 {
-   __Pyx_ImportType_CheckSize_Error_3_0_2 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_2 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_2 = 2
+enum __Pyx_ImportType_CheckSize_3_0_8 {
+   __Pyx_ImportType_CheckSize_Error_3_0_8 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_8 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_8 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_2(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_2 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportDottedModule.proto */
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
@@ -2292,25 +2344,29 @@
     PyObject *func_code;
     PyObject *func_closure;
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
+    size_t defaults_size;
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
+#undef __Pyx_CyOrPyCFunction_Check
 #define __Pyx_CyFunction_Check(obj)  __Pyx_TypeCheck(obj, __pyx_CyFunctionType)
-#define __Pyx_IsCyOrPyCFunction(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
+#define __Pyx_CyOrPyCFunction_Check(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
 #define __Pyx_CyFunction_CheckExact(obj)  __Pyx_IS_TYPE(obj, __pyx_CyFunctionType)
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc);
+#undef __Pyx_IsSameCFunction
+#define __Pyx_IsSameCFunction(func, cfunc)   __Pyx__IsSameCyOrCFunction(func, cfunc)
 static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
                                       int flags, PyObject* qualname,
                                       PyObject *closure,
                                       PyObject *module, PyObject *globals,
                                       PyObject* code);
 static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj);
 static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
@@ -2427,15 +2483,16 @@
 #define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
 #define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_CurrentExceptionType(), err1, err2)
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
-static int __Pyx_check_binary_version(void);
+static unsigned long __Pyx_get_runtime_version(void);
+static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 /* #### Code section: module_declarations ### */
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_4date_4year_year(PyDateTime_Date *__pyx_v_self); /* proto*/
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_4date_5month_month(PyDateTime_Date *__pyx_v_self); /* proto*/
@@ -2508,14 +2565,16 @@
 
 /* Module declarations from "__builtin__" */
 
 /* Module declarations from "cpython.complex" */
 
 /* Module declarations from "cpython.string" */
 
+/* Module declarations from "libc.stddef" */
+
 /* Module declarations from "cpython.unicode" */
 
 /* Module declarations from "cpython.pyport" */
 
 /* Module declarations from "cpython.dict" */
 
 /* Module declarations from "cpython.instance" */
@@ -2909,14 +2968,16 @@
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
   PyTypeObject *__pyx_ptype_7cpython_8datetime_date;
   PyTypeObject *__pyx_ptype_7cpython_8datetime_time;
   PyTypeObject *__pyx_ptype_7cpython_8datetime_datetime;
   PyTypeObject *__pyx_ptype_7cpython_8datetime_timedelta;
   PyTypeObject *__pyx_ptype_7cpython_8datetime_tzinfo;
   #if CYTHON_USE_MODULE_STATE
   #endif
@@ -3806,14 +3867,16 @@
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
+#if CYTHON_USE_MODULE_STATE
+#endif
 #define __pyx_ptype_7cpython_8datetime_date __pyx_mstate_global->__pyx_ptype_7cpython_8datetime_date
 #define __pyx_ptype_7cpython_8datetime_time __pyx_mstate_global->__pyx_ptype_7cpython_8datetime_time
 #define __pyx_ptype_7cpython_8datetime_datetime __pyx_mstate_global->__pyx_ptype_7cpython_8datetime_datetime
 #define __pyx_ptype_7cpython_8datetime_timedelta __pyx_mstate_global->__pyx_ptype_7cpython_8datetime_timedelta
 #define __pyx_ptype_7cpython_8datetime_tzinfo __pyx_mstate_global->__pyx_ptype_7cpython_8datetime_tzinfo
 #if CYTHON_USE_MODULE_STATE
 #endif
@@ -4062,16 +4125,14 @@
  *         cdef inline int year(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_GET_YEAR(self)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_4date_4year_year(PyDateTime_Date *__pyx_v_self) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("year", 0);
 
   /* "cpython/datetime.pxd":73
  *         @property
  *         cdef inline int year(self):
  *             return PyDateTime_GET_YEAR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
@@ -4085,30 +4146,27 @@
  *         cdef inline int year(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_GET_YEAR(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":76
  * 
  *         @property
  *         cdef inline int month(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_GET_MONTH(self)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_4date_5month_month(PyDateTime_Date *__pyx_v_self) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("month", 0);
 
   /* "cpython/datetime.pxd":77
  *         @property
  *         cdef inline int month(self):
  *             return PyDateTime_GET_MONTH(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
@@ -4122,30 +4180,27 @@
  *         cdef inline int month(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_GET_MONTH(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":80
  * 
  *         @property
  *         cdef inline int day(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_GET_DAY(self)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_4date_3day_day(PyDateTime_Date *__pyx_v_self) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("day", 0);
 
   /* "cpython/datetime.pxd":81
  *         @property
  *         cdef inline int day(self):
  *             return PyDateTime_GET_DAY(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef extern class datetime.time[object PyDateTime_Time]:
@@ -4159,30 +4214,27 @@
  *         cdef inline int day(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_GET_DAY(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":85
  *     ctypedef extern class datetime.time[object PyDateTime_Time]:
  *         @property
  *         cdef inline int hour(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_TIME_GET_HOUR(self)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_4time_4hour_hour(PyDateTime_Time *__pyx_v_self) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("hour", 0);
 
   /* "cpython/datetime.pxd":86
  *         @property
  *         cdef inline int hour(self):
  *             return PyDateTime_TIME_GET_HOUR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
@@ -4196,30 +4248,27 @@
  *         cdef inline int hour(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_TIME_GET_HOUR(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":89
  * 
  *         @property
  *         cdef inline int minute(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_TIME_GET_MINUTE(self)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_4time_6minute_minute(PyDateTime_Time *__pyx_v_self) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("minute", 0);
 
   /* "cpython/datetime.pxd":90
  *         @property
  *         cdef inline int minute(self):
  *             return PyDateTime_TIME_GET_MINUTE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
@@ -4233,30 +4282,27 @@
  *         cdef inline int minute(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_TIME_GET_MINUTE(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":93
  * 
  *         @property
  *         cdef inline int second(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_TIME_GET_SECOND(self)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_4time_6second_second(PyDateTime_Time *__pyx_v_self) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("second", 0);
 
   /* "cpython/datetime.pxd":94
  *         @property
  *         cdef inline int second(self):
  *             return PyDateTime_TIME_GET_SECOND(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
@@ -4270,30 +4316,27 @@
  *         cdef inline int second(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_TIME_GET_SECOND(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":97
  * 
  *         @property
  *         cdef inline int microsecond(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_TIME_GET_MICROSECOND(self)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_4time_11microsecond_microsecond(PyDateTime_Time *__pyx_v_self) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("microsecond", 0);
 
   /* "cpython/datetime.pxd":98
  *         @property
  *         cdef inline int microsecond(self):
  *             return PyDateTime_TIME_GET_MICROSECOND(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
@@ -4307,15 +4350,14 @@
  *         cdef inline int microsecond(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_TIME_GET_MICROSECOND(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":101
  * 
  *         @property
  *         cdef inline object tzinfo(self):             # <<<<<<<<<<<<<<
@@ -4323,15 +4365,15 @@
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_7cpython_8datetime_4time_6tzinfo_tzinfo(PyDateTime_Time *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1;
-  __Pyx_RefNannySetupContext("tzinfo", 0);
+  __Pyx_RefNannySetupContext("tzinfo", 1);
 
   /* "cpython/datetime.pxd":102
  *         @property
  *         cdef inline object tzinfo(self):
  *             return <object>PyDateTime_TIME_GET_TZINFO(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
@@ -4363,16 +4405,14 @@
  *         cdef inline int fold(self):             # <<<<<<<<<<<<<<
  *             # For Python < 3.6 this returns 0 no matter what
  *             return PyDateTime_TIME_GET_FOLD(self)
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_4time_4fold_fold(PyDateTime_Time *__pyx_v_self) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("fold", 0);
 
   /* "cpython/datetime.pxd":107
  *         cdef inline int fold(self):
  *             # For Python < 3.6 this returns 0 no matter what
  *             return PyDateTime_TIME_GET_FOLD(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef extern class datetime.datetime[object PyDateTime_DateTime]:
@@ -4386,30 +4426,27 @@
  *         cdef inline int fold(self):             # <<<<<<<<<<<<<<
  *             # For Python < 3.6 this returns 0 no matter what
  *             return PyDateTime_TIME_GET_FOLD(self)
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":111
  *     ctypedef extern class datetime.datetime[object PyDateTime_DateTime]:
  *         @property
  *         cdef inline int year(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_GET_YEAR(self)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_8datetime_4year_year(PyDateTime_DateTime *__pyx_v_self) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("year", 0);
 
   /* "cpython/datetime.pxd":112
  *         @property
  *         cdef inline int year(self):
  *             return PyDateTime_GET_YEAR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
@@ -4423,30 +4460,27 @@
  *         cdef inline int year(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_GET_YEAR(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":115
  * 
  *         @property
  *         cdef inline int month(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_GET_MONTH(self)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_8datetime_5month_month(PyDateTime_DateTime *__pyx_v_self) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("month", 0);
 
   /* "cpython/datetime.pxd":116
  *         @property
  *         cdef inline int month(self):
  *             return PyDateTime_GET_MONTH(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
@@ -4460,30 +4494,27 @@
  *         cdef inline int month(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_GET_MONTH(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":119
  * 
  *         @property
  *         cdef inline int day(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_GET_DAY(self)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_8datetime_3day_day(PyDateTime_DateTime *__pyx_v_self) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("day", 0);
 
   /* "cpython/datetime.pxd":120
  *         @property
  *         cdef inline int day(self):
  *             return PyDateTime_GET_DAY(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
@@ -4497,30 +4528,27 @@
  *         cdef inline int day(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_GET_DAY(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":123
  * 
  *         @property
  *         cdef inline int hour(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_DATE_GET_HOUR(self)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_8datetime_4hour_hour(PyDateTime_DateTime *__pyx_v_self) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("hour", 0);
 
   /* "cpython/datetime.pxd":124
  *         @property
  *         cdef inline int hour(self):
  *             return PyDateTime_DATE_GET_HOUR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
@@ -4534,30 +4562,27 @@
  *         cdef inline int hour(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_DATE_GET_HOUR(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":127
  * 
  *         @property
  *         cdef inline int minute(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_DATE_GET_MINUTE(self)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_8datetime_6minute_minute(PyDateTime_DateTime *__pyx_v_self) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("minute", 0);
 
   /* "cpython/datetime.pxd":128
  *         @property
  *         cdef inline int minute(self):
  *             return PyDateTime_DATE_GET_MINUTE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
@@ -4571,30 +4596,27 @@
  *         cdef inline int minute(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_DATE_GET_MINUTE(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":131
  * 
  *         @property
  *         cdef inline int second(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_DATE_GET_SECOND(self)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_8datetime_6second_second(PyDateTime_DateTime *__pyx_v_self) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("second", 0);
 
   /* "cpython/datetime.pxd":132
  *         @property
  *         cdef inline int second(self):
  *             return PyDateTime_DATE_GET_SECOND(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
@@ -4608,30 +4630,27 @@
  *         cdef inline int second(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_DATE_GET_SECOND(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":135
  * 
  *         @property
  *         cdef inline int microsecond(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_DATE_GET_MICROSECOND(self)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_8datetime_11microsecond_microsecond(PyDateTime_DateTime *__pyx_v_self) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("microsecond", 0);
 
   /* "cpython/datetime.pxd":136
  *         @property
  *         cdef inline int microsecond(self):
  *             return PyDateTime_DATE_GET_MICROSECOND(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
@@ -4645,15 +4664,14 @@
  *         cdef inline int microsecond(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_DATE_GET_MICROSECOND(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":139
  * 
  *         @property
  *         cdef inline object tzinfo(self):             # <<<<<<<<<<<<<<
@@ -4661,15 +4679,15 @@
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_7cpython_8datetime_8datetime_6tzinfo_tzinfo(PyDateTime_DateTime *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1;
-  __Pyx_RefNannySetupContext("tzinfo", 0);
+  __Pyx_RefNannySetupContext("tzinfo", 1);
 
   /* "cpython/datetime.pxd":140
  *         @property
  *         cdef inline object tzinfo(self):
  *             return <object>PyDateTime_DATE_GET_TZINFO(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
@@ -4701,16 +4719,14 @@
  *         cdef inline int fold(self):             # <<<<<<<<<<<<<<
  *             # For Python < 3.6 this returns 0 no matter what
  *             return PyDateTime_DATE_GET_FOLD(self)
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_8datetime_4fold_fold(PyDateTime_DateTime *__pyx_v_self) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("fold", 0);
 
   /* "cpython/datetime.pxd":145
  *         cdef inline int fold(self):
  *             # For Python < 3.6 this returns 0 no matter what
  *             return PyDateTime_DATE_GET_FOLD(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef extern class datetime.timedelta[object PyDateTime_Delta]:
@@ -4724,30 +4740,27 @@
  *         cdef inline int fold(self):             # <<<<<<<<<<<<<<
  *             # For Python < 3.6 this returns 0 no matter what
  *             return PyDateTime_DATE_GET_FOLD(self)
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":149
  *     ctypedef extern class datetime.timedelta[object PyDateTime_Delta]:
  *         @property
  *         cdef inline int day(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_DELTA_GET_DAYS(self)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_9timedelta_3day_day(PyDateTime_Delta *__pyx_v_self) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("day", 0);
 
   /* "cpython/datetime.pxd":150
  *         @property
  *         cdef inline int day(self):
  *             return PyDateTime_DELTA_GET_DAYS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
@@ -4761,30 +4774,27 @@
  *         cdef inline int day(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_DELTA_GET_DAYS(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":153
  * 
  *         @property
  *         cdef inline int second(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_DELTA_GET_SECONDS(self)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_9timedelta_6second_second(PyDateTime_Delta *__pyx_v_self) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("second", 0);
 
   /* "cpython/datetime.pxd":154
  *         @property
  *         cdef inline int second(self):
  *             return PyDateTime_DELTA_GET_SECONDS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
@@ -4798,30 +4808,27 @@
  *         cdef inline int second(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_DELTA_GET_SECONDS(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":157
  * 
  *         @property
  *         cdef inline int microsecond(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_DELTA_GET_MICROSECONDS(self)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_9timedelta_11microsecond_microsecond(PyDateTime_Delta *__pyx_v_self) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("microsecond", 0);
 
   /* "cpython/datetime.pxd":158
  *         @property
  *         cdef inline int microsecond(self):
  *             return PyDateTime_DELTA_GET_MICROSECONDS(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef extern class datetime.tzinfo[object PyDateTime_TZInfo]:
@@ -4835,29 +4842,26 @@
  *         cdef inline int microsecond(self):             # <<<<<<<<<<<<<<
  *             return PyDateTime_DELTA_GET_MICROSECONDS(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":282
  * # Datetime C API initialization function.
  * # You have to call it before any usage of DateTime CAPI functions.
  * cdef inline void import_datetime():             # <<<<<<<<<<<<<<
  *     PyDateTime_IMPORT
  * 
  */
 
 static CYTHON_INLINE void __pyx_f_7cpython_8datetime_import_datetime(void) {
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("import_datetime", 0);
 
   /* "cpython/datetime.pxd":283
  * # You have to call it before any usage of DateTime CAPI functions.
  * cdef inline void import_datetime():
  *     PyDateTime_IMPORT             # <<<<<<<<<<<<<<
  * 
  * # Create date object using DateTime CAPI factory function.
@@ -4869,15 +4873,14 @@
  * # You have to call it before any usage of DateTime CAPI functions.
  * cdef inline void import_datetime():             # <<<<<<<<<<<<<<
  *     PyDateTime_IMPORT
  * 
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "cpython/datetime.pxd":287
  * # Create date object using DateTime CAPI factory function.
  * # Note, there are no range checks for any of the arguments.
  * cdef inline date date_new(int year, int month, int day):             # <<<<<<<<<<<<<<
  *     return PyDateTimeAPI.Date_FromDate(year, month, day, PyDateTimeAPI.DateType)
@@ -4887,15 +4890,15 @@
 static CYTHON_INLINE PyDateTime_Date *__pyx_f_7cpython_8datetime_date_new(int __pyx_v_year, int __pyx_v_month, int __pyx_v_day) {
   PyDateTime_Date *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("date_new", 0);
+  __Pyx_RefNannySetupContext("date_new", 1);
 
   /* "cpython/datetime.pxd":288
  * # Note, there are no range checks for any of the arguments.
  * cdef inline date date_new(int year, int month, int day):
  *     return PyDateTimeAPI.Date_FromDate(year, month, day, PyDateTimeAPI.DateType)             # <<<<<<<<<<<<<<
  * 
  * # Create time object using DateTime CAPI factory function
@@ -4938,15 +4941,15 @@
   int __pyx_v_fold = ((int)0);
   PyDateTime_Time *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("time_new", 0);
+  __Pyx_RefNannySetupContext("time_new", 1);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_fold = __pyx_optional_args->fold;
     }
   }
 
   /* "cpython/datetime.pxd":293
@@ -4995,15 +4998,15 @@
   int __pyx_v_fold = ((int)0);
   PyDateTime_DateTime *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("datetime_new", 0);
+  __Pyx_RefNannySetupContext("datetime_new", 1);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_fold = __pyx_optional_args->fold;
     }
   }
 
   /* "cpython/datetime.pxd":298
@@ -5050,15 +5053,15 @@
 static CYTHON_INLINE PyDateTime_Delta *__pyx_f_7cpython_8datetime_timedelta_new(int __pyx_v_days, int __pyx_v_seconds, int __pyx_v_useconds) {
   PyDateTime_Delta *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("timedelta_new", 0);
+  __Pyx_RefNannySetupContext("timedelta_new", 1);
 
   /* "cpython/datetime.pxd":303
  * # Note, there are no range checks for any of the arguments.
  * cdef inline timedelta timedelta_new(int days, int seconds, int useconds):
  *     return PyDateTimeAPI.Delta_FromDelta(days, seconds, useconds, 1, PyDateTimeAPI.DeltaType)             # <<<<<<<<<<<<<<
  * 
  * # Create timedelta object using DateTime CAPI factory function.
@@ -5103,15 +5106,15 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("timezone_new", 0);
+  __Pyx_RefNannySetupContext("timezone_new", 1);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_name = __pyx_optional_args->name;
     }
   }
 
   /* "cpython/datetime.pxd":307
@@ -5199,15 +5202,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("datetime_from_timestamp", 0);
+  __Pyx_RefNannySetupContext("datetime_from_timestamp", 1);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_tz = __pyx_optional_args->tz;
     }
   }
 
   /* "cpython/datetime.pxd":313
@@ -5294,15 +5297,15 @@
   PyDateTime_Date *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("date_from_timestamp", 0);
+  __Pyx_RefNannySetupContext("date_from_timestamp", 1);
 
   /* "cpython/datetime.pxd":318
  * # Create date object using DB API constructor.
  * cdef inline date date_from_timestamp(timestamp):
  *     return PyDateTimeAPI.Date_FromTimestamp(<PyObject*>PyDateTimeAPI.DateType, (timestamp,))             # <<<<<<<<<<<<<<
  * 
  * # More recognizable getters for date/time/datetime/timedelta.
@@ -5352,15 +5355,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_utc", 0);
+  __Pyx_RefNannySetupContext("get_utc", 1);
 
   /* "cpython/datetime.pxd":327
  * # Get UTC singleton
  * cdef inline object get_utc():
  *     if PY_VERSION_HEX < 0x030700b1:             # <<<<<<<<<<<<<<
  *         raise RuntimeError('Time zones are not available from the C-API.')
  *     return <object>__Pyx_TimeZone_UTC
@@ -5429,15 +5432,15 @@
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_7cpython_8datetime_time_tzinfo(PyObject *__pyx_v_o) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1;
-  __Pyx_RefNannySetupContext("time_tzinfo", 0);
+  __Pyx_RefNannySetupContext("time_tzinfo", 1);
 
   /* "cpython/datetime.pxd":333
  * # Get tzinfo of time
  * cdef inline object time_tzinfo(object o):
  *     return <object>PyDateTime_TIME_GET_TZINFO(o)             # <<<<<<<<<<<<<<
  * 
  * # Get tzinfo of datetime
@@ -5471,15 +5474,15 @@
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_7cpython_8datetime_datetime_tzinfo(PyObject *__pyx_v_o) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1;
-  __Pyx_RefNannySetupContext("datetime_tzinfo", 0);
+  __Pyx_RefNannySetupContext("datetime_tzinfo", 1);
 
   /* "cpython/datetime.pxd":337
  * # Get tzinfo of datetime
  * cdef inline object datetime_tzinfo(object o):
  *     return <object>PyDateTime_DATE_GET_TZINFO(o)             # <<<<<<<<<<<<<<
  * 
  * # Get year of date
@@ -5511,16 +5514,14 @@
  * cdef inline int date_year(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_GET_YEAR(o)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_date_year(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("date_year", 0);
 
   /* "cpython/datetime.pxd":341
  * # Get year of date
  * cdef inline int date_year(object o):
  *     return PyDateTime_GET_YEAR(o)             # <<<<<<<<<<<<<<
  * 
  * # Get month of date
@@ -5534,30 +5535,27 @@
  * cdef inline int date_year(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_GET_YEAR(o)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":344
  * 
  * # Get month of date
  * cdef inline int date_month(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_GET_MONTH(o)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_date_month(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("date_month", 0);
 
   /* "cpython/datetime.pxd":345
  * # Get month of date
  * cdef inline int date_month(object o):
  *     return PyDateTime_GET_MONTH(o)             # <<<<<<<<<<<<<<
  * 
  * # Get day of date
@@ -5571,30 +5569,27 @@
  * cdef inline int date_month(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_GET_MONTH(o)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":348
  * 
  * # Get day of date
  * cdef inline int date_day(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_GET_DAY(o)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_date_day(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("date_day", 0);
 
   /* "cpython/datetime.pxd":349
  * # Get day of date
  * cdef inline int date_day(object o):
  *     return PyDateTime_GET_DAY(o)             # <<<<<<<<<<<<<<
  * 
  * # Get year of datetime
@@ -5608,30 +5603,27 @@
  * cdef inline int date_day(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_GET_DAY(o)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":352
  * 
  * # Get year of datetime
  * cdef inline int datetime_year(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_GET_YEAR(o)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_datetime_year(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("datetime_year", 0);
 
   /* "cpython/datetime.pxd":353
  * # Get year of datetime
  * cdef inline int datetime_year(object o):
  *     return PyDateTime_GET_YEAR(o)             # <<<<<<<<<<<<<<
  * 
  * # Get month of datetime
@@ -5645,30 +5637,27 @@
  * cdef inline int datetime_year(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_GET_YEAR(o)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":356
  * 
  * # Get month of datetime
  * cdef inline int datetime_month(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_GET_MONTH(o)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_datetime_month(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("datetime_month", 0);
 
   /* "cpython/datetime.pxd":357
  * # Get month of datetime
  * cdef inline int datetime_month(object o):
  *     return PyDateTime_GET_MONTH(o)             # <<<<<<<<<<<<<<
  * 
  * # Get day of datetime
@@ -5682,30 +5671,27 @@
  * cdef inline int datetime_month(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_GET_MONTH(o)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":360
  * 
  * # Get day of datetime
  * cdef inline int datetime_day(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_GET_DAY(o)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_datetime_day(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("datetime_day", 0);
 
   /* "cpython/datetime.pxd":361
  * # Get day of datetime
  * cdef inline int datetime_day(object o):
  *     return PyDateTime_GET_DAY(o)             # <<<<<<<<<<<<<<
  * 
  * # Get hour of time
@@ -5719,30 +5705,27 @@
  * cdef inline int datetime_day(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_GET_DAY(o)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":364
  * 
  * # Get hour of time
  * cdef inline int time_hour(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_TIME_GET_HOUR(o)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_time_hour(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("time_hour", 0);
 
   /* "cpython/datetime.pxd":365
  * # Get hour of time
  * cdef inline int time_hour(object o):
  *     return PyDateTime_TIME_GET_HOUR(o)             # <<<<<<<<<<<<<<
  * 
  * # Get minute of time
@@ -5756,30 +5739,27 @@
  * cdef inline int time_hour(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_TIME_GET_HOUR(o)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":368
  * 
  * # Get minute of time
  * cdef inline int time_minute(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_TIME_GET_MINUTE(o)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_time_minute(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("time_minute", 0);
 
   /* "cpython/datetime.pxd":369
  * # Get minute of time
  * cdef inline int time_minute(object o):
  *     return PyDateTime_TIME_GET_MINUTE(o)             # <<<<<<<<<<<<<<
  * 
  * # Get second of time
@@ -5793,30 +5773,27 @@
  * cdef inline int time_minute(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_TIME_GET_MINUTE(o)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":372
  * 
  * # Get second of time
  * cdef inline int time_second(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_TIME_GET_SECOND(o)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_time_second(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("time_second", 0);
 
   /* "cpython/datetime.pxd":373
  * # Get second of time
  * cdef inline int time_second(object o):
  *     return PyDateTime_TIME_GET_SECOND(o)             # <<<<<<<<<<<<<<
  * 
  * # Get microsecond of time
@@ -5830,30 +5807,27 @@
  * cdef inline int time_second(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_TIME_GET_SECOND(o)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":376
  * 
  * # Get microsecond of time
  * cdef inline int time_microsecond(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_TIME_GET_MICROSECOND(o)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_time_microsecond(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("time_microsecond", 0);
 
   /* "cpython/datetime.pxd":377
  * # Get microsecond of time
  * cdef inline int time_microsecond(object o):
  *     return PyDateTime_TIME_GET_MICROSECOND(o)             # <<<<<<<<<<<<<<
  * 
  * # Get fold of time
@@ -5867,30 +5841,27 @@
  * cdef inline int time_microsecond(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_TIME_GET_MICROSECOND(o)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":380
  * 
  * # Get fold of time
  * cdef inline int time_fold(object o):             # <<<<<<<<<<<<<<
  *     # For Python < 3.6 this returns 0 no matter what
  *     return PyDateTime_TIME_GET_FOLD(o)
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_time_fold(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("time_fold", 0);
 
   /* "cpython/datetime.pxd":382
  * cdef inline int time_fold(object o):
  *     # For Python < 3.6 this returns 0 no matter what
  *     return PyDateTime_TIME_GET_FOLD(o)             # <<<<<<<<<<<<<<
  * 
  * # Get hour of datetime
@@ -5904,30 +5875,27 @@
  * cdef inline int time_fold(object o):             # <<<<<<<<<<<<<<
  *     # For Python < 3.6 this returns 0 no matter what
  *     return PyDateTime_TIME_GET_FOLD(o)
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":385
  * 
  * # Get hour of datetime
  * cdef inline int datetime_hour(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_DATE_GET_HOUR(o)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_datetime_hour(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("datetime_hour", 0);
 
   /* "cpython/datetime.pxd":386
  * # Get hour of datetime
  * cdef inline int datetime_hour(object o):
  *     return PyDateTime_DATE_GET_HOUR(o)             # <<<<<<<<<<<<<<
  * 
  * # Get minute of datetime
@@ -5941,30 +5909,27 @@
  * cdef inline int datetime_hour(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_DATE_GET_HOUR(o)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":389
  * 
  * # Get minute of datetime
  * cdef inline int datetime_minute(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_DATE_GET_MINUTE(o)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_datetime_minute(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("datetime_minute", 0);
 
   /* "cpython/datetime.pxd":390
  * # Get minute of datetime
  * cdef inline int datetime_minute(object o):
  *     return PyDateTime_DATE_GET_MINUTE(o)             # <<<<<<<<<<<<<<
  * 
  * # Get second of datetime
@@ -5978,30 +5943,27 @@
  * cdef inline int datetime_minute(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_DATE_GET_MINUTE(o)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":393
  * 
  * # Get second of datetime
  * cdef inline int datetime_second(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_DATE_GET_SECOND(o)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_datetime_second(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("datetime_second", 0);
 
   /* "cpython/datetime.pxd":394
  * # Get second of datetime
  * cdef inline int datetime_second(object o):
  *     return PyDateTime_DATE_GET_SECOND(o)             # <<<<<<<<<<<<<<
  * 
  * # Get microsecond of datetime
@@ -6015,30 +5977,27 @@
  * cdef inline int datetime_second(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_DATE_GET_SECOND(o)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":397
  * 
  * # Get microsecond of datetime
  * cdef inline int datetime_microsecond(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_DATE_GET_MICROSECOND(o)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_datetime_microsecond(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("datetime_microsecond", 0);
 
   /* "cpython/datetime.pxd":398
  * # Get microsecond of datetime
  * cdef inline int datetime_microsecond(object o):
  *     return PyDateTime_DATE_GET_MICROSECOND(o)             # <<<<<<<<<<<<<<
  * 
  * # Get fold of datetime
@@ -6052,30 +6011,27 @@
  * cdef inline int datetime_microsecond(object o):             # <<<<<<<<<<<<<<
  *     return PyDateTime_DATE_GET_MICROSECOND(o)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":401
  * 
  * # Get fold of datetime
  * cdef inline int datetime_fold(object o):             # <<<<<<<<<<<<<<
  *     # For Python < 3.6 this returns 0 no matter what
  *     return PyDateTime_DATE_GET_FOLD(o)
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_datetime_fold(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("datetime_fold", 0);
 
   /* "cpython/datetime.pxd":403
  * cdef inline int datetime_fold(object o):
  *     # For Python < 3.6 this returns 0 no matter what
  *     return PyDateTime_DATE_GET_FOLD(o)             # <<<<<<<<<<<<<<
  * 
  * # Get days of timedelta
@@ -6089,30 +6045,27 @@
  * cdef inline int datetime_fold(object o):             # <<<<<<<<<<<<<<
  *     # For Python < 3.6 this returns 0 no matter what
  *     return PyDateTime_DATE_GET_FOLD(o)
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":406
  * 
  * # Get days of timedelta
  * cdef inline int timedelta_days(object o):             # <<<<<<<<<<<<<<
  *     return (<PyDateTime_Delta*>o).days
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_timedelta_days(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("timedelta_days", 0);
 
   /* "cpython/datetime.pxd":407
  * # Get days of timedelta
  * cdef inline int timedelta_days(object o):
  *     return (<PyDateTime_Delta*>o).days             # <<<<<<<<<<<<<<
  * 
  * # Get seconds of timedelta
@@ -6126,30 +6079,27 @@
  * cdef inline int timedelta_days(object o):             # <<<<<<<<<<<<<<
  *     return (<PyDateTime_Delta*>o).days
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":410
  * 
  * # Get seconds of timedelta
  * cdef inline int timedelta_seconds(object o):             # <<<<<<<<<<<<<<
  *     return (<PyDateTime_Delta*>o).seconds
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_timedelta_seconds(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("timedelta_seconds", 0);
 
   /* "cpython/datetime.pxd":411
  * # Get seconds of timedelta
  * cdef inline int timedelta_seconds(object o):
  *     return (<PyDateTime_Delta*>o).seconds             # <<<<<<<<<<<<<<
  * 
  * # Get microseconds of timedelta
@@ -6163,30 +6113,27 @@
  * cdef inline int timedelta_seconds(object o):             # <<<<<<<<<<<<<<
  *     return (<PyDateTime_Delta*>o).seconds
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":414
  * 
  * # Get microseconds of timedelta
  * cdef inline int timedelta_microseconds(object o):             # <<<<<<<<<<<<<<
  *     return (<PyDateTime_Delta*>o).microseconds
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_timedelta_microseconds(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("timedelta_microseconds", 0);
 
   /* "cpython/datetime.pxd":415
  * # Get microseconds of timedelta
  * cdef inline int timedelta_microseconds(object o):
  *     return (<PyDateTime_Delta*>o).microseconds             # <<<<<<<<<<<<<<
  * 
  * cdef inline double total_seconds(timedelta obj):
@@ -6200,15 +6147,14 @@
  * cdef inline int timedelta_microseconds(object o):             # <<<<<<<<<<<<<<
  *     return (<PyDateTime_Delta*>o).microseconds
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/datetime.pxd":417
  *     return (<PyDateTime_Delta*>o).microseconds
  * 
  * cdef inline double total_seconds(timedelta obj):             # <<<<<<<<<<<<<<
@@ -6217,16 +6163,14 @@
  */
 
 static CYTHON_INLINE double __pyx_f_7cpython_8datetime_total_seconds(PyDateTime_Delta *__pyx_v_obj) {
   double __pyx_v_days;
   double __pyx_v_seconds;
   double __pyx_v_micros;
   double __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("total_seconds", 0);
 
   /* "cpython/datetime.pxd":423
  *     cdef:
  *         double days, seconds, micros
  *     days = <double>PyDateTime_DELTA_GET_DAYS(obj)             # <<<<<<<<<<<<<<
  *     seconds = <double>PyDateTime_DELTA_GET_SECONDS(obj)
  *     micros = <double>PyDateTime_DELTA_GET_MICROSECONDS(obj)
@@ -6264,30 +6208,27 @@
  * cdef inline double total_seconds(timedelta obj):             # <<<<<<<<<<<<<<
  *     # Mirrors the "timedelta.total_seconds()" method.
  *     # Note that this implementation is not guaranteed to give *exactly* the same
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/complex.pxd":19
  * 
  *         @property
  *         cdef inline double real(self):             # <<<<<<<<<<<<<<
  *             return self.cval.real
  * 
  */
 
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4real_real(PyComplexObject *__pyx_v_self) {
   double __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("real", 0);
 
   /* "cpython/complex.pxd":20
  *         @property
  *         cdef inline double real(self):
  *             return self.cval.real             # <<<<<<<<<<<<<<
  * 
  *         @property
@@ -6301,30 +6242,27 @@
  *         cdef inline double real(self):             # <<<<<<<<<<<<<<
  *             return self.cval.real
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/complex.pxd":23
  * 
  *         @property
  *         cdef inline double imag(self):             # <<<<<<<<<<<<<<
  *             return self.cval.imag
  * 
  */
 
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4imag_imag(PyComplexObject *__pyx_v_self) {
   double __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("imag", 0);
 
   /* "cpython/complex.pxd":24
  *         @property
  *         cdef inline double imag(self):
  *             return self.cval.imag             # <<<<<<<<<<<<<<
  * 
  *     # PyTypeObject PyComplex_Type
@@ -6338,15 +6276,14 @@
  *         cdef inline double imag(self):             # <<<<<<<<<<<<<<
  *             return self.cval.imag
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/contextvars.pxd":112
  * 
  * 
  * cdef inline object get_value(var, default_value=None):             # <<<<<<<<<<<<<<
@@ -6362,15 +6299,15 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_value", 0);
+  __Pyx_RefNannySetupContext("get_value", 1);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_default_value = __pyx_optional_args->default_value;
     }
   }
 
   /* "cpython/contextvars.pxd":117
@@ -6492,15 +6429,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_value_no_default", 0);
+  __Pyx_RefNannySetupContext("get_value_no_default", 1);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_default_value = __pyx_optional_args->default_value;
     }
   }
 
   /* "cpython/contextvars.pxd":135
@@ -6577,18 +6514,16 @@
  * cdef inline int PyBytesLike_Check(object o):             # <<<<<<<<<<<<<<
  *     return PyBytes_Check(o) or PyByteArray_Check(o)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7msgpack_9_cmsgpack_PyBytesLike_Check(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
-  __Pyx_RefNannySetupContext("PyBytesLike_Check", 0);
 
   /* "msgpack/_packer.pyx":55
  * 
  * cdef inline int PyBytesLike_Check(object o):
  *     return PyBytes_Check(o) or PyByteArray_Check(o)             # <<<<<<<<<<<<<<
  * 
  * 
@@ -6611,32 +6546,29 @@
  * cdef inline int PyBytesLike_Check(object o):             # <<<<<<<<<<<<<<
  *     return PyBytes_Check(o) or PyByteArray_Check(o)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "msgpack/_packer.pyx":58
  * 
  * 
  * cdef inline int PyBytesLike_CheckExact(object o):             # <<<<<<<<<<<<<<
  *     return PyBytes_CheckExact(o) or PyByteArray_CheckExact(o)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_7msgpack_9_cmsgpack_PyBytesLike_CheckExact(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
-  __Pyx_RefNannySetupContext("PyBytesLike_CheckExact", 0);
 
   /* "msgpack/_packer.pyx":59
  * 
  * cdef inline int PyBytesLike_CheckExact(object o):
  *     return PyBytes_CheckExact(o) or PyByteArray_CheckExact(o)             # <<<<<<<<<<<<<<
  * 
  * 
@@ -6659,15 +6591,14 @@
  * cdef inline int PyBytesLike_CheckExact(object o):             # <<<<<<<<<<<<<<
  *     return PyBytes_CheckExact(o) or PyByteArray_CheckExact(o)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "msgpack/_packer.pyx":116
  *     cdef bint datetime
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
@@ -6676,37 +6607,26 @@
  */
 
 /* Python wrapper */
 static int __pyx_pw_7msgpack_9_cmsgpack_6Packer_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_7msgpack_9_cmsgpack_6Packer_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 116, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return -1;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 0, 0, __pyx_nargs); return -1;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_VARARGS(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__cinit__", 0))) return -1;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("msgpack._cmsgpack.Packer.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7msgpack_9_cmsgpack_6Packer___cinit__(((struct __pyx_obj_7msgpack_9_cmsgpack_Packer *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -6715,15 +6635,15 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__cinit__", 0);
+  __Pyx_RefNannySetupContext("__cinit__", 1);
 
   /* "msgpack/_packer.pyx":117
  * 
  *     def __cinit__(self):
  *         cdef int buf_size = 1024*1024             # <<<<<<<<<<<<<<
  *         self.pk.buf = <char*> PyMem_Malloc(buf_size)
  *         if self.pk.buf == NULL:
@@ -6835,16 +6755,15 @@
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 124, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return -1;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_default,&__pyx_n_s_use_single_float,&__pyx_n_s_autoreset,&__pyx_n_s_use_bin_type,&__pyx_n_s_strict_types,&__pyx_n_s_datetime,&__pyx_n_s_unicode_errors,0};
     values[0] = __Pyx_Arg_NewRef_VARARGS(((PyObject *)Py_None));
 
     /* "msgpack/_packer.pyx":126
@@ -6917,18 +6836,19 @@
     if (values[5]) {
       __pyx_v_datetime = __Pyx_PyObject_IsTrue(values[5]); if (unlikely((__pyx_v_datetime == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 126, __pyx_L3_error)
     } else {
       __pyx_v_datetime = ((int)0);
     }
     __pyx_v_unicode_errors = values[6];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__init__", 1, 0, 0, __pyx_nargs); __PYX_ERR(0, 124, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -6962,15 +6882,15 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   char const *__pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__init__", 0);
+  __Pyx_RefNannySetupContext("__init__", 1);
 
   /* "msgpack/_packer.pyx":127
  *                  bint use_single_float=False, bint autoreset=True, bint use_bin_type=True,
  *                  bint strict_types=False, bint datetime=False, unicode_errors=None):
  *         self.use_float = use_single_float             # <<<<<<<<<<<<<<
  *         self.strict_types = strict_types
  *         self.autoreset = autoreset
@@ -7170,16 +7090,14 @@
   __pyx_pf_7msgpack_9_cmsgpack_6Packer_4__dealloc__(((struct __pyx_obj_7msgpack_9_cmsgpack_Packer *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_7msgpack_9_cmsgpack_6Packer_4__dealloc__(struct __pyx_obj_7msgpack_9_cmsgpack_Packer *__pyx_v_self) {
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__dealloc__", 0);
 
   /* "msgpack/_packer.pyx":144
  * 
  *     def __dealloc__(self):
  *         PyMem_Free(self.pk.buf)             # <<<<<<<<<<<<<<
  *         self.pk.buf = NULL
  * 
@@ -7200,15 +7118,14 @@
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         PyMem_Free(self.pk.buf)
  *         self.pk.buf = NULL
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "msgpack/_packer.pyx":147
  *         self.pk.buf = NULL
  * 
  *     cdef int _pack(self, object o, int nest_limit=DEFAULT_RECURSE_LIMIT) except -1:             # <<<<<<<<<<<<<<
  *         cdef long long llval
@@ -8788,37 +8705,50 @@
  *                 ret = msgpack_pack_array(&self.pk, L)
  *                 if ret == 0:
  *                     for v in o:             # <<<<<<<<<<<<<<
  *                         ret = self._pack(v, nest_limit-1)
  *                         if ret != 0: break
  */
         if (likely(PyList_CheckExact(__pyx_v_o)) || PyTuple_CheckExact(__pyx_v_o)) {
-          __pyx_t_10 = __pyx_v_o; __Pyx_INCREF(__pyx_t_10); __pyx_t_28 = 0;
+          __pyx_t_10 = __pyx_v_o; __Pyx_INCREF(__pyx_t_10);
+          __pyx_t_28 = 0;
           __pyx_t_33 = NULL;
         } else {
           __pyx_t_28 = -1; __pyx_t_10 = PyObject_GetIter(__pyx_v_o); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 263, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_10);
           __pyx_t_33 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_10); if (unlikely(!__pyx_t_33)) __PYX_ERR(0, 263, __pyx_L1_error)
         }
         for (;;) {
           if (likely(!__pyx_t_33)) {
             if (likely(PyList_CheckExact(__pyx_t_10))) {
-              if (__pyx_t_28 >= PyList_GET_SIZE(__pyx_t_10)) break;
+              {
+                Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_10);
+                #if !CYTHON_ASSUME_SAFE_MACROS
+                if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 263, __pyx_L1_error)
+                #endif
+                if (__pyx_t_28 >= __pyx_temp) break;
+              }
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
               __pyx_t_9 = PyList_GET_ITEM(__pyx_t_10, __pyx_t_28); __Pyx_INCREF(__pyx_t_9); __pyx_t_28++; if (unlikely((0 < 0))) __PYX_ERR(0, 263, __pyx_L1_error)
               #else
-              __pyx_t_9 = PySequence_ITEM(__pyx_t_10, __pyx_t_28); __pyx_t_28++; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 263, __pyx_L1_error)
+              __pyx_t_9 = __Pyx_PySequence_ITEM(__pyx_t_10, __pyx_t_28); __pyx_t_28++; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 263, __pyx_L1_error)
               __Pyx_GOTREF(__pyx_t_9);
               #endif
             } else {
-              if (__pyx_t_28 >= PyTuple_GET_SIZE(__pyx_t_10)) break;
+              {
+                Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_10);
+                #if !CYTHON_ASSUME_SAFE_MACROS
+                if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 263, __pyx_L1_error)
+                #endif
+                if (__pyx_t_28 >= __pyx_temp) break;
+              }
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
               __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_10, __pyx_t_28); __Pyx_INCREF(__pyx_t_9); __pyx_t_28++; if (unlikely((0 < 0))) __PYX_ERR(0, 263, __pyx_L1_error)
               #else
-              __pyx_t_9 = PySequence_ITEM(__pyx_t_10, __pyx_t_28); __pyx_t_28++; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 263, __pyx_L1_error)
+              __pyx_t_9 = __Pyx_PySequence_ITEM(__pyx_t_10, __pyx_t_28); __pyx_t_28++; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 263, __pyx_L1_error)
               __Pyx_GOTREF(__pyx_t_9);
               #endif
             }
           } else {
             __pyx_t_9 = __pyx_t_33(__pyx_t_10);
             if (unlikely(!__pyx_t_9)) {
               PyObject* exc_type = PyErr_Occurred();
@@ -9349,32 +9279,27 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   struct __pyx_opt_args_7msgpack_9_cmsgpack_6Packer__pack __pyx_t_9;
   int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("pack", 0);
+  __Pyx_RefNannySetupContext("pack", 1);
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
       __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 294, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      #ifdef __Pyx_CyFunction_USED
-      if (!__Pyx_IsCyOrPyCFunction(__pyx_t_1)
-      #else
-      if (!PyCFunction_Check(__pyx_t_1)
-      #endif
-              || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7msgpack_9_cmsgpack_6Packer_7pack)) {
+      if (!__Pyx_IsSameCFunction(__pyx_t_1, (void*) __pyx_pw_7msgpack_9_cmsgpack_6Packer_7pack)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         __pyx_t_5 = 0;
         #if CYTHON_UNPACK_METHODS
         if (unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -9650,16 +9575,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("pack (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 294, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_obj,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -9686,18 +9610,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_obj = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("pack", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 294, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -9721,15 +9646,15 @@
 static PyObject *__pyx_pf_7msgpack_9_cmsgpack_6Packer_6pack(struct __pyx_obj_7msgpack_9_cmsgpack_Packer *__pyx_v_self, PyObject *__pyx_v_obj) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("pack", 0);
+  __Pyx_RefNannySetupContext("pack", 1);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_f_7msgpack_9_cmsgpack_6Packer_pack(__pyx_v_self, __pyx_v_obj, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 294, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
@@ -9782,16 +9707,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("pack_ext_type (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 308, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_typecode,&__pyx_n_s_data,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -9832,18 +9756,19 @@
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_typecode = values[0];
     __pyx_v_data = values[1];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("pack_ext_type", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 308, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -9869,15 +9794,15 @@
   __Pyx_RefNannyDeclarations
   char __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   char *__pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("pack_ext_type", 0);
+  __Pyx_RefNannySetupContext("pack_ext_type", 1);
 
   /* "msgpack/_packer.pyx":309
  * 
  *     def pack_ext_type(self, typecode, data):
  *         msgpack_pack_ext(&self.pk, typecode, len(data))             # <<<<<<<<<<<<<<
  *         msgpack_pack_raw_body(&self.pk, data, len(data))
  * 
@@ -9954,16 +9879,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("pack_array_header (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 312, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_size,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -9990,18 +9914,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_size = __Pyx_PyInt_As_PY_LONG_LONG(values[0]); if (unlikely((__pyx_v_size == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 312, __pyx_L3_error)
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("pack_array_header", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 312, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -10028,15 +9953,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("pack_array_header", 0);
+  __Pyx_RefNannySetupContext("pack_array_header", 1);
 
   /* "msgpack/_packer.pyx":313
  * 
  *     def pack_array_header(self, long long size):
  *         if size > ITEM_LIMIT:             # <<<<<<<<<<<<<<
  *             raise ValueError
  *         cdef int ret = msgpack_pack_array(&self.pk, size)
@@ -10239,16 +10164,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("pack_map_header (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 325, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_size,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -10275,18 +10199,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_size = __Pyx_PyInt_As_PY_LONG_LONG(values[0]); if (unlikely((__pyx_v_size == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 325, __pyx_L3_error)
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("pack_map_header", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 325, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -10313,15 +10238,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("pack_map_header", 0);
+  __Pyx_RefNannySetupContext("pack_map_header", 1);
 
   /* "msgpack/_packer.pyx":326
  * 
  *     def pack_map_header(self, long long size):
  *         if size > ITEM_LIMIT:             # <<<<<<<<<<<<<<
  *             raise ValueError
  *         cdef int ret = msgpack_pack_map(&self.pk, size)
@@ -10524,16 +10449,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("pack_map_pairs (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 338, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pairs,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -10560,18 +10484,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_pairs = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("pack_map_pairs", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 338, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -10608,15 +10533,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *(*__pyx_t_9)(PyObject *);
   int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("pack_map_pairs", 0);
+  __Pyx_RefNannySetupContext("pack_map_pairs", 1);
 
   /* "msgpack/_packer.pyx":345
  *         (`len(pairs)` and `for k, v in pairs:` should be supported.)
  *         """
  *         cdef int ret = msgpack_pack_map(&self.pk, len(pairs))             # <<<<<<<<<<<<<<
  *         if ret == 0:
  *             for k, v in pairs:
@@ -10638,37 +10563,50 @@
  *         cdef int ret = msgpack_pack_map(&self.pk, len(pairs))
  *         if ret == 0:
  *             for k, v in pairs:             # <<<<<<<<<<<<<<
  *                 ret = self._pack(k)
  *                 if ret != 0: break
  */
     if (likely(PyList_CheckExact(__pyx_v_pairs)) || PyTuple_CheckExact(__pyx_v_pairs)) {
-      __pyx_t_3 = __pyx_v_pairs; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
+      __pyx_t_3 = __pyx_v_pairs; __Pyx_INCREF(__pyx_t_3);
+      __pyx_t_1 = 0;
       __pyx_t_4 = NULL;
     } else {
       __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_pairs); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 347, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 347, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_4)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
-          if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_3)) break;
+          {
+            Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_3);
+            #if !CYTHON_ASSUME_SAFE_MACROS
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 347, __pyx_L1_error)
+            #endif
+            if (__pyx_t_1 >= __pyx_temp) break;
+          }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 347, __pyx_L1_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 347, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 347, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         } else {
-          if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
+          {
+            Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_3);
+            #if !CYTHON_ASSUME_SAFE_MACROS
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 347, __pyx_L1_error)
+            #endif
+            if (__pyx_t_1 >= __pyx_temp) break;
+          }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 347, __pyx_L1_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 347, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 347, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         }
       } else {
         __pyx_t_5 = __pyx_t_4(__pyx_t_3);
         if (unlikely(!__pyx_t_5)) {
           PyObject* exc_type = PyErr_Occurred();
@@ -10960,50 +10898,39 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("reset (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 361, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("reset", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "reset", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("msgpack._cmsgpack.Packer.reset", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7msgpack_9_cmsgpack_6Packer_16reset(((struct __pyx_obj_7msgpack_9_cmsgpack_Packer *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7msgpack_9_cmsgpack_6Packer_16reset(struct __pyx_obj_7msgpack_9_cmsgpack_Packer *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("reset", 0);
+  __Pyx_RefNannySetupContext("reset", 1);
 
   /* "msgpack/_packer.pyx":366
  *         This method is useful only when autoreset=False.
  *         """
  *         self.pk.length = 0             # <<<<<<<<<<<<<<
  * 
  *     def bytes(self):
@@ -11050,54 +10977,43 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("bytes (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 368, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("bytes", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "bytes", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("msgpack._cmsgpack.Packer.bytes", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7msgpack_9_cmsgpack_6Packer_18bytes(((struct __pyx_obj_7msgpack_9_cmsgpack_Packer *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7msgpack_9_cmsgpack_6Packer_18bytes(struct __pyx_obj_7msgpack_9_cmsgpack_Packer *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("bytes", 0);
+  __Pyx_RefNannySetupContext("bytes", 1);
 
   /* "msgpack/_packer.pyx":370
  *     def bytes(self):
  *         """Return internal buffer contents as bytes object"""
  *         return PyBytes_FromStringAndSize(self.pk.buf, self.pk.length)             # <<<<<<<<<<<<<<
  * 
  *     def getbuffer(self):
@@ -11153,54 +11069,43 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("getbuffer (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 372, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("getbuffer", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "getbuffer", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("msgpack._cmsgpack.Packer.getbuffer", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7msgpack_9_cmsgpack_6Packer_20getbuffer(((struct __pyx_obj_7msgpack_9_cmsgpack_Packer *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7msgpack_9_cmsgpack_6Packer_20getbuffer(struct __pyx_obj_7msgpack_9_cmsgpack_Packer *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("getbuffer", 0);
+  __Pyx_RefNannySetupContext("getbuffer", 1);
 
   /* "msgpack/_packer.pyx":374
  *     def getbuffer(self):
  *         """Return view of internal buffer."""
  *         return buff_to_buff(self.pk.buf, self.pk.length)             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
@@ -11252,53 +11157,42 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(4, 1, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("msgpack._cmsgpack.Packer.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7msgpack_9_cmsgpack_6Packer_22__reduce_cython__(((struct __pyx_obj_7msgpack_9_cmsgpack_Packer *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7msgpack_9_cmsgpack_6Packer_22__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7msgpack_9_cmsgpack_Packer *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_RefNannySetupContext("__reduce_cython__", 1);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
@@ -11356,16 +11250,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(4, 3, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -11392,18 +11285,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v___pyx_state = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(4, 3, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -11426,15 +11320,15 @@
 
 static PyObject *__pyx_pf_7msgpack_9_cmsgpack_6Packer_24__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7msgpack_9_cmsgpack_Packer *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
   /* "(tree fragment)":4
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  */
   __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_no_default___reduce___due_to_non, 0, 0);
@@ -11469,15 +11363,15 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("init_ctx", 0);
+  __Pyx_RefNannySetupContext("init_ctx", 1);
 
   /* "msgpack/_unpacker.pyx":69
  *                      Py_ssize_t max_array_len, Py_ssize_t max_map_len,
  *                      Py_ssize_t max_ext_len):
  *     unpack_init(ctx)             # <<<<<<<<<<<<<<
  *     ctx.user.use_list = use_list
  *     ctx.user.raw = raw
@@ -12012,16 +11906,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("default_read_extended_type (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 116, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_typecode,&__pyx_n_s_data,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -12062,18 +11955,19 @@
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_typecode = values[0];
     __pyx_v_data = values[1];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("default_read_extended_type", 1, 2, 2, __pyx_nargs); __PYX_ERR(1, 116, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -12098,15 +11992,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("default_read_extended_type", 0);
+  __Pyx_RefNannySetupContext("default_read_extended_type", 1);
 
   /* "msgpack/_unpacker.pyx":117
  * 
  * def default_read_extended_type(typecode, data):
  *     raise NotImplementedError("Cannot decode extended type with typecode=%d" % typecode)             # <<<<<<<<<<<<<<
  * 
  * cdef inline int get_data_from_buffer(object obj,
@@ -12154,15 +12048,15 @@
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   Py_ssize_t __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_data_from_buffer", 0);
+  __Pyx_RefNannySetupContext("get_data_from_buffer", 1);
 
   /* "msgpack/_unpacker.pyx":125
  *     cdef object contiguous
  *     cdef Py_buffer tmp
  *     if PyObject_GetBuffer(obj, view, PyBUF_FULL_RO) == -1:             # <<<<<<<<<<<<<<
  *         raise
  *     if view.itemsize != 1:
@@ -12348,15 +12242,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__defaults__", 0);
+  __Pyx_RefNannySetupContext("__defaults__", 1);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyDict_NewPresized(14); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_object_hook, Py_None) < 0) __PYX_ERR(1, 143, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_list_hook, Py_None) < 0) __PYX_ERR(1, 143, __pyx_L1_error)
 
   /* "msgpack/_unpacker.pyx":144
@@ -12544,16 +12438,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("unpackb (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 143, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_packed,&__pyx_n_s_object_hook,&__pyx_n_s_list_hook,&__pyx_n_s_use_list,&__pyx_n_s_raw,&__pyx_n_s_timestamp,&__pyx_n_s_strict_map_key,&__pyx_n_s_unicode_errors,&__pyx_n_s_object_pairs_hook,&__pyx_n_s_ext_hook,&__pyx_n_s_max_str_len,&__pyx_n_s_max_bin_len,&__pyx_n_s_max_array_len,&__pyx_n_s_max_map_len,&__pyx_n_s_max_ext_len,0};
     __pyx_defaults *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self);
     values[1] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)Py_None));
@@ -12660,18 +12553,19 @@
     }
     if (values[14]) {
       __pyx_v_max_ext_len = __Pyx_PyIndex_AsSsize_t(values[14]); if (unlikely((__pyx_v_max_ext_len == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 151, __pyx_L3_error)
     } else {
       __pyx_v_max_ext_len = ((Py_ssize_t)((Py_ssize_t)-1L));
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("unpackb", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 143, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -12725,15 +12619,15 @@
   PyObject *__pyx_t_12 = NULL;
   PyObject *__pyx_t_13 = NULL;
   PyObject *__pyx_t_14 = NULL;
   PyObject *__pyx_t_15 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("unpackb", 0);
+  __Pyx_RefNannySetupContext("unpackb", 1);
 
   /* "msgpack/_unpacker.pyx":166
  *     """
  *     cdef unpack_context ctx
  *     cdef Py_ssize_t off = 0             # <<<<<<<<<<<<<<
  *     cdef int ret
  * 
@@ -13254,48 +13148,35 @@
  */
 
 /* Python wrapper */
 static int __pyx_pw_7msgpack_9_cmsgpack_8Unpacker_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_7msgpack_9_cmsgpack_8Unpacker_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 320, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return -1;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 0, 0, __pyx_nargs); return -1;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_VARARGS(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__cinit__", 0))) return -1;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("msgpack._cmsgpack.Unpacker.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7msgpack_9_cmsgpack_8Unpacker___cinit__(((struct __pyx_obj_7msgpack_9_cmsgpack_Unpacker *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static int __pyx_pf_7msgpack_9_cmsgpack_8Unpacker___cinit__(struct __pyx_obj_7msgpack_9_cmsgpack_Unpacker *__pyx_v_self) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__cinit__", 0);
 
   /* "msgpack/_unpacker.pyx":321
  * 
  *     def __cinit__(self):
  *         self.buf = NULL             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
@@ -13308,15 +13189,14 @@
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.buf = NULL
  * 
  */
 
   /* function exit code */
   __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "msgpack/_unpacker.pyx":323
  *         self.buf = NULL
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
@@ -13334,16 +13214,14 @@
   __pyx_pf_7msgpack_9_cmsgpack_8Unpacker_2__dealloc__(((struct __pyx_obj_7msgpack_9_cmsgpack_Unpacker *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_7msgpack_9_cmsgpack_8Unpacker_2__dealloc__(struct __pyx_obj_7msgpack_9_cmsgpack_Unpacker *__pyx_v_self) {
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__dealloc__", 0);
 
   /* "msgpack/_unpacker.pyx":324
  * 
  *     def __dealloc__(self):
  *         PyMem_Free(self.buf)             # <<<<<<<<<<<<<<
  *         self.buf = NULL
  * 
@@ -13364,15 +13242,14 @@
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         PyMem_Free(self.buf)
  *         self.buf = NULL
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "msgpack/_unpacker.pyx":327
  *         self.buf = NULL
  * 
  *     def __init__(self, file_like=None, *, Py_ssize_t read_size=0,             # <<<<<<<<<<<<<<
  *                  bint use_list=True, bint raw=False, int timestamp=0, bint strict_map_key=True,
@@ -13407,16 +13284,15 @@
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 327, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return -1;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_file_like,&__pyx_n_s_read_size,&__pyx_n_s_use_list,&__pyx_n_s_raw,&__pyx_n_s_timestamp,&__pyx_n_s_strict_map_key,&__pyx_n_s_object_hook,&__pyx_n_s_object_pairs_hook,&__pyx_n_s_list_hook,&__pyx_n_s_unicode_errors,&__pyx_n_s_max_buffer_size,&__pyx_n_s_ext_hook,&__pyx_n_s_max_str_len,&__pyx_n_s_max_bin_len,&__pyx_n_s_max_array_len,&__pyx_n_s_max_map_len,&__pyx_n_s_max_ext_len,0};
     values[0] = __Pyx_Arg_NewRef_VARARGS(((PyObject *)Py_None));
 
     /* "msgpack/_unpacker.pyx":329
@@ -13542,18 +13418,19 @@
     }
     if (values[16]) {
       __pyx_v_max_ext_len = __Pyx_PyIndex_AsSsize_t(values[16]); if (unlikely((__pyx_v_max_ext_len == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 336, __pyx_L3_error)
     } else {
       __pyx_v_max_ext_len = ((Py_ssize_t)-1L);
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__init__", 0, 0, 1, __pyx_nargs); __PYX_ERR(1, 327, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -13591,15 +13468,15 @@
   long __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   char const *__pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__init__", 0);
+  __Pyx_RefNannySetupContext("__init__", 1);
 
   /* "msgpack/_unpacker.pyx":337
  *                  Py_ssize_t max_map_len=-1,
  *                  Py_ssize_t max_ext_len=-1):
  *         cdef const char *cerr=NULL             # <<<<<<<<<<<<<<
  * 
  *         self.object_hook = object_hook
@@ -14181,16 +14058,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("feed (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 387, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_next_bytes,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -14217,18 +14093,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_next_bytes = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("feed", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 387, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -14265,15 +14142,15 @@
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("feed", 0);
+  __Pyx_RefNannySetupContext("feed", 1);
 
   /* "msgpack/_unpacker.pyx":393
  *         cdef Py_ssize_t buf_len
  * 
  *         if self.file_like is not None:             # <<<<<<<<<<<<<<
  *             raise AssertionError(
  *                     "unpacker.feed() is not be able to use with `file_like`.")
@@ -14423,15 +14300,15 @@
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   Py_ssize_t __pyx_t_5;
   Py_ssize_t __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("append_buffer", 0);
+  __Pyx_RefNannySetupContext("append_buffer", 1);
 
   /* "msgpack/_unpacker.pyx":405
  *     cdef append_buffer(self, void* _buf, Py_ssize_t _buf_len):
  *         cdef:
  *             char* buf = self.buf             # <<<<<<<<<<<<<<
  *             char* new_buf
  *             Py_ssize_t head = self.buf_head
@@ -14779,15 +14656,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_t_9;
   char *__pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("read_from_file", 0);
+  __Pyx_RefNannySetupContext("read_from_file", 1);
 
   /* "msgpack/_unpacker.pyx":444
  * 
  *     cdef int read_from_file(self) except -1:
  *         cdef Py_ssize_t remains = self.max_buffer_size - (self.buf_tail - self.buf_head)             # <<<<<<<<<<<<<<
  *         if remains <= 0:
  *             raise BufferFull
@@ -14971,15 +14848,15 @@
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("_unpack", 0);
+  __Pyx_RefNannySetupContext("_unpack", 1);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_iter = __pyx_optional_args->iter;
     }
   }
 
   /* "msgpack/_unpacker.pyx":460
@@ -15350,16 +15227,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("read_bytes (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 487, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_nbytes,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -15386,18 +15262,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_nbytes = __Pyx_PyIndex_AsSsize_t(values[0]); if (unlikely((__pyx_v_nbytes == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 487, __pyx_L3_error)
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("read_bytes", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 487, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -15432,15 +15309,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("read_bytes", 0);
+  __Pyx_RefNannySetupContext("read_bytes", 1);
 
   /* "msgpack/_unpacker.pyx":490
  *         """Read a specified number of raw bytes from the stream"""
  *         cdef Py_ssize_t nread
  *         nread = min(self.buf_tail - self.buf_head, nbytes)             # <<<<<<<<<<<<<<
  *         ret = PyBytes_FromStringAndSize(self.buf + self.buf_head, nread)
  *         self.buf_head += nread
@@ -15622,54 +15499,43 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("unpack (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 499, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("unpack", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "unpack", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("msgpack._cmsgpack.Unpacker.unpack", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7msgpack_9_cmsgpack_8Unpacker_10unpack(((struct __pyx_obj_7msgpack_9_cmsgpack_Unpacker *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7msgpack_9_cmsgpack_8Unpacker_10unpack(struct __pyx_obj_7msgpack_9_cmsgpack_Unpacker *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("unpack", 0);
+  __Pyx_RefNannySetupContext("unpack", 1);
 
   /* "msgpack/_unpacker.pyx":504
  *         Raises `OutOfData` when there are no more bytes to unpack.
  *         """
  *         return self._unpack(unpack_construct)             # <<<<<<<<<<<<<<
  * 
  *     def skip(self):
@@ -15725,54 +15591,43 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("skip (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 506, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("skip", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "skip", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("msgpack._cmsgpack.Unpacker.skip", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7msgpack_9_cmsgpack_8Unpacker_12skip(((struct __pyx_obj_7msgpack_9_cmsgpack_Unpacker *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7msgpack_9_cmsgpack_8Unpacker_12skip(struct __pyx_obj_7msgpack_9_cmsgpack_Unpacker *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("skip", 0);
+  __Pyx_RefNannySetupContext("skip", 1);
 
   /* "msgpack/_unpacker.pyx":511
  *         Raises `OutOfData` when there are no more bytes to unpack.
  *         """
  *         return self._unpack(unpack_skip)             # <<<<<<<<<<<<<<
  * 
  *     def read_array_header(self):
@@ -15828,54 +15683,43 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("read_array_header (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 513, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("read_array_header", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "read_array_header", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("msgpack._cmsgpack.Unpacker.read_array_header", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7msgpack_9_cmsgpack_8Unpacker_14read_array_header(((struct __pyx_obj_7msgpack_9_cmsgpack_Unpacker *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7msgpack_9_cmsgpack_8Unpacker_14read_array_header(struct __pyx_obj_7msgpack_9_cmsgpack_Unpacker *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("read_array_header", 0);
+  __Pyx_RefNannySetupContext("read_array_header", 1);
 
   /* "msgpack/_unpacker.pyx":519
  *         Raises `OutOfData` when there are no more bytes to unpack.
  *         """
  *         return self._unpack(read_array_header)             # <<<<<<<<<<<<<<
  * 
  *     def read_map_header(self):
@@ -15931,54 +15775,43 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("read_map_header (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 521, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("read_map_header", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "read_map_header", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("msgpack._cmsgpack.Unpacker.read_map_header", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7msgpack_9_cmsgpack_8Unpacker_16read_map_header(((struct __pyx_obj_7msgpack_9_cmsgpack_Unpacker *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7msgpack_9_cmsgpack_8Unpacker_16read_map_header(struct __pyx_obj_7msgpack_9_cmsgpack_Unpacker *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("read_map_header", 0);
+  __Pyx_RefNannySetupContext("read_map_header", 1);
 
   /* "msgpack/_unpacker.pyx":527
  *         Raises `OutOfData` when there are no more bytes to unpack.
  *         """
  *         return self._unpack(read_map_header)             # <<<<<<<<<<<<<<
  * 
  *     def tell(self):
@@ -16034,54 +15867,43 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("tell (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 529, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("tell", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "tell", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("msgpack._cmsgpack.Unpacker.tell", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7msgpack_9_cmsgpack_8Unpacker_18tell(((struct __pyx_obj_7msgpack_9_cmsgpack_Unpacker *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7msgpack_9_cmsgpack_8Unpacker_18tell(struct __pyx_obj_7msgpack_9_cmsgpack_Unpacker *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("tell", 0);
+  __Pyx_RefNannySetupContext("tell", 1);
 
   /* "msgpack/_unpacker.pyx":534
  *         position of the next object.
  *         """
  *         return self.stream_offset             # <<<<<<<<<<<<<<
  * 
  *     def __iter__(self):
@@ -16134,15 +15956,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7msgpack_9_cmsgpack_8Unpacker_20__iter__(struct __pyx_obj_7msgpack_9_cmsgpack_Unpacker *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__iter__", 0);
+  __Pyx_RefNannySetupContext("__iter__", 1);
 
   /* "msgpack/_unpacker.pyx":537
  * 
  *     def __iter__(self):
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __next__(self):
@@ -16194,15 +16016,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   struct __pyx_opt_args_7msgpack_9_cmsgpack_8Unpacker__unpack __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__next__", 0);
+  __Pyx_RefNannySetupContext("__next__", 1);
 
   /* "msgpack/_unpacker.pyx":540
  * 
  *     def __next__(self):
  *         return self._unpack(unpack_construct, 1)             # <<<<<<<<<<<<<<
  * 
  *     # for debug.
@@ -16258,53 +16080,42 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(4, 1, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("msgpack._cmsgpack.Unpacker.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7msgpack_9_cmsgpack_8Unpacker_24__reduce_cython__(((struct __pyx_obj_7msgpack_9_cmsgpack_Unpacker *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7msgpack_9_cmsgpack_8Unpacker_24__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7msgpack_9_cmsgpack_Unpacker *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_RefNannySetupContext("__reduce_cython__", 1);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
@@ -16362,16 +16173,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(4, 3, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -16398,18 +16208,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v___pyx_state = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(4, 3, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -16432,15 +16243,15 @@
 
 static PyObject *__pyx_pf_7msgpack_9_cmsgpack_8Unpacker_26__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7msgpack_9_cmsgpack_Unpacker *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
   /* "(tree fragment)":4
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  */
   __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_no_default___reduce___due_to_non, 0, 0);
@@ -17747,39 +17558,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_2(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_8(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(6, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(6, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_2(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(7, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_8(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(7, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_2(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(8, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_8(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(8, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("datetime"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_8datetime_date = __Pyx_ImportType_3_0_2(__pyx_t_1, "datetime", "date", sizeof(PyDateTime_Date), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyDateTime_Date),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_7cpython_8datetime_date) __PYX_ERR(2, 70, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_time = __Pyx_ImportType_3_0_2(__pyx_t_1, "datetime", "time", sizeof(PyDateTime_Time), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyDateTime_Time),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_7cpython_8datetime_time) __PYX_ERR(2, 83, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_datetime = __Pyx_ImportType_3_0_2(__pyx_t_1, "datetime", "datetime", sizeof(PyDateTime_DateTime), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyDateTime_DateTime),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_7cpython_8datetime_datetime) __PYX_ERR(2, 109, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_timedelta = __Pyx_ImportType_3_0_2(__pyx_t_1, "datetime", "timedelta", sizeof(PyDateTime_Delta), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyDateTime_Delta),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_7cpython_8datetime_timedelta) __PYX_ERR(2, 147, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_tzinfo = __Pyx_ImportType_3_0_2(__pyx_t_1, "datetime", "tzinfo", sizeof(PyDateTime_TZInfo), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyDateTime_TZInfo),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_7cpython_8datetime_tzinfo) __PYX_ERR(2, 160, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_date = __Pyx_ImportType_3_0_8(__pyx_t_1, "datetime", "date", sizeof(PyDateTime_Date), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyDateTime_Date),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_7cpython_8datetime_date) __PYX_ERR(2, 70, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_time = __Pyx_ImportType_3_0_8(__pyx_t_1, "datetime", "time", sizeof(PyDateTime_Time), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyDateTime_Time),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_7cpython_8datetime_time) __PYX_ERR(2, 83, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_datetime = __Pyx_ImportType_3_0_8(__pyx_t_1, "datetime", "datetime", sizeof(PyDateTime_DateTime), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyDateTime_DateTime),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_7cpython_8datetime_datetime) __PYX_ERR(2, 109, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_timedelta = __Pyx_ImportType_3_0_8(__pyx_t_1, "datetime", "timedelta", sizeof(PyDateTime_Delta), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyDateTime_Delta),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_7cpython_8datetime_timedelta) __PYX_ERR(2, 147, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_tzinfo = __Pyx_ImportType_3_0_8(__pyx_t_1, "datetime", "tzinfo", sizeof(PyDateTime_TZInfo), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyDateTime_TZInfo),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_7cpython_8datetime_tzinfo) __PYX_ERR(2, 160, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -17986,42 +17797,40 @@
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("_cmsgpack", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(5, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to _cmsgpack pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "_cmsgpack" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(5, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(5, 1, __pyx_L1_error)
   #endif
   #endif
   CYTHON_UNUSED_VAR(__pyx_t_1);
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(5, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(5, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(5, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
+  __pyx_b = __Pyx_PyImport_AddModuleRef(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(5, 1, __pyx_L1_error)
+  __pyx_cython_runtime = __Pyx_PyImport_AddModuleRef((const char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(5, 1, __pyx_L1_error)
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(5, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
   __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit__cmsgpack(void)", 0);
-  if (__Pyx_check_binary_version() < 0) __PYX_ERR(5, 1, __pyx_L1_error)
+  if (__Pyx_check_binary_version(__PYX_LIMITED_VERSION_HEX, __Pyx_get_runtime_version(), CYTHON_COMPILING_IN_LIMITED_API) < 0) __PYX_ERR(5, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(5, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(5, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(5, 1, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
@@ -18722,14 +18531,16 @@
         if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
         #endif
             PyException_SetTraceback(value, tb);
     }
     tmp_value = tstate->current_exception;
     tstate->current_exception = value;
     Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
 #else
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     tmp_type = tstate->curexc_type;
     tmp_value = tstate->curexc_value;
     tmp_tb = tstate->curexc_traceback;
     tstate->curexc_type = type;
     tstate->curexc_value = value;
@@ -18779,33 +18590,40 @@
         return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
 #endif
     return PyObject_GetAttr(obj, attr_name);
 }
 #endif
 
 /* PyObjectGetAttrStrNoError */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
 static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         __Pyx_PyErr_Clear();
 }
+#endif
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
     PyObject *result;
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+    (void) PyObject_GetOptionalAttr(obj, attr_name, &result);
+    return result;
+#else
 #if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
         return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
     }
 #endif
     result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
     if (unlikely(!result)) {
         __Pyx_PyObject_GetAttrStr_ClearAttributeError();
     }
     return result;
+#endif
 }
 
 /* GetBuiltinName */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
     PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
     if (unlikely(!result) && !PyErr_Occurred()) {
         PyErr_Format(PyExc_NameError,
@@ -18841,16 +18659,21 @@
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
     ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
         PyErr_SetString(
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
@@ -19214,21 +19037,39 @@
     {
         if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
     for (i = 0; i < n; i++)
     {
         int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
         if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;  // error
+            if (unlikely(eq < 0)) return NULL;
             return kwvalues[i];
         }
     }
-    return NULL;  // not found (no exception set)
+    return NULL;
+}
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
+    Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
+    PyObject *dict;
+    dict = PyDict_New();
+    if (unlikely(!dict))
+        return NULL;
+    for (i=0; i<nkwargs; i++) {
+        PyObject *key = PyTuple_GET_ITEM(kwnames, i);
+        if (unlikely(PyDict_SetItem(dict, key, kwvalues[i]) < 0))
+            goto bad;
+    }
+    return dict;
+bad:
+    Py_DECREF(dict);
+    return NULL;
 }
 #endif
+#endif
 
 /* RaiseArgTupleInvalid */
 static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
     Py_ssize_t num_max,
@@ -19387,15 +19228,15 @@
 #endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_INCREF(value); // transfer ownership of value to values
+            Py_INCREF(value);
             Py_DECREF(key);
 #endif
             key = NULL;
             value = NULL;
             continue;
         }
 #if !CYTHON_AVOID_BORROWED_REFS
@@ -19406,15 +19247,15 @@
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL;  // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -19438,15 +19279,15 @@
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL; // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -19714,17 +19555,23 @@
     PyObject *kwtuple, **k;
     PyObject **d;
     Py_ssize_t nd;
     Py_ssize_t nk;
     PyObject *result;
     assert(kwargs == NULL || PyDict_Check(kwargs));
     nk = kwargs ? PyDict_Size(kwargs) : 0;
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
         return NULL;
     }
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object"))) {
+        return NULL;
+    }
+    #endif
     if (
 #if PY_MAJOR_VERSION >= 3
             co->co_kwonlyargcount == 0 &&
 #endif
             likely(kwargs == NULL || nk == 0) &&
             co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
         if (argdefs == NULL && co->co_argcount == nargs) {
@@ -19791,30 +19638,36 @@
 #endif
 
 /* PyObjectCallMethO */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
     PyObject *self, *result;
     PyCFunction cfunc;
-    cfunc = PyCFunction_GET_FUNCTION(func);
-    self = PyCFunction_GET_SELF(func);
+    cfunc = __Pyx_CyOrPyCFunction_GET_FUNCTION(func);
+    self = __Pyx_CyOrPyCFunction_GET_SELF(func);
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
     result = cfunc(self, arg);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
         PyErr_SetString(
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
 /* PyObjectFastCall */
+#if PY_VERSION_HEX < 0x03090000 || CYTHON_COMPILING_IN_LIMITED_API
 static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
     PyObject *argstuple;
     PyObject *result = 0;
     size_t i;
     argstuple = PyTuple_New((Py_ssize_t)nargs);
     if (unlikely(!argstuple)) return NULL;
     for (i = 0; i < nargs; i++) {
@@ -19822,36 +19675,25 @@
         if (__Pyx_PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]) < 0) goto bad;
     }
     result = __Pyx_PyObject_Call(func, argstuple, kwargs);
   bad:
     Py_DECREF(argstuple);
     return result;
 }
+#endif
 static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
     Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
 #if CYTHON_COMPILING_IN_CPYTHON
     if (nargs == 0 && kwargs == NULL) {
-#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
-        if (__Pyx_IsCyOrPyCFunction(func))
-#else
-        if (PyCFunction_Check(func))
-#endif
-        {
-            if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-                return __Pyx_PyObject_CallMethO(func, NULL);
-            }
-        }
+        if (__Pyx_CyOrPyCFunction_Check(func) && likely( __Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_NOARGS))
+            return __Pyx_PyObject_CallMethO(func, NULL);
     }
     else if (nargs == 1 && kwargs == NULL) {
-        if (PyCFunction_Check(func))
-        {
-            if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-                return __Pyx_PyObject_CallMethO(func, args[0]);
-            }
-        }
+        if (__Pyx_CyOrPyCFunction_Check(func) && likely( __Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_O))
+            return __Pyx_PyObject_CallMethO(func, args[0]);
     }
 #endif
     #if PY_VERSION_HEX < 0x030800B1
     #if CYTHON_FAST_PYCCALL
     if (PyCFunction_Check(func)) {
         if (kwargs) {
             return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
@@ -19867,33 +19709,39 @@
     #endif
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
     }
     #endif
     #endif
-    #if CYTHON_VECTORCALL
-    #if Py_VERSION_HEX < 0x03090000
-    vectorcallfunc f = _PyVectorcall_Function(func);
-    #else
-    vectorcallfunc f = PyVectorcall_Function(func);
-    #endif
-    if (f) {
-        return f(func, args, (size_t)nargs, kwargs);
-    }
-    #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
-    if (__Pyx_CyFunction_CheckExact(func)) {
-        __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
-        if (f) return f(func, args, (size_t)nargs, kwargs);
+    if (kwargs == NULL) {
+        #if CYTHON_VECTORCALL
+        #if PY_VERSION_HEX < 0x03090000
+        vectorcallfunc f = _PyVectorcall_Function(func);
+        #else
+        vectorcallfunc f = PyVectorcall_Function(func);
+        #endif
+        if (f) {
+            return f(func, args, (size_t)nargs, NULL);
+        }
+        #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
+        if (__Pyx_CyFunction_CheckExact(func)) {
+            __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
+            if (f) return f(func, args, (size_t)nargs, NULL);
+        }
+        #endif
     }
-    #endif
     if (nargs == 0) {
         return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
     }
+    #if PY_VERSION_HEX >= 0x03090000 && !CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_VectorcallDict(func, args, (size_t)nargs, kwargs);
+    #else
     return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
+    #endif
 }
 
 /* SwapException */
 #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
   #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
@@ -19944,30 +19792,31 @@
     *value = tmp_value;
     *tb = tmp_tb;
 }
 #endif
 
 /* IterFinish */
 static CYTHON_INLINE int __Pyx_IterFinish(void) {
+    PyObject* exc_type;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
-    PyObject* exc_type = __Pyx_PyErr_CurrentExceptionType();
+    exc_type = __Pyx_PyErr_CurrentExceptionType();
     if (unlikely(exc_type)) {
         if (unlikely(!__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration)))
             return -1;
         __Pyx_PyErr_Clear();
         return 0;
     }
     return 0;
 }
 
 /* PyObjectCallNoArg */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-    PyObject *arg = NULL;
-    return __Pyx_PyObject_FastCall(func, (&arg)+1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+    PyObject *arg[2] = {NULL, NULL};
+    return __Pyx_PyObject_FastCall(func, arg + 1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
 
 /* PyObjectCallOneArg */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
     PyObject *args[2] = {NULL, arg};
     return __Pyx_PyObject_FastCall(func, args+1, 1 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
@@ -20177,14 +20026,17 @@
     Py_XDECREF(value1);
     Py_XDECREF(value2);
     if (decref_tuple) { Py_XDECREF(tuple); }
     return -1;
 }
 
 /* dict_iter */
+#if CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
+#include <string.h>
+#endif
 static CYTHON_INLINE PyObject* __Pyx_dict_iterator(PyObject* iterable, int is_dict, PyObject* method_name,
                                                    Py_ssize_t* p_orig_length, int* p_source_is_dict) {
     is_dict = is_dict || likely(PyDict_CheckExact(iterable));
     *p_source_is_dict = is_dict;
     if (is_dict) {
 #if !CYTHON_COMPILING_IN_PYPY
         *p_orig_length = PyDict_Size(iterable);
@@ -20378,15 +20230,15 @@
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value)
 #else
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name)
 #endif
 {
     PyObject *result;
 #if !CYTHON_AVOID_BORROWED_REFS
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && PY_VERSION_HEX < 0x030d0000
     result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     } else if (unlikely(PyErr_Occurred())) {
         return NULL;
     }
@@ -20705,46 +20557,46 @@
                 "base class '" __Pyx_FMT_TYPENAME "' is not a heap type", b_name);
             __Pyx_DECREF_TypeName(b_name);
 #if CYTHON_AVOID_BORROWED_REFS
             Py_DECREF(b0);
 #endif
             return -1;
         }
-#if !CYTHON_USE_TYPE_SLOTS
-        if (dictoffset == 0) {
-            PyErr_Format(PyExc_TypeError,
-                "extension type '%s.200s': "
-                "unable to validate whether bases have a __dict__ "
-                "when CYTHON_USE_TYPE_SLOTS is off "
-                "(likely because you are building in the limited API). "
-                "Therefore, all extension types with multiple bases "
-                "must add 'cdef dict __dict__' in this compilation mode",
-                type_name);
-#if CYTHON_AVOID_BORROWED_REFS
-            Py_DECREF(b0);
-#endif
-            return -1;
-        }
-#else
-        if (dictoffset == 0 && b->tp_dictoffset)
+        if (dictoffset == 0)
         {
-            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
-            PyErr_Format(PyExc_TypeError,
-                "extension type '%.200s' has no __dict__ slot, "
-                "but base type '" __Pyx_FMT_TYPENAME "' has: "
-                "either add 'cdef dict __dict__' to the extension type "
-                "or add '__slots__ = [...]' to the base type",
-                type_name, b_name);
-            __Pyx_DECREF_TypeName(b_name);
+            Py_ssize_t b_dictoffset = 0;
+#if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
+            b_dictoffset = b->tp_dictoffset;
+#else
+            PyObject *py_b_dictoffset = PyObject_GetAttrString((PyObject*)b, "__dictoffset__");
+            if (!py_b_dictoffset) goto dictoffset_return;
+            b_dictoffset = PyLong_AsSsize_t(py_b_dictoffset);
+            Py_DECREF(py_b_dictoffset);
+            if (b_dictoffset == -1 && PyErr_Occurred()) goto dictoffset_return;
+#endif
+            if (b_dictoffset) {
+                {
+                    __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
+                    PyErr_Format(PyExc_TypeError,
+                        "extension type '%.200s' has no __dict__ slot, "
+                        "but base type '" __Pyx_FMT_TYPENAME "' has: "
+                        "either add 'cdef dict __dict__' to the extension type "
+                        "or add '__slots__ = [...]' to the base type",
+                        type_name, b_name);
+                    __Pyx_DECREF_TypeName(b_name);
+                }
+#if !(CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY)
+              dictoffset_return:
+#endif
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_DECREF(b0);
+                Py_DECREF(b0);
 #endif
-            return -1;
+                return -1;
+            }
         }
-#endif
 #if CYTHON_AVOID_BORROWED_REFS
         Py_DECREF(b0);
 #endif
     }
     return 0;
 }
 #endif
@@ -21082,18 +20934,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_2
-#define __PYX_HAVE_RT_ImportType_3_0_2
-static PyTypeObject *__Pyx_ImportType_3_0_2(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_2 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_8
+#define __PYX_HAVE_RT_ImportType_3_0_8
+static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -21139,23 +20991,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_2 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_8 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_2 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_8 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -21184,15 +21036,15 @@
     #endif
     empty_dict = PyDict_New();
     if (unlikely(!empty_dict))
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
-            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
+            if (strchr(__Pyx_MODULE_NAME, '.') != NULL) {
                 module = PyImport_ImportModuleLevelObject(
                     name, __pyx_d, empty_dict, from_list, 1);
                 if (unlikely(!module)) {
                     if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
                         goto bad;
                     PyErr_Clear();
                 }
@@ -21392,18 +21244,15 @@
         #endif
     }
     return value;
 }
 
 /* FetchSharedCythonModule */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
-    PyObject *abi_module = PyImport_AddModule((char*) __PYX_ABI_MODULE_NAME);
-    if (unlikely(!abi_module)) return NULL;
-    Py_INCREF(abi_module);
-    return abi_module;
+    return __Pyx_PyImport_AddModuleRef((char*) __PYX_ABI_MODULE_NAME);
 }
 
 /* FetchCommonType */
 static int __Pyx_VerifyCachedType(PyObject *cached_type,
                                const char *name,
                                Py_ssize_t basicsize,
                                Py_ssize_t expected_basicsize) {
@@ -21556,14 +21405,28 @@
         return vc(func, args, nargs, NULL);
     }
     return __Pyx_PyVectorcall_FastCallDict_kw(func, vc, args, nargs, kw);
 }
 #endif
 
 /* CythonFunctionShared */
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc) {
+    if (__Pyx_CyFunction_Check(func)) {
+        return PyCFunction_GetFunction(((__pyx_CyFunctionObject*)func)->func) == (PyCFunction) cfunc;
+    } else if (PyCFunction_Check(func)) {
+        return PyCFunction_GetFunction(func) == (PyCFunction) cfunc;
+    }
+    return 0;
+}
+#else
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc) {
+    return __Pyx_CyOrPyCFunction_Check(func) && __Pyx_CyOrPyCFunction_GET_FUNCTION(func) == (PyCFunction) cfunc;
+}
+#endif
 static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     __Pyx_Py_XDECREF_SET(
         __Pyx_CyFunction_GetClassObj(f),
             ((classobj) ? __Pyx_NewRef(classobj) : NULL));
 #else
     __Pyx_Py_XDECREF_SET(
@@ -22704,16 +22567,16 @@
     replace = PyObject_GetAttrString(code, "replace");
     if (likely(replace)) {
         PyObject *result;
         result = PyObject_Call(replace, __pyx_empty_tuple, scratch_dict);
         Py_DECREF(replace);
         return result;
     }
-    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
     PyErr_Clear();
+    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
     {
         PyObject *compiled = NULL, *result = NULL;
         if (unlikely(PyDict_SetItemString(scratch_dict, "code", code))) return NULL;
         if (unlikely(PyDict_SetItemString(scratch_dict, "type", (PyObject*)(&PyType_Type)))) return NULL;
         compiled = Py_CompileString(
             "out = type(code)(\n"
             "  code.co_argcount, code.co_kwonlyargcount, code.co_nlocals, code.co_stacksize,\n"
@@ -22725,14 +22588,16 @@
         Py_DECREF(compiled);
         if (!result) PyErr_Print();
         Py_DECREF(result);
         result = PyDict_GetItemString(scratch_dict, "out");
         if (result) Py_INCREF(result);
         return result;
     }
+    #else
+    return NULL;
     #endif
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyObject *code_object = NULL, *py_py_line = NULL, *py_funcname = NULL, *dict = NULL;
     PyObject *replace = NULL, *getframe = NULL, *frame = NULL;
     PyObject *exc_type, *exc_value, *exc_traceback;
@@ -22822,15 +22687,15 @@
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
     #else
     py_code = PyCode_NewEmpty(filename, funcname, py_line);
     #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_XDECREF(py_funcname);
     return py_code;
 bad:
     Py_XDECREF(py_funcname);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
     #endif
     return NULL;
@@ -23063,15 +22928,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -23336,15 +23201,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -23472,38 +23337,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(int));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntFromPy */
 static CYTHON_INLINE unsigned PY_LONG_LONG __Pyx_PyInt_As_unsigned_PY_LONG_LONG(PyObject *x) {
@@ -23671,15 +23538,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -23944,15 +23811,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -24217,15 +24084,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -24490,15 +24357,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -24626,38 +24493,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(uint64_t),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(uint64_t));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* FormatTypeName */
 #if CYTHON_COMPILING_IN_LIMITED_API
@@ -24704,38 +24573,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* FastTypeChecks */
 #if CYTHON_COMPILING_IN_CPYTHON
@@ -24850,49 +24721,58 @@
         return __Pyx_inner_PyErr_GivenExceptionMatches2(err, exc_type1, exc_type2);
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
-static int __Pyx_check_binary_version(void) {
-    char ctversion[5];
-    int same=1, i, found_dot;
-    const char* rt_from_call = Py_GetVersion();
-    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    found_dot = 0;
-    for (i = 0; i < 4; i++) {
-        if (!ctversion[i]) {
-            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
-            break;
+static unsigned long __Pyx_get_runtime_version(void) {
+#if __PYX_LIMITED_VERSION_HEX >= 0x030B00A4
+    return Py_Version & ~0xFFUL;
+#else
+    const char* rt_version = Py_GetVersion();
+    unsigned long version = 0;
+    unsigned long factor = 0x01000000UL;
+    unsigned int digit = 0;
+    int i = 0;
+    while (factor) {
+        while ('0' <= rt_version[i] && rt_version[i] <= '9') {
+            digit = digit * 10 + (unsigned int) (rt_version[i] - '0');
+            ++i;
         }
-        if (rt_from_call[i] != ctversion[i]) {
-            same = 0;
+        version += factor * digit;
+        if (rt_version[i] != '.')
             break;
-        }
+        digit = 0;
+        factor >>= 8;
+        ++i;
     }
-    if (!same) {
-        char rtversion[5] = {'\0'};
+    return version;
+#endif
+}
+static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer) {
+    const unsigned long MAJOR_MINOR = 0xFFFF0000UL;
+    if ((rt_version & MAJOR_MINOR) == (ct_version & MAJOR_MINOR))
+        return 0;
+    if (likely(allow_newer && (rt_version & MAJOR_MINOR) > (ct_version & MAJOR_MINOR)))
+        return 1;
+    {
         char message[200];
-        for (i=0; i<4; ++i) {
-            if (rt_from_call[i] == '.') {
-                if (found_dot) break;
-                found_dot = 1;
-            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
-                break;
-            }
-            rtversion[i] = rt_from_call[i];
-        }
         PyOS_snprintf(message, sizeof(message),
-                      "compile time version %s of module '%.100s' "
-                      "does not match runtime version %s",
-                      ctversion, __Pyx_MODULE_NAME, rtversion);
+                      "compile time Python version %d.%d "
+                      "of module '%.100s' "
+                      "%s "
+                      "runtime version %d.%d",
+                       (int) (ct_version >> 24), (int) ((ct_version >> 16) & 0xFF),
+                       __Pyx_MODULE_NAME,
+                       (allow_newer) ? "was newer than" : "does not match",
+                       (int) (rt_version >> 24), (int) ((rt_version >> 16) & 0xFF)
+       );
         return PyErr_WarnEx(NULL, message, 1);
     }
-    return 0;
 }
 
 /* InitStrings */
 #if PY_MAJOR_VERSION >= 3
 static int __Pyx_InitString(__Pyx_StringTabEntry t, PyObject **str) {
     if (t.is_unicode | t.is_str) {
         if (t.intern) {
@@ -24930,16 +24810,32 @@
             return -1;
         #endif
         ++t;
     }
     return 0;
 }
 
+#include <string.h>
+static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s) {
+    size_t len = strlen(s);
+    if (unlikely(len > (size_t) PY_SSIZE_T_MAX)) {
+        PyErr_SetString(PyExc_OverflowError, "byte string is too long");
+        return -1;
+    }
+    return (Py_ssize_t) len;
+}
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char* c_str) {
-    return __Pyx_PyUnicode_FromStringAndSize(c_str, (Py_ssize_t)strlen(c_str));
+    Py_ssize_t len = __Pyx_ssize_strlen(c_str);
+    if (unlikely(len < 0)) return NULL;
+    return __Pyx_PyUnicode_FromStringAndSize(c_str, len);
+}
+static CYTHON_INLINE PyObject* __Pyx_PyByteArray_FromString(const char* c_str) {
+    Py_ssize_t len = __Pyx_ssize_strlen(c_str);
+    if (unlikely(len < 0)) return NULL;
+    return PyByteArray_FromStringAndSize(c_str, len);
 }
 static CYTHON_INLINE const char* __Pyx_PyObject_AsString(PyObject* o) {
     Py_ssize_t ignore;
     return __Pyx_PyObject_AsStringAndSize(o, &ignore);
 }
 #if __PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT
 #if !CYTHON_PEP393_ENABLED
```

### Comparing `msgpack-1.0.7/msgpack/_packer.pyx` & `msgpack-1.0.8/msgpack/_packer.pyx`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/msgpack/_unpacker.pyx` & `msgpack-1.0.8/msgpack/_unpacker.pyx`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/msgpack/exceptions.py` & `msgpack-1.0.8/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/msgpack/ext.py` & `msgpack-1.0.8/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/msgpack/fallback.py` & `msgpack-1.0.8/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/msgpack/pack.h` & `msgpack-1.0.8/msgpack/pack.h`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/msgpack/pack_template.h` & `msgpack-1.0.8/msgpack/pack_template.h`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/msgpack/sysdep.h` & `msgpack-1.0.8/msgpack/sysdep.h`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/msgpack/unpack.h` & `msgpack-1.0.8/msgpack/unpack.h`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/msgpack/unpack_define.h` & `msgpack-1.0.8/msgpack/unpack_define.h`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/msgpack/unpack_template.h` & `msgpack-1.0.8/msgpack/unpack_template.h`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/msgpack.egg-info/PKG-INFO` & `msgpack-1.0.8/msgpack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgpack
-Version: 1.0.7
+Version: 1.0.8
 Summary: MessagePack serializer
 Author-email: Inada Naoki <songofacandy@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://msgpack.org/
 Project-URL: Documentation, https://msgpack-python.readthedocs.io/
 Project-URL: Repository, https://github.com/msgpack/msgpack-python/
 Project-URL: Tracker, https://github.com/msgpack/msgpack-python/issues
```

### Comparing `msgpack-1.0.7/msgpack.egg-info/SOURCES.txt` & `msgpack-1.0.8/msgpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/pyproject.toml` & `msgpack-1.0.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 requires = [
     # Also declared in requirements.txt, if updating here please also update
     # there
-    "Cython~=3.0.0",
+    "Cython~=3.0.8",
     "setuptools >= 35.0.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msgpack"
 dynamic = ["version"]
@@ -35,14 +35,18 @@
 [project.urls]
 Homepage = "https://msgpack.org/"
 Documentation = "https://msgpack-python.readthedocs.io/"
 Repository = "https://github.com/msgpack/msgpack-python/"
 Tracker = "https://github.com/msgpack/msgpack-python/issues"
 Changelog = "https://github.com/msgpack/msgpack-python/blob/main/ChangeLog.rst"
 
+[tool.setuptools]
+# Do not install C/C++/Cython source files
+include-package-data = false
+
 [tool.setuptools.dynamic]
 version = {attr = "msgpack.__version__"}
 
 [tool.black]
 line-length = 100
 target-version = ["py37"]
 skip_string_normalization = true
```

### Comparing `msgpack-1.0.7/setup.py` & `msgpack-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/test/test_buffer.py` & `msgpack-1.0.8/test/test_buffer.py`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/test/test_case.py` & `msgpack-1.0.8/test/test_case.py`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/test/test_except.py` & `msgpack-1.0.8/test/test_except.py`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/test/test_extension.py` & `msgpack-1.0.8/test/test_extension.py`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/test/test_format.py` & `msgpack-1.0.8/test/test_format.py`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/test/test_limits.py` & `msgpack-1.0.8/test/test_limits.py`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/test/test_memoryview.py` & `msgpack-1.0.8/test/test_memoryview.py`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/test/test_newspec.py` & `msgpack-1.0.8/test/test_newspec.py`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/test/test_obj.py` & `msgpack-1.0.8/test/test_obj.py`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/test/test_pack.py` & `msgpack-1.0.8/test/test_pack.py`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/test/test_read_size.py` & `msgpack-1.0.8/test/test_read_size.py`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/test/test_seq.py` & `msgpack-1.0.8/test/test_seq.py`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/test/test_sequnpack.py` & `msgpack-1.0.8/test/test_sequnpack.py`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/test/test_stricttype.py` & `msgpack-1.0.8/test/test_stricttype.py`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/test/test_timestamp.py` & `msgpack-1.0.8/test/test_timestamp.py`

 * *Files identical despite different names*

### Comparing `msgpack-1.0.7/test/test_unpack.py` & `msgpack-1.0.8/test/test_unpack.py`

 * *Files identical despite different names*

