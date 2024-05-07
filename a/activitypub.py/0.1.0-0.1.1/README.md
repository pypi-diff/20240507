# Comparing `tmp/activitypub_py-0.1.0.tar.gz` & `tmp/activitypub_py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activitypub_py-0.1.0.tar", max compression
+gzip compressed data, was "activitypub_py-0.1.1.tar", max compression
```

## Comparing `activitypub_py-0.1.0.tar` & `activitypub_py-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0     1069 2024-04-18 07:46:47.567254 activitypub_py-0.1.0/LICENSE
--rw-r--r--   0        0        0       79 2024-04-18 07:53:53.603888 activitypub_py-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-18 07:53:52.464556 activitypub_py-0.1.0/activitypub/__init__.py
--rw-r--r--   0        0        0      477 2024-04-18 07:50:34.170974 activitypub_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 activitypub_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-18 08:10:29.329131 activitypub_py-0.1.1/LICENSE
+-rw-r--r--   0        0        0      157 2024-05-07 09:43:50.976065 activitypub_py-0.1.1/README.md
+-rw-r--r--   0        0        0     1240 2024-05-07 09:43:50.976256 activitypub_py-0.1.1/activitypub/__init__.py
+-rw-r--r--   0        0        0     1956 2024-05-07 11:00:22.977366 activitypub_py-0.1.1/activitypub/helper.py
+-rw-r--r--   0        0        0    19750 2024-05-07 09:43:50.976419 activitypub_py-0.1.1/activitypub/model.py
+-rw-r--r--   0        0        0      541 2024-05-07 11:12:16.529379 activitypub_py-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 activitypub_py-0.1.1/PKG-INFO
```

### Comparing `activitypub_py-0.1.0/LICENSE` & `activitypub_py-0.1.1/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 马特浩倪
+Copyright (c) 2024 Mattholy
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `activitypub_py-0.1.0/PKG-INFO` & `activitypub_py-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 Metadata-Version: 2.1
-Name: activitypub-py
-Version: 0.1.0
+Name: activitypub.py
+Version: 0.1.1
 Summary: Yet another ActivityPUB framework written in Python.
 License: MIT
 Author: Mattholy
 Author-email: smile.used@hotmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: httpsig (>=1.3.0,<2.0.0)
+Requires-Dist: isodate (>=0.6.1,<0.7.0)
+Requires-Dist: pycountry (>=23.12.11,<24.0.0)
 Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
-# activitypub.py [WIP]
+# Activitypub.py [WIP]
 Yet another ActivityPUB framework written in Python.
 
-# 
+# Install
+`pip install activitypub.py`
+
+# Usage
+
+## ActivityPub's Pydantic Model
```

