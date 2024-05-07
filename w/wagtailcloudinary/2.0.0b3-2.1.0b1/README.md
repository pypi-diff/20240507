# Comparing `tmp/wagtailcloudinary-2.0.0b3.tar.gz` & `tmp/wagtailcloudinary-2.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailcloudinary-2.0.0b3.tar", last modified: Mon Mar 13 14:46:24 2023, max compression
+gzip compressed data, was "wagtailcloudinary-2.1.0b1.tar", max compression
```

## Comparing `wagtailcloudinary-2.0.0b3.tar` & `wagtailcloudinary-2.1.0b1.tar`

### file list

```diff
@@ -1,53 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 14:46:24.326899 wagtailcloudinary-2.0.0b3/
--rw-rw-rw-   0 root         (0) root         (0)      740 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      220 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2340 2023-03-13 14:46:24.327900 wagtailcloudinary-2.0.0b3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1549 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/README.md
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-03-13 14:46:24.327900 wagtailcloudinary-2.0.0b3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1689 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 14:46:24.313899 wagtailcloudinary-2.0.0b3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 14:46:24.320899 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      659 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     4714 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/api.py
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     2272 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/blocks.py
--rw-rw-rw-   0 root         (0) root         (0)     1267 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 14:46:24.322899 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 14:46:24.323899 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1372 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/management/commands/import_cloudinary_images.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 14:46:24.323899 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/migrations/
--rwxrwxrwx   0 root         (0) root         (0)     3206 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1955 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 14:46:24.314899 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 14:46:24.314899 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/static/wagtailcloudinary/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 14:46:24.323899 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/static/wagtailcloudinary/css/
--rw-rw-rw-   0 root         (0) root         (0)      159 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/static/wagtailcloudinary/css/main.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 14:46:24.324899 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/static/wagtailcloudinary/js/
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/static/wagtailcloudinary/js/cloudinary-chooser-telepath.js
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/static/wagtailcloudinary/js/cloudinary-chooser.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 14:46:24.315899 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 14:46:24.315899 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/templates/wagtailcloudinary/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 14:46:24.325899 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/templates/wagtailcloudinary/chooser/
--rw-rw-rw-   0 root         (0) root         (0)      894 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/templates/wagtailcloudinary/chooser/chooser.html
--rw-rw-rw-   0 root         (0) root         (0)     1976 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/templates/wagtailcloudinary/chooser/results.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 14:46:24.325899 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/templates/wagtailcloudinary/include/
--rw-rw-rw-   0 root         (0) root         (0)      887 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/templates/wagtailcloudinary/include/cloudinary.html
--rw-rw-rw-   0 root         (0) root         (0)      833 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/templates/wagtailcloudinary/include/pagination_nav.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 14:46:24.326899 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/templates/wagtailcloudinary/widgets/
--rw-rw-rw-   0 root         (0) root         (0)      489 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/templates/wagtailcloudinary/widgets/cloudinary_chooser.html
--rw-rw-rw-   0 root         (0) root         (0)     1337 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 14:46:24.326899 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4100 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/views/chooser.py
--rw-rw-rw-   0 root         (0) root         (0)      755 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/wagtail_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     2091 2023-03-13 14:46:13.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/widgets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 14:46:24.322899 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2340 2023-03-13 14:46:24.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1526 2023-03-13 14:46:24.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-13 14:46:24.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      111 2023-03-13 14:46:24.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-03-13 14:46:24.000000 wagtailcloudinary-2.0.0b3/src/wagtailcloudinary.egg-info/top_level.txt
+-rw-r--r--   0        0        0      747 2024-05-07 21:41:53.080952 wagtailcloudinary-2.1.0b1/LICENSE
+-rw-r--r--   0        0        0     1549 2024-05-07 21:41:53.080952 wagtailcloudinary-2.1.0b1/README.md
+-rw-r--r--   0        0        0      683 2024-05-07 21:41:53.081951 wagtailcloudinary-2.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-07 21:41:53.113951 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/__init__.py
+-rw-r--r--   0        0        0      659 2024-05-07 21:41:53.082952 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/admin.py
+-rw-r--r--   0        0        0     4714 2024-05-07 21:41:53.082952 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/api.py
+-rw-r--r--   0        0        0      181 2024-05-07 21:41:53.082952 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/apps.py
+-rw-r--r--   0        0        0     2272 2024-05-07 21:41:53.082952 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/blocks.py
+-rw-r--r--   0        0        0     1267 2024-05-07 21:41:53.082952 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/fields.py
+-rw-r--r--   0        0        0        0 2024-05-07 21:41:53.113951 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 21:41:53.113951 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/management/commands/__init__.py
+-rw-r--r--   0        0        0     1372 2024-05-07 21:41:53.082952 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/management/commands/import_cloudinary_images.py
+-rwxr-xr-x   0        0        0     3206 2024-05-07 21:41:53.082952 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-07 21:41:53.113951 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/migrations/__init__.py
+-rw-r--r--   0        0        0     1955 2024-05-07 21:41:53.082952 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/models.py
+-rw-r--r--   0        0        0      159 2024-05-07 21:41:53.083952 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/static/wagtailcloudinary/css/main.css
+-rw-r--r--   0        0        0      354 2024-05-07 21:41:53.083952 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/static/wagtailcloudinary/js/cloudinary-chooser-telepath.js
+-rw-r--r--   0        0        0      101 2024-05-07 21:41:53.083952 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/static/wagtailcloudinary/js/cloudinary-chooser.js
+-rw-r--r--   0        0        0      894 2024-05-07 21:41:53.083952 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/templates/wagtailcloudinary/chooser/chooser.html
+-rw-r--r--   0        0        0     1976 2024-05-07 21:41:53.083952 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/templates/wagtailcloudinary/chooser/results.html
+-rw-r--r--   0        0        0      887 2024-05-07 21:41:53.083952 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/templates/wagtailcloudinary/include/cloudinary.html
+-rw-r--r--   0        0        0      833 2024-05-07 21:41:53.083952 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/templates/wagtailcloudinary/include/pagination_nav.html
+-rw-r--r--   0        0        0      489 2024-05-07 21:41:53.083952 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/templates/wagtailcloudinary/widgets/cloudinary_chooser.html
+-rw-r--r--   0        0        0     1337 2024-05-07 21:41:53.083952 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/utils.py
+-rw-r--r--   0        0        0        0 2024-05-07 21:41:53.114951 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/views/__init__.py
+-rw-r--r--   0        0        0     4100 2024-05-07 21:41:53.083952 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/views/chooser.py
+-rw-r--r--   0        0        0      761 2024-05-07 21:41:53.083952 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/wagtail_hooks.py
+-rw-r--r--   0        0        0     2091 2024-05-07 21:41:53.083952 wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/widgets.py
+-rw-r--r--   0        0        0     2273 1970-01-01 00:00:00.000000 wagtailcloudinary-2.1.0b1/PKG-INFO
```

### Comparing `wagtailcloudinary-2.0.0b3/LICENSE` & `wagtailcloudinary-2.1.0b1/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ISC License
 
-Copyright (c) 2023 thelabnyc
+Copyright (c) 2017 - 2024 thelabnyc
 
 Permission to use, copy, modify, and/or distribute this software for any
 purpose with or without fee is hereby granted, provided that the above
 copyright notice and this permission notice appear in all copies.
 
 THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
 REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY
```

### Comparing `wagtailcloudinary-2.0.0b3/PKG-INFO` & `wagtailcloudinary-2.1.0b1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: wagtailcloudinary
-Version: 2.0.0b3
+Version: 2.1.0b1
 Summary: Cloudinary support for Wagtail CMS
 Home-page: https://gitlab.com/thelabnyc/wagtailcloudinary
+License: ISC
 Author: thelabnyc
 Author-email: thelabdev@thelabnyc.com
-License: ISC
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Wagtail
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: cloudinary (>=1,<2)
+Requires-Dist: python-dateutil (>=2.7)
+Requires-Dist: wagtail (>=5.2,<6.0)
+Project-URL: Repository, https://gitlab.com/thelabnyc/wagtailcloudinary
 Description-Content-Type: text/markdown
-Provides-Extra: development
-License-File: LICENSE
 
 # Use cloudinary within wagtail
 
 This project is still maintained, but I prefer this approach instead now https://gitlab.com/thelabnyc/wagtail-cloudinary-image
 
 ## About
 
@@ -90,7 +88,8 @@
         FieldPanel('image', widget=AdminCloudinaryChooser),
     ]
 ```
 
 Or use in a streamfield
 
 `from wagtailcloudinary.blocks import CloudinaryImageBlock`
+
```

### Comparing `wagtailcloudinary-2.0.0b3/README.md` & `wagtailcloudinary-2.1.0b1/README.md`

 * *Files identical despite different names*

### Comparing `wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/admin.py` & `wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/admin.py`

 * *Files identical despite different names*

### Comparing `wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/api.py` & `wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/api.py`

 * *Files identical despite different names*

### Comparing `wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/blocks.py` & `wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/fields.py` & `wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/fields.py`

 * *Files identical despite different names*

### Comparing `wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/management/commands/import_cloudinary_images.py` & `wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/management/commands/import_cloudinary_images.py`

 * *Files identical despite different names*

### Comparing `wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/migrations/0001_initial.py` & `wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/models.py` & `wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/models.py`

 * *Files identical despite different names*

### Comparing `wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/templates/wagtailcloudinary/chooser/chooser.html` & `wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/templates/wagtailcloudinary/chooser/chooser.html`

 * *Files identical despite different names*

### Comparing `wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/templates/wagtailcloudinary/chooser/results.html` & `wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/templates/wagtailcloudinary/chooser/results.html`

 * *Files identical despite different names*

### Comparing `wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/templates/wagtailcloudinary/include/cloudinary.html` & `wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/templates/wagtailcloudinary/include/cloudinary.html`

 * *Files identical despite different names*

### Comparing `wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/templates/wagtailcloudinary/include/pagination_nav.html` & `wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/templates/wagtailcloudinary/include/pagination_nav.html`

 * *Files identical despite different names*

### Comparing `wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/utils.py` & `wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/utils.py`

 * *Files identical despite different names*

### Comparing `wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/views/chooser.py` & `wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/views/chooser.py`

 * *Files identical despite different names*

### Comparing `wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/wagtail_hooks.py` & `wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/wagtail_hooks.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django.templatetags.static import static
 from django.urls import reverse
 from django.utils.html import format_html
 from wagtail import hooks
 from .views.chooser import viewset as cloudinary_viewset
 
 
-@hooks.register("insert_editor_css")
+@hooks.register("insert_global_admin_css")
 def global_admin_css():
     return format_html(
         '<link rel="stylesheet" href="{}">', static("wagtailcloudinary/css/main.css")
     )
 
 
 @hooks.register("insert_editor_js")
```

### Comparing `wagtailcloudinary-2.0.0b3/src/wagtailcloudinary/widgets.py` & `wagtailcloudinary-2.1.0b1/src/wagtailcloudinary/widgets.py`

 * *Files identical despite different names*

