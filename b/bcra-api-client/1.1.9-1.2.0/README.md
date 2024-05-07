# Comparing `tmp/bcra_api_client-1.1.9.tar.gz` & `tmp/bcra_api_client-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcra_api_client-1.1.9.tar", last modified: Sat May  4 19:28:23 2024, max compression
+gzip compressed data, was "bcra_api_client-1.2.0.tar", last modified: Tue May  7 11:20:03 2024, max compression
```

## Comparing `bcra_api_client-1.1.9.tar` & `bcra_api_client-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:28:23.472576 bcra_api_client-1.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-04 19:28:18.000000 bcra_api_client-1.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-04 19:28:23.472576 bcra_api_client-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-04 19:28:18.000000 bcra_api_client-1.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:28:23.472576 bcra_api_client-1.1.9/bcra/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-04 19:28:18.000000 bcra_api_client-1.1.9/bcra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-04 19:28:18.000000 bcra_api_client-1.1.9/bcra/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-04 19:28:18.000000 bcra_api_client-1.1.9/bcra/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-04 19:28:18.000000 bcra_api_client-1.1.9/bcra/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-04 19:28:18.000000 bcra_api_client-1.1.9/bcra/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:28:23.472576 bcra_api_client-1.1.9/bcra/statistics/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-04 19:28:18.000000 bcra_api_client-1.1.9/bcra/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-04 19:28:18.000000 bcra_api_client-1.1.9/bcra/statistics/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:28:23.472576 bcra_api_client-1.1.9/bcra_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-04 19:28:23.000000 bcra_api_client-1.1.9/bcra_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-04 19:28:23.000000 bcra_api_client-1.1.9/bcra_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 19:28:23.000000 bcra_api_client-1.1.9/bcra_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-04 19:28:23.000000 bcra_api_client-1.1.9/bcra_api_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-04 19:28:18.000000 bcra_api_client-1.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 19:28:23.472576 bcra_api_client-1.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:20:03.692585 bcra_api_client-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-07 11:19:59.000000 bcra_api_client-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-07 11:20:03.692585 bcra_api_client-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-07 11:19:59.000000 bcra_api_client-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:20:03.692585 bcra_api_client-1.2.0/bcra/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-07 11:19:59.000000 bcra_api_client-1.2.0/bcra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-07 11:19:59.000000 bcra_api_client-1.2.0/bcra/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-07 11:19:59.000000 bcra_api_client-1.2.0/bcra/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-07 11:19:59.000000 bcra_api_client-1.2.0/bcra/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:20:03.692585 bcra_api_client-1.2.0/bcra/currency/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-07 11:19:59.000000 bcra_api_client-1.2.0/bcra/currency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-07 11:19:59.000000 bcra_api_client-1.2.0/bcra/currency/dollar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-07 11:19:59.000000 bcra_api_client-1.2.0/bcra/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:20:03.692585 bcra_api_client-1.2.0/bcra/statistics/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-07 11:19:59.000000 bcra_api_client-1.2.0/bcra/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-07 11:19:59.000000 bcra_api_client-1.2.0/bcra/statistics/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:20:03.692585 bcra_api_client-1.2.0/bcra_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-07 11:20:03.000000 bcra_api_client-1.2.0/bcra_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-07 11:20:03.000000 bcra_api_client-1.2.0/bcra_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 11:20:03.000000 bcra_api_client-1.2.0/bcra_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 11:20:03.000000 bcra_api_client-1.2.0/bcra_api_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-07 11:19:59.000000 bcra_api_client-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 11:20:03.692585 bcra_api_client-1.2.0/setup.cfg
```

### Comparing `bcra_api_client-1.1.9/LICENSE` & `bcra_api_client-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bcra_api_client-1.1.9/pyproject.toml` & `bcra_api_client-1.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bcra-api-client"
-version = "1.1.9"
+version = "1.2.0"
 authors = [
   { name="Emmanuel Paiva", email="none@email.com"},
 ]
 description = "Consumo de datos de la API del banco central de la Republica Argentina"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

