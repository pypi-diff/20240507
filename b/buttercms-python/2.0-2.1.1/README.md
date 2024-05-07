# Comparing `tmp/buttercms-python-2.0.tar.gz` & `tmp/buttercms_python-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buttercms-python-2.0.tar", last modified: Wed Apr 24 17:13:36 2024, max compression
+gzip compressed data, was "buttercms_python-2.1.1.tar", last modified: Tue May  7 15:30:39 2024, max compression
```

## Comparing `buttercms-python-2.0.tar` & `buttercms_python-2.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-04-24 17:13:36.310475 buttercms-python-2.0/
--rw-rw-r--   0 maria     (1000) maria     (1000)     1076 2023-09-14 13:51:45.000000 buttercms-python-2.0/LICENSE
--rw-rw-r--   0 maria     (1000) maria     (1000)       25 2023-09-14 13:51:45.000000 buttercms-python-2.0/MANIFEST.in
--rw-r--r--   0 maria     (1000) maria     (1000)     4958 2024-04-24 17:13:36.310475 buttercms-python-2.0/PKG-INFO
--rw-rw-r--   0 maria     (1000) maria     (1000)     4135 2023-09-14 13:51:45.000000 buttercms-python-2.0/README.md
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-04-24 17:13:36.306475 buttercms-python-2.0/butter_cms/
--rw-rw-r--   0 maria     (1000) maria     (1000)      565 2023-09-14 13:51:45.000000 buttercms-python-2.0/butter_cms/__init__.py
--rw-rw-r--   0 maria     (1000) maria     (1000)       20 2023-09-14 13:51:45.000000 buttercms-python-2.0/butter_cms/__version__.py
--rw-rw-r--   0 maria     (1000) maria     (1000)      253 2023-09-14 13:51:45.000000 buttercms-python-2.0/butter_cms/author.py
--rw-rw-r--   0 maria     (1000) maria     (1000)      260 2023-09-14 13:51:45.000000 buttercms-python-2.0/butter_cms/category.py
--rw-rw-r--   0 maria     (1000) maria     (1000)     1425 2024-04-24 17:10:33.000000 buttercms-python-2.0/butter_cms/client.py
--rw-rw-r--   0 maria     (1000) maria     (1000)      363 2023-09-14 13:51:45.000000 buttercms-python-2.0/butter_cms/content_field.py
--rw-rw-r--   0 maria     (1000) maria     (1000)      171 2023-09-14 13:51:45.000000 buttercms-python-2.0/butter_cms/feed.py
--rw-rw-r--   0 maria     (1000) maria     (1000)      754 2023-09-14 13:51:45.000000 buttercms-python-2.0/butter_cms/page.py
--rw-rw-r--   0 maria     (1000) maria     (1000)      620 2023-09-14 13:51:45.000000 buttercms-python-2.0/butter_cms/post.py
--rw-rw-r--   0 maria     (1000) maria     (1000)      244 2023-09-14 13:51:45.000000 buttercms-python-2.0/butter_cms/tag.py
--rw-rw-r--   0 maria     (1000) maria     (1000)     4738 2023-09-14 13:51:45.000000 buttercms-python-2.0/butter_cms/unit_tests.py
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-04-24 17:13:36.310475 buttercms-python-2.0/buttercms_python.egg-info/
--rw-r--r--   0 maria     (1000) maria     (1000)     4958 2024-04-24 17:13:36.000000 buttercms-python-2.0/buttercms_python.egg-info/PKG-INFO
--rw-rw-r--   0 maria     (1000) maria     (1000)      489 2024-04-24 17:13:36.000000 buttercms-python-2.0/buttercms_python.egg-info/SOURCES.txt
--rw-rw-r--   0 maria     (1000) maria     (1000)        1 2024-04-24 17:13:36.000000 buttercms-python-2.0/buttercms_python.egg-info/dependency_links.txt
--rw-rw-r--   0 maria     (1000) maria     (1000)        9 2024-04-24 17:13:36.000000 buttercms-python-2.0/buttercms_python.egg-info/requires.txt
--rw-rw-r--   0 maria     (1000) maria     (1000)       11 2024-04-24 17:13:36.000000 buttercms-python-2.0/buttercms_python.egg-info/top_level.txt
--rw-rw-r--   0 maria     (1000) maria     (1000)       67 2024-04-24 17:13:36.310475 buttercms-python-2.0/setup.cfg
--rw-rw-r--   0 maria     (1000) maria     (1000)     1866 2024-04-24 17:10:33.000000 buttercms-python-2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:30:39.644904 buttercms_python-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-07 15:30:34.000000 buttercms_python-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 15:30:34.000000 buttercms_python-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-07 15:30:39.644904 buttercms_python-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-07 15:30:34.000000 buttercms_python-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:30:39.640903 buttercms_python-2.1.1/butter_cms/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-07 15:30:34.000000 buttercms_python-2.1.1/butter_cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-07 15:30:34.000000 buttercms_python-2.1.1/butter_cms/author.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-07 15:30:34.000000 buttercms_python-2.1.1/butter_cms/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-07 15:30:34.000000 buttercms_python-2.1.1/butter_cms/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-07 15:30:34.000000 buttercms_python-2.1.1/butter_cms/content_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-07 15:30:34.000000 buttercms_python-2.1.1/butter_cms/feed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-07 15:30:34.000000 buttercms_python-2.1.1/butter_cms/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-07 15:30:34.000000 buttercms_python-2.1.1/butter_cms/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-07 15:30:34.000000 buttercms_python-2.1.1/butter_cms/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-07 15:30:34.000000 buttercms_python-2.1.1/butter_cms/unit_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 15:30:34.000000 buttercms_python-2.1.1/butter_cms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:30:39.644904 buttercms_python-2.1.1/buttercms_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-07 15:30:39.000000 buttercms_python-2.1.1/buttercms_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-07 15:30:39.000000 buttercms_python-2.1.1/buttercms_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 15:30:39.000000 buttercms_python-2.1.1/buttercms_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 15:30:39.000000 buttercms_python-2.1.1/buttercms_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 15:30:39.000000 buttercms_python-2.1.1/buttercms_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-07 15:30:39.644904 buttercms_python-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-07 15:30:34.000000 buttercms_python-2.1.1/setup.py
```

### Comparing `buttercms-python-2.0/LICENSE` & `buttercms_python-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `buttercms-python-2.0/PKG-INFO` & `buttercms_python-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: buttercms-python
-Version: 2.0
+Version: 2.1.1
 Summary: API First Blogging and CMS platform built for developers
 Home-page: https://github.com/buttercms/buttercms-python
 Download-URL: https://github.com/buttercms/buttercms-python/tarball/0.1
-Author: Adam Yala
-Author-email: adam@adamyala.com
-Keywords: foo,bar,baz
+Author: ButterCMS
+Author-email: support@buttercms.com
+Keywords: buttercms,sdk,cms,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Framework :: Django
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
-# buttercms-python
+# buttercms-python - 2.1.1 <!-- {x-release-please-version} -->
 
 Python Library for ButterCMS API. 
 
 ## Documentation
 
 For a comprehensive list of examples, check out the [API documentation](https://buttercms.com/docs/api/).
```

### Comparing `buttercms-python-2.0/README.md` & `buttercms_python-2.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# buttercms-python
+# buttercms-python - 2.1.1 <!-- {x-release-please-version} -->
 
 Python Library for ButterCMS API. 
 
 ## Documentation
 
 For a comprehensive list of examples, check out the [API documentation](https://buttercms.com/docs/api/).
```

### Comparing `buttercms-python-2.0/butter_cms/__init__.py` & `buttercms_python-2.1.1/butter_cms/__init__.py`

 * *Files identical despite different names*

### Comparing `buttercms-python-2.0/butter_cms/client.py` & `buttercms_python-2.1.1/butter_cms/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 
-from .__version__ import __version__
+from .version import __version__
 from requests.exceptions import HTTPError
 
 
 class Client(object):
     """Client"""
     def __init__(self, auth_token):
         self.auth_token = auth_token
```

### Comparing `buttercms-python-2.0/butter_cms/page.py` & `buttercms_python-2.1.1/butter_cms/page.py`

 * *Files identical despite different names*

### Comparing `buttercms-python-2.0/butter_cms/post.py` & `buttercms_python-2.1.1/butter_cms/post.py`

 * *Files identical despite different names*

### Comparing `buttercms-python-2.0/butter_cms/unit_tests.py` & `buttercms_python-2.1.1/butter_cms/unit_tests.py`

 * *Files identical despite different names*

### Comparing `buttercms-python-2.0/buttercms_python.egg-info/PKG-INFO` & `buttercms_python-2.1.1/buttercms_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: buttercms-python
-Version: 2.0
+Version: 2.1.1
 Summary: API First Blogging and CMS platform built for developers
 Home-page: https://github.com/buttercms/buttercms-python
 Download-URL: https://github.com/buttercms/buttercms-python/tarball/0.1
-Author: Adam Yala
-Author-email: adam@adamyala.com
-Keywords: foo,bar,baz
+Author: ButterCMS
+Author-email: support@buttercms.com
+Keywords: buttercms,sdk,cms,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Framework :: Django
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
-# buttercms-python
+# buttercms-python - 2.1.1 <!-- {x-release-please-version} -->
 
 Python Library for ButterCMS API. 
 
 ## Documentation
 
 For a comprehensive list of examples, check out the [API documentation](https://buttercms.com/docs/api/).
```

### Comparing `buttercms-python-2.0/setup.py` & `buttercms_python-2.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,48 +5,47 @@
     from setuptools import setup, find_packages
 except ImportError:
     from distutils.core import setup
 
 with open('README.md', 'r') as f:
     readme = f.read()
 
-
 install_requires = []
 if sys.version_info < (2, 7, 9):
     raise Exception('ButterCMS uses the requests library to securely talk to https://buttercms.com '
         'which requires Python 2.7.9 or later.\n'
         'Please take a few seconds to upgrade to Python 2.7.9 and try again.\n'
         'https://www.python.org/downloads/')
     # TODO: Add support for < Python 2.7.9
     # install_requires.append('requests[security]')
 else:
     install_requires.append('requests')
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 version = {}
 
-with open(os.path.join(package_root, "butter_cms/__version__.py")) as fp:
+with open(os.path.join(package_root, "butter_cms/version.py")) as fp:
     exec(fp.read(), version)
 
 version = version["__version__"]
 
 setup(
     name = 'buttercms-python',
     packages = find_packages(),
     version = version,
     description = 'API First Blogging and CMS platform built for developers',
     long_description=readme,
     long_description_content_type="text/markdown",
-    author = 'Adam Yala',
-    author_email = 'adam@adamyala.com',
+    author = 'ButterCMS',
+    author_email = 'support@buttercms.com',
     url = 'https://github.com/buttercms/buttercms-python',
     download_url = 'https://github.com/buttercms/buttercms-python/tarball/0.1',
     py_modules=['butter_cms'],
     install_requires=install_requires,
-    keywords = ['foo', 'bar', 'baz'],
+    keywords = ['buttercms', 'sdk', 'cms', 'api'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Environment :: Web Environment',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2.7',
```

