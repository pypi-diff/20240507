# Comparing `tmp/ckanext-doi-3.1.8.tar.gz` & `tmp/ckanext-doi-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-doi-3.1.8.tar", last modified: Mon Jul 17 08:18:19 2023, max compression
+gzip compressed data, was "ckanext-doi-3.1.9.tar", last modified: Mon Sep 25 10:51:34 2023, max compression
```

## Comparing `ckanext-doi-3.1.8.tar` & `ckanext-doi-3.1.9.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:19.923952 ckanext-doi-3.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-07-17 08:18:19.923952 ckanext-doi-3.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:19.919952 ckanext-doi-3.1.8/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:19.919952 ckanext-doi-3.1.8/ckanext/doi/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/ckanext/doi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/ckanext/doi/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/ckanext/doi/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:19.919952 ckanext-doi-3.1.8/ckanext/doi/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/ckanext/doi/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/ckanext/doi/lib/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/ckanext/doi/lib/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/ckanext/doi/lib/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10112 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/ckanext/doi/lib/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/ckanext/doi/lib/xml_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:19.919952 ckanext-doi-3.1.8/ckanext/doi/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/ckanext/doi/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/ckanext/doi/model/crud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/ckanext/doi/model/doi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/ckanext/doi/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:19.915952 ckanext-doi-3.1.8/ckanext/doi/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:19.915952 ckanext-doi-3.1.8/ckanext/doi/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:19.915952 ckanext-doi-3.1.8/ckanext/doi/theme/templates/doi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:19.919952 ckanext-doi-3.1.8/ckanext/doi/theme/templates/doi/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/ckanext/doi/theme/templates/doi/snippets/package_citation.html
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/ckanext/doi/theme/templates/doi/snippets/resource_citation.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:19.919952 ckanext-doi-3.1.8/ckanext/doi/theme/templates/package/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/ckanext/doi/theme/templates/package/read.html
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/ckanext/doi/theme/templates/package/read_base.html
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/ckanext/doi/theme/templates/package/resource_read.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:19.919952 ckanext-doi-3.1.8/ckanext/doi/theme/templates/package/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/ckanext/doi/theme/templates/package/snippets/package_basic_fields.html
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/ckanext/doi/theme/templates/package/snippets/package_metadata_fields.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:19.919952 ckanext-doi-3.1.8/ckanext_doi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-07-17 08:18:19.000000 ckanext-doi-3.1.8/ckanext_doi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-17 08:18:19.000000 ckanext-doi-3.1.8/ckanext_doi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:18:19.000000 ckanext-doi-3.1.8/ckanext_doi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-17 08:18:19.000000 ckanext-doi-3.1.8/ckanext_doi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:18:19.000000 ckanext-doi-3.1.8/ckanext_doi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-17 08:18:19.000000 ckanext-doi-3.1.8/ckanext_doi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 08:18:19.000000 ckanext-doi-3.1.8/ckanext_doi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:19.915952 ckanext-doi-3.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:19.919952 ckanext-doi-3.1.8/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:18:19.923952 ckanext-doi-3.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:19.923952 ckanext-doi-3.1.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:18:19.923952 ckanext-doi-3.1.8/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/tests/helpers/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-17 08:18:06.000000 ckanext-doi-3.1.8/tests/test_generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 10:51:34.437363 ckanext-doi-3.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11555 2023-09-25 10:51:34.437363 ckanext-doi-3.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 10:51:34.429362 ckanext-doi-3.1.9/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 10:51:34.429362 ckanext-doi-3.1.9/ckanext/doi/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/ckanext/doi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/ckanext/doi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/ckanext/doi/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 10:51:34.433363 ckanext-doi-3.1.9/ckanext/doi/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/ckanext/doi/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/ckanext/doi/lib/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/ckanext/doi/lib/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/ckanext/doi/lib/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10112 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/ckanext/doi/lib/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/ckanext/doi/lib/xml_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 10:51:34.433363 ckanext-doi-3.1.9/ckanext/doi/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/ckanext/doi/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/ckanext/doi/model/crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/ckanext/doi/model/doi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/ckanext/doi/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 10:51:34.425362 ckanext-doi-3.1.9/ckanext/doi/theme/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 10:51:34.425362 ckanext-doi-3.1.9/ckanext/doi/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 10:51:34.425362 ckanext-doi-3.1.9/ckanext/doi/theme/templates/doi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 10:51:34.433363 ckanext-doi-3.1.9/ckanext/doi/theme/templates/doi/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/ckanext/doi/theme/templates/doi/snippets/package_citation.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/ckanext/doi/theme/templates/doi/snippets/resource_citation.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 10:51:34.433363 ckanext-doi-3.1.9/ckanext/doi/theme/templates/package/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/ckanext/doi/theme/templates/package/read.html
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/ckanext/doi/theme/templates/package/read_base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/ckanext/doi/theme/templates/package/resource_read.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 10:51:34.433363 ckanext-doi-3.1.9/ckanext/doi/theme/templates/package/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/ckanext/doi/theme/templates/package/snippets/package_basic_fields.html
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/ckanext/doi/theme/templates/package/snippets/package_metadata_fields.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 10:51:34.437363 ckanext-doi-3.1.9/ckanext_doi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11555 2023-09-25 10:51:34.000000 ckanext-doi-3.1.9/ckanext_doi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2023-09-25 10:51:34.000000 ckanext-doi-3.1.9/ckanext_doi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 10:51:34.000000 ckanext-doi-3.1.9/ckanext_doi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2023-09-25 10:51:34.000000 ckanext-doi-3.1.9/ckanext_doi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 10:51:34.000000 ckanext-doi-3.1.9/ckanext_doi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2023-09-25 10:51:34.000000 ckanext-doi-3.1.9/ckanext_doi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2023-09-25 10:51:34.000000 ckanext-doi-3.1.9/ckanext_doi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 10:51:34.429362 ckanext-doi-3.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 10:51:34.437363 ckanext-doi-3.1.9/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-25 10:51:34.437363 ckanext-doi-3.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 10:51:34.437363 ckanext-doi-3.1.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 10:51:34.437363 ckanext-doi-3.1.9/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/tests/helpers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9586 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2023-09-25 10:51:20.000000 ckanext-doi-3.1.9/tests/test_plugin.py
```

### Comparing `ckanext-doi-3.1.8/LICENSE` & `ckanext-doi-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.8/PKG-INFO` & `ckanext-doi-3.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,15 @@
-Metadata-Version: 2.1
-Name: ckanext-doi
-Version: 3.1.8
-Summary: A CKAN extension for assigning a digital object identifier (DOI) to datasets, using the DataCite DOI service.
-Author-email: Natural History Museum <data@nhm.ac.uk>
-License: GPL-3.0-or-later
-Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-doi
-Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-doi/blob/main/CHANGELOG.md
-Keywords: CKAN,data,doi
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 <!--header-start-->
 <img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-doi
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-doi/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-doi/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-doi/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-doi)
-[![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
+[![CKAN](https://img.shields.io/badge/ckan-2.9.9%20%7C%202.10.1-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
 [![Docs](https://img.shields.io/readthedocs/ckanext-doi?style=flat-square)](https://ckanext-doi.readthedocs.io)
 
 _A CKAN extension for assigning a digital object identifier (DOI) to datasets, using the DataCite DOI service._
 
 <!--header-end-->
 
@@ -246,26 +225,30 @@
 <!--usage-end-->
 
 # Testing
 
 <!--testing-start-->
 There is a Docker compose configuration available in this repository to make it easier to run tests. The ckan image uses the Dockerfile in the `docker/` folder.
 
-To run the tests against ckan 2.9.x on Python3:
+To run the tests can be run against ckan 2.9.x and 2.10.x on Python3:
 
 1. Build the required images:
    ```shell
    docker-compose build
    ```
 
 2. Then run the tests.
    The root of the repository is mounted into the ckan container as a volume by the Docker compose
    configuration, so you should only need to rebuild the ckan image if you change the extension's
    dependencies.
    ```shell
-   docker-compose run ckan
+   # run tests against ckan 2.9.x
+   docker-compose run latest
+
+   # run tests against ckan 2.10.x
+   docker-compose run next
    ```
 
 Note that the tests mock the DataCite API and therefore don't require an internet connection nor
 your DataCite credentials to run.
 
 <!--testing-end-->
```

### Comparing `ckanext-doi-3.1.8/README.md` & `ckanext-doi-3.1.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,44 @@
+Metadata-Version: 2.1
+Name: ckanext-doi
+Version: 3.1.9
+Summary: A CKAN extension for assigning a digital object identifier (DOI) to datasets, using the DataCite DOI service.
+Author-email: Natural History Museum <data@nhm.ac.uk>
+License: GPL-3.0-or-later
+Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-doi
+Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-doi/blob/main/CHANGELOG.md
+Keywords: CKAN,data,doi
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: jsonschema==3.0.0
+Requires-Dist: xmltodict==0.12.0
+Requires-Dist: datacite==1.1.2
+Requires-Dist: ckantools>=0.3.0
+Provides-Extra: test
+Requires-Dist: mock; extra == "test"
+Requires-Dist: pytest>=4.6.5; extra == "test"
+Requires-Dist: pytest-cov>=2.7.1; extra == "test"
+Requires-Dist: coveralls; extra == "test"
+
 <!--header-start-->
 <img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-doi
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-doi/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-doi/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-doi/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-doi)
-[![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
+[![CKAN](https://img.shields.io/badge/ckan-2.9.9%20%7C%202.10.1-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
 [![Docs](https://img.shields.io/readthedocs/ckanext-doi?style=flat-square)](https://ckanext-doi.readthedocs.io)
 
 _A CKAN extension for assigning a digital object identifier (DOI) to datasets, using the DataCite DOI service._
 
 <!--header-end-->
 
@@ -225,26 +254,30 @@
 <!--usage-end-->
 
 # Testing
 
 <!--testing-start-->
 There is a Docker compose configuration available in this repository to make it easier to run tests. The ckan image uses the Dockerfile in the `docker/` folder.
 
-To run the tests against ckan 2.9.x on Python3:
+To run the tests can be run against ckan 2.9.x and 2.10.x on Python3:
 
 1. Build the required images:
    ```shell
    docker-compose build
    ```
 
 2. Then run the tests.
    The root of the repository is mounted into the ckan container as a volume by the Docker compose
    configuration, so you should only need to rebuild the ckan image if you change the extension's
    dependencies.
    ```shell
-   docker-compose run ckan
+   # run tests against ckan 2.9.x
+   docker-compose run latest
+
+   # run tests against ckan 2.10.x
+   docker-compose run next
    ```
 
 Note that the tests mock the DataCite API and therefore don't require an internet connection nor
 your DataCite credentials to run.
 
 <!--testing-end-->
```

### Comparing `ckanext-doi-3.1.8/ckanext/doi/cli.py` & `ckanext-doi-3.1.9/ckanext/doi/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.8/ckanext/doi/interfaces.py` & `ckanext-doi-3.1.9/ckanext/doi/interfaces.py`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.8/ckanext/doi/lib/api.py` & `ckanext-doi-3.1.9/ckanext/doi/lib/api.py`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.8/ckanext/doi/lib/helpers.py` & `ckanext-doi-3.1.9/ckanext/doi/lib/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.8/ckanext/doi/lib/metadata.py` & `ckanext-doi-3.1.9/ckanext/doi/lib/metadata.py`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.8/ckanext/doi/lib/xml_utils.py` & `ckanext-doi-3.1.9/ckanext/doi/lib/xml_utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.8/ckanext/doi/model/crud.py` & `ckanext-doi-3.1.9/ckanext/doi/model/crud.py`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.8/ckanext/doi/model/doi.py` & `ckanext-doi-3.1.9/ckanext/doi/model/doi.py`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.8/ckanext/doi/plugin.py` & `ckanext-doi-3.1.9/ckanext/doi/plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -33,46 +33,46 @@
         return cli.get_commands()
 
     ## IConfigurer
     def update_config(self, config):
         """
         Adds templates.
         """
-        toolkit.add_template_directory(config, 'theme/templates')
+        toolkit.add_template_directory(config, "theme/templates")
 
     ## IPackageController
-    def after_create(self, context, pkg_dict):
+    def after_dataset_create(self, context, pkg_dict):
         """
         A new dataset has been created, so we need to create a new DOI.
 
         NB: This is called after creation of a dataset, before resources have been
         added, so state = draft.
         """
-        DOIQuery.read_package(pkg_dict['id'], create_if_none=True)
+        DOIQuery.read_package(pkg_dict["id"], create_if_none=True)
 
     ## IPackageController
-    def after_update(self, context, pkg_dict):
+    def after_dataset_update(self, context, pkg_dict):
         """
         Dataset has been created/updated.
 
         Check status of the dataset to determine if we should publish DOI to datacite
         network.
         """
         # Is this active and public? If so we need to make sure we have an active DOI
-        if pkg_dict.get('state', 'active') == 'active' and not pkg_dict.get(
-            'private', False
+        if pkg_dict.get("state", "active") == "active" and not pkg_dict.get(
+            "private", False
         ):
-            package_id = pkg_dict['id']
+            package_id = pkg_dict["id"]
 
             # remove user-defined update schemas first (if needed)
-            context.pop('schema', None)
+            context.pop("schema", None)
 
             # Load the package_show version of the dict
-            pkg_show_dict = toolkit.get_action('package_show')(
-                context, {'id': package_id}
+            pkg_show_dict = toolkit.get_action("package_show")(
+                context, {"id": package_id}
             )
 
             # Load or create the local DOI (package may not have a DOI if extension was loaded
             # after package creation)
             doi = DOIQuery.read_package(package_id, create_if_none=True)
 
             metadata_dict = build_metadata_dict(pkg_show_dict)
@@ -80,39 +80,57 @@
 
             client = DataciteClient()
 
             if doi.published is None:
                 # metadata gets created before minting
                 client.set_metadata(doi.identifier, xml_dict)
                 client.mint_doi(doi.identifier, package_id)
-                toolkit.h.flash_success('DataCite DOI created')
+                toolkit.h.flash_success("DataCite DOI created")
             else:
                 same = client.check_for_update(doi.identifier, xml_dict)
                 if not same:
                     # Not the same, so we want to update the metadata
                     client.set_metadata(doi.identifier, xml_dict)
-                    toolkit.h.flash_success('DataCite DOI metadata updated')
+                    toolkit.h.flash_success("DataCite DOI metadata updated")
 
         return pkg_dict
 
     # IPackageController
-    def after_show(self, context, pkg_dict):
+    def after_dataset_show(self, context, pkg_dict):
         """
         Add the DOI details to the pkg_dict so it can be displayed.
         """
-        doi = DOIQuery.read_package(pkg_dict['id'])
+        doi = DOIQuery.read_package(pkg_dict["id"])
         if doi:
-            pkg_dict['doi'] = doi.identifier
-            pkg_dict['doi_status'] = True if doi.published else False
-            pkg_dict['domain'] = get_site_url().replace('http://', '')
-            pkg_dict['doi_date_published'] = (
-                datetime.strftime(doi.published, '%Y-%m-%d') if doi.published else None
+            pkg_dict["doi"] = doi.identifier
+            pkg_dict["doi_status"] = True if doi.published else False
+            pkg_dict["domain"] = get_site_url().replace("http://", "")
+            pkg_dict["doi_date_published"] = (
+                datetime.strftime(doi.published, "%Y-%m-%d") if doi.published else None
             )
-            pkg_dict['doi_publisher'] = toolkit.config.get('ckanext.doi.publisher')
+            pkg_dict["doi_publisher"] = toolkit.config.get("ckanext.doi.publisher")
+
+    def after_create(self, *args, **kwargs):
+        """
+        CKAN 2.9 compat version of after_dataset_create.
+        """
+        return self.after_dataset_create(*args, **kwargs)
+
+    def after_update(self, *args, **kwargs):
+        """
+        CKAN 2.9 compat version of after_dataset_update.
+        """
+        return self.after_dataset_update(*args, **kwargs)
+
+    def after_show(self, *args, **kwargs):
+        """
+        CKAN 2.9 compat version of after_dataset_show.
+        """
+        return self.after_dataset_show(*args, **kwargs)
 
     # ITemplateHelpers
     def get_helpers(self):
         return {
-            'package_get_year': package_get_year,
-            'now': datetime.now,
-            'get_site_title': get_site_title,
+            "package_get_year": package_get_year,
+            "now": datetime.now,
+            "get_site_title": get_site_title,
         }
```

### Comparing `ckanext-doi-3.1.8/ckanext/doi/theme/templates/doi/snippets/package_citation.html` & `ckanext-doi-3.1.9/ckanext/doi/theme/templates/doi/snippets/package_citation.html`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.8/ckanext/doi/theme/templates/doi/snippets/resource_citation.html` & `ckanext-doi-3.1.9/ckanext/doi/theme/templates/doi/snippets/resource_citation.html`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.8/ckanext/doi/theme/templates/package/read.html` & `ckanext-doi-3.1.9/ckanext/doi/theme/templates/package/read.html`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.8/ckanext/doi/theme/templates/package/snippets/package_metadata_fields.html` & `ckanext-doi-3.1.9/ckanext/doi/theme/templates/package/snippets/package_metadata_fields.html`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.8/ckanext_doi.egg-info/PKG-INFO` & `ckanext-doi-3.1.9/ckanext_doi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-doi
-Version: 3.1.8
+Version: 3.1.9
 Summary: A CKAN extension for assigning a digital object identifier (DOI) to datasets, using the DataCite DOI service.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-doi
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-doi/blob/main/CHANGELOG.md
 Keywords: CKAN,data,doi
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,25 +12,33 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: jsonschema==3.0.0
+Requires-Dist: xmltodict==0.12.0
+Requires-Dist: datacite==1.1.2
+Requires-Dist: ckantools>=0.3.0
+Provides-Extra: test
+Requires-Dist: mock; extra == "test"
+Requires-Dist: pytest>=4.6.5; extra == "test"
+Requires-Dist: pytest-cov>=2.7.1; extra == "test"
+Requires-Dist: coveralls; extra == "test"
 
 <!--header-start-->
 <img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-doi
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-doi/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-doi/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-doi/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-doi)
-[![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
+[![CKAN](https://img.shields.io/badge/ckan-2.9.9%20%7C%202.10.1-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
 [![Docs](https://img.shields.io/readthedocs/ckanext-doi?style=flat-square)](https://ckanext-doi.readthedocs.io)
 
 _A CKAN extension for assigning a digital object identifier (DOI) to datasets, using the DataCite DOI service._
 
 <!--header-end-->
 
@@ -246,26 +254,30 @@
 <!--usage-end-->
 
 # Testing
 
 <!--testing-start-->
 There is a Docker compose configuration available in this repository to make it easier to run tests. The ckan image uses the Dockerfile in the `docker/` folder.
 
-To run the tests against ckan 2.9.x on Python3:
+To run the tests can be run against ckan 2.9.x and 2.10.x on Python3:
 
 1. Build the required images:
    ```shell
    docker-compose build
    ```
 
 2. Then run the tests.
    The root of the repository is mounted into the ckan container as a volume by the Docker compose
    configuration, so you should only need to rebuild the ckan image if you change the extension's
    dependencies.
    ```shell
-   docker-compose run ckan
+   # run tests against ckan 2.9.x
+   docker-compose run latest
+
+   # run tests against ckan 2.10.x
+   docker-compose run next
    ```
 
 Note that the tests mock the DataCite API and therefore don't require an internet connection nor
 your DataCite credentials to run.
 
 <!--testing-end-->
```

### Comparing `ckanext-doi-3.1.8/ckanext_doi.egg-info/SOURCES.txt` & `ckanext-doi-3.1.9/ckanext_doi.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -30,9 +30,10 @@
 ckanext_doi.egg-info/not-zip-safe
 ckanext_doi.egg-info/requires.txt
 ckanext_doi.egg-info/top_level.txt
 docs/_scripts/gen_api_pages.py
 tests/test_api.py
 tests/test_db.py
 tests/test_generate.py
+tests/test_plugin.py
 tests/helpers/__init__.py
 tests/helpers/constants.py
```

### Comparing `ckanext-doi-3.1.8/docs/_scripts/gen_api_pages.py` & `ckanext-doi-3.1.9/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.8/pyproject.toml` & `ckanext-doi-3.1.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-doi"
-version = "3.1.8"
+version = "3.1.9"
 description = "A CKAN extension for assigning a digital object identifier (DOI) to datasets, using the DataCite DOI service."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -54,15 +54,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.doi.theme" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "3.1.8"
+version = "3.1.9"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
```

### Comparing `ckanext-doi-3.1.8/tests/helpers/constants.py` & `ckanext-doi-3.1.9/tests/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.8/tests/test_api.py` & `ckanext-doi-3.1.9/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.8/tests/test_db.py` & `ckanext-doi-3.1.9/tests/test_db.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,20 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 #
 # This file is part of ckanext-doi
 # Created by the Natural History Museum in London, UK
-import pytest
-from ckan.model import Session
-from ckan.tests import factories
-from datacite.errors import DataCiteNotFoundError
 from unittest.mock import patch, MagicMock
 
-from ckanext.doi.model.doi import DOI, doi_table
-
+import pytest
+from datacite.errors import DataCiteNotFoundError
 
-@pytest.fixture
-def with_doi_table(reset_db):
-    """
-    Simple fixture which resets the database and creates the doi table.
-    """
-    reset_db()
-    doi_table.create(checkfirst=True)
+from ckan.model import Session
+from ckan.tests import factories
+from ckanext.doi.model.doi import DOI
 
 
 @pytest.mark.filterwarnings('ignore::sqlalchemy.exc.SADeprecationWarning')
 @pytest.mark.ckan_config('ckan.plugins', 'doi')
 @pytest.mark.ckan_config('ckanext.doi.prefix', 'testing')
 @pytest.mark.usefixtures('with_doi_table', 'with_plugins')
 @patch('ckanext.doi.lib.api.DataCiteMDSClient')
```

### Comparing `ckanext-doi-3.1.8/tests/test_generate.py` & `ckanext-doi-3.1.9/tests/test_generate.py`

 * *Files identical despite different names*

