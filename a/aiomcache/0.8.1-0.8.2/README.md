# Comparing `tmp/aiomcache-0.8.1.tar.gz` & `tmp/aiomcache-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiomcache-0.8.1.tar", last modified: Fri Feb 10 17:37:38 2023, max compression
+gzip compressed data, was "aiomcache-0.8.2.tar", last modified: Tue May  7 15:03:07 2024, max compression
```

## Comparing `aiomcache-0.8.1.tar` & `aiomcache-0.8.2.tar`

### file list

```diff
@@ -1,28 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 17:37:38.170150 aiomcache-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-02-10 17:37:26.000000 aiomcache-0.8.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-02-10 17:37:26.000000 aiomcache-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-10 17:37:26.000000 aiomcache-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-02-10 17:37:38.170150 aiomcache-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-02-10 17:37:26.000000 aiomcache-0.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 17:37:38.170150 aiomcache-0.8.1/aiomcache/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-02-10 17:37:26.000000 aiomcache-0.8.1/aiomcache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19878 2023-02-10 17:37:26.000000 aiomcache-0.8.1/aiomcache/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-02-10 17:37:26.000000 aiomcache-0.8.1/aiomcache/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-02-10 17:37:26.000000 aiomcache-0.8.1/aiomcache/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-02-10 17:37:26.000000 aiomcache-0.8.1/aiomcache/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 17:37:26.000000 aiomcache-0.8.1/aiomcache/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 17:37:38.170150 aiomcache-0.8.1/aiomcache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-02-10 17:37:38.000000 aiomcache-0.8.1/aiomcache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-02-10 17:37:38.000000 aiomcache-0.8.1/aiomcache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 17:37:38.000000 aiomcache-0.8.1/aiomcache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-10 17:37:38.000000 aiomcache-0.8.1/aiomcache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-10 17:37:38.000000 aiomcache-0.8.1/aiomcache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-02-10 17:37:38.170150 aiomcache-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-02-10 17:37:26.000000 aiomcache-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 17:37:38.170150 aiomcache-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 17:37:26.000000 aiomcache-0.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-02-10 17:37:26.000000 aiomcache-0.8.1/tests/commands_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-02-10 17:37:26.000000 aiomcache-0.8.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-02-10 17:37:26.000000 aiomcache-0.8.1/tests/conn_args_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-02-10 17:37:26.000000 aiomcache-0.8.1/tests/flag_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-02-10 17:37:26.000000 aiomcache-0.8.1/tests/pool_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:03:07.626142 aiomcache-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-07 15:03:01.000000 aiomcache-0.8.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-07 15:03:01.000000 aiomcache-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-07 15:03:01.000000 aiomcache-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-07 15:03:07.626142 aiomcache-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-07 15:03:01.000000 aiomcache-0.8.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:03:07.622142 aiomcache-0.8.2/aiomcache/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-07 15:03:01.000000 aiomcache-0.8.2/aiomcache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19783 2024-05-07 15:03:01.000000 aiomcache-0.8.2/aiomcache/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-07 15:03:01.000000 aiomcache-0.8.2/aiomcache/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-07 15:03:01.000000 aiomcache-0.8.2/aiomcache/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-07 15:03:01.000000 aiomcache-0.8.2/aiomcache/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:03:01.000000 aiomcache-0.8.2/aiomcache/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:03:07.626142 aiomcache-0.8.2/aiomcache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-07 15:03:07.000000 aiomcache-0.8.2/aiomcache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-07 15:03:07.000000 aiomcache-0.8.2/aiomcache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 15:03:07.000000 aiomcache-0.8.2/aiomcache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 15:03:07.000000 aiomcache-0.8.2/aiomcache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 15:03:07.000000 aiomcache-0.8.2/aiomcache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 15:03:07.626142 aiomcache-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-07 15:03:01.000000 aiomcache-0.8.2/setup.py
```

### Comparing `aiomcache-0.8.1/CHANGES.rst` & `aiomcache-0.8.2/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 =======
 CHANGES
 =======
 
 .. towncrier release notes start
 
+0.8.2 (2024-05-07)
+==================
+- Fix a static typing error with ``Client.get()``.
+
 0.8.1 (2023-02-10)
 ==================
 - Add ``conn_args`` to ``Client`` to allow TLS and other options when connecting to memcache.
 
 0.8.0 (2022-12-11)
 ==================
 - Add ``FlagClient`` to support memcached flags.
```

### Comparing `aiomcache-0.8.1/LICENSE` & `aiomcache-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiomcache-0.8.1/PKG-INFO` & `aiomcache-0.8.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: aiomcache
-Version: 0.8.1
+Version: 0.8.2
 Summary: Minimal pure python memcached client
 Home-page: https://github.com/aio-libs/aiomcache/
 Author: Nikolay Kim
 Author-email: fafhrd91@gmail.com
 Maintainer: Nikolay Kim <fafhrd91@gmail.com>, Andrew Svetlov <andrew.svetlov@gmail.com>
 Maintainer-email: aio-libs@googlegroups.com
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: typing_extensions>=4; python_version < "3.11"
 
 memcached client for asyncio
 ============================
 
 asyncio (PEP 3156) library to work with memcached.
 
 
@@ -58,14 +59,18 @@
 
 =======
 CHANGES
 =======
 
 .. towncrier release notes start
 
+0.8.2 (2024-05-07)
+==================
+- Fix a static typing error with ``Client.get()``.
+
 0.8.1 (2023-02-10)
 ==================
 - Add ``conn_args`` to ``Client`` to allow TLS and other options when connecting to memcache.
 
 0.8.0 (2022-12-11)
 ==================
 - Add ``FlagClient`` to support memcached flags.
```

### Comparing `aiomcache-0.8.1/README.rst` & `aiomcache-0.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `aiomcache-0.8.1/aiomcache/client.py` & `aiomcache-0.8.2/aiomcache/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 import functools
 import re
 import sys
-from typing import (Any, Awaitable, Callable, Dict, Generic, Mapping, Optional, Tuple,
-                    TypeVar, Union, overload)
+from typing import (Any, Awaitable, Callable, Dict, Generic, Literal, Mapping, Optional,
+                    Tuple, TypeVar, Union, overload)
 
 from . import constants as const
 from .exceptions import ClientException, ValidationException
 from .pool import Connection, MemcachePool
 
-if sys.version_info >= (3, 8):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
-
 if sys.version_info >= (3, 10):
     from typing import Concatenate, ParamSpec
 else:
     from typing_extensions import Concatenate, ParamSpec
 
 __all__ = ['Client']
 
@@ -197,26 +192,28 @@
         response = await self._execute_simple_command(conn, command)
 
         if response not in (const.DELETED, const.NOT_FOUND):
             raise ClientException('Memcached delete failed', response)
 
         return response == const.DELETED
 
+    @acquire
     @overload
-    async def get(self, key: bytes, default: None = ...) -> Union[bytes, _T, None]:
+    async def get(self, conn: Connection, /, key: bytes,
+                  default: None = ...) -> Union[bytes, _T, None]:
         ...
 
+    @acquire
     @overload
-    async def get(self, key: bytes, default: _U) -> Union[bytes, _T, _U]:
+    async def get(self, conn: Connection, /, key: bytes, default: _U) -> Union[bytes, _T, _U]:
         ...
 
-    # Mypy bug: https://github.com/python/mypy/issues/12716
-    @acquire  # type: ignore[misc]
+    @acquire
     async def get(
-        self, conn: Connection, key: bytes, default: Optional[_U] = None
+        self, conn: Connection, /, key: bytes, default: Optional[_U] = None
     ) -> Union[bytes, _T, _U, None]:
         """Gets a single value from the server.
 
         :param key: ``bytes``, is the key for the item being fetched
         :param default: default value if there is no value.
         :return: ``bytes``, is the data for this specified key.
         """
```

### Comparing `aiomcache-0.8.1/aiomcache/pool.py` & `aiomcache-0.8.2/aiomcache/pool.py`

 * *Files identical despite different names*

### Comparing `aiomcache-0.8.1/aiomcache.egg-info/PKG-INFO` & `aiomcache-0.8.2/aiomcache.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: aiomcache
-Version: 0.8.1
+Version: 0.8.2
 Summary: Minimal pure python memcached client
 Home-page: https://github.com/aio-libs/aiomcache/
 Author: Nikolay Kim
 Author-email: fafhrd91@gmail.com
 Maintainer: Nikolay Kim <fafhrd91@gmail.com>, Andrew Svetlov <andrew.svetlov@gmail.com>
 Maintainer-email: aio-libs@googlegroups.com
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: typing_extensions>=4; python_version < "3.11"
 
 memcached client for asyncio
 ============================
 
 asyncio (PEP 3156) library to work with memcached.
 
 
@@ -58,14 +59,18 @@
 
 =======
 CHANGES
 =======
 
 .. towncrier release notes start
 
+0.8.2 (2024-05-07)
+==================
+- Fix a static typing error with ``Client.get()``.
+
 0.8.1 (2023-02-10)
 ==================
 - Add ``conn_args`` to ``Client`` to allow TLS and other options when connecting to memcache.
 
 0.8.0 (2022-12-11)
 ==================
 - Add ``FlagClient`` to support memcached flags.
```

### Comparing `aiomcache-0.8.1/setup.py` & `aiomcache-0.8.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import codecs
 import os
 import re
 
-from setuptools import find_packages, setup
+from setuptools import setup
 
 
 with codecs.open(os.path.join(os.path.abspath(os.path.dirname(
         __file__)), 'aiomcache', '__init__.py'), 'r', 'latin1') as fp:
     try:
         version = re.findall(r'^__version__ = "([^"]+)"\r?$', fp.read(), re.M)[0]
     except IndexError:
@@ -22,31 +22,31 @@
       description=('Minimal pure python memcached client'),
       long_description='\n\n'.join((read('README.rst'), read('CHANGES.rst'))),
       long_description_content_type='text/x-rst',
       classifiers=[
           'License :: OSI Approved :: BSD License',
           'Intended Audience :: Developers',
           'Programming Language :: Python',
-          'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
           'Programming Language :: Python :: 3.11',
+          'Programming Language :: Python :: 3.12',
           'Operating System :: POSIX',
           'Operating System :: MacOS :: MacOS X',
           'Operating System :: Microsoft :: Windows',
           'Environment :: Web Environment',
           'Framework :: AsyncIO',
       ],
       author='Nikolay Kim',
       author_email='fafhrd91@gmail.com',
       maintainer=', '.join(('Nikolay Kim <fafhrd91@gmail.com>',
                             'Andrew Svetlov <andrew.svetlov@gmail.com>')),
       maintainer_email='aio-libs@googlegroups.com',
       url='https://github.com/aio-libs/aiomcache/',
       license='BSD',
-      packages=find_packages(),
-      python_requires='>=3.7',
+      packages=("aiomcache",),
+      python_requires='>=3.8',
       install_requires=('typing_extensions>=4; python_version<"3.11"',),
       tests_require=("nose",),
       test_suite='nose.collector',
       include_package_data=True)
```

