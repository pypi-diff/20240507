# Comparing `tmp/punkweb_bb-0.1.2.tar.gz` & `tmp/punkweb_bb-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "punkweb_bb-0.1.2.tar", last modified: Tue Apr  9 07:09:59 2024, max compression
+gzip compressed data, was "punkweb_bb-0.1.3.tar", last modified: Tue May  7 06:28:58 2024, max compression
```

## Comparing `punkweb_bb-0.1.2.tar` & `punkweb_bb-0.1.3.tar`

### file list

```diff
@@ -1,255 +1,261 @@
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.819102 punkweb_bb-0.1.2/
--rw-r--r--   0 pork      (1000) pork      (1000)     1507 2024-04-09 06:08:41.000000 punkweb_bb-0.1.2/LICENSE
--rw-r--r--   0 pork      (1000) pork      (1000)       64 2024-04-09 05:47:19.000000 punkweb_bb-0.1.2/MANIFEST.in
--rw-r--r--   0 pork      (1000) pork      (1000)     1710 2024-04-09 07:09:59.819102 punkweb_bb-0.1.2/PKG-INFO
--rw-r--r--   0 pork      (1000) pork      (1000)     1056 2024-04-08 22:22:55.000000 punkweb_bb-0.1.2/README.md
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.811102 punkweb_bb-0.1.2/punkweb_bb/
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.1.2/punkweb_bb/__init__.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.811102 punkweb_bb-0.1.2/punkweb_bb/__pycache__/
--rw-r--r--   0 pork      (1000) pork      (1000)      161 2024-04-09 05:48:25.000000 punkweb_bb-0.1.2/punkweb_bb/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     3679 2024-04-09 05:48:25.000000 punkweb_bb-0.1.2/punkweb_bb/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     2980 2024-04-09 05:48:25.000000 punkweb_bb-0.1.2/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      730 2024-04-09 06:55:15.000000 punkweb_bb-0.1.2/punkweb_bb/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     8534 2024-04-09 06:32:38.000000 punkweb_bb-0.1.2/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      392 2024-04-09 06:44:27.000000 punkweb_bb-0.1.2/punkweb_bb/__pycache__/context_processors.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     4680 2024-04-09 05:48:25.000000 punkweb_bb-0.1.2/punkweb_bb/__pycache__/forms.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1249 2024-04-09 05:48:25.000000 punkweb_bb-0.1.2/punkweb_bb/__pycache__/middleware.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1478 2024-04-09 05:48:25.000000 punkweb_bb-0.1.2/punkweb_bb/__pycache__/mixins.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)    12034 2024-04-09 05:48:25.000000 punkweb_bb-0.1.2/punkweb_bb/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      990 2024-04-09 05:48:25.000000 punkweb_bb-0.1.2/punkweb_bb/__pycache__/pagination.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     5335 2024-04-09 07:07:59.000000 punkweb_bb-0.1.2/punkweb_bb/__pycache__/parsers.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-09 05:48:25.000000 punkweb_bb-0.1.2/punkweb_bb/__pycache__/response.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      563 2024-04-09 06:44:27.000000 punkweb_bb-0.1.2/punkweb_bb/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      864 2024-04-09 05:48:25.000000 punkweb_bb-0.1.2/punkweb_bb/__pycache__/signals.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     2304 2024-04-09 05:48:25.000000 punkweb_bb-0.1.2/punkweb_bb/__pycache__/urls.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)    15313 2024-04-09 05:48:25.000000 punkweb_bb-0.1.2/punkweb_bb/__pycache__/views.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1552 2024-04-09 05:48:25.000000 punkweb_bb-0.1.2/punkweb_bb/__pycache__/widgets.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     2493 2024-04-05 21:20:18.000000 punkweb_bb-0.1.2/punkweb_bb/admin.py
--rw-r--r--   0 pork      (1000) pork      (1000)     1128 2024-04-03 19:18:44.000000 punkweb_bb-0.1.2/punkweb_bb/admin_forms.py
--rw-r--r--   0 pork      (1000) pork      (1000)      207 2024-04-09 06:52:38.000000 punkweb_bb-0.1.2/punkweb_bb/apps.py
--rw-r--r--   0 pork      (1000) pork      (1000)     4419 2024-04-09 06:31:31.000000 punkweb_bb-0.1.2/punkweb_bb/bbcode_tags.py
--rw-r--r--   0 pork      (1000) pork      (1000)      146 2024-04-09 04:54:41.000000 punkweb_bb-0.1.2/punkweb_bb/context_processors.py
--rw-r--r--   0 pork      (1000) pork      (1000)     1977 2024-04-03 19:20:08.000000 punkweb_bb-0.1.2/punkweb_bb/forms.py
--rw-r--r--   0 pork      (1000) pork      (1000)      456 2024-04-05 21:11:30.000000 punkweb_bb-0.1.2/punkweb_bb/middleware.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.811102 punkweb_bb-0.1.2/punkweb_bb/migrations/
--rw-r--r--   0 pork      (1000) pork      (1000)     8950 2024-04-09 07:09:02.000000 punkweb_bb-0.1.2/punkweb_bb/migrations/0001_initial.py
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.1.2/punkweb_bb/migrations/__init__.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.811102 punkweb_bb-0.1.2/punkweb_bb/migrations/__pycache__/
--rw-r--r--   0 pork      (1000) pork      (1000)     6456 2024-04-09 07:09:10.000000 punkweb_bb-0.1.2/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      172 2024-04-09 05:48:25.000000 punkweb_bb-0.1.2/punkweb_bb/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-03 19:16:01.000000 punkweb_bb-0.1.2/punkweb_bb/mixins.py
--rw-r--r--   0 pork      (1000) pork      (1000)     5314 2024-04-08 21:59:09.000000 punkweb_bb-0.1.2/punkweb_bb/models.py
--rw-r--r--   0 pork      (1000) pork      (1000)      409 2024-04-06 08:06:22.000000 punkweb_bb-0.1.2/punkweb_bb/pagination.py
--rw-r--r--   0 pork      (1000) pork      (1000)     2732 2024-04-09 07:07:58.000000 punkweb_bb-0.1.2/punkweb_bb/parsers.py
--rw-r--r--   0 pork      (1000) pork      (1000)      130 2024-04-03 19:15:29.000000 punkweb_bb-0.1.2/punkweb_bb/response.py
--rw-r--r--   0 pork      (1000) pork      (1000)      250 2024-04-09 04:49:49.000000 punkweb_bb-0.1.2/punkweb_bb/settings.py
--rw-r--r--   0 pork      (1000) pork      (1000)      365 2024-04-03 19:18:44.000000 punkweb_bb-0.1.2/punkweb_bb/signals.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.807102 punkweb_bb-0.1.2/punkweb_bb/static/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.811102 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.811102 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/css/
--rw-r--r--   0 pork      (1000) pork      (1000)     1455 2024-04-06 07:32:15.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/css/defaults.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1331 2024-04-06 07:48:47.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/css/index.css
--rw-r--r--   0 pork      (1000) pork      (1000)      234 2024-04-03 22:23:23.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/css/login.css
--rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-08 22:57:27.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/css/members.css
--rw-r--r--   0 pork      (1000) pork      (1000)      321 2024-04-03 21:47:53.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/css/post-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)      799 2024-04-08 23:19:07.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/css/profile.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1296 2024-04-05 22:11:56.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css
--rw-r--r--   0 pork      (1000) pork      (1000)    11284 2024-04-08 22:28:14.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/css/punkweb.css
--rw-r--r--   0 pork      (1000) pork      (1000)      308 2024-04-06 07:53:29.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/css/settings.css
--rw-r--r--   0 pork      (1000) pork      (1000)      333 2024-04-08 23:25:45.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/css/shoutbox.css
--rw-r--r--   0 pork      (1000) pork      (1000)      536 2024-04-06 07:48:52.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/css/subcategory.css
--rw-r--r--   0 pork      (1000) pork      (1000)      329 2024-04-03 19:20:08.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/css/thread-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1508 2024-04-06 07:53:50.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/css/thread.css
--rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-05 15:05:58.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/css/typography.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1154 2024-04-05 19:38:35.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/css/variables.css
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.811102 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/editor/
--rw-r--r--   0 pork      (1000) pork      (1000)     1466 2024-04-06 07:32:28.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1624 2024-04-03 19:20:08.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-04-03 19:20:08.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.css
--rw-r--r--   0 pork      (1000) pork      (1000)      606 2024-04-08 22:10:44.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js
--rw-r--r--   0 pork      (1000) pork      (1000)      318 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/favicon.ico
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.811102 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/img/
--rw-r--r--   0 pork      (1000) pork      (1000)    60475 2024-04-03 19:20:08.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/img/default-profile-image.png
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.811102 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/js/
--rw-r--r--   0 pork      (1000) pork      (1000)      179 2024-04-03 19:20:08.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/js/punkweb-modal.js
--rw-r--r--   0 pork      (1000) pork      (1000)      142 2024-04-08 20:20:47.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/js/shoutbox.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.811102 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/
--rw-r--r--   0 pork      (1000) pork      (1000)    44307 2024-04-03 19:17:23.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    87461 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    10331 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/open-color.css
--rw-r--r--   0 pork      (1000) pork      (1000)     3948 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/prism.css
--rw-r--r--   0 pork      (1000) pork      (1000)   576492 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/prism.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.811102 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/
--rw-r--r--   0 pork      (1000) pork      (1000)     4129 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.815102 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.815102 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/
--rw-r--r--   0 pork      (1000) pork      (1000)    61679 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js
--rw-r--r--   0 pork      (1000) pork      (1000)    26086 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.815102 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/
--rw-r--r--   0 pork      (1000) pork      (1000)    11260 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js
--rw-r--r--   0 pork      (1000) pork      (1000)    15873 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js
--rw-r--r--   0 pork      (1000) pork      (1000)   312959 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js
--rw-r--r--   0 pork      (1000) pork      (1000)   251279 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js
--rw-r--r--   0 pork      (1000) pork      (1000)   277366 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.815102 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/
--rw-r--r--   0 pork      (1000) pork      (1000)     3446 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2571 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2791 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js
--rw-r--r--   0 pork      (1000) pork      (1000)     6306 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2528 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2059 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js
--rw-r--r--   0 pork      (1000) pork      (1000)     9375 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2067 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js
--rw-r--r--   0 pork      (1000) pork      (1000)   249123 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.815102 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.815102 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/
--rw-r--r--   0 pork      (1000) pork      (1000)     1476 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css
--rw-r--r--   0 pork      (1000) pork      (1000)    11194 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css
--rw-r--r--   0 pork      (1000) pork      (1000)    11500 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css
--rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png
--rw-r--r--   0 pork      (1000) pork      (1000)    12943 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css
--rw-r--r--   0 pork      (1000) pork      (1000)    13431 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css
--rw-r--r--   0 pork      (1000) pork      (1000)    14124 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css
--rw-r--r--   0 pork      (1000) pork      (1000)    13183 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.815102 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/
--rw-r--r--   0 pork      (1000) pork      (1000)      756 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1182 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png
--rw-r--r--   0 pork      (1000) pork      (1000)      781 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png
--rw-r--r--   0 pork      (1000) pork      (1000)      972 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png
--rw-r--r--   0 pork      (1000) pork      (1000)      865 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png
--rw-r--r--   0 pork      (1000) pork      (1000)      753 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png
--rw-r--r--   0 pork      (1000) pork      (1000)      965 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png
--rw-r--r--   0 pork      (1000) pork      (1000)      421 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/credits.txt
--rw-r--r--   0 pork      (1000) pork      (1000)      877 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1012 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png
--rw-r--r--   0 pork      (1000) pork      (1000)      991 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png
--rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png
--rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png
--rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png
--rw-r--r--   0 pork      (1000) pork      (1000)      867 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png
--rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png
--rw-r--r--   0 pork      (1000) pork      (1000)      572 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png
--rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png
--rw-r--r--   0 pork      (1000) pork      (1000)      912 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png
--rw-r--r--   0 pork      (1000) pork      (1000)      694 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png
--rw-r--r--   0 pork      (1000) pork      (1000)      804 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png
--rw-r--r--   0 pork      (1000) pork      (1000)      799 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png
--rw-r--r--   0 pork      (1000) pork      (1000)      789 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png
--rw-r--r--   0 pork      (1000) pork      (1000)      780 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png
--rw-r--r--   0 pork      (1000) pork      (1000)      783 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png
--rw-r--r--   0 pork      (1000) pork      (1000)      788 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png
--rw-r--r--   0 pork      (1000) pork      (1000)      930 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1039 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png
--rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png
--rw-r--r--   0 pork      (1000) pork      (1000)      981 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png
--rw-r--r--   0 pork      (1000) pork      (1000)      763 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png
--rw-r--r--   0 pork      (1000) pork      (1000)      718 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png
--rw-r--r--   0 pork      (1000) pork      (1000)      810 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1072 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png
--rw-r--r--   0 pork      (1000) pork      (1000)      791 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png
--rw-r--r--   0 pork      (1000) pork      (1000)     2237 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.819102 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/
--rw-r--r--   0 pork      (1000) pork      (1000)     3235 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2803 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2543 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2879 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2504 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js
--rw-r--r--   0 pork      (1000) pork      (1000)     4020 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js
--rw-r--r--   0 pork      (1000) pork      (1000)      102 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en-US.js
--rw-r--r--   0 pork      (1000) pork      (1000)      250 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2831 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2018 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3577 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2813 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2906 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2802 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2956 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2718 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2981 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3259 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3141 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2797 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2903 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2745 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2739 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2810 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3192 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3017 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2210 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2122 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2772 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2557 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3102 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2913 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.819102 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.819102 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/
--rw-r--r--   0 pork      (1000) pork      (1000)    17567 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js
--rw-r--r--   0 pork      (1000) pork      (1000)     8873 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.819102 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/
--rw-r--r--   0 pork      (1000) pork      (1000)     9203 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js
--rw-r--r--   0 pork      (1000) pork      (1000)    14779 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js
--rw-r--r--   0 pork      (1000) pork      (1000)    91043 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    73632 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    82349 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.819102 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/
--rw-r--r--   0 pork      (1000) pork      (1000)     1417 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1259 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1107 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3667 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1088 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js
--rw-r--r--   0 pork      (1000) pork      (1000)      775 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2760 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js
--rw-r--r--   0 pork      (1000) pork      (1000)      934 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js
--rw-r--r--   0 pork      (1000) pork      (1000)    73296 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.819102 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.819102 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/
--rw-r--r--   0 pork      (1000) pork      (1000)     1016 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)     9307 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)     9570 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png
--rw-r--r--   0 pork      (1000) pork      (1000)    10656 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    12604 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    13148 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    10710 2024-04-03 19:11:51.000000 punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.807102 punkweb_bb-0.1.2/punkweb_bb/templates/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.819102 punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/
--rw-r--r--   0 pork      (1000) pork      (1000)     4034 2024-04-09 04:59:49.000000 punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/base.html
--rw-r--r--   0 pork      (1000) pork      (1000)      460 2024-04-05 19:59:05.000000 punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/base_modal.html
--rw-r--r--   0 pork      (1000) pork      (1000)      396 2024-04-06 07:23:56.000000 punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/bbcode.html
--rw-r--r--   0 pork      (1000) pork      (1000)     8127 2024-04-09 06:45:08.000000 punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/index.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1087 2024-04-06 02:06:29.000000 punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/login.html
--rw-r--r--   0 pork      (1000) pork      (1000)     2729 2024-04-08 23:13:19.000000 punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/members.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.819102 punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/partials/
--rw-r--r--   0 pork      (1000) pork      (1000)      417 2024-04-06 02:06:29.000000 punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/partials/post_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)      565 2024-04-06 02:06:29.000000 punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/partials/post_update.html
--rw-r--r--   0 pork      (1000) pork      (1000)      425 2024-04-06 02:06:29.000000 punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/partials/thread_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)     2948 2024-04-08 23:26:38.000000 punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/profile.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1994 2024-04-07 22:46:43.000000 punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/settings.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.819102 punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/shoutbox/
--rw-r--r--   0 pork      (1000) pork      (1000)      312 2024-04-08 23:26:13.000000 punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html
--rw-r--r--   0 pork      (1000) pork      (1000)      672 2024-04-08 23:49:26.000000 punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1167 2024-04-06 02:06:29.000000 punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/signup.html
--rw-r--r--   0 pork      (1000) pork      (1000)     4682 2024-04-07 22:32:48.000000 punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/subcategory.html
--rw-r--r--   0 pork      (1000) pork      (1000)     7457 2024-04-08 22:04:37.000000 punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/thread.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1399 2024-04-06 02:06:29.000000 punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/thread_create.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1578 2024-04-06 02:06:29.000000 punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/thread_update.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.819102 punkweb_bb-0.1.2/punkweb_bb/templatetags/
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-04-08 21:13:22.000000 punkweb_bb-0.1.2/punkweb_bb/templatetags/__init__.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.819102 punkweb_bb-0.1.2/punkweb_bb/templatetags/__pycache__/
--rw-r--r--   0 pork      (1000) pork      (1000)      174 2024-04-09 05:48:25.000000 punkweb_bb-0.1.2/punkweb_bb/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      833 2024-04-09 07:07:10.000000 punkweb_bb-0.1.2/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      310 2024-04-09 07:07:08.000000 punkweb_bb-0.1.2/punkweb_bb/templatetags/shoutbox_bbcode.py
--rw-r--r--   0 pork      (1000) pork      (1000)     8257 2024-04-03 19:18:44.000000 punkweb_bb-0.1.2/punkweb_bb/tests.py
--rw-r--r--   0 pork      (1000) pork      (1000)     1538 2024-04-08 22:43:34.000000 punkweb_bb-0.1.2/punkweb_bb/urls.py
--rw-r--r--   0 pork      (1000) pork      (1000)    10435 2024-04-08 23:46:58.000000 punkweb_bb-0.1.2/punkweb_bb/views.py
--rw-r--r--   0 pork      (1000) pork      (1000)      840 2024-04-03 19:20:08.000000 punkweb_bb-0.1.2/punkweb_bb/widgets.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-04-09 07:09:59.811102 punkweb_bb-0.1.2/punkweb_bb.egg-info/
--rw-r--r--   0 pork      (1000) pork      (1000)     1710 2024-04-09 07:09:59.000000 punkweb_bb-0.1.2/punkweb_bb.egg-info/PKG-INFO
--rw-r--r--   0 pork      (1000) pork      (1000)    13008 2024-04-09 07:09:59.000000 punkweb_bb-0.1.2/punkweb_bb.egg-info/SOURCES.txt
--rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-04-09 07:09:59.000000 punkweb_bb-0.1.2/punkweb_bb.egg-info/dependency_links.txt
--rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-04-09 07:09:59.000000 punkweb_bb-0.1.2/punkweb_bb.egg-info/not-zip-safe
--rw-r--r--   0 pork      (1000) pork      (1000)       41 2024-04-09 07:09:59.000000 punkweb_bb-0.1.2/punkweb_bb.egg-info/requires.txt
--rw-r--r--   0 pork      (1000) pork      (1000)       11 2024-04-09 07:09:59.000000 punkweb_bb-0.1.2/punkweb_bb.egg-info/top_level.txt
--rw-r--r--   0 pork      (1000) pork      (1000)       38 2024-04-09 07:09:59.819102 punkweb_bb-0.1.2/setup.cfg
--rw-r--r--   0 pork      (1000) pork      (1000)      986 2024-04-09 07:09:15.000000 punkweb_bb-0.1.2/setup.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.333790 punkweb_bb-0.1.3/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1507 2024-04-09 06:08:41.000000 punkweb_bb-0.1.3/LICENSE
+-rw-r--r--   0 pork      (1000) pork      (1000)       64 2024-04-09 05:47:19.000000 punkweb_bb-0.1.3/MANIFEST.in
+-rw-r--r--   0 pork      (1000) pork      (1000)     4843 2024-05-07 06:28:58.333790 punkweb_bb-0.1.3/PKG-INFO
+-rw-r--r--   0 pork      (1000) pork      (1000)     4189 2024-05-07 06:14:42.000000 punkweb_bb-0.1.3/README.md
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.321790 punkweb_bb-0.1.3/punkweb_bb/
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.1.3/punkweb_bb/__init__.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.321790 punkweb_bb-0.1.3/punkweb_bb/__pycache__/
+-rw-r--r--   0 pork      (1000) pork      (1000)      161 2024-04-09 05:48:25.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     3679 2024-04-09 05:48:25.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2980 2024-04-09 05:48:25.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      730 2024-04-09 06:55:15.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     8534 2024-04-09 06:32:38.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      392 2024-04-09 06:44:27.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/context_processors.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     4680 2024-04-09 05:48:25.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/forms.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1249 2024-04-09 05:48:25.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/middleware.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1478 2024-04-09 05:48:25.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/mixins.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)    12308 2024-05-07 05:16:02.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      990 2024-04-09 05:48:25.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/pagination.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     5335 2024-04-09 07:07:59.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/parsers.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-09 05:48:25.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/response.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      665 2024-05-07 02:14:22.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      864 2024-04-09 05:48:25.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/signals.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)    50877 2024-05-07 06:13:11.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/tests.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2304 2024-04-09 05:48:25.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/urls.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)    15592 2024-05-07 06:13:06.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/views.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1552 2024-04-09 05:48:25.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/widgets.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2493 2024-04-05 21:20:18.000000 punkweb_bb-0.1.3/punkweb_bb/admin.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1128 2024-04-03 19:18:44.000000 punkweb_bb-0.1.3/punkweb_bb/admin_forms.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      207 2024-04-09 06:52:38.000000 punkweb_bb-0.1.3/punkweb_bb/apps.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     4419 2024-04-09 06:31:31.000000 punkweb_bb-0.1.3/punkweb_bb/bbcode_tags.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      146 2024-04-09 04:54:41.000000 punkweb_bb-0.1.3/punkweb_bb/context_processors.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1977 2024-04-03 19:20:08.000000 punkweb_bb-0.1.3/punkweb_bb/forms.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      456 2024-04-05 21:11:30.000000 punkweb_bb-0.1.3/punkweb_bb/middleware.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.321790 punkweb_bb-0.1.3/punkweb_bb/migrations/
+-rw-r--r--   0 pork      (1000) pork      (1000)     8950 2024-04-09 07:09:02.000000 punkweb_bb-0.1.3/punkweb_bb/migrations/0001_initial.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      388 2024-05-07 04:24:13.000000 punkweb_bb-0.1.3/punkweb_bb/migrations/0002_thread_view_count.py
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.1.3/punkweb_bb/migrations/__init__.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.321790 punkweb_bb-0.1.3/punkweb_bb/migrations/__pycache__/
+-rw-r--r--   0 pork      (1000) pork      (1000)     6456 2024-04-09 07:09:10.000000 punkweb_bb-0.1.3/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      815 2024-05-07 04:24:16.000000 punkweb_bb-0.1.3/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      172 2024-04-09 05:48:25.000000 punkweb_bb-0.1.3/punkweb_bb/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-03 19:16:01.000000 punkweb_bb-0.1.3/punkweb_bb/mixins.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     5519 2024-05-07 05:16:01.000000 punkweb_bb-0.1.3/punkweb_bb/models.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      409 2024-04-06 08:06:22.000000 punkweb_bb-0.1.3/punkweb_bb/pagination.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     2732 2024-04-09 07:07:58.000000 punkweb_bb-0.1.3/punkweb_bb/parsers.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      130 2024-04-03 19:15:29.000000 punkweb_bb-0.1.3/punkweb_bb/response.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      312 2024-05-07 02:14:21.000000 punkweb_bb-0.1.3/punkweb_bb/settings.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      365 2024-04-03 19:18:44.000000 punkweb_bb-0.1.3/punkweb_bb/signals.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.317790 punkweb_bb-0.1.3/punkweb_bb/static/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.321790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.321790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1455 2024-04-06 07:32:15.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/defaults.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1331 2024-04-06 07:48:47.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/index.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      234 2024-04-03 22:23:23.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/login.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-08 22:57:27.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/members.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      321 2024-04-03 21:47:53.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/post-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      916 2024-05-07 01:46:57.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/profile.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1296 2024-04-05 22:11:56.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    11284 2024-04-08 22:28:14.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/punkweb.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      308 2024-04-06 07:53:29.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/settings.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      333 2024-04-08 23:25:45.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/shoutbox.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      536 2024-04-06 07:48:52.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/subcategory.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      329 2024-04-03 19:20:08.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/thread-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1508 2024-04-06 07:53:50.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/thread.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-05 15:05:58.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/typography.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1154 2024-04-05 19:38:35.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/variables.css
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.321790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/editor/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1466 2024-04-06 07:32:28.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1624 2024-04-03 19:20:08.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-04-03 19:20:08.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      606 2024-04-08 22:10:44.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      318 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/favicon.ico
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.325790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/img/
+-rw-r--r--   0 pork      (1000) pork      (1000)    60475 2024-04-03 19:20:08.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/img/default-profile-image.png
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.325790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/js/
+-rw-r--r--   0 pork      (1000) pork      (1000)      179 2024-04-03 19:20:08.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/js/punkweb-modal.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      142 2024-04-08 20:20:47.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/js/shoutbox.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.325790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/
+-rw-r--r--   0 pork      (1000) pork      (1000)    44307 2024-04-03 19:17:23.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    87461 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    10331 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/open-color.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     3948 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/prism.css
+-rw-r--r--   0 pork      (1000) pork      (1000)   576492 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/prism.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.325790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/
+-rw-r--r--   0 pork      (1000) pork      (1000)     4129 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.325790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.325790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/
+-rw-r--r--   0 pork      (1000) pork      (1000)    61679 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    26086 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.325790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/
+-rw-r--r--   0 pork      (1000) pork      (1000)    11260 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    15873 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   312959 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   251279 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   277366 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.325790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/
+-rw-r--r--   0 pork      (1000) pork      (1000)     3446 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2571 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2791 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     6306 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2528 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2059 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     9375 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2067 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   249123 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.325790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.325790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1476 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    11194 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    11500 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png
+-rw-r--r--   0 pork      (1000) pork      (1000)    12943 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    13431 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    14124 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    13183 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.329790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/
+-rw-r--r--   0 pork      (1000) pork      (1000)      756 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1182 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      781 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      972 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      865 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      753 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      965 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      421 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/credits.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)      877 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1012 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      991 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      867 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      572 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      912 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      694 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      804 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      799 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      789 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      780 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      783 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      788 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      930 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1039 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      981 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      763 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      718 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      810 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1072 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      791 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     2237 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.329790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/
+-rw-r--r--   0 pork      (1000) pork      (1000)     3235 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2803 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2543 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2879 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2504 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     4020 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      102 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en-US.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      250 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2831 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2018 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3577 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2813 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2906 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2802 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2956 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2718 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2981 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3259 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3141 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2797 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2903 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2745 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2739 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2810 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3192 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3017 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2210 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2122 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2772 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2557 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3102 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2913 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.329790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.329790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/
+-rw-r--r--   0 pork      (1000) pork      (1000)    17567 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     8873 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.329790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/
+-rw-r--r--   0 pork      (1000) pork      (1000)     9203 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    14779 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    91043 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    73632 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    82349 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.329790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1417 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1259 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1107 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3667 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1088 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      775 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2760 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      934 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    73296 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.329790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.329790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1016 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     9307 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     9570 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png
+-rw-r--r--   0 pork      (1000) pork      (1000)    10656 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    12604 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    13148 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    10710 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.317790 punkweb_bb-0.1.3/punkweb_bb/templates/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.333790 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/
+-rw-r--r--   0 pork      (1000) pork      (1000)     4037 2024-05-07 02:13:59.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/base.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      460 2024-04-05 19:59:05.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/base_modal.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      396 2024-04-06 07:23:56.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/bbcode.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     8127 2024-04-09 06:45:08.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/index.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1087 2024-04-06 02:06:29.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/login.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     2729 2024-04-08 23:13:19.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/members.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.333790 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/partials/
+-rw-r--r--   0 pork      (1000) pork      (1000)      417 2024-04-06 02:06:29.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/partials/post_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      565 2024-04-06 02:06:29.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/partials/post_update.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      425 2024-04-06 02:06:29.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/partials/thread_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     2948 2024-04-08 23:26:38.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/profile.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1994 2024-04-07 22:46:43.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/settings.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.333790 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/shoutbox/
+-rw-r--r--   0 pork      (1000) pork      (1000)      312 2024-04-08 23:26:13.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      672 2024-04-08 23:49:26.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1167 2024-04-06 02:06:29.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/signup.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     4950 2024-05-07 04:34:46.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/subcategory.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     7595 2024-05-07 04:36:10.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/thread.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1537 2024-05-07 04:34:23.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/thread_create.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1730 2024-05-07 04:35:30.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/thread_update.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.333790 punkweb_bb-0.1.3/punkweb_bb/templatetags/
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-05-07 04:31:09.000000 punkweb_bb-0.1.3/punkweb_bb/templatetags/__init__.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.333790 punkweb_bb-0.1.3/punkweb_bb/templatetags/__pycache__/
+-rw-r--r--   0 pork      (1000) pork      (1000)      174 2024-05-07 04:31:10.000000 punkweb_bb-0.1.3/punkweb_bb/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      621 2024-05-07 04:30:58.000000 punkweb_bb-0.1.3/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      619 2024-05-07 04:31:10.000000 punkweb_bb-0.1.3/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      833 2024-04-09 07:07:10.000000 punkweb_bb-0.1.3/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      248 2024-05-07 04:31:08.000000 punkweb_bb-0.1.3/punkweb_bb/templatetags/humanize_int.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      310 2024-04-09 07:07:08.000000 punkweb_bb-0.1.3/punkweb_bb/templatetags/shoutbox_bbcode.py
+-rw-r--r--   0 pork      (1000) pork      (1000)    25989 2024-05-07 06:12:50.000000 punkweb_bb-0.1.3/punkweb_bb/tests.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1538 2024-04-08 22:43:34.000000 punkweb_bb-0.1.3/punkweb_bb/urls.py
+-rw-r--r--   0 pork      (1000) pork      (1000)    10723 2024-05-07 06:13:06.000000 punkweb_bb-0.1.3/punkweb_bb/views.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      840 2024-04-03 19:20:08.000000 punkweb_bb-0.1.3/punkweb_bb/widgets.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.321790 punkweb_bb-0.1.3/punkweb_bb.egg-info/
+-rw-r--r--   0 pork      (1000) pork      (1000)     4843 2024-05-07 06:28:58.000000 punkweb_bb-0.1.3/punkweb_bb.egg-info/PKG-INFO
+-rw-r--r--   0 pork      (1000) pork      (1000)    13346 2024-05-07 06:28:58.000000 punkweb_bb-0.1.3/punkweb_bb.egg-info/SOURCES.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-05-07 06:28:58.000000 punkweb_bb-0.1.3/punkweb_bb.egg-info/dependency_links.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-04-09 07:09:59.000000 punkweb_bb-0.1.3/punkweb_bb.egg-info/not-zip-safe
+-rw-r--r--   0 pork      (1000) pork      (1000)       41 2024-05-07 06:28:58.000000 punkweb_bb-0.1.3/punkweb_bb.egg-info/requires.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)       11 2024-05-07 06:28:58.000000 punkweb_bb-0.1.3/punkweb_bb.egg-info/top_level.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)       38 2024-05-07 06:28:58.333790 punkweb_bb-0.1.3/setup.cfg
+-rw-r--r--   0 pork      (1000) pork      (1000)      986 2024-05-07 06:28:57.000000 punkweb_bb-0.1.3/setup.py
```

### Comparing `punkweb_bb-0.1.2/LICENSE` & `punkweb_bb-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/__pycache__/admin.cpython-311.pyc` & `punkweb_bb-0.1.3/punkweb_bb/__pycache__/admin.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc` & `punkweb_bb-0.1.3/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/__pycache__/apps.cpython-311.pyc` & `punkweb_bb-0.1.3/punkweb_bb/__pycache__/apps.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc` & `punkweb_bb-0.1.3/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/__pycache__/forms.cpython-311.pyc` & `punkweb_bb-0.1.3/punkweb_bb/__pycache__/forms.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/__pycache__/middleware.cpython-311.pyc` & `punkweb_bb-0.1.3/punkweb_bb/__pycache__/middleware.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/__pycache__/mixins.cpython-311.pyc` & `punkweb_bb-0.1.3/punkweb_bb/__pycache__/mixins.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/__pycache__/models.cpython-311.pyc` & `punkweb_bb-0.1.3/punkweb_bb/__pycache__/models.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,27 +1,28 @@
 magic:    0xa70d0d0a
-moddate:  0xad681466 (Mon Apr  8 21:59:09 2024 UTC)
-files sz: 5314
+moddate:  0x11b93966 (Tue May  7 05:16:01 2024 UTC)
+files sz: 5519
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
       026c036d045a040100640064036c056d065a060100640064046c076d085a
       080100640064056c096d0a5a0a0100640064066c0b6d0c5a0c0100640064
-      076c0d6d0e5a0e0100640064086c0f6d105a106d115a11010002006504a6
-      000000ab0000000000000000005a12640984005a1302004700640a840064
-      0b65116510a6040000ab0400000000000000005a1402004700640c840064
-      0d65116510a6040000ab0400000000000000005a1502004700640e840064
-      0f65116510a6040000ab0400000000000000005a16020047006410840064
-      1165116510a6040000ab0400000000000000005a17020047006412840064
-      1365116510a6040000ab0400000000000000005a18020047006414840064
-      1565116510a6040000ab0400000000000000005a1964015300
+      076c0d6d0e5a0e0100640064086c0f6d105a100100640064096c116d125a
+      126d135a13010002006504a6000000ab0000000000000000005a14640a84
+      005a1502004700640b8400640c65136512a6040000ab0400000000000000
+      005a1602004700640d8400640e65136512a6040000ab0400000000000000
+      005a1702004700640f8400641065136512a6040000ab0400000000000000
+      005a180200470064118400641265136512a6040000ab0400000000000000
+      005a190200470064138400641465136512a6040000ab0400000000000000
+      005a1a0200470064158400641665136512a6040000ab0400000000000000
+      005a1b64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (datetime)
                  8 STORE_NAME               0 (datetime)
    
@@ -53,153 +54,161 @@
                 52 LOAD_CONST               4 (('models',))
                 54 IMPORT_NAME              7 (django.db)
                 56 IMPORT_FROM              8 (models)
                 58 STORE_NAME               8 (models)
                 60 POP_TOP
    
      8          62 LOAD_CONST               0 (0)
-                64 LOAD_CONST               5 (('reverse',))
-                66 IMPORT_NAME              9 (django.urls)
-                68 IMPORT_FROM             10 (reverse)
-                70 STORE_NAME              10 (reverse)
+                64 LOAD_CONST               5 (('ValidationError',))
+                66 IMPORT_NAME              9 (django.forms)
+                68 IMPORT_FROM             10 (ValidationError)
+                70 STORE_NAME              10 (ValidationError)
                 72 POP_TOP
    
      9          74 LOAD_CONST               0 (0)
-                76 LOAD_CONST               6 (('timezone',))
-                78 IMPORT_NAME             11 (django.utils)
-                80 IMPORT_FROM             12 (timezone)
-                82 STORE_NAME              12 (timezone)
+                76 LOAD_CONST               6 (('reverse',))
+                78 IMPORT_NAME             11 (django.urls)
+                80 IMPORT_FROM             12 (reverse)
+                82 STORE_NAME              12 (reverse)
                 84 POP_TOP
    
     10          86 LOAD_CONST               0 (0)
-                88 LOAD_CONST               7 (('BBCodeTextField',))
-                90 IMPORT_NAME             13 (precise_bbcode.fields)
-                92 IMPORT_FROM             14 (BBCodeTextField)
-                94 STORE_NAME              14 (BBCodeTextField)
+                88 LOAD_CONST               7 (('timezone',))
+                90 IMPORT_NAME             13 (django.utils)
+                92 IMPORT_FROM             14 (timezone)
+                94 STORE_NAME              14 (timezone)
                 96 POP_TOP
    
-    12          98 LOAD_CONST               0 (0)
-               100 LOAD_CONST               8 (('TimestampMixin', 'UUIDPrimaryKeyMixin'))
-               102 IMPORT_NAME             15 (punkweb_bb.mixins)
-               104 IMPORT_FROM             16 (TimestampMixin)
-               106 STORE_NAME              16 (TimestampMixin)
-               108 IMPORT_FROM             17 (UUIDPrimaryKeyMixin)
-               110 STORE_NAME              17 (UUIDPrimaryKeyMixin)
-               112 POP_TOP
+    11          98 LOAD_CONST               0 (0)
+               100 LOAD_CONST               8 (('BBCodeTextField',))
+               102 IMPORT_NAME             15 (precise_bbcode.fields)
+               104 IMPORT_FROM             16 (BBCodeTextField)
+               106 STORE_NAME              16 (BBCodeTextField)
+               108 POP_TOP
    
-    14         114 PUSH_NULL
-               116 LOAD_NAME                4 (get_user_model)
-               118 PRECALL                  0
-               122 CALL                     0
-               132 STORE_NAME              18 (User)
+    13         110 LOAD_CONST               0 (0)
+               112 LOAD_CONST               9 (('TimestampMixin', 'UUIDPrimaryKeyMixin'))
+               114 IMPORT_NAME             17 (punkweb_bb.mixins)
+               116 IMPORT_FROM             18 (TimestampMixin)
+               118 STORE_NAME              18 (TimestampMixin)
+               120 IMPORT_FROM             19 (UUIDPrimaryKeyMixin)
+               122 STORE_NAME              19 (UUIDPrimaryKeyMixin)
+               124 POP_TOP
    
-    17         134 LOAD_CONST               9 (<code object profile_image_upload_to, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 17>)
-               136 MAKE_FUNCTION            0
-               138 STORE_NAME              19 (profile_image_upload_to)
+    15         126 PUSH_NULL
+               128 LOAD_NAME                4 (get_user_model)
+               130 PRECALL                  0
+               134 CALL                     0
+               144 STORE_NAME              20 (User)
    
-    22         140 PUSH_NULL
-               142 LOAD_BUILD_CLASS
-               144 LOAD_CONST              10 (<code object BoardProfile, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 22>)
-               146 MAKE_FUNCTION            0
-               148 LOAD_CONST              11 ('BoardProfile')
-               150 LOAD_NAME               17 (UUIDPrimaryKeyMixin)
-               152 LOAD_NAME               16 (TimestampMixin)
-               154 PRECALL                  4
-               158 CALL                     4
-               168 STORE_NAME              20 (BoardProfile)
+    18         146 LOAD_CONST              10 (<code object profile_image_upload_to, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 18>)
+               148 MAKE_FUNCTION            0
+               150 STORE_NAME              21 (profile_image_upload_to)
    
-    45         170 PUSH_NULL
-               172 LOAD_BUILD_CLASS
-               174 LOAD_CONST              12 (<code object Category, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 45>)
-               176 MAKE_FUNCTION            0
-               178 LOAD_CONST              13 ('Category')
-               180 LOAD_NAME               17 (UUIDPrimaryKeyMixin)
-               182 LOAD_NAME               16 (TimestampMixin)
-               184 PRECALL                  4
-               188 CALL                     4
-               198 STORE_NAME              21 (Category)
+    23         152 PUSH_NULL
+               154 LOAD_BUILD_CLASS
+               156 LOAD_CONST              11 (<code object BoardProfile, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 23>)
+               158 MAKE_FUNCTION            0
+               160 LOAD_CONST              12 ('BoardProfile')
+               162 LOAD_NAME               19 (UUIDPrimaryKeyMixin)
+               164 LOAD_NAME               18 (TimestampMixin)
+               166 PRECALL                  4
+               170 CALL                     4
+               180 STORE_NAME              22 (BoardProfile)
    
-    63         200 PUSH_NULL
-               202 LOAD_BUILD_CLASS
-               204 LOAD_CONST              14 (<code object Subcategory, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 63>)
-               206 MAKE_FUNCTION            0
-               208 LOAD_CONST              15 ('Subcategory')
-               210 LOAD_NAME               17 (UUIDPrimaryKeyMixin)
-               212 LOAD_NAME               16 (TimestampMixin)
-               214 PRECALL                  4
-               218 CALL                     4
-               228 STORE_NAME              22 (Subcategory)
+    46         182 PUSH_NULL
+               184 LOAD_BUILD_CLASS
+               186 LOAD_CONST              13 (<code object Category, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 46>)
+               188 MAKE_FUNCTION            0
+               190 LOAD_CONST              14 ('Category')
+               192 LOAD_NAME               19 (UUIDPrimaryKeyMixin)
+               194 LOAD_NAME               18 (TimestampMixin)
+               196 PRECALL                  4
+               200 CALL                     4
+               210 STORE_NAME              23 (Category)
    
-   100         230 PUSH_NULL
-               232 LOAD_BUILD_CLASS
-               234 LOAD_CONST              16 (<code object Thread, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 100>)
-               236 MAKE_FUNCTION            0
-               238 LOAD_CONST              17 ('Thread')
-               240 LOAD_NAME               17 (UUIDPrimaryKeyMixin)
-               242 LOAD_NAME               16 (TimestampMixin)
-               244 PRECALL                  4
-               248 CALL                     4
-               258 STORE_NAME              23 (Thread)
+    64         212 PUSH_NULL
+               214 LOAD_BUILD_CLASS
+               216 LOAD_CONST              15 (<code object Subcategory, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 64>)
+               218 MAKE_FUNCTION            0
+               220 LOAD_CONST              16 ('Subcategory')
+               222 LOAD_NAME               19 (UUIDPrimaryKeyMixin)
+               224 LOAD_NAME               18 (TimestampMixin)
+               226 PRECALL                  4
+               230 CALL                     4
+               240 STORE_NAME              24 (Subcategory)
    
-   133         260 PUSH_NULL
-               262 LOAD_BUILD_CLASS
-               264 LOAD_CONST              18 (<code object Post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 133>)
-               266 MAKE_FUNCTION            0
-               268 LOAD_CONST              19 ('Post')
-               270 LOAD_NAME               17 (UUIDPrimaryKeyMixin)
-               272 LOAD_NAME               16 (TimestampMixin)
-               274 PRECALL                  4
-               278 CALL                     4
-               288 STORE_NAME              24 (Post)
+   101         242 PUSH_NULL
+               244 LOAD_BUILD_CLASS
+               246 LOAD_CONST              17 (<code object Thread, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 101>)
+               248 MAKE_FUNCTION            0
+               250 LOAD_CONST              18 ('Thread')
+               252 LOAD_NAME               19 (UUIDPrimaryKeyMixin)
+               254 LOAD_NAME               18 (TimestampMixin)
+               256 PRECALL                  4
+               260 CALL                     4
+               270 STORE_NAME              25 (Thread)
    
-   170         290 PUSH_NULL
-               292 LOAD_BUILD_CLASS
-               294 LOAD_CONST              20 (<code object Shout, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 170>)
-               296 MAKE_FUNCTION            0
-               298 LOAD_CONST              21 ('Shout')
-               300 LOAD_NAME               17 (UUIDPrimaryKeyMixin)
-               302 LOAD_NAME               16 (TimestampMixin)
-               304 PRECALL                  4
-               308 CALL                     4
-               318 STORE_NAME              25 (Shout)
-               320 LOAD_CONST               1 (None)
-               322 RETURN_VALUE
+   135         272 PUSH_NULL
+               274 LOAD_BUILD_CLASS
+               276 LOAD_CONST              19 (<code object Post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 135>)
+               278 MAKE_FUNCTION            0
+               280 LOAD_CONST              20 ('Post')
+               282 LOAD_NAME               19 (UUIDPrimaryKeyMixin)
+               284 LOAD_NAME               18 (TimestampMixin)
+               286 PRECALL                  4
+               290 CALL                     4
+               300 STORE_NAME              26 (Post)
+   
+   174         302 PUSH_NULL
+               304 LOAD_BUILD_CLASS
+               306 LOAD_CONST              21 (<code object Shout, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 174>)
+               308 MAKE_FUNCTION            0
+               310 LOAD_CONST              22 ('Shout')
+               312 LOAD_NAME               19 (UUIDPrimaryKeyMixin)
+               314 LOAD_NAME               18 (TimestampMixin)
+               316 PRECALL                  4
+               320 CALL                     4
+               330 STORE_NAME              27 (Shout)
+               332 LOAD_CONST               1 (None)
+               334 RETURN_VALUE
    consts
       0
       None
       ('get_user_model',)
       ('cache',)
       ('models',)
+      ('ValidationError',)
       ('reverse',)
       ('timezone',)
       ('BBCodeTextField',)
       ('TimestampMixin', 'UUIDPrimaryKeyMixin')
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 4
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000007c01a6010000ab010000000000
             0000006401190000000000000000007d0264027c006a0300000000000000
             006a0400000000000000009b0064037c029b009d045300
-          17           0 RESUME                   0
+          18           0 RESUME                   0
          
-          18           2 LOAD_GLOBAL              0 (os)
+          19           2 LOAD_GLOBAL              0 (os)
                       14 LOAD_ATTR                1 (path)
                       24 LOAD_METHOD              2 (splitext)
                       46 LOAD_FAST                1 (filename)
                       48 PRECALL                  1
                       52 CALL                     1
                       62 LOAD_CONST               1 (-1)
                       64 BINARY_SUBSCR
                       74 STORE_FAST               2 (ext)
          
-          19          76 LOAD_CONST               2 ('punkweb_bb/board_profiles/')
+          20          76 LOAD_CONST               2 ('punkweb_bb/board_profiles/')
                       78 LOAD_FAST                0 (instance)
                       80 LOAD_ATTR                3 (user)
                       90 LOAD_ATTR                4 (username)
                      100 FORMAT_VALUE             0
                      102 LOAD_CONST               3 ('/image')
                      104 LOAD_FAST                2 (ext)
                      106 FORMAT_VALUE             0
@@ -212,98 +221,98 @@
             '/image'
          names      ('os', 'path', 'splitext', 'user', 'username')
          varnames   ('instance', 'filename', 'ext')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'profile_image_upload_to'
-         firstlineno 17
+         firstlineno 18
          lnotab 0x02014a01
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a02020065036a0400000000000000006505640165
             036a060000000000000000ac02a6030000ab0300000000000000005a0702
             0065036a080000000000000000650964036403ac04a6030000ab03000000
             00000000005a0a0200650b640564036403ac06a6030000ab030000000000
             0000005a0c02004700640784006408a6020000ab0200000000000000005a
             0d650e64098400a6000000ab0000000000000000005a0f650e640a8400a6
             000000ab0000000000000000005a10640b84005a11640c5300
-          22           0 RESUME                   0
+          23           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('BoardProfile')
                        8 STORE_NAME               2 (__qualname__)
          
-          23          10 PUSH_NULL
+          24          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (OneToOneField)
                       24 LOAD_NAME                5 (User)
                       26 LOAD_CONST               1 ('profile')
                       28 LOAD_NAME                3 (models)
                       30 LOAD_ATTR                6 (CASCADE)
                       40 KW_NAMES                 2
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_NAME               7 (user)
          
-          24          58 PUSH_NULL
+          25          58 PUSH_NULL
                       60 LOAD_NAME                3 (models)
                       62 LOAD_ATTR                8 (ImageField)
                       72 LOAD_NAME                9 (profile_image_upload_to)
                       74 LOAD_CONST               3 (True)
                       76 LOAD_CONST               3 (True)
                       78 KW_NAMES                 4
                       80 PRECALL                  3
                       84 CALL                     3
                       94 STORE_NAME              10 (image)
          
-          25          96 PUSH_NULL
+          26          96 PUSH_NULL
                       98 LOAD_NAME               11 (BBCodeTextField)
                      100 LOAD_CONST               5 (1024)
                      102 LOAD_CONST               3 (True)
                      104 LOAD_CONST               3 (True)
                      106 KW_NAMES                 6
                      108 PRECALL                  3
                      112 CALL                     3
                      122 STORE_NAME              12 (signature)
          
-          27         124 PUSH_NULL
+          28         124 PUSH_NULL
                      126 LOAD_BUILD_CLASS
-                     128 LOAD_CONST               7 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 27>)
+                     128 LOAD_CONST               7 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 28>)
                      130 MAKE_FUNCTION            0
                      132 LOAD_CONST               8 ('Meta')
                      134 PRECALL                  2
                      138 CALL                     2
                      148 STORE_NAME              13 (Meta)
          
-          30         150 LOAD_NAME               14 (property)
+          31         150 LOAD_NAME               14 (property)
          
-          31         152 LOAD_CONST               9 (<code object is_online, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 30>)
+          32         152 LOAD_CONST               9 (<code object is_online, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 31>)
                      154 MAKE_FUNCTION            0
          
-          30         156 PRECALL                  0
+          31         156 PRECALL                  0
                      160 CALL                     0
          
-          31         170 STORE_NAME              15 (is_online)
+          32         170 STORE_NAME              15 (is_online)
          
-          37         172 LOAD_NAME               14 (property)
+          38         172 LOAD_NAME               14 (property)
          
-          38         174 LOAD_CONST              10 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 37>)
+          39         174 LOAD_CONST              10 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 38>)
                      176 MAKE_FUNCTION            0
          
-          37         178 PRECALL                  0
+          38         178 PRECALL                  0
                      182 CALL                     0
          
-          38         192 STORE_NAME              16 (post_count)
+          39         192 STORE_NAME              16 (post_count)
          
-          41         194 LOAD_CONST              11 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 41>)
+          42         194 LOAD_CONST              11 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 42>)
                      196 MAKE_FUNCTION            0
                      198 STORE_NAME              17 (__str__)
                      200 LOAD_CONST              12 (None)
                      202 RETURN_VALUE
          consts
             'BoardProfile'
             'profile'
@@ -314,110 +323,110 @@
             ('max_length', 'blank', 'null')
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025300
-                27           0 RESUME                   0
+                28           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('BoardProfile.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-                28          10 LOAD_CONST               1 (('user__username',))
+                29          10 LOAD_CONST               1 (('user__username',))
                             12 STORE_NAME               3 (ordering)
                             14 LOAD_CONST               2 (None)
                             16 RETURN_VALUE
                consts
                   'BoardProfile.Meta'
                   ('user__username',)
                   None
                names      ('__name__', '__module__', '__qualname__', 'ordering')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 27
+               firstlineno 28
                lnotab 0x0a01
             'Meta'
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x97007401000000000000000000006a01000000000000000064017c006a
                   0200000000000000009b009d02a6010000ab0100000000000000007d017c
                   01722d7407000000000000000000006a040000000000000000a6000000ab
                   0000000000000000007c01740b000000000000000000006a060000000000
                   0000006402ac03a6010000ab0100000000000000007a0000006b00000000
                   00530064045300
-                30           0 RESUME                   0
+                31           0 RESUME                   0
                
-                32           2 LOAD_GLOBAL              1 (NULL + cache)
+                33           2 LOAD_GLOBAL              1 (NULL + cache)
                             14 LOAD_ATTR                1 (get)
                             24 LOAD_CONST               1 ('profile_online_')
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (id)
                             38 FORMAT_VALUE             0
                             40 BUILD_STRING             2
                             42 PRECALL                  1
                             46 CALL                     1
                             56 STORE_FAST               1 (last_seen)
                
-                33          58 LOAD_FAST                1 (last_seen)
+                34          58 LOAD_FAST                1 (last_seen)
                             60 POP_JUMP_FORWARD_IF_FALSE    45 (to 152)
                
-                34          62 LOAD_GLOBAL              7 (NULL + timezone)
+                35          62 LOAD_GLOBAL              7 (NULL + timezone)
                             74 LOAD_ATTR                4 (now)
                             84 PRECALL                  0
                             88 CALL                     0
                             98 LOAD_FAST                1 (last_seen)
                            100 LOAD_GLOBAL             11 (NULL + datetime)
                            112 LOAD_ATTR                6 (timedelta)
                            122 LOAD_CONST               2 (5)
                            124 KW_NAMES                 3
                            126 PRECALL                  1
                            130 CALL                     1
                            140 BINARY_OP                0 (+)
                            144 COMPARE_OP               0 (<)
                            150 RETURN_VALUE
                
-                35     >>  152 LOAD_CONST               4 (False)
+                36     >>  152 LOAD_CONST               4 (False)
                            154 RETURN_VALUE
                consts
                   None
                   'profile_online_'
                   5
                   ('minutes',)
                   False
                names      ('cache', 'get', 'id', 'timezone', 'now', 'datetime', 'timedelta')
                varnames   ('self', 'last_seen')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'is_online'
-               firstlineno 30
+               firstlineno 31
                lnotab 0x0202380104015a01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000006a010000000000000000a002000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   007c006a0000000000000000006a030000000000000000a0020000000000
                   000000000000000000000000000000a6000000ab0000000000000000007a
                   0000005300
-                37           0 RESUME                   0
+                38           0 RESUME                   0
                
-                39           2 LOAD_FAST                0 (self)
+                40           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (user)
                             14 LOAD_ATTR                1 (threads)
                             24 LOAD_METHOD              2 (count)
                             46 PRECALL                  0
                             50 CALL                     0
                             60 LOAD_FAST                0 (self)
                             62 LOAD_ATTR                0 (user)
@@ -431,108 +440,108 @@
                   None
                names      ('user', 'threads', 'count', 'posts')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'post_count'
-               firstlineno 37
+               firstlineno 38
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000006a0100000000000000005300
-                41           0 RESUME                   0
+                42           0 RESUME                   0
                
-                42           2 LOAD_FAST                0 (self)
+                43           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (user)
                             14 LOAD_ATTR                1 (username)
                             24 RETURN_VALUE
                consts
                   None
                names      ('user', 'username')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 41
+               firstlineno 42
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'OneToOneField', 'User', 'CASCADE', 'user', 'ImageField', 'profile_image_upload_to', 'image', 'BBCodeTextField', 'signature', 'Meta', 'property', 'is_online', 'post_count', '__str__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'BoardProfile'
-         firstlineno 22
+         firstlineno 23
          lnotab 0x0a01300126011c021a03020104ff0e010206020104ff0e010203
       'BoardProfile'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a02020065036a0400000000000000006401ac02a6
             010000ab0100000000000000005a05020065036a06000000000000000064
             036404ac05a6020000ab0200000000000000005a07020065036a08000000
             00000000006406ac07a6010000ab0100000000000000005a090200470064
             0884006409a6020000ab0200000000000000005a0a640a84005a0b640b84
             005a0c640c5300
-          45           0 RESUME                   0
+          46           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Category')
                        8 STORE_NAME               2 (__qualname__)
          
-          46          10 PUSH_NULL
+          47          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (CharField)
                       24 LOAD_CONST               1 (255)
                       26 KW_NAMES                 2
                       28 PRECALL                  1
                       32 CALL                     1
                       42 STORE_NAME               5 (name)
          
-          47          44 PUSH_NULL
+          48          44 PUSH_NULL
                       46 LOAD_NAME                3 (models)
                       48 LOAD_ATTR                6 (SlugField)
                       58 LOAD_CONST               3 (1024)
                       60 LOAD_CONST               4 (True)
                       62 KW_NAMES                 5
                       64 PRECALL                  2
                       68 CALL                     2
                       78 STORE_NAME               7 (slug)
          
-          48          80 PUSH_NULL
+          49          80 PUSH_NULL
                       82 LOAD_NAME                3 (models)
                       84 LOAD_ATTR                8 (PositiveIntegerField)
                       94 LOAD_CONST               6 (0)
                       96 KW_NAMES                 7
                       98 PRECALL                  1
                      102 CALL                     1
                      112 STORE_NAME               9 (order)
          
-          50         114 PUSH_NULL
+          51         114 PUSH_NULL
                      116 LOAD_BUILD_CLASS
-                     118 LOAD_CONST               8 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 50>)
+                     118 LOAD_CONST               8 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 51>)
                      120 MAKE_FUNCTION            0
                      122 LOAD_CONST               9 ('Meta')
                      124 PRECALL                  2
                      128 CALL                     2
                      138 STORE_NAME              10 (Meta)
          
-          55         140 LOAD_CONST              10 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 55>)
+          56         140 LOAD_CONST              10 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 56>)
                      142 MAKE_FUNCTION            0
                      144 STORE_NAME              11 (__str__)
          
-          58         146 LOAD_CONST              11 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 58>)
+          59         146 LOAD_CONST              11 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 59>)
                      148 MAKE_FUNCTION            0
                      150 STORE_NAME              12 (get_absolute_url)
                      152 LOAD_CONST              12 (None)
                      154 RETURN_VALUE
          consts
             'Category'
             255
@@ -544,27 +553,27 @@
             ('default',)
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025a0464035a0564045300
-                50           0 RESUME                   0
+                51           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Category.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-                51          10 LOAD_CONST               1 ('category')
+                52          10 LOAD_CONST               1 ('category')
                             12 STORE_NAME               3 (verbose_name)
                
-                52          14 LOAD_CONST               2 ('categories')
+                53          14 LOAD_CONST               2 ('categories')
                             16 STORE_NAME               4 (verbose_name_plural)
                
-                53          18 LOAD_CONST               3 (('order',))
+                54          18 LOAD_CONST               3 (('order',))
                             20 STORE_NAME               5 (ordering)
                             22 LOAD_CONST               4 (None)
                             24 RETURN_VALUE
                consts
                   'Category.Meta'
                   'category'
                   'categories'
@@ -572,28 +581,28 @@
                   None
                names      ('__name__', '__module__', '__qualname__', 'verbose_name', 'verbose_name_plural', 'ordering')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 50
+               firstlineno 51
                lnotab 0x0a0104010401
             'Meta'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000009b0064017c006a0100000000000000
                   009b009d035300
-                55           0 RESUME                   0
+                56           0 RESUME                   0
                
-                56           2 LOAD_FAST                0 (self)
+                57           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (order)
                             14 FORMAT_VALUE             0
                             16 LOAD_CONST               1 ('. ')
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (name)
                             30 FORMAT_VALUE             0
                             32 BUILD_STRING             3
@@ -603,34 +612,34 @@
                   '. '
                names      ('order', 'name')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 55
+               firstlineno 56
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x97007401000000000000000000006401a6010000ab0100000000000000
                   007d017c019b0064027c006a0100000000000000009b0064037c006a0200
                   000000000000009b009d055300
-                58           0 RESUME                   0
+                59           0 RESUME                   0
                
-                59           2 LOAD_GLOBAL              1 (NULL + reverse)
+                60           2 LOAD_GLOBAL              1 (NULL + reverse)
                             14 LOAD_CONST               1 ('punkweb_bb:index')
                             16 PRECALL                  1
                             20 CALL                     1
                             30 STORE_FAST               1 (index_url)
                
-                60          32 LOAD_FAST                1 (index_url)
+                61          32 LOAD_FAST                1 (index_url)
                             34 FORMAT_VALUE             0
                             36 LOAD_CONST               2 ('#')
                             38 LOAD_FAST                0 (self)
                             40 LOAD_ATTR                1 (slug)
                             50 FORMAT_VALUE             0
                             52 LOAD_CONST               3 ('.')
                             54 LOAD_FAST                0 (self)
@@ -645,24 +654,24 @@
                   '.'
                names      ('reverse', 'slug', 'order')
                varnames   ('self', 'index_url')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'get_absolute_url'
-               firstlineno 58
+               firstlineno 59
                lnotab 0x02011e01
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'CharField', 'name', 'SlugField', 'slug', 'PositiveIntegerField', 'order', 'Meta', '__str__', 'get_absolute_url')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Category'
-         firstlineno 45
+         firstlineno 46
          lnotab 0x0a012201240122021a050603
       'Category'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
@@ -675,124 +684,124 @@
             0000005a0d020065036a0e00000000000000006409ac0aa6010000ab0100
             000000000000005a0f020065036a100000000000000000640bac0aa60100
             00ab0100000000000000005a1102004700640c8400640da6020000ab0200
             000000000000005a126513640e8400a6000000ab0000000000000000005a
             146513640f8400a6000000ab0000000000000000005a15651364108400a6
             000000ab0000000000000000005a16641184005a17641284005a18641353
             00
-          63           0 RESUME                   0
+          64           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Subcategory')
                        8 STORE_NAME               2 (__qualname__)
          
-          64          10 PUSH_NULL
+          65          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (ForeignKey)
          
-          65          24 LOAD_NAME                5 (Category)
+          66          24 LOAD_NAME                5 (Category)
                       26 LOAD_CONST               1 ('subcategories')
                       28 LOAD_NAME                3 (models)
                       30 LOAD_ATTR                6 (CASCADE)
          
-          64          40 KW_NAMES                 2
+          65          40 KW_NAMES                 2
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_NAME               7 (category)
          
-          67          58 PUSH_NULL
+          68          58 PUSH_NULL
                       60 LOAD_NAME                3 (models)
                       62 LOAD_ATTR                8 (CharField)
                       72 LOAD_CONST               3 (255)
                       74 KW_NAMES                 4
                       76 PRECALL                  1
                       80 CALL                     1
                       90 STORE_NAME               9 (name)
          
-          68          92 PUSH_NULL
+          69          92 PUSH_NULL
                       94 LOAD_NAME                3 (models)
                       96 LOAD_ATTR               10 (SlugField)
                      106 LOAD_CONST               5 (1024)
                      108 LOAD_CONST               6 (True)
                      110 KW_NAMES                 7
                      112 PRECALL                  2
                      116 CALL                     2
                      126 STORE_NAME              11 (slug)
          
-          69         128 PUSH_NULL
+          70         128 PUSH_NULL
                      130 LOAD_NAME               12 (BBCodeTextField)
                      132 LOAD_CONST               6 (True)
                      134 LOAD_CONST               6 (True)
                      136 KW_NAMES                 8
                      138 PRECALL                  2
                      142 CALL                     2
                      152 STORE_NAME              13 (description)
          
-          70         154 PUSH_NULL
+          71         154 PUSH_NULL
                      156 LOAD_NAME                3 (models)
                      158 LOAD_ATTR               14 (PositiveIntegerField)
                      168 LOAD_CONST               9 (0)
                      170 KW_NAMES                10
                      172 PRECALL                  1
                      176 CALL                     1
                      186 STORE_NAME              15 (order)
          
-          71         188 PUSH_NULL
+          72         188 PUSH_NULL
                      190 LOAD_NAME                3 (models)
                      192 LOAD_ATTR               16 (BooleanField)
                      202 LOAD_CONST              11 (False)
                      204 KW_NAMES                10
                      206 PRECALL                  1
                      210 CALL                     1
                      220 STORE_NAME              17 (staff_post_only)
          
-          73         222 PUSH_NULL
+          74         222 PUSH_NULL
                      224 LOAD_BUILD_CLASS
-                     226 LOAD_CONST              12 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 73>)
+                     226 LOAD_CONST              12 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 74>)
                      228 MAKE_FUNCTION            0
                      230 LOAD_CONST              13 ('Meta')
                      232 PRECALL                  2
                      236 CALL                     2
                      246 STORE_NAME              18 (Meta)
          
-          81         248 LOAD_NAME               19 (property)
+          82         248 LOAD_NAME               19 (property)
          
-          82         250 LOAD_CONST              14 (<code object thread_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 81>)
+          83         250 LOAD_CONST              14 (<code object thread_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 82>)
                      252 MAKE_FUNCTION            0
          
-          81         254 PRECALL                  0
+          82         254 PRECALL                  0
                      258 CALL                     0
          
-          82         268 STORE_NAME              20 (thread_count)
+          83         268 STORE_NAME              20 (thread_count)
          
-          85         270 LOAD_NAME               19 (property)
+          86         270 LOAD_NAME               19 (property)
          
-          86         272 LOAD_CONST              15 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 85>)
+          87         272 LOAD_CONST              15 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 86>)
                      274 MAKE_FUNCTION            0
          
-          85         276 PRECALL                  0
+          86         276 PRECALL                  0
                      280 CALL                     0
          
-          86         290 STORE_NAME              21 (post_count)
+          87         290 STORE_NAME              21 (post_count)
          
-          89         292 LOAD_NAME               19 (property)
+          90         292 LOAD_NAME               19 (property)
          
-          90         294 LOAD_CONST              16 (<code object latest_thread, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 89>)
+          91         294 LOAD_CONST              16 (<code object latest_thread, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 90>)
                      296 MAKE_FUNCTION            0
          
-          89         298 PRECALL                  0
+          90         298 PRECALL                  0
                      302 CALL                     0
          
-          90         312 STORE_NAME              22 (latest_thread)
+          91         312 STORE_NAME              22 (latest_thread)
          
-          93         314 LOAD_CONST              17 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 93>)
+          94         314 LOAD_CONST              17 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 94>)
                      316 MAKE_FUNCTION            0
                      318 STORE_NAME              23 (__str__)
          
-          96         320 LOAD_CONST              18 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 96>)
+          97         320 LOAD_CONST              18 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 97>)
                      322 MAKE_FUNCTION            0
                      324 STORE_NAME              24 (get_absolute_url)
                      326 LOAD_CONST              19 (None)
                      328 RETURN_VALUE
          consts
             'Subcategory'
             'subcategories'
@@ -808,27 +817,27 @@
             False
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025a0464035a0564045300
-                73           0 RESUME                   0
+                74           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Subcategory.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-                74          10 LOAD_CONST               1 ('subcategory')
+                75          10 LOAD_CONST               1 ('subcategory')
                             12 STORE_NAME               3 (verbose_name)
                
-                75          14 LOAD_CONST               2 ('subcategories')
+                76          14 LOAD_CONST               2 ('subcategories')
                             16 STORE_NAME               4 (verbose_name_plural)
                
-                76          18 LOAD_CONST               3 (('category__order', 'order'))
+                77          18 LOAD_CONST               3 (('category__order', 'order'))
                             20 STORE_NAME               5 (ordering)
                             22 LOAD_CONST               4 (None)
                             24 RETURN_VALUE
                consts
                   'Subcategory.Meta'
                   'subcategory'
                   'subcategories'
@@ -836,57 +845,57 @@
                   None
                names      ('__name__', '__module__', '__qualname__', 'verbose_name', 'verbose_name_plural', 'ordering')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 73
+               firstlineno 74
                lnotab 0x0a0104010401
             'Meta'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab0000000000000000005300
-                81           0 RESUME                   0
+                82           0 RESUME                   0
                
-                83           2 LOAD_FAST                0 (self)
+                84           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (threads)
                             14 LOAD_METHOD              1 (count)
                             36 PRECALL                  0
                             40 CALL                     0
                             50 RETURN_VALUE
                consts
                   None
                names      ('threads', 'count')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'thread_count'
-               firstlineno 81
+               firstlineno 82
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x9700740100000000000000000000640184007c006a0100000000000000
                   00a0020000000000000000000000000000000000000000a6000000ab0000
                   000000000000004400a6000000ab000000000000000000a6010000ab0100
                   000000000000005300
-                85           0 RESUME                   0
+                86           0 RESUME                   0
                
-                87           2 LOAD_GLOBAL              1 (NULL + sum)
-                            14 LOAD_CONST               1 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 87>)
+                88           2 LOAD_GLOBAL              1 (NULL + sum)
+                            14 LOAD_CONST               1 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 88>)
                             16 MAKE_FUNCTION            0
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (threads)
                             30 LOAD_METHOD              2 (all)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 GET_ITER
@@ -899,15 +908,15 @@
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d097d017c016a00000000000000000091028c0a5300
-                      87           0 RESUME                   0
+                      88           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 9 (to 26)
                                    8 STORE_FAST               1 (thread)
                                   10 LOAD_FAST                1 (thread)
                                   12 LOAD_ATTR                0 (post_count)
                                   22 LIST_APPEND              2
@@ -916,37 +925,37 @@
                      consts
                      names      ('post_count',)
                      varnames   ('.0', 'thread')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                      name       '<listcomp>'
-                     firstlineno 87
+                     firstlineno 88
                      lnotab 0x
                names      ('sum', 'threads', 'all')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'post_count'
-               firstlineno 85
+               firstlineno 86
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000a0020000000000
                   000000000000000000000000000000a6000000ab00000000000000000053
                   00
-                89           0 RESUME                   0
+                90           0 RESUME                   0
                
-                91           2 LOAD_FAST                0 (self)
+                92           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (threads)
                             14 LOAD_METHOD              1 (order_by)
                             36 LOAD_CONST               1 ('-last_post_created_at')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 LOAD_METHOD              2 (first)
                             74 PRECALL                  0
@@ -957,27 +966,27 @@
                   '-last_post_created_at'
                names      ('threads', 'order_by', 'first')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'latest_thread'
-               firstlineno 89
+               firstlineno 90
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007c006a0000000000000000009b0064017c006a0100000000000000
                   009b0064027c006a0200000000000000009b009d055300
-                93           0 RESUME                   0
+                94           0 RESUME                   0
                
-                94           2 LOAD_FAST                0 (self)
+                95           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (category)
                             14 FORMAT_VALUE             0
                             16 LOAD_CONST               1 (' > ')
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (order)
                             30 FORMAT_VALUE             0
                             32 LOAD_CONST               2 ('. ')
@@ -992,27 +1001,27 @@
                   '. '
                names      ('category', 'order', 'name')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 93
+               firstlineno 94
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x970074010000000000000000000064017c006a01000000000000000067
                   01ac02a6020000ab0200000000000000005300
-                96           0 RESUME                   0
+                97           0 RESUME                   0
                
-                97           2 LOAD_GLOBAL              1 (NULL + reverse)
+                98           2 LOAD_GLOBAL              1 (NULL + reverse)
                             14 LOAD_CONST               1 ('punkweb_bb:subcategory')
                             16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (slug)
                             28 BUILD_LIST               1
                             30 KW_NAMES                 2
                             32 PRECALL                  2
                             36 CALL                     2
@@ -1023,24 +1032,24 @@
                   ('args',)
                names      ('reverse', 'slug')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'get_absolute_url'
-               firstlineno 96
+               firstlineno 97
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'Category', 'CASCADE', 'category', 'CharField', 'name', 'SlugField', 'slug', 'BBCodeTextField', 'description', 'PositiveIntegerField', 'order', 'BooleanField', 'staff_post_only', 'Meta', 'property', 'thread_count', 'post_count', 'latest_thread', '__str__', 'get_absolute_url')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Subcategory'
-         firstlineno 63
+         firstlineno 64
          lnotab
             0x0a010e0110ff1203220124011a01220122021a08020104ff0e01020302
             0104ff0e010203020104ff0e0102030603
       'Subcategory'
       code
          argcount  : 0
          nlocals   : 0
@@ -1051,230 +1060,241 @@
             036a060000000000000000ac02a6030000ab0300000000000000005a0702
             0065036a0400000000000000006508640165036a060000000000000000ac
             02a6030000ab0300000000000000005a09020065036a0a00000000000000
             006403ac04a6010000ab0100000000000000005a0b0200650ca6000000ab
             0000000000000000005a0d020065036a0e00000000000000006405ac06a6
             010000ab0100000000000000005a0f020065036a0e000000000000000064
             05ac06a6010000ab0100000000000000005a10020065036a110000000000
-            0000006407ac08a6010000ab0100000000000000005a1202004700640984
-            00640aa6020000ab0200000000000000005a13640b84005a146515640c84
-            00a6000000ab0000000000000000005a166515640d8400a6000000ab0000
-            000000000000005a17640e84005a18640f5300
-         100           0 RESUME                   0
+            0000006407ac08a6010000ab0100000000000000005a12020065036a1300
+            000000000000006409ac06a6010000ab0100000000000000005a14020047
+            00640a8400640ba6020000ab0200000000000000005a15640c84005a1665
+            17640d8400a6000000ab0000000000000000005a186517640e8400a60000
+            00ab0000000000000000005a19640f84005a1a64105300
+         101           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Thread')
                        8 STORE_NAME               2 (__qualname__)
          
-         101          10 PUSH_NULL
+         102          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (ForeignKey)
          
-         102          24 LOAD_NAME                5 (Subcategory)
+         103          24 LOAD_NAME                5 (Subcategory)
                       26 LOAD_CONST               1 ('threads')
                       28 LOAD_NAME                3 (models)
                       30 LOAD_ATTR                6 (CASCADE)
          
-         101          40 KW_NAMES                 2
+         102          40 KW_NAMES                 2
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_NAME               7 (subcategory)
          
-         104          58 PUSH_NULL
+         105          58 PUSH_NULL
                       60 LOAD_NAME                3 (models)
                       62 LOAD_ATTR                4 (ForeignKey)
                       72 LOAD_NAME                8 (User)
                       74 LOAD_CONST               1 ('threads')
                       76 LOAD_NAME                3 (models)
                       78 LOAD_ATTR                6 (CASCADE)
                       88 KW_NAMES                 2
                       90 PRECALL                  3
                       94 CALL                     3
                      104 STORE_NAME               9 (user)
          
-         105         106 PUSH_NULL
+         106         106 PUSH_NULL
                      108 LOAD_NAME                3 (models)
                      110 LOAD_ATTR               10 (CharField)
                      120 LOAD_CONST               3 (255)
                      122 KW_NAMES                 4
                      124 PRECALL                  1
                      128 CALL                     1
                      138 STORE_NAME              11 (title)
          
-         106         140 PUSH_NULL
+         107         140 PUSH_NULL
                      142 LOAD_NAME               12 (BBCodeTextField)
                      144 PRECALL                  0
                      148 CALL                     0
                      158 STORE_NAME              13 (content)
          
-         107         160 PUSH_NULL
+         108         160 PUSH_NULL
                      162 LOAD_NAME                3 (models)
                      164 LOAD_ATTR               14 (BooleanField)
                      174 LOAD_CONST               5 (False)
                      176 KW_NAMES                 6
                      178 PRECALL                  1
                      182 CALL                     1
                      192 STORE_NAME              15 (is_pinned)
          
-         108         194 PUSH_NULL
+         109         194 PUSH_NULL
                      196 LOAD_NAME                3 (models)
                      198 LOAD_ATTR               14 (BooleanField)
                      208 LOAD_CONST               5 (False)
                      210 KW_NAMES                 6
                      212 PRECALL                  1
                      216 CALL                     1
                      226 STORE_NAME              16 (is_closed)
          
-         109         228 PUSH_NULL
+         110         228 PUSH_NULL
                      230 LOAD_NAME                3 (models)
                      232 LOAD_ATTR               17 (DateTimeField)
                      242 LOAD_CONST               7 (True)
                      244 KW_NAMES                 8
                      246 PRECALL                  1
                      250 CALL                     1
                      260 STORE_NAME              18 (last_post_created_at)
          
          111         262 PUSH_NULL
-                     264 LOAD_BUILD_CLASS
-                     266 LOAD_CONST               9 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 111>)
-                     268 MAKE_FUNCTION            0
-                     270 LOAD_CONST              10 ('Meta')
-                     272 PRECALL                  2
-                     276 CALL                     2
-                     286 STORE_NAME              19 (Meta)
-         
-         118         288 LOAD_CONST              11 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 118>)
-                     290 MAKE_FUNCTION            0
-                     292 STORE_NAME              20 (__str__)
-         
-         121         294 LOAD_NAME               21 (property)
-         
-         122         296 LOAD_CONST              12 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 121>)
-                     298 MAKE_FUNCTION            0
-         
-         121         300 PRECALL                  0
-                     304 CALL                     0
-         
-         122         314 STORE_NAME              22 (post_count)
-         
-         125         316 LOAD_NAME               21 (property)
-         
-         126         318 LOAD_CONST              13 (<code object latest_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 125>)
-                     320 MAKE_FUNCTION            0
-         
-         125         322 PRECALL                  0
-                     326 CALL                     0
-         
-         126         336 STORE_NAME              23 (latest_post)
-         
-         129         338 LOAD_CONST              14 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 129>)
-                     340 MAKE_FUNCTION            0
-                     342 STORE_NAME              24 (get_absolute_url)
-                     344 LOAD_CONST              15 (None)
-                     346 RETURN_VALUE
+                     264 LOAD_NAME                3 (models)
+                     266 LOAD_ATTR               19 (PositiveIntegerField)
+                     276 LOAD_CONST               9 (0)
+                     278 KW_NAMES                 6
+                     280 PRECALL                  1
+                     284 CALL                     1
+                     294 STORE_NAME              20 (view_count)
+         
+         113         296 PUSH_NULL
+                     298 LOAD_BUILD_CLASS
+                     300 LOAD_CONST              10 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 113>)
+                     302 MAKE_FUNCTION            0
+                     304 LOAD_CONST              11 ('Meta')
+                     306 PRECALL                  2
+                     310 CALL                     2
+                     320 STORE_NAME              21 (Meta)
+         
+         120         322 LOAD_CONST              12 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 120>)
+                     324 MAKE_FUNCTION            0
+                     326 STORE_NAME              22 (__str__)
+         
+         123         328 LOAD_NAME               23 (property)
+         
+         124         330 LOAD_CONST              13 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 123>)
+                     332 MAKE_FUNCTION            0
+         
+         123         334 PRECALL                  0
+                     338 CALL                     0
+         
+         124         348 STORE_NAME              24 (post_count)
+         
+         127         350 LOAD_NAME               23 (property)
+         
+         128         352 LOAD_CONST              14 (<code object latest_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 127>)
+                     354 MAKE_FUNCTION            0
+         
+         127         356 PRECALL                  0
+                     360 CALL                     0
+         
+         128         370 STORE_NAME              25 (latest_post)
+         
+         131         372 LOAD_CONST              15 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 131>)
+                     374 MAKE_FUNCTION            0
+                     376 STORE_NAME              26 (get_absolute_url)
+                     378 LOAD_CONST              16 (None)
+                     380 RETURN_VALUE
          consts
             'Thread'
             'threads'
             ('related_name', 'on_delete')
             255
             ('max_length',)
             False
             ('default',)
             True
             ('auto_now_add',)
+            0
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025300
-               111           0 RESUME                   0
+               113           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Thread.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               112          10 LOAD_CONST               1 (('subcategory', '-is_pinned', '-last_post_created_at'))
+               114          10 LOAD_CONST               1 (('subcategory', '-is_pinned', '-last_post_created_at'))
                             12 STORE_NAME               3 (ordering)
                             14 LOAD_CONST               2 (None)
                             16 RETURN_VALUE
                consts
                   'Thread.Meta'
                   ('subcategory', '-is_pinned', '-last_post_created_at')
                   None
                names      ('__name__', '__module__', '__qualname__', 'ordering')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 111
+               firstlineno 113
                lnotab 0x0a01
             'Meta'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000009b005300
-               118           0 RESUME                   0
+               120           0 RESUME                   0
                
-               119           2 LOAD_FAST                0 (self)
+               121           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (title)
                             14 FORMAT_VALUE             0
                             16 RETURN_VALUE
                consts
                   None
                names      ('title',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 118
+               firstlineno 120
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab0000000000000000005300
-               121           0 RESUME                   0
+               123           0 RESUME                   0
                
-               123           2 LOAD_FAST                0 (self)
+               125           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (posts)
                             14 LOAD_METHOD              1 (count)
                             36 PRECALL                  0
                             40 CALL                     0
                             50 RETURN_VALUE
                consts
                   None
                names      ('posts', 'count')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'post_count'
-               firstlineno 121
+               firstlineno 123
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000a0020000000000
                   000000000000000000000000000000a6000000ab00000000000000000053
                   00
-               125           0 RESUME                   0
+               127           0 RESUME                   0
                
-               127           2 LOAD_FAST                0 (self)
+               129           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (posts)
                             14 LOAD_METHOD              1 (order_by)
                             36 LOAD_CONST               1 ('-created_at')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 LOAD_METHOD              2 (first)
                             74 PRECALL                  0
@@ -1285,27 +1305,27 @@
                   '-created_at'
                names      ('posts', 'order_by', 'first')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'latest_post'
-               firstlineno 125
+               firstlineno 127
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x970074010000000000000000000064017c006a01000000000000000067
                   01ac02a6020000ab0200000000000000005300
-               129           0 RESUME                   0
+               131           0 RESUME                   0
                
-               130           2 LOAD_GLOBAL              1 (NULL + reverse)
+               132           2 LOAD_GLOBAL              1 (NULL + reverse)
                             14 LOAD_CONST               1 ('punkweb_bb:thread')
                             16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (id)
                             28 BUILD_LIST               1
                             30 KW_NAMES                 2
                             32 PRECALL                  2
                             36 CALL                     2
@@ -1316,27 +1336,27 @@
                   ('args',)
                names      ('reverse', 'id')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'get_absolute_url'
-               firstlineno 129
+               firstlineno 131
                lnotab 0x0201
             None
-         names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'Subcategory', 'CASCADE', 'subcategory', 'User', 'user', 'CharField', 'title', 'BBCodeTextField', 'content', 'BooleanField', 'is_pinned', 'is_closed', 'DateTimeField', 'last_post_created_at', 'Meta', '__str__', 'property', 'post_count', 'latest_post', 'get_absolute_url')
+         names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'Subcategory', 'CASCADE', 'subcategory', 'User', 'user', 'CharField', 'title', 'BBCodeTextField', 'content', 'BooleanField', 'is_pinned', 'is_closed', 'DateTimeField', 'last_post_created_at', 'PositiveIntegerField', 'view_count', 'Meta', '__str__', 'property', 'post_count', 'latest_post', 'get_absolute_url')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Thread'
-         firstlineno 100
+         firstlineno 101
          lnotab
-            0x0a010e0110ff12033001220114012201220122021a070603020104ff0e
-            010203020104ff0e010203
+            0x0a010e0110ff120330012201140122012201220122021a070603020104
+            ff0e010203020104ff0e010203
       'Thread'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
@@ -1346,90 +1366,90 @@
             00ac02a6030000ab0300000000000000005a090200650aa6000000ab0000
             000000000000005a0b02004700640384006404a6020000ab020000000000
             0000005a0c640584005a0d650e64068400a6000000ab0000000000000000
             005a0f650e64078400a6000000ab0000000000000000005a10640884005a
             1188006601640984085a12880078015a135300
                        0 MAKE_CELL                0 (__class__)
          
-         133           2 RESUME                   0
+         135           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Post')
                       10 STORE_NAME               2 (__qualname__)
          
-         134          12 PUSH_NULL
+         136          12 PUSH_NULL
                       14 LOAD_NAME                3 (models)
                       16 LOAD_ATTR                4 (ForeignKey)
                       26 LOAD_NAME                5 (Thread)
                       28 LOAD_CONST               1 ('posts')
                       30 LOAD_NAME                3 (models)
                       32 LOAD_ATTR                6 (CASCADE)
                       42 KW_NAMES                 2
                       44 PRECALL                  3
                       48 CALL                     3
                       58 STORE_NAME               7 (thread)
          
-         135          60 PUSH_NULL
+         137          60 PUSH_NULL
                       62 LOAD_NAME                3 (models)
                       64 LOAD_ATTR                4 (ForeignKey)
                       74 LOAD_NAME                8 (User)
                       76 LOAD_CONST               1 ('posts')
                       78 LOAD_NAME                3 (models)
                       80 LOAD_ATTR                6 (CASCADE)
                       90 KW_NAMES                 2
                       92 PRECALL                  3
                       96 CALL                     3
                      106 STORE_NAME               9 (user)
          
-         136         108 PUSH_NULL
+         138         108 PUSH_NULL
                      110 LOAD_NAME               10 (BBCodeTextField)
                      112 PRECALL                  0
                      116 CALL                     0
                      126 STORE_NAME              11 (content)
          
-         138         128 PUSH_NULL
+         140         128 PUSH_NULL
                      130 LOAD_BUILD_CLASS
-                     132 LOAD_CONST               3 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 138>)
+                     132 LOAD_CONST               3 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 140>)
                      134 MAKE_FUNCTION            0
                      136 LOAD_CONST               4 ('Meta')
                      138 PRECALL                  2
                      142 CALL                     2
                      152 STORE_NAME              12 (Meta)
          
-         141         154 LOAD_CONST               5 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 141>)
+         143         154 LOAD_CONST               5 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 143>)
                      156 MAKE_FUNCTION            0
                      158 STORE_NAME              13 (__str__)
          
-         144         160 LOAD_NAME               14 (property)
+         146         160 LOAD_NAME               14 (property)
          
-         145         162 LOAD_CONST               6 (<code object index, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 144>)
+         147         162 LOAD_CONST               6 (<code object index, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 146>)
                      164 MAKE_FUNCTION            0
          
-         144         166 PRECALL                  0
+         146         166 PRECALL                  0
                      170 CALL                     0
          
-         145         180 STORE_NAME              15 (index)
+         147         180 STORE_NAME              15 (index)
          
-         152         182 LOAD_NAME               14 (property)
+         154         182 LOAD_NAME               14 (property)
          
-         153         184 LOAD_CONST               7 (<code object page_number, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 152>)
+         155         184 LOAD_CONST               7 (<code object page_number, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 154>)
                      186 MAKE_FUNCTION            0
          
-         152         188 PRECALL                  0
+         154         188 PRECALL                  0
                      192 CALL                     0
          
-         153         202 STORE_NAME              16 (page_number)
+         155         202 STORE_NAME              16 (page_number)
          
-         156         204 LOAD_CONST               8 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 156>)
+         158         204 LOAD_CONST               8 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 158>)
                      206 MAKE_FUNCTION            0
                      208 STORE_NAME              17 (get_absolute_url)
          
-         163         210 LOAD_CLOSURE             0 (__class__)
+         165         210 LOAD_CLOSURE             0 (__class__)
                      212 BUILD_TUPLE              1
-                     214 LOAD_CONST               9 (<code object save, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 163>)
+                     214 LOAD_CONST               9 (<code object save, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 165>)
                      216 MAKE_FUNCTION            8 (closure)
                      218 STORE_NAME              18 (save)
                      220 LOAD_CLOSURE             0 (__class__)
                      222 COPY                     1
                      224 STORE_NAME              19 (__classcell__)
                      226 RETURN_VALUE
          consts
@@ -1438,48 +1458,48 @@
             ('related_name', 'on_delete')
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025300
-               138           0 RESUME                   0
+               140           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Post.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               139          10 LOAD_CONST               1 (('created_at',))
+               141          10 LOAD_CONST               1 (('created_at',))
                             12 STORE_NAME               3 (ordering)
                             14 LOAD_CONST               2 (None)
                             16 RETURN_VALUE
                consts
                   'Post.Meta'
                   ('created_at',)
                   None
                names      ('__name__', '__module__', '__qualname__', 'ordering')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 138
+               firstlineno 140
                lnotab 0x0a01
             'Meta'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007c006a0000000000000000009b0064017c006a0100000000000000
                   009b0064017c006a0200000000000000009b009d055300
-               141           0 RESUME                   0
+               143           0 RESUME                   0
                
-               142           2 LOAD_FAST                0 (self)
+               144           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (thread)
                             14 FORMAT_VALUE             0
                             16 LOAD_CONST               1 (' > ')
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (user)
                             30 FORMAT_VALUE             0
                             32 LOAD_CONST               1 (' > ')
@@ -1493,41 +1513,41 @@
                   ' > '
                names      ('thread', 'user', 'created_at')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 141
+               firstlineno 143
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a0000000000000000006a010000000000000000a002000000
                   00000000000000000000000000000000006401a6010000ab010000000000
                   0000007d017407000000000000000000007c01a004000000000000000000
                   000000000000000000000064026403ac04a6020000ab0200000000000000
                   00a6010000ab010000000000000000a00500000000000000000000000000
                   000000000000007c006a060000000000000000a6010000ab010000000000
                   0000007d027c0264057a0000005300
-               144           0 RESUME                   0
+               146           0 RESUME                   0
                
-               148           2 LOAD_FAST                0 (self)
+               150           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (thread)
                             14 LOAD_ATTR                1 (posts)
                             24 LOAD_METHOD              2 (order_by)
                             46 LOAD_CONST               1 ('created_at')
                             48 PRECALL                  1
                             52 CALL                     1
                             62 STORE_FAST               1 (qs)
                
-               149          64 LOAD_GLOBAL              7 (NULL + list)
+               151          64 LOAD_GLOBAL              7 (NULL + list)
                             76 LOAD_FAST                1 (qs)
                             78 LOAD_METHOD              4 (values_list)
                            100 LOAD_CONST               2 ('id')
                            102 LOAD_CONST               3 (True)
                            104 KW_NAMES                 4
                            106 PRECALL                  2
                            110 CALL                     2
@@ -1536,15 +1556,15 @@
                            134 LOAD_METHOD              5 (index)
                            156 LOAD_FAST                0 (self)
                            158 LOAD_ATTR                6 (id)
                            168 PRECALL                  1
                            172 CALL                     1
                            182 STORE_FAST               2 (index)
                
-               150         184 LOAD_FAST                2 (index)
+               152         184 LOAD_FAST                2 (index)
                            186 LOAD_CONST               5 (1)
                            188 BINARY_OP                0 (+)
                            192 RETURN_VALUE
                consts
                   None
                   'created_at'
                   'id'
@@ -1553,27 +1573,27 @@
                   1
                names      ('thread', 'posts', 'order_by', 'list', 'values_list', 'index', 'id')
                varnames   ('self', 'qs', 'index')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'index'
-               firstlineno 144
+               firstlineno 146
                lnotab 0x02043e017801
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007c006a0200
                   0000000000000064017a0b0000a6010000ab0100000000000000005300
-               152           0 RESUME                   0
+               154           0 RESUME                   0
                
-               154           2 LOAD_GLOBAL              1 (NULL + math)
+               156           2 LOAD_GLOBAL              1 (NULL + math)
                             14 LOAD_ATTR                1 (ceil)
                             24 LOAD_FAST                0 (self)
                             26 LOAD_ATTR                2 (index)
                             36 LOAD_CONST               1 (10)
                             38 BINARY_OP               11 (/)
                             42 PRECALL                  1
                             46 CALL                     1
@@ -1583,135 +1603,149 @@
                   10
                names      ('math', 'ceil', 'index')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'page_number'
-               firstlineno 152
+               firstlineno 154
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x970074010000000000000000000064017c006a0100000000000000006a
                   0200000000000000006701ac02a6020000ab0200000000000000007d017c
                   0164037c006a0300000000000000009b0064047c006a0200000000000000
                   009b009d047a0d00007d017c015300
-               156           0 RESUME                   0
+               158           0 RESUME                   0
                
-               157           2 LOAD_GLOBAL              1 (NULL + reverse)
+               159           2 LOAD_GLOBAL              1 (NULL + reverse)
                             14 LOAD_CONST               1 ('punkweb_bb:thread')
                             16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (thread)
                             28 LOAD_ATTR                2 (id)
                             38 BUILD_LIST               1
                             40 KW_NAMES                 2
                             42 PRECALL                  2
                             46 CALL                     2
                             56 STORE_FAST               1 (thread_url)
                
-               159          58 LOAD_FAST                1 (thread_url)
+               161          58 LOAD_FAST                1 (thread_url)
                             60 LOAD_CONST               3 ('?page=')
                             62 LOAD_FAST                0 (self)
                             64 LOAD_ATTR                3 (page_number)
                             74 FORMAT_VALUE             0
                             76 LOAD_CONST               4 ('#post-')
                             78 LOAD_FAST                0 (self)
                             80 LOAD_ATTR                2 (id)
                             90 FORMAT_VALUE             0
                             92 BUILD_STRING             4
                             94 BINARY_OP               13 (+=)
                             98 STORE_FAST               1 (thread_url)
                
-               161         100 LOAD_FAST                1 (thread_url)
+               163         100 LOAD_FAST                1 (thread_url)
                            102 RETURN_VALUE
                consts
                   None
                   'punkweb_bb:thread'
                   ('args',)
                   '?page='
                   '#post-'
                names      ('reverse', 'thread', 'id', 'page_number')
                varnames   ('self', 'thread_url')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'get_absolute_url'
-               firstlineno 156
+               firstlineno 158
                lnotab 0x020138022a02
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code
-                  0x950197007c006a0000000000000000006a010000000000000000723674
-                  05000000000000000000006a030000000000000000a6000000ab00000000
-                  00000000007c006a0400000000000000005f0500000000000000007c006a
-                  040000000000000000a00600000000000000000000000000000000000000
-                  00a6000000ab00000000000000000001000200740f000000000000000000
-                  00a6000000ab0000000000000000006a0600000000000000007c0169007c
-                  02a4018e01010064005300
+                  0x950197007c006a0000000000000000006a010000000000000000720f74
+                  05000000000000000000006401a6010000ab01000000000000000082017c
+                  006a0300000000000000006a0400000000000000007236740b0000000000
+                  00000000006a060000000000000000a6000000ab0000000000000000007c
+                  006a0000000000000000005f0700000000000000007c006a000000000000
+                  000000a0080000000000000000000000000000000000000000a6000000ab
+                  00000000000000000001000200741300000000000000000000a6000000ab
+                  0000000000000000006a0800000000000000007c0169007c02a4018e0101
+                  0064005300
                              0 COPY_FREE_VARS           1
                
-               163           2 RESUME                   0
+               165           2 RESUME                   0
+               
+               166           4 LOAD_FAST                0 (self)
+                             6 LOAD_ATTR                0 (thread)
+                            16 LOAD_ATTR                1 (is_closed)
+                            26 POP_JUMP_FORWARD_IF_FALSE    15 (to 58)
                
-               164           4 LOAD_FAST                0 (self)
-                             6 LOAD_ATTR                0 (_state)
-                            16 LOAD_ATTR                1 (adding)
-                            26 POP_JUMP_FORWARD_IF_FALSE    54 (to 136)
-               
-               165          28 LOAD_GLOBAL              5 (NULL + timezone)
-                            40 LOAD_ATTR                3 (now)
-                            50 PRECALL                  0
-                            54 CALL                     0
-                            64 LOAD_FAST                0 (self)
-                            66 LOAD_ATTR                4 (thread)
-                            76 STORE_ATTR               5 (last_post_created_at)
-               
-               166          86 LOAD_FAST                0 (self)
-                            88 LOAD_ATTR                4 (thread)
-                            98 LOAD_METHOD              6 (save)
-                           120 PRECALL                  0
-                           124 CALL                     0
-                           134 POP_TOP
-               
-               167     >>  136 PUSH_NULL
-                           138 LOAD_GLOBAL             15 (NULL + super)
-                           150 PRECALL                  0
-                           154 CALL                     0
-                           164 LOAD_ATTR                6 (save)
-                           174 LOAD_FAST                1 (args)
-                           176 BUILD_MAP                0
-                           178 LOAD_FAST                2 (kwargs)
-                           180 DICT_MERGE               1
-                           182 CALL_FUNCTION_EX         1
-                           184 POP_TOP
-                           186 LOAD_CONST               0 (None)
-                           188 RETURN_VALUE
+               167          28 LOAD_GLOBAL              5 (NULL + ValidationError)
+                            40 LOAD_CONST               1 ('Cannot add posts to a closed thread.')
+                            42 PRECALL                  1
+                            46 CALL                     1
+                            56 RAISE_VARARGS            1
+               
+               168     >>   58 LOAD_FAST                0 (self)
+                            60 LOAD_ATTR                3 (_state)
+                            70 LOAD_ATTR                4 (adding)
+                            80 POP_JUMP_FORWARD_IF_FALSE    54 (to 190)
+               
+               169          82 LOAD_GLOBAL             11 (NULL + timezone)
+                            94 LOAD_ATTR                6 (now)
+                           104 PRECALL                  0
+                           108 CALL                     0
+                           118 LOAD_FAST                0 (self)
+                           120 LOAD_ATTR                0 (thread)
+                           130 STORE_ATTR               7 (last_post_created_at)
+               
+               170         140 LOAD_FAST                0 (self)
+                           142 LOAD_ATTR                0 (thread)
+                           152 LOAD_METHOD              8 (save)
+                           174 PRECALL                  0
+                           178 CALL                     0
+                           188 POP_TOP
+               
+               171     >>  190 PUSH_NULL
+                           192 LOAD_GLOBAL             19 (NULL + super)
+                           204 PRECALL                  0
+                           208 CALL                     0
+                           218 LOAD_ATTR                8 (save)
+                           228 LOAD_FAST                1 (args)
+                           230 BUILD_MAP                0
+                           232 LOAD_FAST                2 (kwargs)
+                           234 DICT_MERGE               1
+                           236 CALL_FUNCTION_EX         1
+                           238 POP_TOP
+                           240 LOAD_CONST               0 (None)
+                           242 RETURN_VALUE
                consts
                   None
-               names      ('_state', 'adding', 'timezone', 'now', 'thread', 'last_post_created_at', 'save', 'super')
+                  'Cannot add posts to a closed thread.'
+               names      ('thread', 'is_closed', 'ValidationError', '_state', 'adding', 'timezone', 'now', 'last_post_created_at', 'save', 'super')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'save'
-               firstlineno 163
-               lnotab 0x040118013a013201
+               firstlineno 165
+               lnotab 0x040118011e0118013a013201
          names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'Thread', 'CASCADE', 'thread', 'User', 'user', 'BBCodeTextField', 'content', 'Meta', '__str__', 'property', 'index', 'page_number', 'get_absolute_url', 'save', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Post'
-         firstlineno 133
+         firstlineno 135
          lnotab
             0x0c013001300114021a030603020104ff0e010207020104ff0e01020306
             07
       'Post'
       code
          argcount  : 0
          nlocals   : 0
@@ -1719,97 +1753,97 @@
          flags     : 0
          code
             0x970065005a0164005a02020065036a0400000000000000006505640165
             036a060000000000000000ac02a6030000ab0300000000000000005a0702
             0065036a080000000000000000a6000000ab0000000000000000005a0902
             004700640384006404a6020000ab0200000000000000005a0a640584005a
             0b64065300
-         170           0 RESUME                   0
+         174           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Shout')
                        8 STORE_NAME               2 (__qualname__)
          
-         171          10 PUSH_NULL
+         175          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (ForeignKey)
                       24 LOAD_NAME                5 (User)
                       26 LOAD_CONST               1 ('shouts')
                       28 LOAD_NAME                3 (models)
                       30 LOAD_ATTR                6 (CASCADE)
                       40 KW_NAMES                 2
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_NAME               7 (user)
          
-         172          58 PUSH_NULL
+         176          58 PUSH_NULL
                       60 LOAD_NAME                3 (models)
                       62 LOAD_ATTR                8 (TextField)
                       72 PRECALL                  0
                       76 CALL                     0
                       86 STORE_NAME               9 (content)
          
-         174          88 PUSH_NULL
+         178          88 PUSH_NULL
                       90 LOAD_BUILD_CLASS
-                      92 LOAD_CONST               3 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 174>)
+                      92 LOAD_CONST               3 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 178>)
                       94 MAKE_FUNCTION            0
                       96 LOAD_CONST               4 ('Meta')
                       98 PRECALL                  2
                      102 CALL                     2
                      112 STORE_NAME              10 (Meta)
          
-         177         114 LOAD_CONST               5 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 177>)
+         181         114 LOAD_CONST               5 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 181>)
                      116 MAKE_FUNCTION            0
                      118 STORE_NAME              11 (__str__)
                      120 LOAD_CONST               6 (None)
                      122 RETURN_VALUE
          consts
             'Shout'
             'shouts'
             ('related_name', 'on_delete')
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025300
-               174           0 RESUME                   0
+               178           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Shout.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               175          10 LOAD_CONST               1 (('-created_at',))
+               179          10 LOAD_CONST               1 (('-created_at',))
                             12 STORE_NAME               3 (ordering)
                             14 LOAD_CONST               2 (None)
                             16 RETURN_VALUE
                consts
                   'Shout.Meta'
                   ('-created_at',)
                   None
                names      ('__name__', '__module__', '__qualname__', 'ordering')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 174
+               firstlineno 178
                lnotab 0x0a01
             'Meta'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000009b0064017c006a0100000000000000
                   009b009d035300
-               177           0 RESUME                   0
+               181           0 RESUME                   0
                
-               178           2 LOAD_FAST                0 (self)
+               182           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (user)
                             14 FORMAT_VALUE             0
                             16 LOAD_CONST               1 (' > ')
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (created_at)
                             30 FORMAT_VALUE             0
                             32 BUILD_STRING             3
@@ -1819,29 +1853,29 @@
                   ' > '
                names      ('user', 'created_at')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 177
+               firstlineno 181
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'User', 'CASCADE', 'user', 'TextField', 'content', 'Meta', '__str__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Shout'
-         firstlineno 170
+         firstlineno 174
          lnotab 0x0a0130011e021a03
       'Shout'
-   names      ('datetime', 'math', 'os', 'django.contrib.auth', 'get_user_model', 'django.core.cache', 'cache', 'django.db', 'models', 'django.urls', 'reverse', 'django.utils', 'timezone', 'precise_bbcode.fields', 'BBCodeTextField', 'punkweb_bb.mixins', 'TimestampMixin', 'UUIDPrimaryKeyMixin', 'User', 'profile_image_upload_to', 'BoardProfile', 'Category', 'Subcategory', 'Thread', 'Post', 'Shout')
+   names      ('datetime', 'math', 'os', 'django.contrib.auth', 'get_user_model', 'django.core.cache', 'cache', 'django.db', 'models', 'django.forms', 'ValidationError', 'django.urls', 'reverse', 'django.utils', 'timezone', 'precise_bbcode.fields', 'BBCodeTextField', 'punkweb_bb.mixins', 'TimestampMixin', 'UUIDPrimaryKeyMixin', 'User', 'profile_image_upload_to', 'BoardProfile', 'Category', 'Subcategory', 'Thread', 'Post', 'Shout')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010801080108020c010c010c010c010c010c021002140306051e
-      171e121e251e211e25
+      0x00ff02010801080108020c010c010c010c010c010c010c021002140306
+      051e171e121e251e221e27
```

### Comparing `punkweb_bb-0.1.2/punkweb_bb/__pycache__/pagination.cpython-311.pyc` & `punkweb_bb-0.1.3/punkweb_bb/__pycache__/pagination.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/__pycache__/parsers.cpython-311.pyc` & `punkweb_bb-0.1.3/punkweb_bb/__pycache__/parsers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/__pycache__/settings.cpython-311.pyc` & `punkweb_bb-0.1.3/punkweb_bb/__pycache__/settings.cpython-311.pyc`

 * *Files 24% similar despite different names*

#### Python bytecode

```diff
@@ -1,22 +1,24 @@
 magic:    0xa70d0d0a
-moddate:  0xedc81466 (Tue Apr  9 04:49:49 2024 UTC)
-files sz: 250
+moddate:  0x7d8e3966 (Tue May  7 02:14:21 2024 UTC)
+files sz: 312
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a01010002006502650164026900a6030000ab
       0300000000000000005a036503a004000000000000000000000000000000
       000000000064036404a6020000ab0200000000000000005a056503a00400
       0000000000000000000000000000000000000064056406a6020000ab0200
       000000000000005a066503a0040000000000000000000000000000000000
-      00000064076408a6020000ab0200000000000000005a0764095300
+      00000064076408a6020000ab0200000000000000005a076503a004000000
+      00000000000000000000000000000000006409640aa6020000ab02000000
+      00000000005a08640b5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('settings',))
                  6 IMPORT_NAME              0 (django.conf)
                  8 IMPORT_FROM              1 (settings)
                 10 STORE_NAME               1 (settings)
@@ -45,33 +47,43 @@
                110 LOAD_CONST               6 ('PunkwebBB')
                112 PRECALL                  2
                116 CALL                     2
                126 STORE_NAME               6 (SITE_TITLE)
    
      7         128 LOAD_NAME                3 (PUNKWEB_BB)
                130 LOAD_METHOD              4 (get)
-               152 LOAD_CONST               7 ('SHOUTBOX_ENABLED')
-               154 LOAD_CONST               8 (True)
+               152 LOAD_CONST               7 ('FAVICON')
+               154 LOAD_CONST               8 ('punkweb_bb/favicon.ico')
                156 PRECALL                  2
                160 CALL                     2
-               170 STORE_NAME               7 (SHOUTBOX_ENABLED)
-               172 LOAD_CONST               9 (None)
-               174 RETURN_VALUE
+               170 STORE_NAME               7 (FAVICON)
+   
+     8         172 LOAD_NAME                3 (PUNKWEB_BB)
+               174 LOAD_METHOD              4 (get)
+               196 LOAD_CONST               9 ('SHOUTBOX_ENABLED')
+               198 LOAD_CONST              10 (True)
+               200 PRECALL                  2
+               204 CALL                     2
+               214 STORE_NAME               8 (SHOUTBOX_ENABLED)
+               216 LOAD_CONST              11 (None)
+               218 RETURN_VALUE
    consts
       0
       ('settings',)
       'PUNKWEB_BB'
       'SITE_NAME'
       'PUNKWEB'
       'SITE_TITLE'
       'PunkwebBB'
+      'FAVICON'
+      'punkweb_bb/favicon.ico'
       'SHOUTBOX_ENABLED'
       True
       None
-   names      ('django.conf', 'settings', 'getattr', 'PUNKWEB_BB', 'get', 'SITE_NAME', 'SITE_TITLE', 'SHOUTBOX_ENABLED')
+   names      ('django.conf', 'settings', 'getattr', 'PUNKWEB_BB', 'get', 'SITE_NAME', 'SITE_TITLE', 'FAVICON', 'SHOUTBOX_ENABLED')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/settings.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c021a022c012c01
+   lnotab 0x00ff02010c021a022c012c012c01
```

### Comparing `punkweb_bb-0.1.2/punkweb_bb/__pycache__/signals.cpython-311.pyc` & `punkweb_bb-0.1.3/punkweb_bb/__pycache__/signals.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/__pycache__/urls.cpython-311.pyc` & `punkweb_bb-0.1.3/punkweb_bb/__pycache__/urls.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/__pycache__/views.cpython-311.pyc` & `punkweb_bb-0.1.3/punkweb_bb/__pycache__/views.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xf2811466 (Mon Apr  8 23:46:58 2024 UTC)
-files sz: 10435
+moddate:  0x72c63966 (Tue May  7 06:13:06 2024 UTC)
+files sz: 10723
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a026d035a036d045a046d
@@ -150,140 +150,140 @@
                220 MAKE_FUNCTION            0
                222 STORE_NAME              38 (profile_view)
    
    110         224 LOAD_CONST              16 (<code object members_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 110>)
                226 MAKE_FUNCTION            0
                228 STORE_NAME              39 (members_view)
    
-   119         230 PUSH_NULL
+   121         230 PUSH_NULL
                232 LOAD_NAME                7 (login_required)
                234 LOAD_CONST              17 ('/login/')
                236 KW_NAMES                18
                238 PRECALL                  1
                242 CALL                     1
    
-   120         252 LOAD_CONST              19 (<code object settings_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 119>)
+   122         252 LOAD_CONST              19 (<code object settings_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 121>)
                254 MAKE_FUNCTION            0
    
-   119         256 PRECALL                  0
+   121         256 PRECALL                  0
                260 CALL                     0
    
-   120         270 STORE_NAME              40 (settings_view)
+   122         270 STORE_NAME              40 (settings_view)
    
-   142         272 LOAD_CONST              20 (<code object subcategory_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 142>)
+   144         272 LOAD_CONST              20 (<code object subcategory_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 144>)
                274 MAKE_FUNCTION            0
                276 STORE_NAME              41 (subcategory_view)
    
-   154         278 PUSH_NULL
+   156         278 PUSH_NULL
                280 LOAD_NAME                7 (login_required)
                282 LOAD_CONST              17 ('/login/')
                284 KW_NAMES                18
                286 PRECALL                  1
                290 CALL                     1
    
-   155         300 LOAD_CONST              21 (<code object thread_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 154>)
+   157         300 LOAD_CONST              21 (<code object thread_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 156>)
                302 MAKE_FUNCTION            0
    
-   154         304 PRECALL                  0
+   156         304 PRECALL                  0
                308 CALL                     0
    
-   155         318 STORE_NAME              42 (thread_create_view)
+   157         318 STORE_NAME              42 (thread_create_view)
    
-   181         320 LOAD_CONST              22 (<code object thread_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 181>)
+   183         320 LOAD_CONST              22 (<code object thread_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 183>)
                322 MAKE_FUNCTION            0
                324 STORE_NAME              43 (thread_view)
    
-   196         326 PUSH_NULL
+   205         326 PUSH_NULL
                328 LOAD_NAME                7 (login_required)
                330 LOAD_CONST              17 ('/login/')
                332 KW_NAMES                18
                334 PRECALL                  1
                338 CALL                     1
    
-   197         348 LOAD_CONST              23 (<code object thread_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 196>)
+   206         348 LOAD_CONST              23 (<code object thread_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 205>)
                350 MAKE_FUNCTION            0
    
-   196         352 PRECALL                  0
+   205         352 PRECALL                  0
                356 CALL                     0
    
-   197         366 STORE_NAME              44 (thread_update_view)
+   206         366 STORE_NAME              44 (thread_update_view)
    
-   217         368 PUSH_NULL
+   226         368 PUSH_NULL
                370 LOAD_NAME                7 (login_required)
                372 LOAD_CONST              17 ('/login/')
                374 KW_NAMES                18
                376 PRECALL                  1
                380 CALL                     1
    
-   218         390 LOAD_CONST              24 (<code object thread_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 217>)
+   227         390 LOAD_CONST              24 (<code object thread_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 226>)
                392 MAKE_FUNCTION            0
    
-   217         394 PRECALL                  0
+   226         394 PRECALL                  0
                398 CALL                     0
    
-   218         408 STORE_NAME              45 (thread_delete_view)
+   227         408 STORE_NAME              45 (thread_delete_view)
    
-   233         410 PUSH_NULL
+   242         410 PUSH_NULL
                412 LOAD_NAME                7 (login_required)
                414 LOAD_CONST              17 ('/login/')
                416 KW_NAMES                18
                418 PRECALL                  1
                422 CALL                     1
    
-   234         432 LOAD_CONST              25 (<code object post_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 233>)
+   243         432 LOAD_CONST              25 (<code object post_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 242>)
                434 MAKE_FUNCTION            0
    
-   233         436 PRECALL                  0
+   242         436 PRECALL                  0
                440 CALL                     0
    
-   234         450 STORE_NAME              46 (post_create_view)
+   243         450 STORE_NAME              46 (post_create_view)
    
-   251         452 PUSH_NULL
+   260         452 PUSH_NULL
                454 LOAD_NAME                7 (login_required)
                456 LOAD_CONST              17 ('/login/')
                458 KW_NAMES                18
                460 PRECALL                  1
                464 CALL                     1
    
-   252         474 LOAD_CONST              26 (<code object post_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 251>)
+   261         474 LOAD_CONST              26 (<code object post_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 260>)
                476 MAKE_FUNCTION            0
    
-   251         478 PRECALL                  0
+   260         478 PRECALL                  0
                482 CALL                     0
    
-   252         492 STORE_NAME              47 (post_update_view)
+   261         492 STORE_NAME              47 (post_update_view)
    
-   273         494 PUSH_NULL
+   282         494 PUSH_NULL
                496 LOAD_NAME                7 (login_required)
                498 LOAD_CONST              17 ('/login/')
                500 KW_NAMES                18
                502 PRECALL                  1
                506 CALL                     1
    
-   274         516 LOAD_CONST              27 (<code object post_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 273>)
+   283         516 LOAD_CONST              27 (<code object post_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 282>)
                518 MAKE_FUNCTION            0
    
-   273         520 PRECALL                  0
+   282         520 PRECALL                  0
                524 CALL                     0
    
-   274         534 STORE_NAME              48 (post_delete_view)
+   283         534 STORE_NAME              48 (post_delete_view)
    
-   289         536 LOAD_CONST              28 (<code object current_shouts, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 289>)
+   298         536 LOAD_CONST              28 (<code object current_shouts, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 298>)
                538 MAKE_FUNCTION            0
                540 STORE_NAME              49 (current_shouts)
    
-   295         542 LOAD_CONST              29 (<code object shout_list_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 295>)
+   304         542 LOAD_CONST              29 (<code object shout_list_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 304>)
                544 MAKE_FUNCTION            0
                546 STORE_NAME              50 (shout_list_view)
    
-   304         548 LOAD_CONST              30 (<code object shout_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 304>)
+   313         548 LOAD_CONST              30 (<code object shout_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 313>)
                550 MAKE_FUNCTION            0
                552 STORE_NAME              51 (shout_create_view)
    
-   327         554 LOAD_CONST              31 (<code object bbcode_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 327>)
+   336         554 LOAD_CONST              31 (<code object bbcode_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 336>)
                556 MAKE_FUNCTION            0
                558 STORE_NAME              52 (bbcode_view)
                560 LOAD_CONST               1 (None)
                562 RETURN_VALUE
    consts
       0
       None
@@ -812,62 +812,66 @@
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000007c007402000000000000000000006a
             020000000000000000a00300000000000000000000000000000000000000
             006401a6010000ab010000000000000000a0040000000000000000000000
-            000000000000000000a6000000ab000000000000000000a6020000ab0200
-            000000000000007d0164027c0169017d02740b000000000000000000007c
-            0064037c02ac04a6030000ab0300000000000000005300
+            0000000000000000006402a6010000ab010000000000000000a6020000ab
+            0200000000000000007d0164037c0169017d02740b000000000000000000
+            007c0064047c02ac05a6030000ab0300000000000000005300
          110           0 RESUME                   0
          
          111           2 LOAD_GLOBAL              1 (NULL + paginate_qs)
-                      14 LOAD_FAST                0 (request)
+         
+         112          14 LOAD_FAST                0 (request)
                       16 LOAD_GLOBAL              2 (User)
                       28 LOAD_ATTR                2 (objects)
                       38 LOAD_METHOD              3 (select_related)
                       60 LOAD_CONST               1 ('profile')
                       62 PRECALL                  1
                       66 CALL                     1
-                      76 LOAD_METHOD              4 (all)
-                      98 PRECALL                  0
-                     102 CALL                     0
-                     112 PRECALL                  2
-                     116 CALL                     2
-                     126 STORE_FAST               1 (users)
-         
-         114         128 LOAD_CONST               2 ('users')
-                     130 LOAD_FAST                1 (users)
-         
-         113         132 BUILD_MAP                1
-                     134 STORE_FAST               2 (context)
-         
-         116         136 LOAD_GLOBAL             11 (NULL + render)
-                     148 LOAD_FAST                0 (request)
-                     150 LOAD_CONST               3 ('punkweb_bb/members.html')
-                     152 LOAD_FAST                2 (context)
-                     154 KW_NAMES                 4
-                     156 PRECALL                  3
-                     160 CALL                     3
-                     170 RETURN_VALUE
+                      76 LOAD_METHOD              4 (order_by)
+                      98 LOAD_CONST               2 ('username')
+                     100 PRECALL                  1
+                     104 CALL                     1
+         
+         111         114 PRECALL                  2
+                     118 CALL                     2
+                     128 STORE_FAST               1 (users)
+         
+         116         130 LOAD_CONST               3 ('users')
+                     132 LOAD_FAST                1 (users)
+         
+         115         134 BUILD_MAP                1
+                     136 STORE_FAST               2 (context)
+         
+         118         138 LOAD_GLOBAL             11 (NULL + render)
+                     150 LOAD_FAST                0 (request)
+                     152 LOAD_CONST               4 ('punkweb_bb/members.html')
+                     154 LOAD_FAST                2 (context)
+                     156 KW_NAMES                 5
+                     158 PRECALL                  3
+                     162 CALL                     3
+                     172 RETURN_VALUE
          consts
             None
             'profile'
+            'username'
             'users'
             'punkweb_bb/members.html'
             ('context',)
-         names      ('paginate_qs', 'User', 'objects', 'select_related', 'all', 'render')
+         names      ('paginate_qs', 'User', 'objects', 'select_related', 'order_by', 'render')
          varnames   ('request', 'users', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'members_view'
          firstlineno 110
-         lnotab 0x02017e0304ff0403
+         lnotab 0x02010c0164ff100504ff0403
       '/login/'
       ('login_url',)
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
@@ -880,82 +884,82 @@
             000000000000000000000000000000a6000000ab00000000000000000001
             007411000000000000000000006403a6010000ab01000000000000000053
             007413000000000000000000007c00640464057c016901ac06a6030000ab
             03000000000000000053007403000000000000000000007c006a04000000
             00000000006a050000000000000000ac02a6010000ab0100000000000000
             007d0164057c0169017d027413000000000000000000007c0064047c02ac
             06a6030000ab0300000000000000005300
-         119           0 RESUME                   0
+         121           0 RESUME                   0
          
-         121           2 LOAD_FAST                0 (request)
+         123           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (method)
                       14 LOAD_CONST               1 ('POST')
                       16 COMPARE_OP               2 (==)
                       22 POP_JUMP_FORWARD_IF_FALSE   113 (to 250)
          
-         122          24 LOAD_GLOBAL              3 (NULL + BoardProfileModelForm)
+         124          24 LOAD_GLOBAL              3 (NULL + BoardProfileModelForm)
          
-         123          36 LOAD_FAST                0 (request)
+         125          36 LOAD_FAST                0 (request)
                       38 LOAD_ATTR                2 (POST)
                       48 LOAD_FAST                0 (request)
                       50 LOAD_ATTR                3 (FILES)
                       60 LOAD_FAST                0 (request)
                       62 LOAD_ATTR                4 (user)
                       72 LOAD_ATTR                5 (profile)
          
-         122          82 KW_NAMES                 2
+         124          82 KW_NAMES                 2
                       84 PRECALL                  3
                       88 CALL                     3
                       98 STORE_FAST               1 (form)
          
-         126         100 LOAD_FAST                1 (form)
+         128         100 LOAD_FAST                1 (form)
                      102 LOAD_METHOD              6 (is_valid)
                      124 PRECALL                  0
                      128 CALL                     0
                      138 POP_JUMP_FORWARD_IF_FALSE    35 (to 210)
          
-         127         140 LOAD_FAST                1 (form)
+         129         140 LOAD_FAST                1 (form)
                      142 LOAD_METHOD              7 (save)
                      164 PRECALL                  0
                      168 CALL                     0
                      178 POP_TOP
          
-         129         180 LOAD_GLOBAL             17 (NULL + redirect)
+         131         180 LOAD_GLOBAL             17 (NULL + redirect)
                      192 LOAD_CONST               3 ('punkweb_bb:settings')
                      194 PRECALL                  1
                      198 CALL                     1
                      208 RETURN_VALUE
          
-         131     >>  210 LOAD_GLOBAL             19 (NULL + render)
+         133     >>  210 LOAD_GLOBAL             19 (NULL + render)
                      222 LOAD_FAST                0 (request)
                      224 LOAD_CONST               4 ('punkweb_bb/settings.html')
                      226 LOAD_CONST               5 ('form')
                      228 LOAD_FAST                1 (form)
                      230 BUILD_MAP                1
                      232 KW_NAMES                 6
                      234 PRECALL                  3
                      238 CALL                     3
                      248 RETURN_VALUE
          
-         133     >>  250 LOAD_GLOBAL              3 (NULL + BoardProfileModelForm)
+         135     >>  250 LOAD_GLOBAL              3 (NULL + BoardProfileModelForm)
                      262 LOAD_FAST                0 (request)
                      264 LOAD_ATTR                4 (user)
                      274 LOAD_ATTR                5 (profile)
                      284 KW_NAMES                 2
                      286 PRECALL                  1
                      290 CALL                     1
                      300 STORE_FAST               1 (form)
          
-         136         302 LOAD_CONST               5 ('form')
+         138         302 LOAD_CONST               5 ('form')
                      304 LOAD_FAST                1 (form)
          
-         135         306 BUILD_MAP                1
+         137         306 BUILD_MAP                1
                      308 STORE_FAST               2 (context)
          
-         139         310 LOAD_GLOBAL             19 (NULL + render)
+         141         310 LOAD_GLOBAL             19 (NULL + render)
                      322 LOAD_FAST                0 (request)
                      324 LOAD_CONST               4 ('punkweb_bb/settings.html')
                      326 LOAD_FAST                2 (context)
                      328 KW_NAMES                 6
                      330 PRECALL                  3
                      334 CALL                     3
                      344 RETURN_VALUE
@@ -969,58 +973,58 @@
             ('context',)
          names      ('method', 'BoardProfileModelForm', 'POST', 'FILES', 'user', 'profile', 'is_valid', 'save', 'redirect', 'render')
          varnames   ('request', 'form', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'settings_view'
-         firstlineno 119
+         firstlineno 121
          lnotab 0x020216010c012eff1204280128021e022802340304ff0404
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 5
          flags     : 3
          code
             0x97007401000000000000000000007402000000000000000000007c01ac
             01a6020000ab0200000000000000007d027405000000000000000000007c
             007c026a030000000000000000a004000000000000000000000000000000
             0000000000a6000000ab000000000000000000a6020000ab020000000000
             0000007d037c027c0364029c027d04740b000000000000000000007c0064
             037c04ac04a6030000ab0300000000000000005300
-         142           0 RESUME                   0
+         144           0 RESUME                   0
          
-         143           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         145           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Subcategory)
                       26 LOAD_FAST                1 (subcategory_slug)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (subcategory)
          
-         145          46 LOAD_GLOBAL              5 (NULL + paginate_qs)
+         147          46 LOAD_GLOBAL              5 (NULL + paginate_qs)
                       58 LOAD_FAST                0 (request)
                       60 LOAD_FAST                2 (subcategory)
                       62 LOAD_ATTR                3 (threads)
                       72 LOAD_METHOD              4 (all)
                       94 PRECALL                  0
                       98 CALL                     0
                      108 PRECALL                  2
                      112 CALL                     2
                      122 STORE_FAST               3 (threads)
          
-         148         124 LOAD_FAST                2 (subcategory)
+         150         124 LOAD_FAST                2 (subcategory)
          
-         149         126 LOAD_FAST                3 (threads)
+         151         126 LOAD_FAST                3 (threads)
          
-         147         128 LOAD_CONST               2 (('subcategory', 'threads'))
+         149         128 LOAD_CONST               2 (('subcategory', 'threads'))
                      130 BUILD_CONST_KEY_MAP      2
                      132 STORE_FAST               4 (context)
          
-         151         134 LOAD_GLOBAL             11 (NULL + render)
+         153         134 LOAD_GLOBAL             11 (NULL + render)
                      146 LOAD_FAST                0 (request)
                      148 LOAD_CONST               3 ('punkweb_bb/subcategory.html')
                      150 LOAD_FAST                4 (context)
                      152 KW_NAMES                 4
                      154 PRECALL                  3
                      158 CALL                     3
                      168 RETURN_VALUE
@@ -1032,15 +1036,15 @@
             ('context',)
          names      ('get_object_or_404', 'Subcategory', 'paginate_qs', 'threads', 'all', 'render')
          varnames   ('request', 'subcategory_slug', 'subcategory', 'threads', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'subcategory_view'
-         firstlineno 142
+         firstlineno 144
          lnotab 0x02012c024e03020102fe0604
       code
          argcount  : 2
          nlocals   : 6
          stacksize : 5
          flags     : 3
          code
@@ -1055,102 +1059,102 @@
             006403ac04a6010000ab0100000000000000007d047c027c045f0b000000
             00000000007c006a0300000000000000007c045f0300000000000000007c
             04a00a0000000000000000000000000000000000000000a6000000ab0000
             000000000000000100740b000000000000000000007c04a6010000ab0100
             0000000000000053006e0e740f00000000000000000000a6000000ab0000
             000000000000007d037c027c0364059c027d057419000000000000000000
             007c0064067c05ac07a6030000ab0300000000000000005300
-         154           0 RESUME                   0
+         156           0 RESUME                   0
          
-         156           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         158           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Subcategory)
                       26 LOAD_FAST                1 (subcategory_slug)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (subcategory)
          
-         158          46 LOAD_FAST                2 (subcategory)
+         160          46 LOAD_FAST                2 (subcategory)
                       48 LOAD_ATTR                2 (staff_post_only)
                       58 POP_JUMP_FORWARD_IF_FALSE    27 (to 114)
                       60 LOAD_FAST                0 (request)
                       62 LOAD_ATTR                3 (user)
                       72 LOAD_ATTR                4 (is_staff)
                       82 POP_JUMP_FORWARD_IF_TRUE    15 (to 114)
          
-         159          84 LOAD_GLOBAL             11 (NULL + redirect)
+         161          84 LOAD_GLOBAL             11 (NULL + redirect)
                       96 LOAD_FAST                2 (subcategory)
                       98 PRECALL                  1
                      102 CALL                     1
                      112 RETURN_VALUE
          
-         161     >>  114 LOAD_FAST                0 (request)
+         163     >>  114 LOAD_FAST                0 (request)
                      116 LOAD_ATTR                6 (method)
                      126 LOAD_CONST               2 ('POST')
                      128 COMPARE_OP               2 (==)
                      134 POP_JUMP_FORWARD_IF_FALSE   117 (to 370)
          
-         162         136 LOAD_GLOBAL             15 (NULL + ThreadModelForm)
+         164         136 LOAD_GLOBAL             15 (NULL + ThreadModelForm)
                      148 LOAD_FAST                0 (request)
                      150 LOAD_ATTR                8 (POST)
                      160 PRECALL                  1
                      164 CALL                     1
                      174 STORE_FAST               3 (form)
          
-         164         176 LOAD_FAST                3 (form)
+         166         176 LOAD_FAST                3 (form)
                      178 LOAD_METHOD              9 (is_valid)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_JUMP_FORWARD_IF_FALSE    76 (to 368)
          
-         165         216 LOAD_FAST                3 (form)
+         167         216 LOAD_FAST                3 (form)
                      218 LOAD_METHOD             10 (save)
                      240 LOAD_CONST               3 (False)
                      242 KW_NAMES                 4
                      244 PRECALL                  1
                      248 CALL                     1
                      258 STORE_FAST               4 (thread)
          
-         166         260 LOAD_FAST                2 (subcategory)
+         168         260 LOAD_FAST                2 (subcategory)
                      262 LOAD_FAST                4 (thread)
                      264 STORE_ATTR              11 (subcategory)
          
-         167         274 LOAD_FAST                0 (request)
+         169         274 LOAD_FAST                0 (request)
                      276 LOAD_ATTR                3 (user)
                      286 LOAD_FAST                4 (thread)
                      288 STORE_ATTR               3 (user)
          
-         168         298 LOAD_FAST                4 (thread)
+         170         298 LOAD_FAST                4 (thread)
                      300 LOAD_METHOD             10 (save)
                      322 PRECALL                  0
                      326 CALL                     0
                      336 POP_TOP
          
-         170         338 LOAD_GLOBAL             11 (NULL + redirect)
+         172         338 LOAD_GLOBAL             11 (NULL + redirect)
                      350 LOAD_FAST                4 (thread)
                      352 PRECALL                  1
                      356 CALL                     1
                      366 RETURN_VALUE
          
-         164     >>  368 JUMP_FORWARD            14 (to 398)
+         166     >>  368 JUMP_FORWARD            14 (to 398)
          
-         172     >>  370 LOAD_GLOBAL             15 (NULL + ThreadModelForm)
+         174     >>  370 LOAD_GLOBAL             15 (NULL + ThreadModelForm)
                      382 PRECALL                  0
                      386 CALL                     0
                      396 STORE_FAST               3 (form)
          
-         175     >>  398 LOAD_FAST                2 (subcategory)
+         177     >>  398 LOAD_FAST                2 (subcategory)
          
-         176         400 LOAD_FAST                3 (form)
+         178         400 LOAD_FAST                3 (form)
          
-         174         402 LOAD_CONST               5 (('subcategory', 'form'))
+         176         402 LOAD_CONST               5 (('subcategory', 'form'))
                      404 BUILD_CONST_KEY_MAP      2
                      406 STORE_FAST               5 (context)
          
-         178         408 LOAD_GLOBAL             25 (NULL + render)
+         180         408 LOAD_GLOBAL             25 (NULL + render)
                      420 LOAD_FAST                0 (request)
                      422 LOAD_CONST               6 ('punkweb_bb/thread_create.html')
                      424 LOAD_FAST                5 (context)
                      426 KW_NAMES                 7
                      428 PRECALL                  3
                      432 CALL                     3
                      442 RETURN_VALUE
@@ -1165,89 +1169,134 @@
             ('context',)
          names      ('get_object_or_404', 'Subcategory', 'staff_post_only', 'user', 'is_staff', 'redirect', 'method', 'ThreadModelForm', 'POST', 'is_valid', 'save', 'subcategory', 'render')
          varnames   ('request', 'subcategory_slug', 'subcategory', 'form', 'thread', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'thread_create_view'
-         firstlineno 154
+         firstlineno 156
          lnotab
             0x02022c0226011e021601280228012c010e01180128021efa02081c0302
             0102fe0604
       code
          argcount  : 2
-         nlocals   : 6
+         nlocals   : 7
          stacksize : 5
          flags     : 3
          code
             0x97007401000000000000000000007402000000000000000000007c01ac
             01a6020000ab0200000000000000007d027405000000000000000000007c
             007c026a030000000000000000a004000000000000000000000000000000
             0000000000a6000000ab000000000000000000a6020000ab020000000000
             0000007d03740b00000000000000000000a6000000ab0000000000000000
-            007d047c027c037c0464029c037d05740d000000000000000000007c0064
-            037c05ac04a6030000ab0300000000000000005300
-         181           0 RESUME                   0
+            007d047c006a060000000000000000a00700000000000000000000000000
+            0000000000000064026700a6020000ab0200000000000000007d057c017c
+            05760172327c0278016a08000000000000000064037a0d000063025f0800
+            000000000000007c02a00900000000000000000000000000000000000000
+            00a6000000ab00000000000000000001007c057c0167017a0000007c006a
+            06000000000000000064023c0000007c027c037c0464049c037d06741500
+            0000000000000000007c0064057c06ac06a6030000ab0300000000000000
+            005300
+         183           0 RESUME                   0
          
-         182           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         184           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Thread)
                       26 LOAD_FAST                1 (thread_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (thread)
          
-         184          46 LOAD_GLOBAL              5 (NULL + paginate_qs)
+         186          46 LOAD_GLOBAL              5 (NULL + paginate_qs)
                       58 LOAD_FAST                0 (request)
                       60 LOAD_FAST                2 (thread)
                       62 LOAD_ATTR                3 (posts)
                       72 LOAD_METHOD              4 (all)
                       94 PRECALL                  0
                       98 CALL                     0
                      108 PRECALL                  2
                      112 CALL                     2
                      122 STORE_FAST               3 (posts)
          
-         186         124 LOAD_GLOBAL             11 (NULL + PostModelForm)
+         188         124 LOAD_GLOBAL             11 (NULL + PostModelForm)
                      136 PRECALL                  0
                      140 CALL                     0
                      150 STORE_FAST               4 (post_form)
          
-         189         152 LOAD_FAST                2 (thread)
-         
-         190         154 LOAD_FAST                3 (posts)
-         
-         191         156 LOAD_FAST                4 (post_form)
-         
-         188         158 LOAD_CONST               2 (('thread', 'posts', 'post_form'))
-                     160 BUILD_CONST_KEY_MAP      3
-                     162 STORE_FAST               5 (context)
-         
-         193         164 LOAD_GLOBAL             13 (NULL + render)
-                     176 LOAD_FAST                0 (request)
-                     178 LOAD_CONST               3 ('punkweb_bb/thread.html')
-                     180 LOAD_FAST                5 (context)
-                     182 KW_NAMES                 4
-                     184 PRECALL                  3
-                     188 CALL                     3
-                     198 RETURN_VALUE
+         191         152 LOAD_FAST                0 (request)
+                     154 LOAD_ATTR                6 (session)
+                     164 LOAD_METHOD              7 (get)
+                     186 LOAD_CONST               2 ('viewed_threads')
+                     188 BUILD_LIST               0
+                     190 PRECALL                  2
+                     194 CALL                     2
+                     204 STORE_FAST               5 (viewed_threads)
+         
+         192         206 LOAD_FAST                1 (thread_id)
+                     208 LOAD_FAST                5 (viewed_threads)
+                     210 CONTAINS_OP              1
+                     212 POP_JUMP_FORWARD_IF_FALSE    50 (to 314)
+         
+         193         214 LOAD_FAST                2 (thread)
+                     216 COPY                     1
+                     218 LOAD_ATTR                8 (view_count)
+                     228 LOAD_CONST               3 (1)
+                     230 BINARY_OP               13 (+=)
+                     234 SWAP                     2
+                     236 STORE_ATTR               8 (view_count)
+         
+         194         246 LOAD_FAST                2 (thread)
+                     248 LOAD_METHOD              9 (save)
+                     270 PRECALL                  0
+                     274 CALL                     0
+                     284 POP_TOP
+         
+         195         286 LOAD_FAST                5 (viewed_threads)
+                     288 LOAD_FAST                1 (thread_id)
+                     290 BUILD_LIST               1
+                     292 BINARY_OP                0 (+)
+                     296 LOAD_FAST                0 (request)
+                     298 LOAD_ATTR                6 (session)
+                     308 LOAD_CONST               2 ('viewed_threads')
+                     310 STORE_SUBSCR
+         
+         198     >>  314 LOAD_FAST                2 (thread)
+         
+         199         316 LOAD_FAST                3 (posts)
+         
+         200         318 LOAD_FAST                4 (post_form)
+         
+         197         320 LOAD_CONST               4 (('thread', 'posts', 'post_form'))
+                     322 BUILD_CONST_KEY_MAP      3
+                     324 STORE_FAST               6 (context)
+         
+         202         326 LOAD_GLOBAL             21 (NULL + render)
+                     338 LOAD_FAST                0 (request)
+                     340 LOAD_CONST               5 ('punkweb_bb/thread.html')
+                     342 LOAD_FAST                6 (context)
+                     344 KW_NAMES                 6
+                     346 PRECALL                  3
+                     350 CALL                     3
+                     360 RETURN_VALUE
          consts
             None
             ('pk',)
+            'viewed_threads'
+            1
             ('thread', 'posts', 'post_form')
             'punkweb_bb/thread.html'
             ('context',)
-         names      ('get_object_or_404', 'Thread', 'paginate_qs', 'posts', 'all', 'PostModelForm', 'render')
-         varnames   ('request', 'thread_id', 'thread', 'posts', 'post_form', 'context')
+         names      ('get_object_or_404', 'Thread', 'paginate_qs', 'posts', 'all', 'PostModelForm', 'session', 'get', 'view_count', 'save', 'render')
+         varnames   ('request', 'thread_id', 'thread', 'posts', 'post_form', 'viewed_threads', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'thread_view'
-         firstlineno 181
-         lnotab 0x02012c024e021c030201020102fd0605
+         firstlineno 183
+         lnotab 0x02012c024e021c0336010801200128011c030201020102fd0605
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 5
          flags     : 3
          code
             0x97007401000000000000000000007402000000000000000000007c017c
@@ -1257,77 +1306,77 @@
             0000007d037c03a0060000000000000000000000000000000000000000a6
             000000ab00000000000000000072237c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007d027411000000
             000000000000007c02a6010000ab01000000000000000053006e10740900
             0000000000000000007c02ac03a6010000ab0100000000000000007d037c
             027c0364049c027d047413000000000000000000007c0064057c04ac06a6
             030000ab0300000000000000005300
-         196           0 RESUME                   0
+         205           0 RESUME                   0
          
-         198           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         207           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Thread)
                       26 LOAD_FAST                1 (thread_id)
                       28 LOAD_FAST                0 (request)
                       30 LOAD_ATTR                2 (user)
                       40 KW_NAMES                 1
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_FAST               2 (thread)
          
-         200          58 LOAD_FAST                0 (request)
+         209          58 LOAD_FAST                0 (request)
                       60 LOAD_ATTR                3 (method)
                       70 LOAD_CONST               2 ('POST')
                       72 COMPARE_OP               2 (==)
                       78 POP_JUMP_FORWARD_IF_FALSE    78 (to 236)
          
-         201          80 LOAD_GLOBAL              9 (NULL + ThreadModelForm)
+         210          80 LOAD_GLOBAL              9 (NULL + ThreadModelForm)
                       92 LOAD_FAST                0 (request)
                       94 LOAD_ATTR                5 (POST)
                      104 LOAD_FAST                2 (thread)
                      106 KW_NAMES                 3
                      108 PRECALL                  2
                      112 CALL                     2
                      122 STORE_FAST               3 (form)
          
-         203         124 LOAD_FAST                3 (form)
+         212         124 LOAD_FAST                3 (form)
                      126 LOAD_METHOD              6 (is_valid)
                      148 PRECALL                  0
                      152 CALL                     0
                      162 POP_JUMP_FORWARD_IF_FALSE    35 (to 234)
          
-         204         164 LOAD_FAST                3 (form)
+         213         164 LOAD_FAST                3 (form)
                      166 LOAD_METHOD              7 (save)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 STORE_FAST               2 (thread)
          
-         206         204 LOAD_GLOBAL             17 (NULL + redirect)
+         215         204 LOAD_GLOBAL             17 (NULL + redirect)
                      216 LOAD_FAST                2 (thread)
                      218 PRECALL                  1
                      222 CALL                     1
                      232 RETURN_VALUE
          
-         203     >>  234 JUMP_FORWARD            16 (to 268)
+         212     >>  234 JUMP_FORWARD            16 (to 268)
          
-         208     >>  236 LOAD_GLOBAL              9 (NULL + ThreadModelForm)
+         217     >>  236 LOAD_GLOBAL              9 (NULL + ThreadModelForm)
                      248 LOAD_FAST                2 (thread)
                      250 KW_NAMES                 3
                      252 PRECALL                  1
                      256 CALL                     1
                      266 STORE_FAST               3 (form)
          
-         211     >>  268 LOAD_FAST                2 (thread)
+         220     >>  268 LOAD_FAST                2 (thread)
          
-         212         270 LOAD_FAST                3 (form)
+         221         270 LOAD_FAST                3 (form)
          
-         210         272 LOAD_CONST               4 (('thread', 'form'))
+         219         272 LOAD_CONST               4 (('thread', 'form'))
                      274 BUILD_CONST_KEY_MAP      2
                      276 STORE_FAST               4 (context)
          
-         214         278 LOAD_GLOBAL             19 (NULL + render)
+         223         278 LOAD_GLOBAL             19 (NULL + render)
                      290 LOAD_FAST                0 (request)
                      292 LOAD_CONST               5 ('punkweb_bb/thread_update.html')
                      294 LOAD_FAST                4 (context)
                      296 KW_NAMES                 6
                      298 PRECALL                  3
                      302 CALL                     3
                      312 RETURN_VALUE
@@ -1341,15 +1390,15 @@
             ('context',)
          names      ('get_object_or_404', 'Thread', 'user', 'method', 'ThreadModelForm', 'POST', 'is_valid', 'save', 'redirect', 'render')
          varnames   ('request', 'thread_id', 'thread', 'form', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'thread_update_view'
-         firstlineno 196
+         firstlineno 205
          lnotab 0x0202380216012c02280128021efd02052003020102fe0604
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 5
          flags     : 3
          code
@@ -1358,55 +1407,55 @@
             006a03000000000000000064026b0200000000723a7c02a0040000000000
             000000000000000000000000000000a6000000ab00000000000000000001
             00740b000000000000000000007c026a060000000000000000a007000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00a6010000ab010000000000000000530064037c0269017d037411000000
             000000000000007c0064047c03ac05a6030000ab03000000000000000053
             00
-         217           0 RESUME                   0
+         226           0 RESUME                   0
          
-         219           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         228           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Thread)
                       26 LOAD_FAST                1 (thread_id)
                       28 LOAD_FAST                0 (request)
                       30 LOAD_ATTR                2 (user)
                       40 KW_NAMES                 1
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_FAST               2 (thread)
          
-         221          58 LOAD_FAST                0 (request)
+         230          58 LOAD_FAST                0 (request)
                       60 LOAD_ATTR                3 (method)
                       70 LOAD_CONST               2 ('DELETE')
                       72 COMPARE_OP               2 (==)
                       78 POP_JUMP_FORWARD_IF_FALSE    58 (to 196)
          
-         222          80 LOAD_FAST                2 (thread)
+         231          80 LOAD_FAST                2 (thread)
                       82 LOAD_METHOD              4 (delete)
                      104 PRECALL                  0
                      108 CALL                     0
                      118 POP_TOP
          
-         224         120 LOAD_GLOBAL             11 (NULL + htmx_redirect)
+         233         120 LOAD_GLOBAL             11 (NULL + htmx_redirect)
                      132 LOAD_FAST                2 (thread)
                      134 LOAD_ATTR                6 (subcategory)
                      144 LOAD_METHOD              7 (get_absolute_url)
                      166 PRECALL                  0
                      170 CALL                     0
                      180 PRECALL                  1
                      184 CALL                     1
                      194 RETURN_VALUE
          
-         227     >>  196 LOAD_CONST               3 ('thread')
+         236     >>  196 LOAD_CONST               3 ('thread')
                      198 LOAD_FAST                2 (thread)
          
-         226         200 BUILD_MAP                1
+         235         200 BUILD_MAP                1
                      202 STORE_FAST               3 (context)
          
-         230         204 LOAD_GLOBAL             17 (NULL + render)
+         239         204 LOAD_GLOBAL             17 (NULL + render)
                      216 LOAD_FAST                0 (request)
                      218 LOAD_CONST               4 ('punkweb_bb/partials/thread_delete.html')
                      220 LOAD_FAST                3 (context)
                      222 KW_NAMES                 5
                      224 PRECALL                  3
                      228 CALL                     3
                      238 RETURN_VALUE
@@ -1419,15 +1468,15 @@
             ('context',)
          names      ('get_object_or_404', 'Thread', 'user', 'method', 'delete', 'htmx_redirect', 'subcategory', 'get_absolute_url', 'render')
          varnames   ('request', 'thread_id', 'thread', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'thread_delete_view'
-         firstlineno 217
+         firstlineno 226
          lnotab 0x02023802160128024c0304ff0404
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 4
          flags     : 3
          code
@@ -1438,91 +1487,91 @@
             0100000000000000007d037c03a006000000000000000000000000000000
             0000000000a6000000ab000000000000000000724c7c03a0070000000000
             0000000000000000000000000000006403ac04a6010000ab010000000000
             0000007d047c027c045f0800000000000000007c006a0900000000000000
             007c045f0900000000000000007c04a00700000000000000000000000000
             00000000000000a6000000ab000000000000000000010074150000000000
             00000000007c04a6010000ab010000000000000000530064005300
-         233           0 RESUME                   0
+         242           0 RESUME                   0
          
-         235           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         244           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Thread)
                       26 LOAD_FAST                1 (thread_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (thread)
          
-         237          46 LOAD_FAST                2 (thread)
+         246          46 LOAD_FAST                2 (thread)
                       48 LOAD_ATTR                2 (is_closed)
                       58 POP_JUMP_FORWARD_IF_FALSE    15 (to 90)
          
-         238          60 LOAD_GLOBAL              7 (NULL + HttpResponseForbidden)
-                      72 LOAD_CONST               2 ('This thread is closed.')
+         247          60 LOAD_GLOBAL              7 (NULL + HttpResponseForbidden)
+                      72 LOAD_CONST               2 ('Cannot add posts to a closed thread.')
                       74 PRECALL                  1
                       78 CALL                     1
                       88 RETURN_VALUE
          
-         240     >>   90 LOAD_GLOBAL              9 (NULL + PostModelForm)
+         249     >>   90 LOAD_GLOBAL              9 (NULL + PostModelForm)
                      102 LOAD_FAST                0 (request)
                      104 LOAD_ATTR                5 (POST)
                      114 PRECALL                  1
                      118 CALL                     1
                      128 STORE_FAST               3 (form)
          
-         242         130 LOAD_FAST                3 (form)
+         251         130 LOAD_FAST                3 (form)
                      132 LOAD_METHOD              6 (is_valid)
                      154 PRECALL                  0
                      158 CALL                     0
                      168 POP_JUMP_FORWARD_IF_FALSE    76 (to 322)
          
-         243         170 LOAD_FAST                3 (form)
+         252         170 LOAD_FAST                3 (form)
                      172 LOAD_METHOD              7 (save)
                      194 LOAD_CONST               3 (False)
                      196 KW_NAMES                 4
                      198 PRECALL                  1
                      202 CALL                     1
                      212 STORE_FAST               4 (post)
          
-         244         214 LOAD_FAST                2 (thread)
+         253         214 LOAD_FAST                2 (thread)
                      216 LOAD_FAST                4 (post)
                      218 STORE_ATTR               8 (thread)
          
-         245         228 LOAD_FAST                0 (request)
+         254         228 LOAD_FAST                0 (request)
                      230 LOAD_ATTR                9 (user)
                      240 LOAD_FAST                4 (post)
                      242 STORE_ATTR               9 (user)
          
-         246         252 LOAD_FAST                4 (post)
+         255         252 LOAD_FAST                4 (post)
                      254 LOAD_METHOD              7 (save)
                      276 PRECALL                  0
                      280 CALL                     0
                      290 POP_TOP
          
-         248         292 LOAD_GLOBAL             21 (NULL + redirect)
+         257         292 LOAD_GLOBAL             21 (NULL + redirect)
                      304 LOAD_FAST                4 (post)
                      306 PRECALL                  1
                      310 CALL                     1
                      320 RETURN_VALUE
          
-         242     >>  322 LOAD_CONST               0 (None)
+         251     >>  322 LOAD_CONST               0 (None)
                      324 RETURN_VALUE
          consts
             None
             ('pk',)
-            'This thread is closed.'
+            'Cannot add posts to a closed thread.'
             False
             ('commit',)
          names      ('get_object_or_404', 'Thread', 'is_closed', 'HttpResponseForbidden', 'PostModelForm', 'POST', 'is_valid', 'save', 'thread', 'user', 'redirect')
          varnames   ('request', 'thread_id', 'thread', 'form', 'post')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'post_create_view'
-         firstlineno 233
+         firstlineno 242
          lnotab 0x02022c020e011e02280228012c010e01180128021efa
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 5
          flags     : 3
          code
@@ -1533,75 +1582,75 @@
             0000007d037c03a0060000000000000000000000000000000000000000a6
             000000ab00000000000000000072237c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007d027411000000
             000000000000007c02a6010000ab01000000000000000053007409000000
             000000000000007c02ac03a6010000ab0100000000000000007d037c027c
             0364049c027d047413000000000000000000007c0064057c04ac06a60300
             00ab0300000000000000005300
-         251           0 RESUME                   0
+         260           0 RESUME                   0
          
-         253           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         262           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Post)
                       26 LOAD_FAST                1 (post_id)
                       28 LOAD_FAST                0 (request)
                       30 LOAD_ATTR                2 (user)
                       40 KW_NAMES                 1
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_FAST               2 (post)
          
-         255          58 LOAD_FAST                0 (request)
+         264          58 LOAD_FAST                0 (request)
                       60 LOAD_ATTR                3 (method)
                       70 LOAD_CONST               2 ('POST')
                       72 COMPARE_OP               2 (==)
                       78 POP_JUMP_FORWARD_IF_FALSE    77 (to 234)
          
-         256          80 LOAD_GLOBAL              9 (NULL + PostModelForm)
+         265          80 LOAD_GLOBAL              9 (NULL + PostModelForm)
                       92 LOAD_FAST                0 (request)
                       94 LOAD_ATTR                5 (POST)
                      104 LOAD_FAST                2 (post)
                      106 KW_NAMES                 3
                      108 PRECALL                  2
                      112 CALL                     2
                      122 STORE_FAST               3 (form)
          
-         258         124 LOAD_FAST                3 (form)
+         267         124 LOAD_FAST                3 (form)
                      126 LOAD_METHOD              6 (is_valid)
                      148 PRECALL                  0
                      152 CALL                     0
                      162 POP_JUMP_FORWARD_IF_FALSE    35 (to 234)
          
-         259         164 LOAD_FAST                3 (form)
+         268         164 LOAD_FAST                3 (form)
                      166 LOAD_METHOD              7 (save)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 STORE_FAST               2 (post)
          
-         261         204 LOAD_GLOBAL             17 (NULL + redirect)
+         270         204 LOAD_GLOBAL             17 (NULL + redirect)
                      216 LOAD_FAST                2 (post)
                      218 PRECALL                  1
                      222 CALL                     1
                      232 RETURN_VALUE
          
-         263     >>  234 LOAD_GLOBAL              9 (NULL + PostModelForm)
+         272     >>  234 LOAD_GLOBAL              9 (NULL + PostModelForm)
                      246 LOAD_FAST                2 (post)
                      248 KW_NAMES                 3
                      250 PRECALL                  1
                      254 CALL                     1
                      264 STORE_FAST               3 (form)
          
-         266         266 LOAD_FAST                2 (post)
+         275         266 LOAD_FAST                2 (post)
          
-         267         268 LOAD_FAST                3 (form)
+         276         268 LOAD_FAST                3 (form)
          
-         265         270 LOAD_CONST               4 (('post', 'form'))
+         274         270 LOAD_CONST               4 (('post', 'form'))
                      272 BUILD_CONST_KEY_MAP      2
                      274 STORE_FAST               4 (context)
          
-         270         276 LOAD_GLOBAL             19 (NULL + render)
+         279         276 LOAD_GLOBAL             19 (NULL + render)
                      288 LOAD_FAST                0 (request)
                      290 LOAD_CONST               5 ('punkweb_bb/partials/post_update.html')
                      292 LOAD_FAST                4 (context)
                      294 KW_NAMES                 6
                      296 PRECALL                  3
                      300 CALL                     3
                      310 RETURN_VALUE
@@ -1615,15 +1664,15 @@
             ('context',)
          names      ('get_object_or_404', 'Post', 'user', 'method', 'PostModelForm', 'POST', 'is_valid', 'save', 'redirect', 'render')
          varnames   ('request', 'post_id', 'post', 'form', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'post_update_view'
-         firstlineno 251
+         firstlineno 260
          lnotab 0x0202380216012c02280128021e022003020102fe0605
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 5
          flags     : 3
          code
@@ -1632,55 +1681,55 @@
             006a03000000000000000064026b0200000000723a7c02a0040000000000
             000000000000000000000000000000a6000000ab00000000000000000001
             00740b000000000000000000007c026a060000000000000000a007000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00a6010000ab010000000000000000530064037c0269017d037411000000
             000000000000007c0064047c03ac05a6030000ab03000000000000000053
             00
-         273           0 RESUME                   0
+         282           0 RESUME                   0
          
-         275           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         284           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Post)
                       26 LOAD_FAST                1 (post_id)
                       28 LOAD_FAST                0 (request)
                       30 LOAD_ATTR                2 (user)
                       40 KW_NAMES                 1
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_FAST               2 (post)
          
-         277          58 LOAD_FAST                0 (request)
+         286          58 LOAD_FAST                0 (request)
                       60 LOAD_ATTR                3 (method)
                       70 LOAD_CONST               2 ('DELETE')
                       72 COMPARE_OP               2 (==)
                       78 POP_JUMP_FORWARD_IF_FALSE    58 (to 196)
          
-         278          80 LOAD_FAST                2 (post)
+         287          80 LOAD_FAST                2 (post)
                       82 LOAD_METHOD              4 (delete)
                      104 PRECALL                  0
                      108 CALL                     0
                      118 POP_TOP
          
-         280         120 LOAD_GLOBAL             11 (NULL + htmx_redirect)
+         289         120 LOAD_GLOBAL             11 (NULL + htmx_redirect)
                      132 LOAD_FAST                2 (post)
                      134 LOAD_ATTR                6 (thread)
                      144 LOAD_METHOD              7 (get_absolute_url)
                      166 PRECALL                  0
                      170 CALL                     0
                      180 PRECALL                  1
                      184 CALL                     1
                      194 RETURN_VALUE
          
-         283     >>  196 LOAD_CONST               3 ('post')
+         292     >>  196 LOAD_CONST               3 ('post')
                      198 LOAD_FAST                2 (post)
          
-         282         200 BUILD_MAP                1
+         291         200 BUILD_MAP                1
                      202 STORE_FAST               3 (context)
          
-         286         204 LOAD_GLOBAL             17 (NULL + render)
+         295         204 LOAD_GLOBAL             17 (NULL + render)
                      216 LOAD_FAST                0 (request)
                      218 LOAD_CONST               4 ('punkweb_bb/partials/post_delete.html')
                      220 LOAD_FAST                3 (context)
                      222 KW_NAMES                 5
                      224 PRECALL                  3
                      228 CALL                     3
                      238 RETURN_VALUE
@@ -1693,94 +1742,94 @@
             ('context',)
          names      ('get_object_or_404', 'Post', 'user', 'method', 'delete', 'htmx_redirect', 'thread', 'get_absolute_url', 'render')
          varnames   ('request', 'post_id', 'post', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'post_delete_view'
-         firstlineno 273
+         firstlineno 282
          lnotab 0x02023802160128024c0304ff0404
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000007407000000000000000000006a
             040000000000000000a6000000ab000000000000000000740b0000000000
             00000000006a0600000000000000006401ac02a6010000ab010000000000
             0000007a0a0000ac03a6010000ab010000000000000000a0070000000000
             0000000000000000000000000000006404a6010000ab0100000000000000
             005300
-         289           0 RESUME                   0
+         298           0 RESUME                   0
          
-         290           2 LOAD_GLOBAL              0 (Shout)
+         299           2 LOAD_GLOBAL              0 (Shout)
                       14 LOAD_ATTR                1 (objects)
                       24 LOAD_METHOD              2 (filter)
          
-         291          46 LOAD_GLOBAL              7 (NULL + timezone)
+         300          46 LOAD_GLOBAL              7 (NULL + timezone)
                       58 LOAD_ATTR                4 (now)
                       68 PRECALL                  0
                       72 CALL                     0
                       82 LOAD_GLOBAL             11 (NULL + datetime)
                       94 LOAD_ATTR                6 (timedelta)
                      104 LOAD_CONST               1 (12)
                      106 KW_NAMES                 2
                      108 PRECALL                  1
                      112 CALL                     1
                      122 BINARY_OP               10 (-)
          
-         290         126 KW_NAMES                 3
+         299         126 KW_NAMES                 3
                      128 PRECALL                  1
                      132 CALL                     1
          
-         292         142 LOAD_METHOD              7 (order_by)
+         301         142 LOAD_METHOD              7 (order_by)
                      164 LOAD_CONST               4 ('created_at')
                      166 PRECALL                  1
                      170 CALL                     1
          
-         290         180 RETURN_VALUE
+         299         180 RETURN_VALUE
          consts
             None
             12
             ('hours',)
             ('created_at__gt',)
             'created_at'
          names      ('Shout', 'objects', 'filter', 'timezone', 'now', 'datetime', 'timedelta', 'order_by')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'current_shouts'
-         firstlineno 289
+         firstlineno 298
          lnotab 0x02012c0150ff100226fe
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 5
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab0000000000000000007d
             0164017c0169017d027403000000000000000000007c0064027c02ac03a6
             030000ab0300000000000000005300
-         295           0 RESUME                   0
+         304           0 RESUME                   0
          
-         296           2 LOAD_GLOBAL              1 (NULL + current_shouts)
+         305           2 LOAD_GLOBAL              1 (NULL + current_shouts)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 STORE_FAST               1 (shouts)
          
-         299          30 LOAD_CONST               1 ('shouts')
+         308          30 LOAD_CONST               1 ('shouts')
                       32 LOAD_FAST                1 (shouts)
          
-         298          34 BUILD_MAP                1
+         307          34 BUILD_MAP                1
                       36 STORE_FAST               2 (context)
          
-         301          38 LOAD_GLOBAL              3 (NULL + render)
+         310          38 LOAD_GLOBAL              3 (NULL + render)
                       50 LOAD_FAST                0 (request)
                       52 LOAD_CONST               2 ('punkweb_bb/shoutbox/shout_list.html')
                       54 LOAD_FAST                2 (context)
                       56 KW_NAMES                 3
                       58 PRECALL                  3
                       62 CALL                     3
                       72 RETURN_VALUE
@@ -1791,15 +1840,15 @@
             ('context',)
          names      ('current_shouts', 'render')
          varnames   ('request', 'shouts', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'shout_list_view'
-         firstlineno 295
+         firstlineno 304
          lnotab 0x02011c0304ff0403
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 5
          flags     : 3
          code
@@ -1812,99 +1861,99 @@
             00a6000000ab000000000000000000725a7c02a008000000000000000000
             00000000000000000000006405ac06a6010000ab0100000000000000007d
             037c006a0000000000000000007c035f0000000000000000007c03a00800
             00000000000000000000000000000000000000a6000000ab000000000000
             00000001006401740500000000000000000000a6000000ab000000000000
             00000069017d017407000000000000000000007c0064027c01ac03a60300
             00ab03000000000000000053006400530064005300
-         304           0 RESUME                   0
+         313           0 RESUME                   0
          
-         305           2 LOAD_FAST                0 (request)
+         314           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (user)
                       14 LOAD_ATTR                1 (is_authenticated)
                       24 POP_JUMP_FORWARD_IF_TRUE    34 (to 94)
          
-         307          26 LOAD_CONST               1 ('shouts')
+         316          26 LOAD_CONST               1 ('shouts')
                       28 LOAD_GLOBAL              5 (NULL + current_shouts)
                       40 PRECALL                  0
                       44 CALL                     0
          
-         306          54 BUILD_MAP                1
+         315          54 BUILD_MAP                1
                       56 STORE_FAST               1 (context)
          
-         309          58 LOAD_GLOBAL              7 (NULL + render)
+         318          58 LOAD_GLOBAL              7 (NULL + render)
                       70 LOAD_FAST                0 (request)
                       72 LOAD_CONST               2 ('punkweb_bb/shoutbox/shout_list.html')
                       74 LOAD_FAST                1 (context)
                       76 KW_NAMES                 3
                       78 PRECALL                  3
                       82 CALL                     3
                       92 RETURN_VALUE
          
-         311     >>   94 LOAD_FAST                0 (request)
+         320     >>   94 LOAD_FAST                0 (request)
                       96 LOAD_ATTR                4 (method)
                      106 LOAD_CONST               4 ('POST')
                      108 COMPARE_OP               2 (==)
                      114 POP_JUMP_FORWARD_IF_FALSE   128 (to 372)
          
-         312         116 LOAD_GLOBAL             11 (NULL + ShoutModelForm)
+         321         116 LOAD_GLOBAL             11 (NULL + ShoutModelForm)
                      128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                6 (POST)
                      140 PRECALL                  1
                      144 CALL                     1
                      154 STORE_FAST               2 (form)
          
-         314         156 LOAD_FAST                2 (form)
+         323         156 LOAD_FAST                2 (form)
                      158 LOAD_METHOD              7 (is_valid)
                      180 PRECALL                  0
                      184 CALL                     0
                      194 POP_JUMP_FORWARD_IF_FALSE    90 (to 376)
          
-         315         196 LOAD_FAST                2 (form)
+         324         196 LOAD_FAST                2 (form)
                      198 LOAD_METHOD              8 (save)
                      220 LOAD_CONST               5 (False)
                      222 KW_NAMES                 6
                      224 PRECALL                  1
                      228 CALL                     1
                      238 STORE_FAST               3 (shout)
          
-         316         240 LOAD_FAST                0 (request)
+         325         240 LOAD_FAST                0 (request)
                      242 LOAD_ATTR                0 (user)
                      252 LOAD_FAST                3 (shout)
                      254 STORE_ATTR               0 (user)
          
-         317         264 LOAD_FAST                3 (shout)
+         326         264 LOAD_FAST                3 (shout)
                      266 LOAD_METHOD              8 (save)
                      288 PRECALL                  0
                      292 CALL                     0
                      302 POP_TOP
          
-         320         304 LOAD_CONST               1 ('shouts')
+         329         304 LOAD_CONST               1 ('shouts')
                      306 LOAD_GLOBAL              5 (NULL + current_shouts)
                      318 PRECALL                  0
                      322 CALL                     0
          
-         319         332 BUILD_MAP                1
+         328         332 BUILD_MAP                1
                      334 STORE_FAST               1 (context)
          
-         322         336 LOAD_GLOBAL              7 (NULL + render)
+         331         336 LOAD_GLOBAL              7 (NULL + render)
          
-         323         348 LOAD_FAST                0 (request)
+         332         348 LOAD_FAST                0 (request)
                      350 LOAD_CONST               2 ('punkweb_bb/shoutbox/shout_list.html')
                      352 LOAD_FAST                1 (context)
          
-         322         354 KW_NAMES                 3
+         331         354 KW_NAMES                 3
                      356 PRECALL                  3
                      360 CALL                     3
                      370 RETURN_VALUE
          
-         311     >>  372 LOAD_CONST               0 (None)
+         320     >>  372 LOAD_CONST               0 (None)
                      374 RETURN_VALUE
          
-         314     >>  376 LOAD_CONST               0 (None)
+         323     >>  376 LOAD_CONST               0 (None)
                      378 RETURN_VALUE
          consts
             None
             'shouts'
             'punkweb_bb/shoutbox/shout_list.html'
             ('context',)
             'POST'
@@ -1912,64 +1961,64 @@
             ('commit',)
          names      ('user', 'is_authenticated', 'current_shouts', 'render', 'method', 'ShoutModelForm', 'POST', 'is_valid', 'save')
          varnames   ('request', 'context', 'form', 'shout')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'shout_create_view'
-         firstlineno 304
+         firstlineno 313
          lnotab
             0x020118021cff040324021601280228012c01180128031cff04030c0106
             ff12f50403
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 5
          flags     : 3
          code
             0x970064017d0164027c0169017d027401000000000000000000007c0064
             037c02ac04a6030000ab0300000000000000005300
-         327           0 RESUME                   0
+         336           0 RESUME                   0
          
-         328           2 LOAD_CONST               1 ((('Bold', '[b]Bold Text[/b]'), ('Italic', '[i]Italic Text[/i]'), ('Underline', '[u]Underlined Text[/u]'), ('Strikethrough', '[s]Strikethrough Text[/s]'), ('Quote', '[quote=Example]Quoted Text[/quote]'), ('Center', '[center]Centered Text[/center]'), ('Color', '[color=red]Red Text[/color]'), ('Url', '[url=https://google.com]Link Text[/url]'), ('Image', '[img]https://punkweb.net/media/music/artists/system-lynx_EklOGpj.png.200x200_q85_crop.png[/img]'), ('Horizontal Rule', '[hr]'), ('Code', '\n[code=python]\nclass ThreadModelForm(forms.ModelForm):\n    class Meta:\n        model = Thread\n        fields = (\n            "title",\n            "content",\n        )\n        widgets = {\n            "title": forms.TextInput(attrs={"autofocus": True, "class": "pw-input"}),\n            "content": BBCodeEditorWidget(),\n        }\n[/code]\n'), ('Email', '[email=test@example.com]Example[/email]'), ('Font', '[font=serif]Serif Text[/font]'), ('Ordered List', '[ol][li]Item 1[/li][li]Item 2[/li][/ol]'), ('Unordered List', '[ul][li]Item 1[/li][li]Item 2[/li][/ul]'), ('Shadow', '[shadow=red]Red Shadow Text[/shadow]'), ('Size', '[size=7]Size 7 Text[/size]'), ('Checkbox', '\n[n]Unchecked\n[y]Checked\n            '), ('Superscript', 'Sup [sup]Superscript Text[/sup]'), ('Subscript', 'Sub [sub]Subscript Text[/sub]'), ('Left', '[left]Left Text[/left]'), ('Right', '[right]Right Text[/right]'), ('Escape', '[escape][b]Escaped bbcode[/b][/escape]')))
+         337           2 LOAD_CONST               1 ((('Bold', '[b]Bold Text[/b]'), ('Italic', '[i]Italic Text[/i]'), ('Underline', '[u]Underlined Text[/u]'), ('Strikethrough', '[s]Strikethrough Text[/s]'), ('Quote', '[quote=Example]Quoted Text[/quote]'), ('Center', '[center]Centered Text[/center]'), ('Color', '[color=red]Red Text[/color]'), ('Url', '[url=https://google.com]Link Text[/url]'), ('Image', '[img]https://placehold.co/400[/img]'), ('Horizontal Rule', '[hr]'), ('Code', '\n[code=python]\nclass ThreadModelForm(forms.ModelForm):\n    class Meta:\n        model = Thread\n        fields = (\n            "title",\n            "content",\n        )\n        widgets = {\n            "title": forms.TextInput(attrs={"autofocus": True, "class": "pw-input"}),\n            "content": BBCodeEditorWidget(),\n        }\n[/code]\n'), ('Email', '[email=test@example.com]Example[/email]'), ('Font', '[font=serif]Serif Text[/font]'), ('Ordered List', '[ol][li]Item 1[/li][li]Item 2[/li][/ol]'), ('Unordered List', '[ul][li]Item 1[/li][li]Item 2[/li][/ul]'), ('Shadow', '[shadow=red]Red Shadow Text[/shadow]'), ('Size', '[size=7]Size 7 Text[/size]'), ('Checkbox', '\n[n]Unchecked\n[y]Checked\n            '), ('Superscript', 'Sup [sup]Superscript Text[/sup]'), ('Subscript', 'Sub [sub]Subscript Text[/sub]'), ('Left', '[left]Left Text[/left]'), ('Right', '[right]Right Text[/right]'), ('Escape', '[escape][b]Escaped bbcode[/b][/escape]')))
                        4 STORE_FAST               1 (codes)
          
-         382           6 LOAD_CONST               2 ('codes')
+         391           6 LOAD_CONST               2 ('codes')
                        8 LOAD_FAST                1 (codes)
          
-         381          10 BUILD_MAP                1
+         390          10 BUILD_MAP                1
                       12 STORE_FAST               2 (context)
          
-         385          14 LOAD_GLOBAL              1 (NULL + render)
+         394          14 LOAD_GLOBAL              1 (NULL + render)
                       26 LOAD_FAST                0 (request)
                       28 LOAD_CONST               3 ('punkweb_bb/bbcode.html')
                       30 LOAD_FAST                2 (context)
                       32 KW_NAMES                 4
                       34 PRECALL                  3
                       38 CALL                     3
                       48 RETURN_VALUE
          consts
             None
-            (('Bold', '[b]Bold Text[/b]'), ('Italic', '[i]Italic Text[/i]'), ('Underline', '[u]Underlined Text[/u]'), ('Strikethrough', '[s]Strikethrough Text[/s]'), ('Quote', '[quote=Example]Quoted Text[/quote]'), ('Center', '[center]Centered Text[/center]'), ('Color', '[color=red]Red Text[/color]'), ('Url', '[url=https://google.com]Link Text[/url]'), ('Image', '[img]https://punkweb.net/media/music/artists/system-lynx_EklOGpj.png.200x200_q85_crop.png[/img]'), ('Horizontal Rule', '[hr]'), ('Code', '\n[code=python]\nclass ThreadModelForm(forms.ModelForm):\n    class Meta:\n        model = Thread\n        fields = (\n            "title",\n            "content",\n        )\n        widgets = {\n            "title": forms.TextInput(attrs={"autofocus": True, "class": "pw-input"}),\n            "content": BBCodeEditorWidget(),\n        }\n[/code]\n'), ('Email', '[email=test@example.com]Example[/email]'), ('Font', '[font=serif]Serif Text[/font]'), ('Ordered List', '[ol][li]Item 1[/li][li]Item 2[/li][/ol]'), ('Unordered List', '[ul][li]Item 1[/li][li]Item 2[/li][/ul]'), ('Shadow', '[shadow=red]Red Shadow Text[/shadow]'), ('Size', '[size=7]Size 7 Text[/size]'), ('Checkbox', '\n[n]Unchecked\n[y]Checked\n            '), ('Superscript', 'Sup [sup]Superscript Text[/sup]'), ('Subscript', 'Sub [sub]Subscript Text[/sub]'), ('Left', '[left]Left Text[/left]'), ('Right', '[right]Right Text[/right]'), ('Escape', '[escape][b]Escaped bbcode[/b][/escape]'))
+            (('Bold', '[b]Bold Text[/b]'), ('Italic', '[i]Italic Text[/i]'), ('Underline', '[u]Underlined Text[/u]'), ('Strikethrough', '[s]Strikethrough Text[/s]'), ('Quote', '[quote=Example]Quoted Text[/quote]'), ('Center', '[center]Centered Text[/center]'), ('Color', '[color=red]Red Text[/color]'), ('Url', '[url=https://google.com]Link Text[/url]'), ('Image', '[img]https://placehold.co/400[/img]'), ('Horizontal Rule', '[hr]'), ('Code', '\n[code=python]\nclass ThreadModelForm(forms.ModelForm):\n    class Meta:\n        model = Thread\n        fields = (\n            "title",\n            "content",\n        )\n        widgets = {\n            "title": forms.TextInput(attrs={"autofocus": True, "class": "pw-input"}),\n            "content": BBCodeEditorWidget(),\n        }\n[/code]\n'), ('Email', '[email=test@example.com]Example[/email]'), ('Font', '[font=serif]Serif Text[/font]'), ('Ordered List', '[ol][li]Item 1[/li][li]Item 2[/li][/ol]'), ('Unordered List', '[ul][li]Item 1[/li][li]Item 2[/li][/ul]'), ('Shadow', '[shadow=red]Red Shadow Text[/shadow]'), ('Size', '[size=7]Size 7 Text[/size]'), ('Checkbox', '\n[n]Unchecked\n[y]Checked\n            '), ('Superscript', 'Sup [sup]Superscript Text[/sup]'), ('Subscript', 'Sub [sub]Subscript Text[/sub]'), ('Left', '[left]Left Text[/left]'), ('Right', '[right]Right Text[/right]'), ('Escape', '[escape][b]Escaped bbcode[/b][/escape]'))
             'codes'
             'punkweb_bb/bbcode.html'
             ('context',)
          names      ('render',)
          varnames   ('request', 'codes', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'bbcode_view'
-         firstlineno 327
+         firstlineno 336
          lnotab 0x0201043604ff0404
    names      ('datetime', 'django.contrib.auth', 'authenticate', 'get_user_model', 'login', 'logout', 'django.contrib.auth.decorators', 'login_required', 'django.http', 'HttpResponseForbidden', 'django.shortcuts', 'get_object_or_404', 'redirect', 'render', 'django.utils', 'timezone', 'punkweb_bb.forms', 'BoardProfileModelForm', 'LoginForm', 'PostModelForm', 'ShoutModelForm', 'SignUpForm', 'ThreadModelForm', 'punkweb_bb.models', 'Category', 'Post', 'Shout', 'Subcategory', 'Thread', 'punkweb_bb.pagination', 'paginate_qs', 'punkweb_bb.response', 'htmx_redirect', 'User', 'index_view', 'login_view', 'logout_view', 'signup_view', 'profile_view', 'members_view', 'settings_view', 'subcategory_view', 'thread_create_view', 'thread_view', 'thread_update_view', 'thread_delete_view', 'post_create_view', 'post_update_view', 'post_delete_view', 'current_shouts', 'shout_list_view', 'shout_create_view', 'bbcode_view')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201080218010c010c0114010c0220081c010c010c021403061a06
-      1a0605061406090609160104ff0e010216060c160104ff0e01021a060f16
+      1a060506140609060b160104ff0e010216060c160104ff0e01021a061616
       0104ff0e010214160104ff0e01020f160104ff0e010211160104ff0e0102
       15160104ff0e01020f060606090617
```

### Comparing `punkweb_bb-0.1.2/punkweb_bb/__pycache__/widgets.cpython-311.pyc` & `punkweb_bb-0.1.3/punkweb_bb/__pycache__/widgets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/admin.py` & `punkweb_bb-0.1.3/punkweb_bb/admin.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/admin_forms.py` & `punkweb_bb-0.1.3/punkweb_bb/admin_forms.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/bbcode_tags.py` & `punkweb_bb-0.1.3/punkweb_bb/bbcode_tags.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/forms.py` & `punkweb_bb-0.1.3/punkweb_bb/forms.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/migrations/0001_initial.py` & `punkweb_bb-0.1.3/punkweb_bb/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc` & `punkweb_bb-0.1.3/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/models.py` & `punkweb_bb-0.1.3/punkweb_bb/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 import math
 import os
 
 from django.contrib.auth import get_user_model
 from django.core.cache import cache
 from django.db import models
+from django.forms import ValidationError
 from django.urls import reverse
 from django.utils import timezone
 from precise_bbcode.fields import BBCodeTextField
 
 from punkweb_bb.mixins import TimestampMixin, UUIDPrimaryKeyMixin
 
 User = get_user_model()
@@ -103,14 +104,15 @@
     )
     user = models.ForeignKey(User, related_name="threads", on_delete=models.CASCADE)
     title = models.CharField(max_length=255)
     content = BBCodeTextField()
     is_pinned = models.BooleanField(default=False)
     is_closed = models.BooleanField(default=False)
     last_post_created_at = models.DateTimeField(auto_now_add=True)
+    view_count = models.PositiveIntegerField(default=0)
 
     class Meta:
         ordering = (
             "subcategory",
             "-is_pinned",
             "-last_post_created_at",
         )
@@ -157,14 +159,16 @@
         thread_url = reverse("punkweb_bb:thread", args=[self.thread.id])
 
         thread_url += f"?page={self.page_number}#post-{self.id}"
 
         return thread_url
 
     def save(self, *args, **kwargs):
+        if self.thread.is_closed:
+            raise ValidationError("Cannot add posts to a closed thread.")
         if self._state.adding:
             self.thread.last_post_created_at = timezone.now()
             self.thread.save()
         super().save(*args, **kwargs)
 
 
 class Shout(UUIDPrimaryKeyMixin, TimestampMixin):
```

### Comparing `punkweb_bb-0.1.2/punkweb_bb/parsers.py` & `punkweb_bb-0.1.3/punkweb_bb/parsers.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/css/defaults.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/defaults.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/css/index.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/index.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/css/profile.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/profile.css`

 * *Files 26% similar despite different names*

```diff
@@ -49,7 +49,14 @@
   color: var(--oc-gray-6);
   font-size: 0.875rem;
 }
 
 .profile__thread:not(:last-of-type) {
   border-bottom: 1px solid var(--border);
 }
+
+@media screen and (max-width: 768px) {
+  .profile__info {
+    align-items: start;
+    flex-direction: column;
+  }
+}
```

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/css/punkweb.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/punkweb.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/css/subcategory.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/subcategory.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/css/thread.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/thread.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/css/variables.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/variables.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/img/default-profile-image.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/img/default-profile-image.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/open-color.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/open-color.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/prism.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/prism.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/prism.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/prism.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css` & `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/base.html` & `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/base.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <!DOCTYPE html>
 <html lang="en">
 <head>
   <meta charset="UTF-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   <title>{% block title_prefix %}{% endblock %}{{ punkweb_bb.settings.SITE_TITLE|default:"PunkwebBB" }}</title>
-  <link rel="icon" href="{% static 'punkweb_bb/favicon.ico' %}" />
+  <link rel="icon" href="{% static punkweb_bb.settings.FAVICON %}" />
   <link rel="stylesheet" href="{% static 'punkweb_bb/vendor/open-color.css' %}" />
   <link rel="stylesheet" href="{% static 'punkweb_bb/vendor/prism.css' %}" />
   <link rel="stylesheet" href="{% static 'punkweb_bb/css/defaults.css' %}" />
   <link rel="stylesheet" href="{% static 'punkweb_bb/css/variables.css' %}" />
   <link rel="stylesheet" href="{% static 'punkweb_bb/css/typography.css' %}" />
   <link rel="stylesheet" href="{% static 'punkweb_bb/css/punkweb.css' %}" />
   <link rel="stylesheet" href="{% static 'punkweb_bb/css/punkweb-modal.css' %}" />
```

### Comparing `punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/index.html` & `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/index.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/login.html` & `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/login.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/members.html` & `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/members.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/partials/post_update.html` & `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/partials/post_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/profile.html` & `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/profile.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/settings.html` & `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/settings.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html` & `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/signup.html` & `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/signup.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/subcategory.html` & `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/subcategory.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 {% extends 'punkweb_bb/base.html' %}
-{% load static %}
+{% load static humanize_int %}
 
 {% block title_prefix %}{{subcategory.name}} | {% endblock%}
 
 {% block extra_head %}
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/subcategory.css' %}" />
 {% endblock %}
 
 {% block content %}
 
 <nav>
   <ul class="pw-breadcrumb">
     <li class="pw-breadcrumb-item">
       <a href="{% url 'punkweb_bb:index' %}">Home</a>
     </li>
+    <li class="pw-breadcrumb-item">
+      <a href="{{subcategory.category.get_absolute_url}}">{{subcategory.category.name}}</a>
+    </li>
     <li class="pw-breadcrumb-item active">
       {{subcategory.name}}
     </li>
   </ul>
 </nav>
 
 <div class="subcategory__header">
@@ -40,20 +43,22 @@
 
 <div class="pw-card fluid margin">
   <div class="pw-table-container">
     <table class="pw-table">
       <colgroup>
         <col span="1">
         <col span="1" width="96px">
+        <col span="1" width="96px">
         <col span="1" width="160px">
       </colgroup>
       <thead>
         <tr>
           <th>Title</th>
           <th>Posts</th>
+          <th>Views</th>
           <th></th>
         </tr>
       </thead>
       <tbody>
         {% for thread in threads %}
         <tr>
           <td>
@@ -70,14 +75,15 @@
               <a href="{% url 'punkweb_bb:profile' thread.user.id %}">
                 {{thread.user.username}}
               </a>
               •
               {{thread.created_at|date:'M j, Y'}}</div>
           </td>
           <td>{{thread.post_count}}</td>
+          <td>{{thread.view_count | humanize_int}}</td>
           <td>
             {% if thread.latest_post %}
             <div class="thread__latestPost">
               <div class="thread__latestPost__info">
                 <a class="thread__latestPost__info__title" href="{{ thread.latest_post.get_absolute_url }}"
                   title="{{thread.latest_post.title}}">
                   <time datetime="{{thread.latest_post.created_at|date:'c'}}">
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-{% extends 'punkweb_bb/base.html' %} {% load static %} {% block title_prefix %}
-{{subcategory.name}} | {% endblock%} {% block extra_head %}
+{% extends 'punkweb_bb/base.html' %} {% load static humanize_int %} {% block
+title_prefix %}{{subcategory.name}} | {% endblock%} {% block extra_head %}
 {% endblock %} {% block content %}
     * _H_o_m_e
+    * _{_{_s_u_b_c_a_t_e_g_o_r_y_._c_a_t_e_g_o_r_y_._n_a_m_e_}_}
     * {{subcategory.name}}
 ************ {{{{ssuubbccaatteeggoorryy..nnaammee}}}} ************
 {% if request.user.is_authenticated %} {% if not subcategory.staff_post_only or
 request.user.is_staff %} _C_r_e_a_t_e_ _T_h_r_e_a_d {% else %} Create Thread {% endif %} {%
 endif %}
-TTiittllee                    PPoossttss
-_{_{_t_h_r_e_a_d_._t_i_t_l_e_}_} {% if                        {% if thread.latest_post %}
-thread.is_pinned %} keep                      _{_{_t_h_r_e_a_d_._l_a_t_e_s_t___p_o_s_t_._c_r_e_a_t_e_d___a_t_|_d_a_t_e_:_'_M_ _j_,
-{% endif %} {% if                             _Y_'_}_}
-thread.is_closed %} lock                      _{_{_t_h_r_e_a_d_._l_a_t_e_s_t___p_o_s_t_._u_s_e_r_._u_s_e_r_n_a_m_e_}_}
-{% endif %}              {                    {% if thread.latest_post.user.profile.image
-_{_{_t_h_r_e_a_d_._u_s_e_r_._u_s_e_r_n_a_m_e_}_} {thread.post_count}} %} [{
-â¢ {                                         {thread.latest_post.user.profile.image.url}}]
-{thread.created_at|date:                      {% else %} [{% static 'punkweb_bb/img/
-'M j, Y'}}                                    default-profile-image.png' %}]{% endif %}
-                                              {% else %} No posts {% endif %}
+TTiittllee                    PPoossttss                VViieewwss
+_{_{_t_h_r_e_a_d_._t_i_t_l_e_}_} {% if                                           {% if thread.latest_post %}
+thread.is_pinned %} keep                                         _{_{_t_h_r_e_a_d_._l_a_t_e_s_t___p_o_s_t_._c_r_e_a_t_e_d___a_t_|_d_a_t_e_:_'_M_ _j_,
+{% endif %} {% if                                                _Y_'_}_}
+thread.is_closed %} lock                      {                  _{_{_t_h_r_e_a_d_._l_a_t_e_s_t___p_o_s_t_._u_s_e_r_._u_s_e_r_n_a_m_e_}_}
+{% endif %}              {                    {thread.view_count {% if thread.latest_post.user.profile.image
+_{_{_t_h_r_e_a_d_._u_s_e_r_._u_s_e_r_n_a_m_e_}_} {thread.post_count}} | humanize_int}}   %} [{
+â¢ {                                                            {thread.latest_post.user.profile.image.url}}]
+{thread.created_at|date:                                         {% else %} [{% static 'punkweb_bb/img/
+'M j, Y'}}                                                       default-profile-image.png' %}]{% endif %}
+                                                                 {% else %} No posts {% endif %}
 {% if threads.has_other_pages %}
     * {% if threads.has_previous %}
     * _P_r_e_v
     * {% else %}
     * _P_r_e_v
     * {% endif %} {% for i in threads.paginator.page_range %} {% if
       threads.number == i %}
```

### Comparing `punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/thread.html` & `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/thread.html`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 
 <nav>
   <ul class="pw-breadcrumb">
     <li class="pw-breadcrumb-item">
       <a href="{% url 'punkweb_bb:index' %}">Home</a>
     </li>
     <li class="pw-breadcrumb-item">
+      <a href="{{thread.subcategory.category.get_absolute_url}}">{{thread.subcategory.category.name}}</a>
+    </li>
+    <li class="pw-breadcrumb-item">
       <a href="{{thread.subcategory.get_absolute_url}}">{{thread.subcategory.name}}</a>
     </li>
     <li class="pw-breadcrumb-item active">
       {{thread.title}}
     </li>
   </ul>
 </nav>
@@ -52,15 +55,15 @@
           {{thread.user.username}}
         </a>
       </div>
       <div class="thread__user__info">
         <div class="thread__user__info__row">
           <div class="thread__user__info__label">Joined:</div>
           <div class="thread__user__info__value">
-            {{thread.user.profile.created_at|date:"M d, Y"}}
+            {{thread.user.date_joined|date:"M d, Y"}}
           </div>
         </div>
         <div class="thread__user__info__row">
           <div class="thread__user__info__label">Posts:</div>
           <div class="thread__user__info__value">{{thread.user.profile.post_count}}</div>
         </div>
       </div>
@@ -113,15 +116,15 @@
           {{post.user.username}}
         </a>
       </div>
       <div class="thread__user__info">
         <div class="thread__user__info__row">
           <div class="thread__user__info__label">Joined:</div>
           <div class="thread__user__info__value">
-            {{post.user.profile.created_at|date:"M d, Y"}}
+            {{post.user.date_joined|date:"M d, Y"}}
           </div>
         </div>
         <div class="thread__user__info__row">
           <div class="thread__user__info__label">Posts:</div>
           <div class="thread__user__info__value">{{post.user.profile.post_count}}</div>
         </div>
       </div>
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
 {% extends 'punkweb_bb/base.html' %} {% load static %} {% block title_prefix %}
 {{thread.title}} | {% endblock %} {% block extra_head %}
 {{post_form.media.css}} {% endblock %} {% block extra_script %} {
 {post_form.media.js}} {% endblock %} {% block content %}
     * _H_o_m_e
+    * _{_{_t_h_r_e_a_d_._s_u_b_c_a_t_e_g_o_r_y_._c_a_t_e_g_o_r_y_._n_a_m_e_}_}
     * _{_{_t_h_r_e_a_d_._s_u_b_c_a_t_e_g_o_r_y_._n_a_m_e_}_}
     * {{thread.title}}
 {% if posts.number == 1 %}
 ************ {{{{tthhrreeaadd..ttiittllee}}}} ************
 {{thread.created_at|date:'M d, Y'}}
 {% if thread.user.profile.image %} [{{thread.user.username}}]{% else %} [{
 {thread.user.username}}]{% endif %}
 {% if thread.user.profile.is_online %}
 {% endif %} _{_{_t_h_r_e_a_d_._u_s_e_r_._u_s_e_r_n_a_m_e_}_}
 Joined:
-{{thread.user.profile.created_at|date:"M d, Y"}}
+{{thread.user.date_joined|date:"M d, Y"}}
 Posts:
 {{thread.user.profile.post_count}}
 {{thread.content.rendered}}
 {% if thread.user.profile.signature.rendered %}
 {{thread.user.profile.signature.rendered}}
 {% endif %} {% if thread.user == request.user %}
 _E_d_i_t Delete
@@ -29,15 +30,15 @@
 [{{post.user.username}}]
 {% else %}
 [{{post.user.username}}]
 {% endif %}
 {% if post.user.profile.is_online %}
 {% endif %} _{_{_p_o_s_t_._u_s_e_r_._u_s_e_r_n_a_m_e_}_}
 Joined:
-{{post.user.profile.created_at|date:"M d, Y"}}
+{{post.user.date_joined|date:"M d, Y"}}
 Posts:
 {{post.user.profile.post_count}}
 {{post.content.rendered}}
 {% if post.user.profile.signature.rendered %}
 {{post.user.profile.signature.rendered}}
 {% endif %} {% if post.user == request.user %}
 Edit Delete
```

### Comparing `punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/thread_create.html` & `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/thread_create.html`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 
 <nav>
   <ul class="pw-breadcrumb">
     <li class="pw-breadcrumb-item">
       <a href="{% url 'punkweb_bb:index' %}">Home</a>
     </li>
     <li class="pw-breadcrumb-item">
+      <a href="{{subcategory.category.get_absolute_url}}">{{subcategory.category.name}}</a>
+    </li>
+    <li class="pw-breadcrumb-item">
       <a href="{{subcategory.get_absolute_url}}">{{subcategory.name}}</a>
     </li>
     <li class="pw-breadcrumb-item active">
       Create Thread
     </li>
   </ul>
 </nav>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 {% extends 'punkweb_bb/base.html' %} {% load static %} {% block title_prefix
 %}Create Thread | {% endblock %} {% block extra_head %} {{form.media.css}}
 {% endblock %} {% block content %}
     * _H_o_m_e
+    * _{_{_s_u_b_c_a_t_e_g_o_r_y_._c_a_t_e_g_o_r_y_._n_a_m_e_}_}
     * _{_{_s_u_b_c_a_t_e_g_o_r_y_._n_a_m_e_}_}
     * Create Thread
 Create Thread
 {% csrf_token %} {% for field in form %}
 {{ field.label }} {{ field }}
 {% endfor %} {% if form.non_field_errors %} {{ form.non_field_errors }} {%
 endif %}
```

### Comparing `punkweb_bb-0.1.2/punkweb_bb/templates/punkweb_bb/thread_update.html` & `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/thread_update.html`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 
 <nav>
   <ul class="pw-breadcrumb">
     <li class="pw-breadcrumb-item">
       <a href="{% url 'punkweb_bb:index' %}">Home</a>
     </li>
     <li class="pw-breadcrumb-item">
+      <a href="{{thread.subcategory.category.get_absolute_url}}">{{thread.subcategory.category.name}}</a>
+    </li>
+    <li class="pw-breadcrumb-item">
       <a href="{{thread.subcategory.get_absolute_url}}">{{thread.subcategory.name}}</a>
     </li>
     <li class="pw-breadcrumb-item">
       <a href="{{thread.get_absolute_url}}">{{thread.title}}</a>
     </li>
     <li class="pw-breadcrumb-item active">
       Edit
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 {% extends 'punkweb_bb/base.html' %} {% load static %} {% block title_prefix
 %}Edit Thread | {% endblock %} {% block extra_head %} {{form.media.css}}
 {% endblock %} {% block content %}
     * _H_o_m_e
+    * _{_{_t_h_r_e_a_d_._s_u_b_c_a_t_e_g_o_r_y_._c_a_t_e_g_o_r_y_._n_a_m_e_}_}
     * _{_{_t_h_r_e_a_d_._s_u_b_c_a_t_e_g_o_r_y_._n_a_m_e_}_}
     * _{_{_t_h_r_e_a_d_._t_i_t_l_e_}_}
     * Edit
 Edit Thread
 {% csrf_token %} {% for field in form %}
 {{ field.label }} {{ field }}
 {% endfor %} {% if form.non_field_errors %} {{ form.non_field_errors }} {%
```

### Comparing `punkweb_bb-0.1.2/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc` & `punkweb_bb-0.1.3/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/urls.py` & `punkweb_bb-0.1.3/punkweb_bb/urls.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb/views.py` & `punkweb_bb-0.1.3/punkweb_bb/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,17 @@
     context = {
         "user": user,
     }
     return render(request, "punkweb_bb/profile.html", context=context)
 
 
 def members_view(request):
-    users = paginate_qs(request, User.objects.select_related("profile").all())
+    users = paginate_qs(
+        request, User.objects.select_related("profile").order_by("username")
+    )
 
     context = {
         "users": users,
     }
     return render(request, "punkweb_bb/members.html", context=context)
 
 
@@ -181,14 +183,21 @@
 def thread_view(request, thread_id):
     thread = get_object_or_404(Thread, pk=thread_id)
 
     posts = paginate_qs(request, thread.posts.all())
 
     post_form = PostModelForm()
 
+    # Increment view count if this session hasn't viewed the thread before
+    viewed_threads = request.session.get("viewed_threads", [])
+    if thread_id not in viewed_threads:
+        thread.view_count += 1
+        thread.save()
+        request.session["viewed_threads"] = viewed_threads + [thread_id]
+
     context = {
         "thread": thread,
         "posts": posts,
         "post_form": post_form,
     }
     return render(request, "punkweb_bb/thread.html", context=context)
 
@@ -231,15 +240,15 @@
 
 
 @login_required(login_url="/login/")
 def post_create_view(request, thread_id):
     thread = get_object_or_404(Thread, pk=thread_id)
 
     if thread.is_closed:
-        return HttpResponseForbidden("This thread is closed.")
+        return HttpResponseForbidden("Cannot add posts to a closed thread.")
 
     form = PostModelForm(request.POST)
 
     if form.is_valid():
         post = form.save(commit=False)
         post.thread = thread
         post.user = request.user
@@ -332,15 +341,15 @@
         ("Strikethrough", "[s]Strikethrough Text[/s]"),
         ("Quote", "[quote=Example]Quoted Text[/quote]"),
         ("Center", "[center]Centered Text[/center]"),
         ("Color", "[color=red]Red Text[/color]"),
         ("Url", "[url=https://google.com]Link Text[/url]"),
         (
             "Image",
-            "[img]https://punkweb.net/media/music/artists/system-lynx_EklOGpj.png.200x200_q85_crop.png[/img]",
+            "[img]https://placehold.co/400[/img]",
         ),
         # Custom
         ("Horizontal Rule", "[hr]"),
         (
             "Code",
             """
 [code=python]
```

### Comparing `punkweb_bb-0.1.2/punkweb_bb/widgets.py` & `punkweb_bb-0.1.3/punkweb_bb/widgets.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.2/punkweb_bb.egg-info/SOURCES.txt` & `punkweb_bb-0.1.3/punkweb_bb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,20 +38,23 @@
 punkweb_bb/__pycache__/mixins.cpython-311.pyc
 punkweb_bb/__pycache__/models.cpython-311.pyc
 punkweb_bb/__pycache__/pagination.cpython-311.pyc
 punkweb_bb/__pycache__/parsers.cpython-311.pyc
 punkweb_bb/__pycache__/response.cpython-311.pyc
 punkweb_bb/__pycache__/settings.cpython-311.pyc
 punkweb_bb/__pycache__/signals.cpython-311.pyc
+punkweb_bb/__pycache__/tests.cpython-311.pyc
 punkweb_bb/__pycache__/urls.cpython-311.pyc
 punkweb_bb/__pycache__/views.cpython-311.pyc
 punkweb_bb/__pycache__/widgets.cpython-311.pyc
 punkweb_bb/migrations/0001_initial.py
+punkweb_bb/migrations/0002_thread_view_count.py
 punkweb_bb/migrations/__init__.py
 punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc
+punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc
 punkweb_bb/migrations/__pycache__/__init__.cpython-311.pyc
 punkweb_bb/static/punkweb_bb/favicon.ico
 punkweb_bb/static/punkweb_bb/css/defaults.css
 punkweb_bb/static/punkweb_bb/css/index.css
 punkweb_bb/static/punkweb_bb/css/login.css
 punkweb_bb/static/punkweb_bb/css/members.css
 punkweb_bb/static/punkweb_bb/css/post-form.css
@@ -210,10 +213,13 @@
 punkweb_bb/templates/punkweb_bb/thread_update.html
 punkweb_bb/templates/punkweb_bb/partials/post_delete.html
 punkweb_bb/templates/punkweb_bb/partials/post_update.html
 punkweb_bb/templates/punkweb_bb/partials/thread_delete.html
 punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html
 punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html
 punkweb_bb/templatetags/__init__.py
+punkweb_bb/templatetags/humanize_int.py
 punkweb_bb/templatetags/shoutbox_bbcode.py
 punkweb_bb/templatetags/__pycache__/__init__.cpython-311.pyc
+punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc
+punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc
 punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc
```

### Comparing `punkweb_bb-0.1.2/setup.py` & `punkweb_bb-0.1.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="punkweb_bb",
-    version="0.1.2",
+    version="0.1.3",
     author="Punkweb",
     author_email="punkwebnet@gmail.com",
     packages=["punkweb_bb"],
     url="https://github.com/Punkweb/PunkwebBB",
     license="BSD-3-Clause",
     description="Django application that provides a simple and modern forum board software for your Django website.",
     long_description=open("README.md").read(),
```

