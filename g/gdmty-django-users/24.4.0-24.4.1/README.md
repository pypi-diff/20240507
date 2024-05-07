# Comparing `tmp/gdmty_django_users-24.4.0.tar.gz` & `tmp/gdmty_django_users-24.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdmty_django_users-24.4.0.tar", last modified: Mon May  6 03:30:51 2024, max compression
+gzip compressed data, was "gdmty_django_users-24.4.1.tar", last modified: Tue May  7 06:24:29 2024, max compression
```

## Comparing `gdmty_django_users-24.4.0.tar` & `gdmty_django_users-24.4.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 03:30:51.037202 gdmty_django_users-24.4.0/
--rw-rw-rw-   0        0        0    35182 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.0/LICENSE
--rw-rw-rw-   0        0        0       51 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0    43751 2024-05-06 03:30:51.037202 gdmty_django_users-24.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     2100 2024-05-06 03:29:06.000000 gdmty_django_users-24.4.0/README.md
--rw-rw-rw-   0        0        0     1577 2024-05-06 03:30:10.000000 gdmty_django_users-24.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-06 03:30:51.038274 gdmty_django_users-24.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-06 03:30:51.014047 gdmty_django_users-24.4.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 03:30:51.029530 gdmty_django_users-24.4.0/src/gdmty_django_users/
--rw-rw-rw-   0        0        0     1368 2024-05-06 03:30:10.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/__init__.py
--rw-rw-rw-   0        0        0     2480 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/admin.py
--rw-rw-rw-   0        0        0     1051 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/apps.py
--rw-rw-rw-   0        0        0      563 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/decorators.py
--rw-rw-rw-   0        0        0     1458 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/managers.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:30:51.035045 gdmty_django_users-24.4.0/src/gdmty_django_users/migrations/
--rw-rw-rw-   0        0        0     3284 2024-03-17 01:44:29.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/migrations/__init__.py
--rw-rw-rw-   0        0        0     2330 2024-05-06 03:29:06.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/models.py
--rw-rw-rw-   0        0        0      945 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/permissions.py
--rw-rw-rw-   0        0        0      889 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/serializers.py
--rw-rw-rw-   0        0        0     1070 2024-03-17 09:01:57.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/settings.py
--rw-rw-rw-   0        0        0      913 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/tests.py
--rw-rw-rw-   0        0        0      882 2024-05-06 03:29:06.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/urls.py
--rw-rw-rw-   0        0        0      877 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/views.py
--rw-rw-rw-   0        0        0     4816 2024-05-06 03:29:06.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/viewsets.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:30:51.036056 gdmty_django_users-24.4.0/src/gdmty_django_users.egg-info/
--rw-rw-rw-   0        0        0    43751 2024-05-06 03:30:51.000000 gdmty_django_users-24.4.0/src/gdmty_django_users.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      813 2024-05-06 03:30:51.000000 gdmty_django_users-24.4.0/src/gdmty_django_users.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 03:30:51.000000 gdmty_django_users-24.4.0/src/gdmty_django_users.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2024-05-06 03:30:51.000000 gdmty_django_users-24.4.0/src/gdmty_django_users.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-06 03:30:51.000000 gdmty_django_users-24.4.0/src/gdmty_django_users.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 06:24:29.502471 gdmty_django_users-24.4.1/
+-rw-rw-rw-   0        0        0    35182 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.1/LICENSE
+-rw-rw-rw-   0        0        0       51 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    43751 2024-05-07 06:24:29.502471 gdmty_django_users-24.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2100 2024-05-06 03:29:06.000000 gdmty_django_users-24.4.1/README.md
+-rw-rw-rw-   0        0        0     1577 2024-05-07 06:24:03.000000 gdmty_django_users-24.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-07 06:24:29.502471 gdmty_django_users-24.4.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-07 06:24:29.481779 gdmty_django_users-24.4.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 06:24:29.494392 gdmty_django_users-24.4.1/src/gdmty_django_users/
+-rw-rw-rw-   0        0        0     1368 2024-05-07 06:24:03.000000 gdmty_django_users-24.4.1/src/gdmty_django_users/__init__.py
+-rw-rw-rw-   0        0        0     2478 2024-05-07 06:22:05.000000 gdmty_django_users-24.4.1/src/gdmty_django_users/admin.py
+-rw-rw-rw-   0        0        0     1049 2024-05-07 06:22:05.000000 gdmty_django_users-24.4.1/src/gdmty_django_users/apps.py
+-rw-rw-rw-   0        0        0     1438 2024-05-07 06:23:41.000000 gdmty_django_users-24.4.1/src/gdmty_django_users/decorators.py
+-rw-rw-rw-   0        0        0     2333 2024-05-07 06:23:41.000000 gdmty_django_users-24.4.1/src/gdmty_django_users/managers.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:24:29.500461 gdmty_django_users-24.4.1/src/gdmty_django_users/migrations/
+-rw-rw-rw-   0        0        0     3284 2024-03-17 01:44:29.000000 gdmty_django_users-24.4.1/src/gdmty_django_users/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.1/src/gdmty_django_users/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3205 2024-05-07 06:23:41.000000 gdmty_django_users-24.4.1/src/gdmty_django_users/models.py
+-rw-rw-rw-   0        0        0     1820 2024-05-07 06:23:41.000000 gdmty_django_users-24.4.1/src/gdmty_django_users/permissions.py
+-rw-rw-rw-   0        0        0     1764 2024-05-07 06:23:41.000000 gdmty_django_users-24.4.1/src/gdmty_django_users/serializers.py
+-rw-rw-rw-   0        0        0     1066 2024-05-07 06:23:41.000000 gdmty_django_users-24.4.1/src/gdmty_django_users/settings.py
+-rw-rw-rw-   0        0        0      911 2024-05-07 06:22:05.000000 gdmty_django_users-24.4.1/src/gdmty_django_users/tests.py
+-rw-rw-rw-   0        0        0     1757 2024-05-07 06:23:41.000000 gdmty_django_users-24.4.1/src/gdmty_django_users/urls.py
+-rw-rw-rw-   0        0        0     4812 2024-05-07 06:23:41.000000 gdmty_django_users-24.4.1/src/gdmty_django_users/viewsets.py
+-rw-rw-rw-   0        0        0     1472 2024-05-07 06:23:41.000000 gdmty_django_users-24.4.1/src/gdmty_django_users/wagtail_forms.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:24:29.500461 gdmty_django_users-24.4.1/src/gdmty_django_users.egg-info/
+-rw-rw-rw-   0        0        0    43751 2024-05-07 06:24:29.000000 gdmty_django_users-24.4.1/src/gdmty_django_users.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      821 2024-05-07 06:24:29.000000 gdmty_django_users-24.4.1/src/gdmty_django_users.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 06:24:29.000000 gdmty_django_users-24.4.1/src/gdmty_django_users.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2024-05-07 06:24:29.000000 gdmty_django_users-24.4.1/src/gdmty_django_users.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-07 06:24:29.000000 gdmty_django_users-24.4.1/src/gdmty_django_users.egg-info/top_level.txt
```

### Comparing `gdmty_django_users-24.4.0/LICENSE` & `gdmty_django_users-24.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.4.0/PKG-INFO` & `gdmty_django_users-24.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdmty-django-users
-Version: 24.4.0
+Version: 24.4.1
 Summary: Custom Django Rest Framework authentication backend based on email and password for users in Administration panel with reCaptcha token verification.
 Author-email: Gobierno de Monterrey <cesar.benjamin@monterrey.gob.mx>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `gdmty_django_users-24.4.0/README.md` & `gdmty_django_users-24.4.1/README.md`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.4.0/pyproject.toml` & `gdmty_django_users-24.4.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gdmty-django-users"
-version = "24.4.0"
+version = "24.4.1"
 description = "Custom Django Rest Framework authentication backend based on email and password for users in Administration panel with reCaptcha token verification."
 readme = "README.md"
 authors = [{ name="Gobierno de Monterrey", email="cesar.benjamin@monterrey.gob.mx" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Programming Language :: Python",
@@ -31,15 +31,15 @@
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 "Homepage" = "https://github.com/gobiernodigital/gdmty-django-users"
 "Bug Tracker" = "https://github.com/gobiernodigital/gdmty-django-users/issues"
 
 [tool.bumpver]
-current_version = "24.4.0"
+current_version = "24.4.1"
 version_pattern = "MAJOR.MINOR.PATCH[-PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = true
```

### Comparing `gdmty_django_users-24.4.0/src/gdmty_django_users/__init__.py` & `gdmty_django_users-24.4.1/src/gdmty_django_users/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Package: gdmty_django_users
 PyPi: https://pypi.org/project/gdmty-django-users/
 License: GNU Affero General Public License v3 or later (AGPLv3+)
 
 """
 
 __title__ = "gdmty_django_users"
-__version__ = "24.4.0"
+__version__ = "24.4.1"
 __description__ = "Django module for Users models and permission adding reCAPTCHA token verification."
 __url__ = "https://github.com/SIGAMty/gdmty-django-recaptcha-enterprise"
 __author__ = "César Benjamín"
 __author_email__ = "mathereall@gmail.com"
 __license__ = "GNU Affero General Public License v3 or later (AGPLv3+)"
 __keywords__ = ["django", "users"]
 VERSION = __version__
```

### Comparing `gdmty_django_users-24.4.0/src/gdmty_django_users/admin.py` & `gdmty_django_users-24.4.1/src/gdmty_django_users/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', 'Miguel Angel Hernández Cortés
 <miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <chechar.2001@gmail.com>']
 Email: gobiernodigital@monterrey.gob.mx
 GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
 Package: gdmty_django_users
 PyPi: https://pypi.org/project/gdmty-django-users/
-License: Apache 2.0
+License: AGPL-3.0
 
 """
 
 from django.contrib import admin
 from django.contrib.auth.models import Group as GroupDjango
 from .models import User, Group
 from django.contrib.auth.admin import UserAdmin as UserAdminDjango
```

### Comparing `gdmty_django_users-24.4.0/src/gdmty_django_users/apps.py` & `gdmty_django_users-24.4.1/src/gdmty_django_users/apps.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', 'Miguel Angel Hernández Cortés
 <miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <chechar.2001@gmail.com>']
 Email: gobiernodigital@monterrey.gob.mx
 GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
 Package: gdmty_django_users
 PyPi: https://pypi.org/project/gdmty-django-users/
-License: Apache 2.0
+License: AGPL-3.0
 
 """
 
 from django.apps import AppConfig
 
 
 class GdmtyDjangoUsersConfig(AppConfig):
```

### Comparing `gdmty_django_users-24.4.0/src/gdmty_django_users/managers.py` & `gdmty_django_users-24.4.1/src/gdmty_django_users/managers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+#!-*- coding: utf-8 -*-
+"""
+Authentication backend for Django's Administration panel users based on email and password
+This packages adds features such as group permissions and reCaptcha enterprise token verification.
+
+This package is published as free software under the terms of the Apache License, Version 2.0. Is developed by
+Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
+
+Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', 'Miguel Angel Hernández Cortés
+<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <chechar.2001@gmail.com>']
+Email: gobiernodigital@monterrey.gob.mx
+GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
+Package: gdmty_django_users
+PyPi: https://pypi.org/project/gdmty-django-users/
+License: AGPL-3.0
+"""
+
 from django.contrib.auth.base_user import BaseUserManager
 from django.utils.translation import gettext_lazy as _
 
 
 class CustomUserManager(BaseUserManager):
     """
     Custom user model manager where email is the unique identifiers
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gdmty_django_users-24.4.0/src/gdmty_django_users/migrations/0001_initial.py` & `gdmty_django_users-24.4.1/src/gdmty_django_users/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.4.0/src/gdmty_django_users/permissions.py` & `gdmty_django_users-24.4.1/src/gdmty_django_users/permissions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+#!-*- coding: utf-8 -*-
+"""
+Authentication backend for Django's Administration panel users based on email and password
+This packages adds features such as group permissions and reCaptcha enterprise token verification.
+
+This package is published as free software under the terms of the Apache License, Version 2.0. Is developed by
+Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
+
+Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', 'Miguel Angel Hernández Cortés
+<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <chechar.2001@gmail.com>']
+Email: gobiernodigital@monterrey.gob.mx
+GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
+Package: gdmty_django_users
+PyPi: https://pypi.org/project/gdmty-django-users/
+License: AGPL-3.0
+"""
+
 from rest_framework import permissions
 from rest_framework.permissions import SAFE_METHODS
 
 #
 
 
 class IsAuthenticatedAndSelfOrIsStaff(permissions.BasePermission):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gdmty_django_users-24.4.0/src/gdmty_django_users/serializers.py` & `gdmty_django_users-24.4.1/src/gdmty_django_users/serializers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+#!-*- coding: utf-8 -*-
+"""
+Authentication backend for Django's Administration panel users based on email and password
+This packages adds features such as group permissions and reCaptcha enterprise token verification.
+
+This package is published as free software under the terms of the Apache License, Version 2.0. Is developed by
+Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
+
+Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', 'Miguel Angel Hernández Cortés
+<miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <chechar.2001@gmail.com>']
+Email: gobiernodigital@monterrey.gob.mx
+GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
+Package: gdmty_django_users
+PyPi: https://pypi.org/project/gdmty-django-users/
+License: AGPL-3.0
+"""
+
 from rest_framework import serializers
 from .models import User, Group
 from django.contrib.auth.models import Permission
 
 #
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gdmty_django_users-24.4.0/src/gdmty_django_users/settings.py` & `gdmty_django_users-24.4.1/src/gdmty_django_users/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 
 Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', 'Miguel Angel Hernández Cortés
 <miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <chechar.2001@gmail.com>']
 Email: gobiernodigital@monterrey.gob.mx
 GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
 Package: gdmty_django_users
 PyPi: https://pypi.org/project/gdmty-django-users/
-License: Apache 2.0
-
+License: AGPL-3.0
 """
 
 import os
 from django.conf import settings
 import logging
 from . import __title__
```

### Comparing `gdmty_django_users-24.4.0/src/gdmty_django_users/tests.py` & `gdmty_django_users-24.4.1/src/gdmty_django_users/decorators.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,12 +8,25 @@
 
 Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', 'Miguel Angel Hernández Cortés
 <miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <chechar.2001@gmail.com>']
 Email: gobiernodigital@monterrey.gob.mx
 GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
 Package: gdmty_django_users
 PyPi: https://pypi.org/project/gdmty-django-users/
-License: Apache 2.0
-
+License: AGPL-3.0
 """
 
-from django.test import TestCase
+from functools import wraps
+from gdmty_django_recaptcha_enterprise.decorators import requires_recaptcha_token
+from .settings import ENABLE_RECAPTCHA
+
+
+def recaptcha_verify(action=None):
+    def decorator(view_func):
+        @wraps(view_func)
+        def _wrapped_view(request, *args, **kwargs):
+            if ENABLE_RECAPTCHA:
+                return requires_recaptcha_token(action)(view_func)(request, *args, **kwargs)
+            else:
+                return view_func(request, *args, **kwargs)
+        return _wrapped_view
+    return decorator
```

### Comparing `gdmty_django_users-24.4.0/src/gdmty_django_users/viewsets.py` & `gdmty_django_users-24.4.1/src/gdmty_django_users/viewsets.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 
 Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', 'Miguel Angel Hernández Cortés
 <miguelhdezc12@gmail.com>', 'César Guillermo Vázquez Álvarez <chechar.2001@gmail.com>']
 Email: gobiernodigital@monterrey.gob.mx
 GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
 Package: gdmty_django_users
 PyPi: https://pypi.org/project/gdmty-django-users/
-License: Apache 2.0
-
+License: AGPL-3.0
 """
 
 from rest_framework import viewsets
 from .models import User, Group
 from django.contrib.auth.models import Permission
 from .serializers import UserSerializer, GroupSerializer, PermissionSerializer
 from .permissions import IsAuthenticatedAndSelfOrIsStaff
```

### Comparing `gdmty_django_users-24.4.0/src/gdmty_django_users.egg-info/PKG-INFO` & `gdmty_django_users-24.4.1/src/gdmty_django_users.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdmty-django-users
-Version: 24.4.0
+Version: 24.4.1
 Summary: Custom Django Rest Framework authentication backend based on email and password for users in Administration panel with reCaptcha token verification.
 Author-email: Gobierno de Monterrey <cesar.benjamin@monterrey.gob.mx>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `gdmty_django_users-24.4.0/src/gdmty_django_users.egg-info/SOURCES.txt` & `gdmty_django_users-24.4.1/src/gdmty_django_users.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 src/gdmty_django_users/managers.py
 src/gdmty_django_users/models.py
 src/gdmty_django_users/permissions.py
 src/gdmty_django_users/serializers.py
 src/gdmty_django_users/settings.py
 src/gdmty_django_users/tests.py
 src/gdmty_django_users/urls.py
-src/gdmty_django_users/views.py
 src/gdmty_django_users/viewsets.py
+src/gdmty_django_users/wagtail_forms.py
 src/gdmty_django_users.egg-info/PKG-INFO
 src/gdmty_django_users.egg-info/SOURCES.txt
 src/gdmty_django_users.egg-info/dependency_links.txt
 src/gdmty_django_users.egg-info/requires.txt
 src/gdmty_django_users.egg-info/top_level.txt
 src/gdmty_django_users/migrations/0001_initial.py
 src/gdmty_django_users/migrations/__init__.py
```

