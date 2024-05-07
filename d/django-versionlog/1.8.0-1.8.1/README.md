# Comparing `tmp/django-versionlog-1.8.0.tar.gz` & `tmp/django-versionlog-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-versionlog-1.8.0.tar", last modified: Mon May  6 08:20:38 2024, max compression
+gzip compressed data, was "dist/django-versionlog-1.8.1.tar", last modified: Tue May  7 09:23:53 2024, max compression
```

## Comparing `django-versionlog-1.8.0.tar` & `django-versionlog-1.8.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/
--rw-r--r--   0 root         (0) root         (0)     6014 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1514 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/version_log/
--rw-r--r--   0 root         (0) root         (0)     1769 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/urls.py
--rw-r--r--   0 root         (0) root         (0)     1043 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/apps.py
--rw-r--r--   0 root         (0) root         (0)     6936 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/version_log/migrations/
--rw-r--r--   0 root         (0) root         (0)      750 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1452 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/migrations/0001_initial.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/version_log/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/version_log/static/version_log/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/version_log/static/version_log/js/
--rw-r--r--   0 root         (0) root         (0)    40547 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/static/version_log/js/jquery.mCustomScrollbar.concat.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/version_log/static/version_log/images/
--rw-r--r--   0 root         (0) root         (0)      297 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/static/version_log/images/down.svg
--rw-r--r--   0 root         (0) root         (0)     1048 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/static/version_log/images/up.svg
--rw-r--r--   0 root         (0) root         (0)      144 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/static/version_log/images/back.svg
--rw-r--r--   0 root         (0) root         (0)      474 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/static/version_log/images/homepage.svg
--rw-r--r--   0 root         (0) root         (0)    11143 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/static/version_log/images/error.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/version_log/static/version_log/css/
--rw-r--r--   0 root         (0) root         (0)     1579 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/static/version_log/css/version-log-gitbook-page.css
--rw-r--r--   0 root         (0) root         (0)     2761 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/static/version_log/css/version-log-page.css
--rw-r--r--   0 root         (0) root         (0)    52607 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/static/version_log/css/jquery.mCustomScrollbar.css
--rw-r--r--   0 root         (0) root         (0)     2233 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/models.py
--rw-r--r--   0 root         (0) root         (0)      750 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5909 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/utils.py
--rw-r--r--   0 root         (0) root         (0)     2698 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/version_log/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/version_log/templates/version_log/
--rw-r--r--   0 root         (0) root         (0)     3226 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/templates/version_log/version_logs_page.html
--rw-r--r--   0 root         (0) root         (0)     5197 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/templates/version_log/version_logs_block.html
--rw-r--r--   0 root         (0) root         (0)     2343 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/templates/version_log/version_logs_dialog_page.html
--rw-r--r--   0 root         (0) root         (0)     3461 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/config.py
--rw-r--r--   0 root         (0) root         (0)     3127 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/docs/img/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/docs/img/icons/
--rw-r--r--   0 root         (0) root         (0)   146107 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/docs/img/icons/django-versionlog.png
--rw-r--r--   0 root         (0) root         (0)  2421404 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/docs/img/icons/qr_code.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/docs/img/demos/
--rw-r--r--   0 root         (0) root         (0)    52475 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/docs/img/demos/gitbook-page.png
--rw-r--r--   0 root         (0) root         (0)   169230 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/docs/img/demos/dialog.png
--rw-r--r--   0 root         (0) root         (0)   134216 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/docs/img/demos/dialog-page.png
--rw-r--r--   0 root         (0) root         (0)     1097 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/docs/contributing.md
--rw-r--r--   0 root         (0) root         (0)      690 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/docs/structure.md
--rw-r--r--   0 root         (0) root         (0)      876 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/docs/feature.md
--rw-r--r--   0 root         (0) root         (0)     3836 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/docs/usage.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/django_versionlog.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6014 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/django_versionlog.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/django_versionlog.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/django_versionlog.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/django_versionlog.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/django_versionlog.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1452 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/django_versionlog.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1069 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      210 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4888 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 09:23:53.000000 django-versionlog-1.8.1/
+-rw-r--r--   0 root         (0) root         (0)     6014 2024-05-07 09:23:53.000000 django-versionlog-1.8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1514 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 09:23:53.000000 django-versionlog-1.8.1/version_log/
+-rw-r--r--   0 root         (0) root         (0)     1769 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/version_log/urls.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/version_log/apps.py
+-rw-r--r--   0 root         (0) root         (0)     6936 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/version_log/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 09:23:53.000000 django-versionlog-1.8.1/version_log/migrations/
+-rw-r--r--   0 root         (0) root         (0)      750 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/version_log/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/version_log/migrations/0001_initial.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 09:23:53.000000 django-versionlog-1.8.1/version_log/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 09:23:53.000000 django-versionlog-1.8.1/version_log/static/version_log/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 09:23:53.000000 django-versionlog-1.8.1/version_log/static/version_log/js/
+-rw-r--r--   0 root         (0) root         (0)    40547 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/version_log/static/version_log/js/jquery.mCustomScrollbar.concat.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 09:23:53.000000 django-versionlog-1.8.1/version_log/static/version_log/images/
+-rw-r--r--   0 root         (0) root         (0)      297 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/version_log/static/version_log/images/down.svg
+-rw-r--r--   0 root         (0) root         (0)     1048 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/version_log/static/version_log/images/up.svg
+-rw-r--r--   0 root         (0) root         (0)      144 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/version_log/static/version_log/images/back.svg
+-rw-r--r--   0 root         (0) root         (0)      474 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/version_log/static/version_log/images/homepage.svg
+-rw-r--r--   0 root         (0) root         (0)    11143 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/version_log/static/version_log/images/error.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 09:23:53.000000 django-versionlog-1.8.1/version_log/static/version_log/css/
+-rw-r--r--   0 root         (0) root         (0)     1579 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/version_log/static/version_log/css/version-log-gitbook-page.css
+-rw-r--r--   0 root         (0) root         (0)     2761 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/version_log/static/version_log/css/version-log-page.css
+-rw-r--r--   0 root         (0) root         (0)    52607 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/version_log/static/version_log/css/jquery.mCustomScrollbar.css
+-rw-r--r--   0 root         (0) root         (0)     2233 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/version_log/models.py
+-rw-r--r--   0 root         (0) root         (0)      750 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/version_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5909 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/version_log/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2698 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/version_log/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 09:23:53.000000 django-versionlog-1.8.1/version_log/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 09:23:53.000000 django-versionlog-1.8.1/version_log/templates/version_log/
+-rw-r--r--   0 root         (0) root         (0)     3226 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/version_log/templates/version_log/version_logs_page.html
+-rw-r--r--   0 root         (0) root         (0)     5197 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/version_log/templates/version_log/version_logs_block.html
+-rw-r--r--   0 root         (0) root         (0)     2343 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/version_log/templates/version_log/version_logs_dialog_page.html
+-rw-r--r--   0 root         (0) root         (0)     3461 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/version_log/config.py
+-rw-r--r--   0 root         (0) root         (0)     3127 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/version_log/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 09:23:53.000000 django-versionlog-1.8.1/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 09:23:53.000000 django-versionlog-1.8.1/docs/img/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 09:23:53.000000 django-versionlog-1.8.1/docs/img/icons/
+-rw-r--r--   0 root         (0) root         (0)   146107 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/docs/img/icons/django-versionlog.png
+-rw-r--r--   0 root         (0) root         (0)  2421404 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/docs/img/icons/qr_code.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 09:23:53.000000 django-versionlog-1.8.1/docs/img/demos/
+-rw-r--r--   0 root         (0) root         (0)    52475 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/docs/img/demos/gitbook-page.png
+-rw-r--r--   0 root         (0) root         (0)   169230 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/docs/img/demos/dialog.png
+-rw-r--r--   0 root         (0) root         (0)   134216 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/docs/img/demos/dialog-page.png
+-rw-r--r--   0 root         (0) root         (0)     1097 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/docs/contributing.md
+-rw-r--r--   0 root         (0) root         (0)      690 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/docs/structure.md
+-rw-r--r--   0 root         (0) root         (0)      876 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/docs/feature.md
+-rw-r--r--   0 root         (0) root         (0)     3836 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/docs/usage.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 09:23:53.000000 django-versionlog-1.8.1/django_versionlog.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6014 2024-05-07 09:23:53.000000 django-versionlog-1.8.1/django_versionlog.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-07 09:23:53.000000 django-versionlog-1.8.1/django_versionlog.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-07 09:23:53.000000 django-versionlog-1.8.1/django_versionlog.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 09:23:53.000000 django-versionlog-1.8.1/django_versionlog.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 09:23:53.000000 django-versionlog-1.8.1/django_versionlog.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1452 2024-05-07 09:23:53.000000 django-versionlog-1.8.1/django_versionlog.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 09:23:53.000000 django-versionlog-1.8.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      210 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4888 2024-05-07 09:23:51.000000 django-versionlog-1.8.1/README.md
```

### Comparing `django-versionlog-1.8.0/PKG-INFO` & `django-versionlog-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-versionlog
-Version: 1.8.0
+Version: 1.8.1
 Summary: version log module
 Home-page: https://github.com/TencentBlueKing/django-versionlog
 Author: blueking
 Author-email: blueking@tencent.com
 License: UNKNOWN
 Description: # django-versionlog
```

### Comparing `django-versionlog-1.8.0/setup.py` & `django-versionlog-1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,21 +19,21 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-versionlog',
-    version='1.8.0',
+    version='1.8.1',
     packages=find_packages(),
     include_package_data=True,
     url="https://github.com/TencentBlueKing/django-versionlog",
     description='version log module',
     long_description=README,
     long_description_content_type='text/markdown',
     author='blueking',
     author_email='blueking@tencent.com',
     install_requires=[
-        'mistune==0.8.4'
+        'mistune>=0.8.4'
     ],
     zip_safe=False,
 )
```

### Comparing `django-versionlog-1.8.0/version_log/urls.py` & `django-versionlog-1.8.1/version_log/urls.py`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/version_log/apps.py` & `django-versionlog-1.8.1/version_log/apps.py`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/version_log/views.py` & `django-versionlog-1.8.1/version_log/views.py`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/version_log/migrations/__init__.py` & `django-versionlog-1.8.1/version_log/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/version_log/migrations/0001_initial.py` & `django-versionlog-1.8.1/version_log/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/version_log/static/version_log/js/jquery.mCustomScrollbar.concat.min.js` & `django-versionlog-1.8.1/version_log/static/version_log/js/jquery.mCustomScrollbar.concat.min.js`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/version_log/static/version_log/images/up.svg` & `django-versionlog-1.8.1/version_log/static/version_log/images/up.svg`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/version_log/static/version_log/images/error.png` & `django-versionlog-1.8.1/version_log/static/version_log/images/error.png`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/version_log/static/version_log/css/version-log-gitbook-page.css` & `django-versionlog-1.8.1/version_log/static/version_log/css/version-log-gitbook-page.css`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/version_log/static/version_log/css/version-log-page.css` & `django-versionlog-1.8.1/version_log/static/version_log/css/version-log-page.css`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/version_log/static/version_log/css/jquery.mCustomScrollbar.css` & `django-versionlog-1.8.1/version_log/static/version_log/css/jquery.mCustomScrollbar.css`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/version_log/models.py` & `django-versionlog-1.8.1/version_log/models.py`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/version_log/__init__.py` & `django-versionlog-1.8.1/version_log/__init__.py`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/version_log/utils.py` & `django-versionlog-1.8.1/version_log/utils.py`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/version_log/decorators.py` & `django-versionlog-1.8.1/version_log/decorators.py`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/version_log/templates/version_log/version_logs_page.html` & `django-versionlog-1.8.1/version_log/templates/version_log/version_logs_page.html`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/version_log/templates/version_log/version_logs_block.html` & `django-versionlog-1.8.1/version_log/templates/version_log/version_logs_block.html`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/version_log/templates/version_log/version_logs_dialog_page.html` & `django-versionlog-1.8.1/version_log/templates/version_log/version_logs_dialog_page.html`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/version_log/config.py` & `django-versionlog-1.8.1/version_log/config.py`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/version_log/middleware.py` & `django-versionlog-1.8.1/version_log/middleware.py`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/docs/img/icons/django-versionlog.png` & `django-versionlog-1.8.1/docs/img/icons/django-versionlog.png`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/docs/img/icons/qr_code.png` & `django-versionlog-1.8.1/docs/img/icons/qr_code.png`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/docs/img/demos/gitbook-page.png` & `django-versionlog-1.8.1/docs/img/demos/gitbook-page.png`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/docs/img/demos/dialog.png` & `django-versionlog-1.8.1/docs/img/demos/dialog.png`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/docs/img/demos/dialog-page.png` & `django-versionlog-1.8.1/docs/img/demos/dialog-page.png`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/docs/contributing.md` & `django-versionlog-1.8.1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/docs/structure.md` & `django-versionlog-1.8.1/docs/structure.md`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/docs/feature.md` & `django-versionlog-1.8.1/docs/feature.md`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/docs/usage.md` & `django-versionlog-1.8.1/docs/usage.md`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/django_versionlog.egg-info/PKG-INFO` & `django-versionlog-1.8.1/django_versionlog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-versionlog
-Version: 1.8.0
+Version: 1.8.1
 Summary: version log module
 Home-page: https://github.com/TencentBlueKing/django-versionlog
 Author: blueking
 Author-email: blueking@tencent.com
 License: UNKNOWN
 Description: # django-versionlog
```

### Comparing `django-versionlog-1.8.0/django_versionlog.egg-info/SOURCES.txt` & `django-versionlog-1.8.1/django_versionlog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/LICENSE` & `django-versionlog-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.8.0/README.md` & `django-versionlog-1.8.1/README.md`

 * *Files identical despite different names*

