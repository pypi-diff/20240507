# Comparing `tmp/jxlpy-0.9.4.tar.gz` & `tmp/jxlpy-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jxlpy-0.9.4.tar", last modified: Sat Mar  2 18:09:01 2024, max compression
+gzip compressed data, was "jxlpy-0.9.5.tar", last modified: Tue May  7 08:49:21 2024, max compression
```

## Comparing `jxlpy-0.9.4.tar` & `jxlpy-0.9.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 18:09:01.807567 jxlpy-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-02 18:06:17.000000 jxlpy-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-03-02 18:09:01.807567 jxlpy-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-03-02 18:06:17.000000 jxlpy-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 18:09:01.803568 jxlpy-0.9.4/_jxlpy/
--rw-r--r--   0 runner    (1001) docker     (127)   851079 2024-03-02 18:09:01.000000 jxlpy-0.9.4/_jxlpy/_jxl.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 18:09:01.803568 jxlpy-0.9.4/jxlpy/
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-03-02 18:06:17.000000 jxlpy-0.9.4/jxlpy/JXLImagePlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-02 18:06:17.000000 jxlpy-0.9.4/jxlpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 18:09:01.807567 jxlpy-0.9.4/jxlpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-03-02 18:09:01.000000 jxlpy-0.9.4/jxlpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-02 18:09:01.000000 jxlpy-0.9.4/jxlpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 18:09:01.000000 jxlpy-0.9.4/jxlpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-02 18:09:01.000000 jxlpy-0.9.4/jxlpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-02 18:09:01.000000 jxlpy-0.9.4/jxlpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-02 18:06:17.000000 jxlpy-0.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-02 18:09:01.807567 jxlpy-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-03-02 18:06:17.000000 jxlpy-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:49:21.759989 jxlpy-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-07 08:46:33.000000 jxlpy-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-07 08:49:21.759989 jxlpy-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-07 08:46:33.000000 jxlpy-0.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:49:21.755989 jxlpy-0.9.5/_jxlpy/
+-rw-r--r--   0 runner    (1001) docker     (127)   851026 2024-05-07 08:49:21.000000 jxlpy-0.9.5/_jxlpy/_jxl.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:49:21.759989 jxlpy-0.9.5/jxlpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-07 08:46:33.000000 jxlpy-0.9.5/jxlpy/JXLImagePlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-07 08:46:33.000000 jxlpy-0.9.5/jxlpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:49:21.759989 jxlpy-0.9.5/jxlpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-07 08:49:21.000000 jxlpy-0.9.5/jxlpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-07 08:49:21.000000 jxlpy-0.9.5/jxlpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 08:49:21.000000 jxlpy-0.9.5/jxlpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-07 08:49:21.000000 jxlpy-0.9.5/jxlpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 08:49:21.000000 jxlpy-0.9.5/jxlpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-07 08:46:33.000000 jxlpy-0.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 08:49:21.759989 jxlpy-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-07 08:46:33.000000 jxlpy-0.9.5/setup.py
```

### Comparing `jxlpy-0.9.4/LICENSE` & `jxlpy-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jxlpy-0.9.4/PKG-INFO` & `jxlpy-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jxlpy
-Version: 0.9.4
+Version: 0.9.5
 Summary: JPEG XL integration in Python
 Home-page: http://github.com/olokelo/jxlpy
 Author: oloke
 Author-email: olokelo@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `jxlpy-0.9.4/README.md` & `jxlpy-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `jxlpy-0.9.4/_jxlpy/_jxl.cpp` & `jxlpy-0.9.5/_jxlpy/_jxl.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "-O2"
@@ -41,18 +41,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -136,14 +136,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -197,14 +199,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -258,60 +262,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -394,14 +421,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -753,16 +783,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1106,15 +1141,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1193,15 +1228,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1320,32 +1355,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -2403,15 +2421,15 @@
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_math[] = "math";
 static const char __pyx_k_name[] = "name";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_size[] = "size";
 static const char __pyx_k_spec[] = "__spec__";
 static const char __pyx_k_test[] = "__test__";
-static const char __pyx_k_0_9_4[] = "0.9.4";
+static const char __pyx_k_0_9_5[] = "0.9.5";
 static const char __pyx_k_bytes[] = "bytes";
 static const char __pyx_k_close[] = "close";
 static const char __pyx_k_float[] = "float";
 static const char __pyx_k_jxlpy[] = "_jxlpy";
 static const char __pyx_k_print[] = "print";
 static const char __pyx_k_range[] = "_range";
 static const char __pyx_k_super[] = "super";
@@ -2630,15 +2648,15 @@
   #endif
   #if CYTHON_USE_MODULE_STATE
   PyObject *__pyx_type_6_jxlpy_JXLPyEncoder;
   PyObject *__pyx_type_6_jxlpy_JXLPyDecoder;
   #endif
   PyTypeObject *__pyx_ptype_6_jxlpy_JXLPyEncoder;
   PyTypeObject *__pyx_ptype_6_jxlpy_JXLPyDecoder;
-  PyObject *__pyx_kp_u_0_9_4;
+  PyObject *__pyx_kp_u_0_9_5;
   PyObject *__pyx_kp_u_Floating_point_decoding_not_supp;
   PyObject *__pyx_n_s_JXLPyDecoder;
   PyObject *__pyx_n_s_JXLPyDecoder___reduce_cython;
   PyObject *__pyx_n_s_JXLPyDecoder___setstate_cython;
   PyObject *__pyx_n_s_JXLPyDecoder_close;
   PyObject *__pyx_n_s_JXLPyDecoder_get_colorspace;
   PyObject *__pyx_n_s_JXLPyDecoder_get_frame;
@@ -2834,19 +2852,17 @@
   PyObject *__pyx_float_6_4;
   PyObject *__pyx_float_0_09;
   PyObject *__pyx_float_6_25;
   PyObject *__pyx_float_0_235;
   PyObject *__pyx_float_12_65;
   PyObject *__pyx_int_0;
   PyObject *__pyx_int_1;
-  PyObject *__pyx_int_3;
   PyObject *__pyx_int_4;
   PyObject *__pyx_int_7;
   PyObject *__pyx_int_8;
-  PyObject *__pyx_int_9;
   PyObject *__pyx_int_10;
   PyObject *__pyx_int_16;
   PyObject *__pyx_int_30;
   PyObject *__pyx_int_32;
   PyObject *__pyx_int_100;
   PyObject *__pyx_k_;
   PyObject *__pyx_k__2;
@@ -2938,15 +2954,15 @@
   #ifdef __Pyx_FusedFunction_USED
   Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
   #endif
   Py_CLEAR(clear_module_state->__pyx_ptype_6_jxlpy_JXLPyEncoder);
   Py_CLEAR(clear_module_state->__pyx_type_6_jxlpy_JXLPyEncoder);
   Py_CLEAR(clear_module_state->__pyx_ptype_6_jxlpy_JXLPyDecoder);
   Py_CLEAR(clear_module_state->__pyx_type_6_jxlpy_JXLPyDecoder);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_0_9_4);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_0_9_5);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Floating_point_decoding_not_supp);
   Py_CLEAR(clear_module_state->__pyx_n_s_JXLPyDecoder);
   Py_CLEAR(clear_module_state->__pyx_n_s_JXLPyDecoder___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_JXLPyDecoder___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_JXLPyDecoder_close);
   Py_CLEAR(clear_module_state->__pyx_n_s_JXLPyDecoder_get_colorspace);
   Py_CLEAR(clear_module_state->__pyx_n_s_JXLPyDecoder_get_frame);
@@ -3142,19 +3158,17 @@
   Py_CLEAR(clear_module_state->__pyx_float_6_4);
   Py_CLEAR(clear_module_state->__pyx_float_0_09);
   Py_CLEAR(clear_module_state->__pyx_float_6_25);
   Py_CLEAR(clear_module_state->__pyx_float_0_235);
   Py_CLEAR(clear_module_state->__pyx_float_12_65);
   Py_CLEAR(clear_module_state->__pyx_int_0);
   Py_CLEAR(clear_module_state->__pyx_int_1);
-  Py_CLEAR(clear_module_state->__pyx_int_3);
   Py_CLEAR(clear_module_state->__pyx_int_4);
   Py_CLEAR(clear_module_state->__pyx_int_7);
   Py_CLEAR(clear_module_state->__pyx_int_8);
-  Py_CLEAR(clear_module_state->__pyx_int_9);
   Py_CLEAR(clear_module_state->__pyx_int_10);
   Py_CLEAR(clear_module_state->__pyx_int_16);
   Py_CLEAR(clear_module_state->__pyx_int_30);
   Py_CLEAR(clear_module_state->__pyx_int_32);
   Py_CLEAR(clear_module_state->__pyx_int_100);
   Py_CLEAR(clear_module_state->__pyx_k_);
   Py_CLEAR(clear_module_state->__pyx_k__2);
@@ -3224,15 +3238,15 @@
   #ifdef __Pyx_FusedFunction_USED
   Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
   #endif
   Py_VISIT(traverse_module_state->__pyx_ptype_6_jxlpy_JXLPyEncoder);
   Py_VISIT(traverse_module_state->__pyx_type_6_jxlpy_JXLPyEncoder);
   Py_VISIT(traverse_module_state->__pyx_ptype_6_jxlpy_JXLPyDecoder);
   Py_VISIT(traverse_module_state->__pyx_type_6_jxlpy_JXLPyDecoder);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_0_9_4);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_0_9_5);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Floating_point_decoding_not_supp);
   Py_VISIT(traverse_module_state->__pyx_n_s_JXLPyDecoder);
   Py_VISIT(traverse_module_state->__pyx_n_s_JXLPyDecoder___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_JXLPyDecoder___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_JXLPyDecoder_close);
   Py_VISIT(traverse_module_state->__pyx_n_s_JXLPyDecoder_get_colorspace);
   Py_VISIT(traverse_module_state->__pyx_n_s_JXLPyDecoder_get_frame);
@@ -3428,19 +3442,17 @@
   Py_VISIT(traverse_module_state->__pyx_float_6_4);
   Py_VISIT(traverse_module_state->__pyx_float_0_09);
   Py_VISIT(traverse_module_state->__pyx_float_6_25);
   Py_VISIT(traverse_module_state->__pyx_float_0_235);
   Py_VISIT(traverse_module_state->__pyx_float_12_65);
   Py_VISIT(traverse_module_state->__pyx_int_0);
   Py_VISIT(traverse_module_state->__pyx_int_1);
-  Py_VISIT(traverse_module_state->__pyx_int_3);
   Py_VISIT(traverse_module_state->__pyx_int_4);
   Py_VISIT(traverse_module_state->__pyx_int_7);
   Py_VISIT(traverse_module_state->__pyx_int_8);
-  Py_VISIT(traverse_module_state->__pyx_int_9);
   Py_VISIT(traverse_module_state->__pyx_int_10);
   Py_VISIT(traverse_module_state->__pyx_int_16);
   Py_VISIT(traverse_module_state->__pyx_int_30);
   Py_VISIT(traverse_module_state->__pyx_int_32);
   Py_VISIT(traverse_module_state->__pyx_int_100);
   Py_VISIT(traverse_module_state->__pyx_k_);
   Py_VISIT(traverse_module_state->__pyx_k__2);
@@ -3528,15 +3540,15 @@
 #endif
 #if CYTHON_USE_MODULE_STATE
 #define __pyx_type_6_jxlpy_JXLPyEncoder __pyx_mstate_global->__pyx_type_6_jxlpy_JXLPyEncoder
 #define __pyx_type_6_jxlpy_JXLPyDecoder __pyx_mstate_global->__pyx_type_6_jxlpy_JXLPyDecoder
 #endif
 #define __pyx_ptype_6_jxlpy_JXLPyEncoder __pyx_mstate_global->__pyx_ptype_6_jxlpy_JXLPyEncoder
 #define __pyx_ptype_6_jxlpy_JXLPyDecoder __pyx_mstate_global->__pyx_ptype_6_jxlpy_JXLPyDecoder
-#define __pyx_kp_u_0_9_4 __pyx_mstate_global->__pyx_kp_u_0_9_4
+#define __pyx_kp_u_0_9_5 __pyx_mstate_global->__pyx_kp_u_0_9_5
 #define __pyx_kp_u_Floating_point_decoding_not_supp __pyx_mstate_global->__pyx_kp_u_Floating_point_decoding_not_supp
 #define __pyx_n_s_JXLPyDecoder __pyx_mstate_global->__pyx_n_s_JXLPyDecoder
 #define __pyx_n_s_JXLPyDecoder___reduce_cython __pyx_mstate_global->__pyx_n_s_JXLPyDecoder___reduce_cython
 #define __pyx_n_s_JXLPyDecoder___setstate_cython __pyx_mstate_global->__pyx_n_s_JXLPyDecoder___setstate_cython
 #define __pyx_n_s_JXLPyDecoder_close __pyx_mstate_global->__pyx_n_s_JXLPyDecoder_close
 #define __pyx_n_s_JXLPyDecoder_get_colorspace __pyx_mstate_global->__pyx_n_s_JXLPyDecoder_get_colorspace
 #define __pyx_n_s_JXLPyDecoder_get_frame __pyx_mstate_global->__pyx_n_s_JXLPyDecoder_get_frame
@@ -3732,19 +3744,17 @@
 #define __pyx_float_6_4 __pyx_mstate_global->__pyx_float_6_4
 #define __pyx_float_0_09 __pyx_mstate_global->__pyx_float_0_09
 #define __pyx_float_6_25 __pyx_mstate_global->__pyx_float_6_25
 #define __pyx_float_0_235 __pyx_mstate_global->__pyx_float_0_235
 #define __pyx_float_12_65 __pyx_mstate_global->__pyx_float_12_65
 #define __pyx_int_0 __pyx_mstate_global->__pyx_int_0
 #define __pyx_int_1 __pyx_mstate_global->__pyx_int_1
-#define __pyx_int_3 __pyx_mstate_global->__pyx_int_3
 #define __pyx_int_4 __pyx_mstate_global->__pyx_int_4
 #define __pyx_int_7 __pyx_mstate_global->__pyx_int_7
 #define __pyx_int_8 __pyx_mstate_global->__pyx_int_8
-#define __pyx_int_9 __pyx_mstate_global->__pyx_int_9
 #define __pyx_int_10 __pyx_mstate_global->__pyx_int_10
 #define __pyx_int_16 __pyx_mstate_global->__pyx_int_16
 #define __pyx_int_30 __pyx_mstate_global->__pyx_int_30
 #define __pyx_int_32 __pyx_mstate_global->__pyx_int_32
 #define __pyx_int_100 __pyx_mstate_global->__pyx_int_100
 #define __pyx_k_ __pyx_mstate_global->__pyx_k_
 #define __pyx_k__2 __pyx_mstate_global->__pyx_k__2
@@ -5356,15 +5366,15 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 1);
 
   /* "_jxlpy/_jxl.pyx":1050
  *                  endianness: str='native', num_threads: int=0, icc_profile: bytes=b''):
  * 
  *         _check_arg(quality, 'quality', (0, 100))             # <<<<<<<<<<<<<<
- *         _check_arg(effort, 'effort', (3, 9))
+ *         _check_arg(effort, 'effort', (1, 10))
  *         _check_arg(decoding_speed, 'decoding_speed', (0, 4))
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_check_arg); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1050, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
@@ -5388,15 +5398,15 @@
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "_jxlpy/_jxl.pyx":1051
  * 
  *         _check_arg(quality, 'quality', (0, 100))
- *         _check_arg(effort, 'effort', (3, 9))             # <<<<<<<<<<<<<<
+ *         _check_arg(effort, 'effort', (1, 10))             # <<<<<<<<<<<<<<
  *         _check_arg(decoding_speed, 'decoding_speed', (0, 4))
  *         _check_arg(num_threads, 'num_threads', (0, 32))
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_check_arg); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1051, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
@@ -5420,15 +5430,15 @@
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "_jxlpy/_jxl.pyx":1052
  *         _check_arg(quality, 'quality', (0, 100))
- *         _check_arg(effort, 'effort', (3, 9))
+ *         _check_arg(effort, 'effort', (1, 10))
  *         _check_arg(decoding_speed, 'decoding_speed', (0, 4))             # <<<<<<<<<<<<<<
  *         _check_arg(num_threads, 'num_threads', (0, 32))
  *         _check_arg(bit_depth, 'bit_depth', (1, 16))
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_check_arg); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1052, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
@@ -5452,15 +5462,15 @@
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1052, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "_jxlpy/_jxl.pyx":1053
- *         _check_arg(effort, 'effort', (3, 9))
+ *         _check_arg(effort, 'effort', (1, 10))
  *         _check_arg(decoding_speed, 'decoding_speed', (0, 4))
  *         _check_arg(num_threads, 'num_threads', (0, 32))             # <<<<<<<<<<<<<<
  *         _check_arg(bit_depth, 'bit_depth', (1, 16))
  *         # alpha_bit_depth is ignored if appropriate colorspace is not set, however it also can be 0
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_check_arg); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1053, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
@@ -11947,15 +11957,15 @@
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 /* #### Code section: pystring_table ### */
 
 static int __Pyx_CreateStringTabAndInitStrings(void) {
   __Pyx_StringTabEntry __pyx_string_tab[] = {
-    {&__pyx_kp_u_0_9_4, __pyx_k_0_9_4, sizeof(__pyx_k_0_9_4), 0, 1, 0, 0},
+    {&__pyx_kp_u_0_9_5, __pyx_k_0_9_5, sizeof(__pyx_k_0_9_5), 0, 1, 0, 0},
     {&__pyx_kp_u_Floating_point_decoding_not_supp, __pyx_k_Floating_point_decoding_not_supp, sizeof(__pyx_k_Floating_point_decoding_not_supp), 0, 1, 0, 0},
     {&__pyx_n_s_JXLPyDecoder, __pyx_k_JXLPyDecoder, sizeof(__pyx_k_JXLPyDecoder), 0, 0, 1, 1},
     {&__pyx_n_s_JXLPyDecoder___reduce_cython, __pyx_k_JXLPyDecoder___reduce_cython, sizeof(__pyx_k_JXLPyDecoder___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_JXLPyDecoder___setstate_cython, __pyx_k_JXLPyDecoder___setstate_cython, sizeof(__pyx_k_JXLPyDecoder___setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_JXLPyDecoder_close, __pyx_k_JXLPyDecoder_close, sizeof(__pyx_k_JXLPyDecoder_close), 0, 0, 1, 1},
     {&__pyx_n_s_JXLPyDecoder_get_colorspace, __pyx_k_JXLPyDecoder_get_colorspace, sizeof(__pyx_k_JXLPyDecoder_get_colorspace), 0, 0, 1, 1},
     {&__pyx_n_s_JXLPyDecoder_get_frame, __pyx_k_JXLPyDecoder_get_frame, sizeof(__pyx_k_JXLPyDecoder_get_frame), 0, 0, 1, 1},
@@ -12167,45 +12177,45 @@
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
   /* "_jxlpy/_jxl.pyx":1050
  *                  endianness: str='native', num_threads: int=0, icc_profile: bytes=b''):
  * 
  *         _check_arg(quality, 'quality', (0, 100))             # <<<<<<<<<<<<<<
- *         _check_arg(effort, 'effort', (3, 9))
+ *         _check_arg(effort, 'effort', (1, 10))
  *         _check_arg(decoding_speed, 'decoding_speed', (0, 4))
  */
   __pyx_tuple__7 = PyTuple_Pack(2, __pyx_int_0, __pyx_int_100); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 1050, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
   /* "_jxlpy/_jxl.pyx":1051
  * 
  *         _check_arg(quality, 'quality', (0, 100))
- *         _check_arg(effort, 'effort', (3, 9))             # <<<<<<<<<<<<<<
+ *         _check_arg(effort, 'effort', (1, 10))             # <<<<<<<<<<<<<<
  *         _check_arg(decoding_speed, 'decoding_speed', (0, 4))
  *         _check_arg(num_threads, 'num_threads', (0, 32))
  */
-  __pyx_tuple__8 = PyTuple_Pack(2, __pyx_int_3, __pyx_int_9); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 1051, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(2, __pyx_int_1, __pyx_int_10); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 1051, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
   /* "_jxlpy/_jxl.pyx":1052
  *         _check_arg(quality, 'quality', (0, 100))
- *         _check_arg(effort, 'effort', (3, 9))
+ *         _check_arg(effort, 'effort', (1, 10))
  *         _check_arg(decoding_speed, 'decoding_speed', (0, 4))             # <<<<<<<<<<<<<<
  *         _check_arg(num_threads, 'num_threads', (0, 32))
  *         _check_arg(bit_depth, 'bit_depth', (1, 16))
  */
   __pyx_tuple__9 = PyTuple_Pack(2, __pyx_int_0, __pyx_int_4); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 1052, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
   /* "_jxlpy/_jxl.pyx":1053
- *         _check_arg(effort, 'effort', (3, 9))
+ *         _check_arg(effort, 'effort', (1, 10))
  *         _check_arg(decoding_speed, 'decoding_speed', (0, 4))
  *         _check_arg(num_threads, 'num_threads', (0, 32))             # <<<<<<<<<<<<<<
  *         _check_arg(bit_depth, 'bit_depth', (1, 16))
  *         # alpha_bit_depth is ignored if appropriate colorspace is not set, however it also can be 0
  */
   __pyx_tuple__10 = PyTuple_Pack(2, __pyx_int_0, __pyx_int_32); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 1053, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
@@ -12514,19 +12524,17 @@
   __pyx_float_6_4 = PyFloat_FromDouble(6.4); if (unlikely(!__pyx_float_6_4)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_0_09 = PyFloat_FromDouble(0.09); if (unlikely(!__pyx_float_0_09)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_6_25 = PyFloat_FromDouble(6.25); if (unlikely(!__pyx_float_6_25)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_0_235 = PyFloat_FromDouble(0.235); if (unlikely(!__pyx_float_0_235)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_12_65 = PyFloat_FromDouble(12.65); if (unlikely(!__pyx_float_12_65)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_3 = PyInt_FromLong(3); if (unlikely(!__pyx_int_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_4 = PyInt_FromLong(4); if (unlikely(!__pyx_int_4)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_7 = PyInt_FromLong(7); if (unlikely(!__pyx_int_7)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_8 = PyInt_FromLong(8); if (unlikely(!__pyx_int_8)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_9 = PyInt_FromLong(9); if (unlikely(!__pyx_int_9)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_10 = PyInt_FromLong(10); if (unlikely(!__pyx_int_10)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_16 = PyInt_FromLong(16); if (unlikely(!__pyx_int_16)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_30 = PyInt_FromLong(30); if (unlikely(!__pyx_int_30)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_32 = PyInt_FromLong(32); if (unlikely(!__pyx_int_32)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_100 = PyInt_FromLong(100); if (unlikely(!__pyx_int_100)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
@@ -12939,29 +12947,29 @@
   #endif
 
   /* "_jxlpy/_jxl.pyx":8
  * from libcpp.vector cimport vector
  * from libcpp.utility cimport pair
  * import math             # <<<<<<<<<<<<<<
  * 
- * __version__ = '0.9.4'
+ * __version__ = '0.9.5'
  */
   __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_math, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_math, __pyx_t_2) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_jxlpy/_jxl.pyx":10
  * import math
  * 
- * __version__ = '0.9.4'             # <<<<<<<<<<<<<<
+ * __version__ = '0.9.5'             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_0_9_4) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_0_9_5) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
 
   /* "_jxlpy/_jxl.pyx":966
  * 
  * 
  * class JXLPyError(Exception):             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, msg, code=None):
@@ -16714,15 +16722,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `jxlpy-0.9.4/jxlpy/JXLImagePlugin.py` & `jxlpy-0.9.5/jxlpy/JXLImagePlugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,19 @@
         
         if self._jxlinfo['bits_per_sample'] != 8:
             raise NotImplementedError('bits_per_sample not equals 8')
 
         self._size = (self._jxlinfo['xsize'], self._jxlinfo['ysize'])
         self.is_animated = self._jxlinfo['have_animation']
         self.n_frames = self._decoder.get_n_frames()
-        self._mode = self.rawmode = self._decoder.get_colorspace()
+        mode = self._decoder.get_colorspace()
+        try:
+            self.mode = self.rawmode = mode
+        except AttributeError:
+            self._mode = self.rawmode = mode
 
         self.info['icc'] = self._decoder.get_icc_profile()
         
         self.tile = []
 
         self._rewind()
```

### Comparing `jxlpy-0.9.4/jxlpy.egg-info/PKG-INFO` & `jxlpy-0.9.5/jxlpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jxlpy
-Version: 0.9.4
+Version: 0.9.5
 Summary: JPEG XL integration in Python
 Home-page: http://github.com/olokelo/jxlpy
 Author: oloke
 Author-email: olokelo@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `jxlpy-0.9.4/setup.py` & `jxlpy-0.9.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     extra_compile_args=['-O2'],
     extra_link_args=['-ljxl', '-ljxl_threads'],
     language='c++',
 )
 
 
 setup(name='jxlpy',
-      version='0.9.4',
+      version='0.9.5',
       description='JPEG XL integration in Python',
       long_description=long_description,
       long_description_content_type='text/markdown',
       license='MIT License',
       author='oloke',
       author_email='olokelo@gmail.com',
       url='http://github.com/olokelo/jxlpy',
```

