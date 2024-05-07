# Comparing `tmp/django-admin-thumbnails-0.2.8.tar.gz` & `tmp/django-admin-thumbnails-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-admin-thumbnails-0.2.8.tar", last modified: Thu Jun  1 14:50:13 2023, max compression
+gzip compressed data, was "django-admin-thumbnails-0.2.9.tar", last modified: Tue May  7 06:47:21 2024, max compression
```

## Comparing `django-admin-thumbnails-0.2.8.tar` & `django-admin-thumbnails-0.2.9.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-06-01 14:50:13.000000 django-admin-thumbnails-0.2.8/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    10244 2023-06-01 14:50:13.000000 django-admin-thumbnails-0.2.8/PKG-INFO
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-06-01 14:50:13.000000 django-admin-thumbnails-0.2.8/django_admin_thumbnails.egg-info/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    10244 2023-06-01 14:50:13.000000 django-admin-thumbnails-0.2.8/django_admin_thumbnails.egg-info/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2019-04-07 12:40:08.000000 django-admin-thumbnails-0.2.8/django_admin_thumbnails.egg-info/not-zip-safe
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      404 2023-06-01 14:50:13.000000 django-admin-thumbnails-0.2.8/django_admin_thumbnails.egg-info/SOURCES.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       93 2023-06-01 14:50:13.000000 django-admin-thumbnails-0.2.8/django_admin_thumbnails.egg-info/requires.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       17 2023-06-01 14:50:13.000000 django-admin-thumbnails-0.2.8/django_admin_thumbnails.egg-info/top_level.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2023-06-01 14:50:13.000000 django-admin-thumbnails-0.2.8/django_admin_thumbnails.egg-info/dependency_links.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       58 2019-04-07 10:23:12.000000 django-admin-thumbnails-0.2.8/MANIFEST.in
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-06-01 14:50:13.000000 django-admin-thumbnails-0.2.8/admin_thumbnails/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4806 2023-06-01 14:48:48.000000 django-admin-thumbnails-0.2.8/admin_thumbnails/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      248 2019-10-10 09:50:06.000000 django-admin-thumbnails-0.2.8/admin_thumbnails/utils.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1300 2019-04-16 19:16:08.000000 django-admin-thumbnails-0.2.8/admin_thumbnails/settings.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     7443 2023-04-19 11:54:42.000000 django-admin-thumbnails-0.2.8/README.md
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2298 2023-06-01 14:47:54.000000 django-admin-thumbnails-0.2.8/setup.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       79 2023-06-01 14:50:13.000000 django-admin-thumbnails-0.2.8/setup.cfg
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-07 06:47:21.247693 django-admin-thumbnails-0.2.9/
+-rw-r--r--   0 james      (501) staff       (20)     1070 2019-04-07 10:23:02.000000 django-admin-thumbnails-0.2.9/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)       58 2019-04-07 10:23:12.000000 django-admin-thumbnails-0.2.9/MANIFEST.in
+-rw-r--r--   0 james      (501) staff       (20)     8871 2024-05-07 06:47:21.247944 django-admin-thumbnails-0.2.9/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     7469 2024-05-07 06:42:42.000000 django-admin-thumbnails-0.2.9/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-07 06:47:21.243254 django-admin-thumbnails-0.2.9/admin_thumbnails/
+-rw-r--r--   0 james      (501) staff       (20)     4806 2023-06-01 14:48:48.000000 django-admin-thumbnails-0.2.9/admin_thumbnails/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1300 2019-04-16 19:16:08.000000 django-admin-thumbnails-0.2.9/admin_thumbnails/settings.py
+-rw-r--r--   0 james      (501) staff       (20)      248 2019-10-10 09:50:06.000000 django-admin-thumbnails-0.2.9/admin_thumbnails/utils.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-07 06:47:21.247283 django-admin-thumbnails-0.2.9/django_admin_thumbnails.egg-info/
+-rw-rw-r--   0 james      (501) staff       (20)     8871 2024-05-07 06:47:21.000000 django-admin-thumbnails-0.2.9/django_admin_thumbnails.egg-info/PKG-INFO
+-rw-rw-r--   0 james      (501) staff       (20)      412 2024-05-07 06:47:21.000000 django-admin-thumbnails-0.2.9/django_admin_thumbnails.egg-info/SOURCES.txt
+-rw-rw-r--   0 james      (501) staff       (20)        1 2024-05-07 06:47:21.000000 django-admin-thumbnails-0.2.9/django_admin_thumbnails.egg-info/dependency_links.txt
+-rw-rw-r--   0 james      (501) staff       (20)        1 2019-04-07 12:40:08.000000 django-admin-thumbnails-0.2.9/django_admin_thumbnails.egg-info/not-zip-safe
+-rw-rw-r--   0 james      (501) staff       (20)       93 2024-05-07 06:47:21.000000 django-admin-thumbnails-0.2.9/django_admin_thumbnails.egg-info/requires.txt
+-rw-rw-r--   0 james      (501) staff       (20)       17 2024-05-07 06:47:21.000000 django-admin-thumbnails-0.2.9/django_admin_thumbnails.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       79 2024-05-07 06:47:21.248844 django-admin-thumbnails-0.2.9/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     2298 2024-05-07 06:45:36.000000 django-admin-thumbnails-0.2.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-admin-thumbnails-0.2.8/PKG-INFO` & `django-admin-thumbnails-0.2.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,192 +1,15 @@
 Metadata-Version: 2.1
 Name: django-admin-thumbnails
-Version: 0.2.8
+Version: 0.2.9
 Summary: A Django app for DRY thumbnails in admin list views and forms.
 Home-page: http://github.com/BigglesZX/django-admin-thumbnails
 Author: James Tiplady
 Maintainer: James Tiplady
 License: MIT
-Description: # django-admin-thumbnails
-        
-        A Django app to assist in adding thumbnails for your model's image fields to admin list views and forms in a reasonably DRY manner.
-        
-        ## Rationale
-        
-        When working with models that include `ImageField`s, `FileField`s or when using `ThumbnailerImageField` from `easy_thumbnails`, it can often be desirable to include a thumbnail preview of the field as part of the admin form, fieldset or in list views. Various methods to achieve this exist but all seem to involve a degree of duplication. I've made a few attempts to DRY out such code over the years and this library represents my most recent solution. So, please enjoy!
-        
-        ## Compatibility
-        
-        I've not exhaustively tested all the below combinations, however I believe this table to be accurate.
-        
-        |                | Django 1.10 | 1.11 | 2.0 | 2.1 | 2.2 | 3.0 | 3.1 | 3.2 | 4.0 | 4.1 | 4.2 |
-        | -------------: | :---------: | :--: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
-        | **Python** 2.7 |      ✔      |  ✔   |     |     |     |     |     |     |     |     |     |
-        |            3.6 |      ✔      |  ✔   |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |     |     |     |
-        |         >= 3.8 |             |      |     |     |     |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |
-        
-        ## Installation
-        
-        ```
-        $ pip install django-admin-thumbnails
-        ```
-        
-        ## Usage
-        
-        The app adds fields to your `ModelAdmin` or `*Inline` class; one for each thumbnail you want to display. These are appended to the class's `readonly_fields` tuple (unless you specify otherwise) so they will be displayed at the bottom of your admin form, or you can include them by name in your `fieldsets` or `list_display` definitions.
-        
-        `django-admin-thumbnails` will handle `ImageField`, `FileField` (so you can use SVG, for example) and (if `easy_thumbnails` is installed) `ThumbnailerImageField`. In the latter case a thumbnail alias will be used, which you can specify in settings.
-        
-        ### Basic usage
-        
-        To create an admin thumbnail field, decorate your `ModelAdmin` or `*Inline` class and optionally specify what to do with the newly created field.
-        
-        Assuming a model like the following:
-        
-        ```python
-        class Person(models.Model):
-            name = models.CharField('Name', max_length=100)
-            image = models.ImageField('Image')
-            # ...
-        ```
-        
-        In the simplest use-case, to add a thumbnail field to the bottom of the admin form, simply decorate the `ModelAdmin` or `*Inline` class (the order of decorators is important), supplying the name of the field from which the thumbnail will be taken:
-        
-        ```python
-        import admin_thumbnails
-        
-        @admin.register(models.Person)
-        @admin_thumbnails.thumbnail('image')
-        class PersonAdmin(admin.ModelAdmin):
-            pass
-        ```
-        
-        This will add a field called `image_thumbnail` (`FOO_thumbnail` where `FOO` is the origin field's name) to your `ModelAdmin` or `*Inline` definition. To override the title given to the new field, pass a second string argument to the decorator:
-        
-        ```python
-        @admin_thumbnails.thumbnail('image', 'Thumbnail')
-        ```
-        
-        To add the thumbnail to the columns shown in the model's list view, add the new field name to `list_display`:
-        
-        ```python
-        @admin.register(models.Person)
-        @admin_thumbnails.thumbnail('image')
-        class PersonAdmin(admin.ModelAdmin):
-            list_display = ('name', 'image_thumbnail')
-        ```
-        
-        Or include it in your `fieldsets` similarly:
-        
-        ```python
-        @admin.register(models.Person)
-        @admin_thumbnails.thumbnail('image')
-        class PersonAdmin(admin.ModelAdmin):
-            fieldsets = (
-                (None, {
-                    'fields': ('name', 'image_thumbnail'),
-                }),
-            )
-        ```
-        
-        ### Using thumbnails in the list view only
-        
-        By default the new field will be appended to the `readonly_fields` tuple – if this is undesirable (e.g. if you want to include the thumbnail in the list view but _not_ in the default form fields), pass `append=False` to the decorator:
-        
-        ```python
-        @admin.register(models.Person)
-        @admin_thumbnails.thumbnail('image', append=False)
-        class PersonAdmin(admin.ModelAdmin):
-            list_display = ('name', 'image_thumbnail')
-        ```
-        
-        This isn't necessary if you're using `fieldsets`, as by doing so you will control the inclusion (or omission) and position of the thumbnail field.
-        
-        ### Using a property on the model as the thumbnail source
-        
-        As of version 0.2.7, the name passed to the `thumbnail` decorator can refer to a property on the model rather than a field. For example:
-        
-        ```python
-        class Person(models.Model):
-            # ...
-            @property
-            def primary_image(self):
-                if self.images.count():
-                    return self.images.first().image
-                return None
-        ```
-        
-        Provided the specified property returns an instance of a `FieldFile` (i.e. a file stored in a field that is an instance of Django's `ImageField`, `FileField`, or `easy_thumbnails`' `ThumbnailerImageField`), this will work as normal.
-        
-        This also works with Django's [`cached_property`](https://docs.djangoproject.com/en/dev/ref/utils/#django.utils.functional.cached_property) decorator.
-        
-        ### Adding a background to displayed thumbnails
-        
-        If your field contains images that are designed to be shown on a dark background, you can supply `background=True` to the decorator to add one to the thumbnail (via CSS) when displayed:
-        
-        ```python
-        @admin_thumbnails.thumbnail('image', background=True)
-        ```
-        
-        If you're using `easy_thumbnails` and want to override the alias used to generate your thumbnail on a per-field basis (as opposed to using the `ADMIN_THUMBNAIL_THUMBNAIL_ALIAS` setting; see below), you can use the `alias` argument to the decorator:
-        
-        ```python
-        @admin_thumbnails.thumbnail('image', alias='admin_thumbnail_alternative')
-        ```
-        
-        ## Configuration
-        
-        ### `ADMIN_THUMBNAIL_DEFAULT_LABEL`
-        
-        **Default:** `'Preview'`
-        
-        Setting this overrides the default column name / title used by thumbnails.
-        
-        ### `ADMIN_THUMBNAIL_FIELD_SUFFIX`
-        
-        **Default:** `'_thumbnail'`
-        
-        Setting this overrides the suffix given to newly created thumbnail fields. Change if you have collision issues with other field names you want to use. Don't forget to update `list_display` and/or `fieldsets` in your `ModelAdmin` as necessary.
-        
-        ### `ADMIN_THUMBNAIL_THUMBNAIL_ALIAS`
-        
-        **Default:** `'admin_thumbnail'`
-        
-        If `easy_thumbnails` is installed and available, any model field using `ThumbnailerImageField` will be resized using a thumbnail alias called `admin_thumbnail` if it's defined. You can either define this alias in your settings (more info from the `easy_thumbnails` documentation [here](https://easy-thumbnails.readthedocs.io/en/stable/usage/#thumbnail-aliases)) or supply a different alias name as the value of this setting.
-        
-        ### `ADMIN_THUMBNAIL_STYLE`
-        
-        **Default:** `{'display': 'block', 'width': '100px', 'height': 'auto'}`
-        
-        A dictionary of CSS property/value pairs that will be added to the `style` attribute of any thumbnail image when output in the admin. Override to supply your own styles.
-        
-        ### `ADMIN_THUMBNAIL_BACKGROUND_STYLE`
-        
-        **Default:** `{'background': '#000'}`
-        
-        A dictionary of CSS property/value pairs added when the `background=True` option is used (see **Usage** above). Override to supply your own styles. Note that these styles are used _in addition_ to any defined in `ADMIN_THUMBNAIL_STYLE`.
-        
-        ## Development installation
-        
-        If working locally on the package you can install the development tools via `pip`:
-        
-        ```shell
-        $ pip install -e .[dev]
-        ```
-        
-        To lint with `flake8`:
-        
-        ```shell
-        $ flake8
-        ```
-        
-        ## Issues, suggestions, contributions
-        
-        ...are welcome on GitHub. Thanks for your interest in `django-admin-thumbnails`!
-        
 Keywords: django
 Platform: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -206,7 +29,186 @@
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Requires-Python: >=2.6,<4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# django-admin-thumbnails
+
+A Django app to assist in adding thumbnails for your model's image fields to admin list views and forms in a reasonably DRY manner.
+
+## Rationale
+
+When working with models that include `ImageField`s, `FileField`s or when using `ThumbnailerImageField` from `easy_thumbnails`, it can often be desirable to include a thumbnail preview of the field as part of the admin form, fieldset or in list views. Various methods to achieve this exist but all seem to involve a degree of duplication. I've made a few attempts to DRY out such code over the years and this library represents my most recent solution. So, please enjoy!
+
+## Compatibility
+
+I've not exhaustively tested all the below combinations, however I believe this table to be accurate.
+
+|                | Django 1.10 | 1.11 | 2.0 | 2.1 | 2.2 | 3.0 | 3.1 | 3.2 | 4.0 | 4.1 | 4.2 |
+| -------------: | :---------: | :--: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
+| **Python** 2.7 |      ✔      |  ✔   |     |     |     |     |     |     |     |     |     |
+|            3.6 |      ✔      |  ✔   |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |     |     |     |
+|         >= 3.8 |             |      |     |     |     |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |
+
+## Installation
+
+```
+$ pip install django-admin-thumbnails
+```
+
+## Usage
+
+The app adds fields to your `ModelAdmin` or `*Inline` class; one for each thumbnail you want to display. These are appended to the class's `readonly_fields` tuple (unless you specify otherwise) so they will be displayed at the bottom of your admin form, or you can include them by name in your `fieldsets` or `list_display` definitions.
+
+`django-admin-thumbnails` will handle `ImageField`, `FileField` (so you can use SVG, for example) and (if `easy_thumbnails` is installed) `ThumbnailerImageField`. In the latter case a thumbnail alias will be used, which you can specify in settings.
+
+### Basic usage
+
+To create an admin thumbnail field, decorate your `ModelAdmin` or `*Inline` class and optionally specify what to do with the newly created field.
+
+Assuming a model like the following:
+
+```python
+class Person(models.Model):
+    name = models.CharField('Name', max_length=100)
+    image = models.ImageField('Image')
+    # ...
+```
+
+In the simplest use-case, to add a thumbnail field to the bottom of the admin form, simply decorate the `ModelAdmin` or `*Inline` class (the order of decorators is important), supplying the name of the field from which the thumbnail will be taken:
+
+```python
+import admin_thumbnails
+
+@admin.register(models.Person)
+@admin_thumbnails.thumbnail('image')
+class PersonAdmin(admin.ModelAdmin):
+    pass
+```
+
+This will add a field called `image_thumbnail` (`FOO_thumbnail` where `FOO` is the origin field's name) to your `ModelAdmin` or `*Inline` definition. To override the title given to the new field, pass a second string argument to the decorator:
+
+```python
+@admin_thumbnails.thumbnail('image', 'Thumbnail')
+```
+
+To add the thumbnail to the columns shown in the model's list view, add the new field name to `list_display`:
+
+```python
+@admin.register(models.Person)
+@admin_thumbnails.thumbnail('image')
+class PersonAdmin(admin.ModelAdmin):
+    list_display = ('name', 'image_thumbnail')
+```
+
+Or include it in your `fieldsets` similarly:
+
+```python
+@admin.register(models.Person)
+@admin_thumbnails.thumbnail('image')
+class PersonAdmin(admin.ModelAdmin):
+    fieldsets = (
+        (None, {
+            'fields': ('name', 'image_thumbnail'),
+        }),
+    )
+```
+
+### Using thumbnails in the list view only
+
+By default the new field will be appended to the `readonly_fields` tuple – if this is undesirable (e.g. if you want to include the thumbnail in the list view but _not_ in the default form fields), pass `append=False` to the decorator:
+
+```python
+@admin.register(models.Person)
+@admin_thumbnails.thumbnail('image', append=False)
+class PersonAdmin(admin.ModelAdmin):
+    list_display = ('name', 'image_thumbnail')
+```
+
+This isn't necessary if you're using `fieldsets`, as by doing so you will control the inclusion (or omission) and position of the thumbnail field.
+
+### Using a property on the model as the thumbnail source
+
+As of version 0.2.7, the name passed to the `thumbnail` decorator can refer to a property on the model rather than a field. For example:
+
+```python
+class Person(models.Model):
+    # ...
+    @property
+    def primary_image(self):
+        first_image = self.images.first()
+        if first_image:
+            return first_image.image
+        return None
+```
+
+Provided the specified property returns an instance of a `FieldFile` (i.e. a file stored in a field that is an instance of Django's `ImageField`, `FileField`, or `easy_thumbnails`' `ThumbnailerImageField`), this will work as normal.
+
+This also works with Django's [`cached_property`](https://docs.djangoproject.com/en/dev/ref/utils/#django.utils.functional.cached_property) decorator.
+
+### Adding a background to displayed thumbnails
+
+If your field contains images that are designed to be shown on a dark background, you can supply `background=True` to the decorator to add one to the thumbnail (via CSS) when displayed:
+
+```python
+@admin_thumbnails.thumbnail('image', background=True)
+```
+
+If you're using `easy_thumbnails` and want to override the alias used to generate your thumbnail on a per-field basis (as opposed to using the `ADMIN_THUMBNAIL_THUMBNAIL_ALIAS` setting; see below), you can use the `alias` argument to the decorator:
+
+```python
+@admin_thumbnails.thumbnail('image', alias='admin_thumbnail_alternative')
+```
+
+## Configuration
+
+### `ADMIN_THUMBNAIL_DEFAULT_LABEL`
+
+**Default:** `'Preview'`
+
+Setting this overrides the default column name / title used by thumbnails.
+
+### `ADMIN_THUMBNAIL_FIELD_SUFFIX`
+
+**Default:** `'_thumbnail'`
+
+Setting this overrides the suffix given to newly created thumbnail fields. Change if you have collision issues with other field names you want to use. Don't forget to update `list_display` and/or `fieldsets` in your `ModelAdmin` as necessary.
+
+### `ADMIN_THUMBNAIL_THUMBNAIL_ALIAS`
+
+**Default:** `'admin_thumbnail'`
+
+If `easy_thumbnails` is installed and available, any model field using `ThumbnailerImageField` will be resized using a thumbnail alias called `admin_thumbnail` if it's defined. You can either define this alias in your settings (more info from the `easy_thumbnails` documentation [here](https://easy-thumbnails.readthedocs.io/en/stable/usage/#thumbnail-aliases)) or supply a different alias name as the value of this setting.
+
+### `ADMIN_THUMBNAIL_STYLE`
+
+**Default:** `{'display': 'block', 'width': '100px', 'height': 'auto'}`
+
+A dictionary of CSS property/value pairs that will be added to the `style` attribute of any thumbnail image when output in the admin. Override to supply your own styles.
+
+### `ADMIN_THUMBNAIL_BACKGROUND_STYLE`
+
+**Default:** `{'background': '#000'}`
+
+A dictionary of CSS property/value pairs added when the `background=True` option is used (see **Usage** above). Override to supply your own styles. Note that these styles are used _in addition_ to any defined in `ADMIN_THUMBNAIL_STYLE`.
+
+## Development installation
+
+If working locally on the package you can install the development tools via `pip`:
+
+```shell
+$ pip install -e .[dev]
+```
+
+To lint with `flake8`:
+
+```shell
+$ flake8
+```
+
+## Issues, suggestions, contributions
+
+...are welcome on GitHub. Thanks for your interest in `django-admin-thumbnails`!
```

### Comparing `django-admin-thumbnails-0.2.8/django_admin_thumbnails.egg-info/PKG-INFO` & `django-admin-thumbnails-0.2.9/django_admin_thumbnails.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,192 +1,15 @@
 Metadata-Version: 2.1
 Name: django-admin-thumbnails
-Version: 0.2.8
+Version: 0.2.9
 Summary: A Django app for DRY thumbnails in admin list views and forms.
 Home-page: http://github.com/BigglesZX/django-admin-thumbnails
 Author: James Tiplady
 Maintainer: James Tiplady
 License: MIT
-Description: # django-admin-thumbnails
-        
-        A Django app to assist in adding thumbnails for your model's image fields to admin list views and forms in a reasonably DRY manner.
-        
-        ## Rationale
-        
-        When working with models that include `ImageField`s, `FileField`s or when using `ThumbnailerImageField` from `easy_thumbnails`, it can often be desirable to include a thumbnail preview of the field as part of the admin form, fieldset or in list views. Various methods to achieve this exist but all seem to involve a degree of duplication. I've made a few attempts to DRY out such code over the years and this library represents my most recent solution. So, please enjoy!
-        
-        ## Compatibility
-        
-        I've not exhaustively tested all the below combinations, however I believe this table to be accurate.
-        
-        |                | Django 1.10 | 1.11 | 2.0 | 2.1 | 2.2 | 3.0 | 3.1 | 3.2 | 4.0 | 4.1 | 4.2 |
-        | -------------: | :---------: | :--: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
-        | **Python** 2.7 |      ✔      |  ✔   |     |     |     |     |     |     |     |     |     |
-        |            3.6 |      ✔      |  ✔   |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |     |     |     |
-        |         >= 3.8 |             |      |     |     |     |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |
-        
-        ## Installation
-        
-        ```
-        $ pip install django-admin-thumbnails
-        ```
-        
-        ## Usage
-        
-        The app adds fields to your `ModelAdmin` or `*Inline` class; one for each thumbnail you want to display. These are appended to the class's `readonly_fields` tuple (unless you specify otherwise) so they will be displayed at the bottom of your admin form, or you can include them by name in your `fieldsets` or `list_display` definitions.
-        
-        `django-admin-thumbnails` will handle `ImageField`, `FileField` (so you can use SVG, for example) and (if `easy_thumbnails` is installed) `ThumbnailerImageField`. In the latter case a thumbnail alias will be used, which you can specify in settings.
-        
-        ### Basic usage
-        
-        To create an admin thumbnail field, decorate your `ModelAdmin` or `*Inline` class and optionally specify what to do with the newly created field.
-        
-        Assuming a model like the following:
-        
-        ```python
-        class Person(models.Model):
-            name = models.CharField('Name', max_length=100)
-            image = models.ImageField('Image')
-            # ...
-        ```
-        
-        In the simplest use-case, to add a thumbnail field to the bottom of the admin form, simply decorate the `ModelAdmin` or `*Inline` class (the order of decorators is important), supplying the name of the field from which the thumbnail will be taken:
-        
-        ```python
-        import admin_thumbnails
-        
-        @admin.register(models.Person)
-        @admin_thumbnails.thumbnail('image')
-        class PersonAdmin(admin.ModelAdmin):
-            pass
-        ```
-        
-        This will add a field called `image_thumbnail` (`FOO_thumbnail` where `FOO` is the origin field's name) to your `ModelAdmin` or `*Inline` definition. To override the title given to the new field, pass a second string argument to the decorator:
-        
-        ```python
-        @admin_thumbnails.thumbnail('image', 'Thumbnail')
-        ```
-        
-        To add the thumbnail to the columns shown in the model's list view, add the new field name to `list_display`:
-        
-        ```python
-        @admin.register(models.Person)
-        @admin_thumbnails.thumbnail('image')
-        class PersonAdmin(admin.ModelAdmin):
-            list_display = ('name', 'image_thumbnail')
-        ```
-        
-        Or include it in your `fieldsets` similarly:
-        
-        ```python
-        @admin.register(models.Person)
-        @admin_thumbnails.thumbnail('image')
-        class PersonAdmin(admin.ModelAdmin):
-            fieldsets = (
-                (None, {
-                    'fields': ('name', 'image_thumbnail'),
-                }),
-            )
-        ```
-        
-        ### Using thumbnails in the list view only
-        
-        By default the new field will be appended to the `readonly_fields` tuple – if this is undesirable (e.g. if you want to include the thumbnail in the list view but _not_ in the default form fields), pass `append=False` to the decorator:
-        
-        ```python
-        @admin.register(models.Person)
-        @admin_thumbnails.thumbnail('image', append=False)
-        class PersonAdmin(admin.ModelAdmin):
-            list_display = ('name', 'image_thumbnail')
-        ```
-        
-        This isn't necessary if you're using `fieldsets`, as by doing so you will control the inclusion (or omission) and position of the thumbnail field.
-        
-        ### Using a property on the model as the thumbnail source
-        
-        As of version 0.2.7, the name passed to the `thumbnail` decorator can refer to a property on the model rather than a field. For example:
-        
-        ```python
-        class Person(models.Model):
-            # ...
-            @property
-            def primary_image(self):
-                if self.images.count():
-                    return self.images.first().image
-                return None
-        ```
-        
-        Provided the specified property returns an instance of a `FieldFile` (i.e. a file stored in a field that is an instance of Django's `ImageField`, `FileField`, or `easy_thumbnails`' `ThumbnailerImageField`), this will work as normal.
-        
-        This also works with Django's [`cached_property`](https://docs.djangoproject.com/en/dev/ref/utils/#django.utils.functional.cached_property) decorator.
-        
-        ### Adding a background to displayed thumbnails
-        
-        If your field contains images that are designed to be shown on a dark background, you can supply `background=True` to the decorator to add one to the thumbnail (via CSS) when displayed:
-        
-        ```python
-        @admin_thumbnails.thumbnail('image', background=True)
-        ```
-        
-        If you're using `easy_thumbnails` and want to override the alias used to generate your thumbnail on a per-field basis (as opposed to using the `ADMIN_THUMBNAIL_THUMBNAIL_ALIAS` setting; see below), you can use the `alias` argument to the decorator:
-        
-        ```python
-        @admin_thumbnails.thumbnail('image', alias='admin_thumbnail_alternative')
-        ```
-        
-        ## Configuration
-        
-        ### `ADMIN_THUMBNAIL_DEFAULT_LABEL`
-        
-        **Default:** `'Preview'`
-        
-        Setting this overrides the default column name / title used by thumbnails.
-        
-        ### `ADMIN_THUMBNAIL_FIELD_SUFFIX`
-        
-        **Default:** `'_thumbnail'`
-        
-        Setting this overrides the suffix given to newly created thumbnail fields. Change if you have collision issues with other field names you want to use. Don't forget to update `list_display` and/or `fieldsets` in your `ModelAdmin` as necessary.
-        
-        ### `ADMIN_THUMBNAIL_THUMBNAIL_ALIAS`
-        
-        **Default:** `'admin_thumbnail'`
-        
-        If `easy_thumbnails` is installed and available, any model field using `ThumbnailerImageField` will be resized using a thumbnail alias called `admin_thumbnail` if it's defined. You can either define this alias in your settings (more info from the `easy_thumbnails` documentation [here](https://easy-thumbnails.readthedocs.io/en/stable/usage/#thumbnail-aliases)) or supply a different alias name as the value of this setting.
-        
-        ### `ADMIN_THUMBNAIL_STYLE`
-        
-        **Default:** `{'display': 'block', 'width': '100px', 'height': 'auto'}`
-        
-        A dictionary of CSS property/value pairs that will be added to the `style` attribute of any thumbnail image when output in the admin. Override to supply your own styles.
-        
-        ### `ADMIN_THUMBNAIL_BACKGROUND_STYLE`
-        
-        **Default:** `{'background': '#000'}`
-        
-        A dictionary of CSS property/value pairs added when the `background=True` option is used (see **Usage** above). Override to supply your own styles. Note that these styles are used _in addition_ to any defined in `ADMIN_THUMBNAIL_STYLE`.
-        
-        ## Development installation
-        
-        If working locally on the package you can install the development tools via `pip`:
-        
-        ```shell
-        $ pip install -e .[dev]
-        ```
-        
-        To lint with `flake8`:
-        
-        ```shell
-        $ flake8
-        ```
-        
-        ## Issues, suggestions, contributions
-        
-        ...are welcome on GitHub. Thanks for your interest in `django-admin-thumbnails`!
-        
 Keywords: django
 Platform: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -206,7 +29,186 @@
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Requires-Python: >=2.6,<4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# django-admin-thumbnails
+
+A Django app to assist in adding thumbnails for your model's image fields to admin list views and forms in a reasonably DRY manner.
+
+## Rationale
+
+When working with models that include `ImageField`s, `FileField`s or when using `ThumbnailerImageField` from `easy_thumbnails`, it can often be desirable to include a thumbnail preview of the field as part of the admin form, fieldset or in list views. Various methods to achieve this exist but all seem to involve a degree of duplication. I've made a few attempts to DRY out such code over the years and this library represents my most recent solution. So, please enjoy!
+
+## Compatibility
+
+I've not exhaustively tested all the below combinations, however I believe this table to be accurate.
+
+|                | Django 1.10 | 1.11 | 2.0 | 2.1 | 2.2 | 3.0 | 3.1 | 3.2 | 4.0 | 4.1 | 4.2 |
+| -------------: | :---------: | :--: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
+| **Python** 2.7 |      ✔      |  ✔   |     |     |     |     |     |     |     |     |     |
+|            3.6 |      ✔      |  ✔   |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |     |     |     |
+|         >= 3.8 |             |      |     |     |     |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |
+
+## Installation
+
+```
+$ pip install django-admin-thumbnails
+```
+
+## Usage
+
+The app adds fields to your `ModelAdmin` or `*Inline` class; one for each thumbnail you want to display. These are appended to the class's `readonly_fields` tuple (unless you specify otherwise) so they will be displayed at the bottom of your admin form, or you can include them by name in your `fieldsets` or `list_display` definitions.
+
+`django-admin-thumbnails` will handle `ImageField`, `FileField` (so you can use SVG, for example) and (if `easy_thumbnails` is installed) `ThumbnailerImageField`. In the latter case a thumbnail alias will be used, which you can specify in settings.
+
+### Basic usage
+
+To create an admin thumbnail field, decorate your `ModelAdmin` or `*Inline` class and optionally specify what to do with the newly created field.
+
+Assuming a model like the following:
+
+```python
+class Person(models.Model):
+    name = models.CharField('Name', max_length=100)
+    image = models.ImageField('Image')
+    # ...
+```
+
+In the simplest use-case, to add a thumbnail field to the bottom of the admin form, simply decorate the `ModelAdmin` or `*Inline` class (the order of decorators is important), supplying the name of the field from which the thumbnail will be taken:
+
+```python
+import admin_thumbnails
+
+@admin.register(models.Person)
+@admin_thumbnails.thumbnail('image')
+class PersonAdmin(admin.ModelAdmin):
+    pass
+```
+
+This will add a field called `image_thumbnail` (`FOO_thumbnail` where `FOO` is the origin field's name) to your `ModelAdmin` or `*Inline` definition. To override the title given to the new field, pass a second string argument to the decorator:
+
+```python
+@admin_thumbnails.thumbnail('image', 'Thumbnail')
+```
+
+To add the thumbnail to the columns shown in the model's list view, add the new field name to `list_display`:
+
+```python
+@admin.register(models.Person)
+@admin_thumbnails.thumbnail('image')
+class PersonAdmin(admin.ModelAdmin):
+    list_display = ('name', 'image_thumbnail')
+```
+
+Or include it in your `fieldsets` similarly:
+
+```python
+@admin.register(models.Person)
+@admin_thumbnails.thumbnail('image')
+class PersonAdmin(admin.ModelAdmin):
+    fieldsets = (
+        (None, {
+            'fields': ('name', 'image_thumbnail'),
+        }),
+    )
+```
+
+### Using thumbnails in the list view only
+
+By default the new field will be appended to the `readonly_fields` tuple – if this is undesirable (e.g. if you want to include the thumbnail in the list view but _not_ in the default form fields), pass `append=False` to the decorator:
+
+```python
+@admin.register(models.Person)
+@admin_thumbnails.thumbnail('image', append=False)
+class PersonAdmin(admin.ModelAdmin):
+    list_display = ('name', 'image_thumbnail')
+```
+
+This isn't necessary if you're using `fieldsets`, as by doing so you will control the inclusion (or omission) and position of the thumbnail field.
+
+### Using a property on the model as the thumbnail source
+
+As of version 0.2.7, the name passed to the `thumbnail` decorator can refer to a property on the model rather than a field. For example:
+
+```python
+class Person(models.Model):
+    # ...
+    @property
+    def primary_image(self):
+        first_image = self.images.first()
+        if first_image:
+            return first_image.image
+        return None
+```
+
+Provided the specified property returns an instance of a `FieldFile` (i.e. a file stored in a field that is an instance of Django's `ImageField`, `FileField`, or `easy_thumbnails`' `ThumbnailerImageField`), this will work as normal.
+
+This also works with Django's [`cached_property`](https://docs.djangoproject.com/en/dev/ref/utils/#django.utils.functional.cached_property) decorator.
+
+### Adding a background to displayed thumbnails
+
+If your field contains images that are designed to be shown on a dark background, you can supply `background=True` to the decorator to add one to the thumbnail (via CSS) when displayed:
+
+```python
+@admin_thumbnails.thumbnail('image', background=True)
+```
+
+If you're using `easy_thumbnails` and want to override the alias used to generate your thumbnail on a per-field basis (as opposed to using the `ADMIN_THUMBNAIL_THUMBNAIL_ALIAS` setting; see below), you can use the `alias` argument to the decorator:
+
+```python
+@admin_thumbnails.thumbnail('image', alias='admin_thumbnail_alternative')
+```
+
+## Configuration
+
+### `ADMIN_THUMBNAIL_DEFAULT_LABEL`
+
+**Default:** `'Preview'`
+
+Setting this overrides the default column name / title used by thumbnails.
+
+### `ADMIN_THUMBNAIL_FIELD_SUFFIX`
+
+**Default:** `'_thumbnail'`
+
+Setting this overrides the suffix given to newly created thumbnail fields. Change if you have collision issues with other field names you want to use. Don't forget to update `list_display` and/or `fieldsets` in your `ModelAdmin` as necessary.
+
+### `ADMIN_THUMBNAIL_THUMBNAIL_ALIAS`
+
+**Default:** `'admin_thumbnail'`
+
+If `easy_thumbnails` is installed and available, any model field using `ThumbnailerImageField` will be resized using a thumbnail alias called `admin_thumbnail` if it's defined. You can either define this alias in your settings (more info from the `easy_thumbnails` documentation [here](https://easy-thumbnails.readthedocs.io/en/stable/usage/#thumbnail-aliases)) or supply a different alias name as the value of this setting.
+
+### `ADMIN_THUMBNAIL_STYLE`
+
+**Default:** `{'display': 'block', 'width': '100px', 'height': 'auto'}`
+
+A dictionary of CSS property/value pairs that will be added to the `style` attribute of any thumbnail image when output in the admin. Override to supply your own styles.
+
+### `ADMIN_THUMBNAIL_BACKGROUND_STYLE`
+
+**Default:** `{'background': '#000'}`
+
+A dictionary of CSS property/value pairs added when the `background=True` option is used (see **Usage** above). Override to supply your own styles. Note that these styles are used _in addition_ to any defined in `ADMIN_THUMBNAIL_STYLE`.
+
+## Development installation
+
+If working locally on the package you can install the development tools via `pip`:
+
+```shell
+$ pip install -e .[dev]
+```
+
+To lint with `flake8`:
+
+```shell
+$ flake8
+```
+
+## Issues, suggestions, contributions
+
+...are welcome on GitHub. Thanks for your interest in `django-admin-thumbnails`!
```

### Comparing `django-admin-thumbnails-0.2.8/admin_thumbnails/__init__.py` & `django-admin-thumbnails-0.2.9/admin_thumbnails/__init__.py`

 * *Files identical despite different names*

### Comparing `django-admin-thumbnails-0.2.8/admin_thumbnails/settings.py` & `django-admin-thumbnails-0.2.9/admin_thumbnails/settings.py`

 * *Files identical despite different names*

### Comparing `django-admin-thumbnails-0.2.8/README.md` & `django-admin-thumbnails-0.2.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -98,16 +98,17 @@
 As of version 0.2.7, the name passed to the `thumbnail` decorator can refer to a property on the model rather than a field. For example:
 
 ```python
 class Person(models.Model):
     # ...
     @property
     def primary_image(self):
-        if self.images.count():
-            return self.images.first().image
+        first_image = self.images.first()
+        if first_image:
+            return first_image.image
         return None
 ```
 
 Provided the specified property returns an instance of a `FieldFile` (i.e. a file stored in a field that is an instance of Django's `ImageField`, `FileField`, or `easy_thumbnails`' `ThumbnailerImageField`), this will work as normal.
 
 This also works with Django's [`cached_property`](https://docs.djangoproject.com/en/dev/ref/utils/#django.utils.functional.cached_property) decorator.
```

### Comparing `django-admin-thumbnails-0.2.8/setup.py` & `django-admin-thumbnails-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     4. $ git tag -a x.x.x  # see `git tags` for latest
     5. $ git push origin master
     6. $ git push --tags
     7. $ python setup.py register sdist
     8. $ twine upload dist/*
 '''
 
-VERSION = '.'.join(('0', '2', '8'))
+VERSION = '.'.join(('0', '2', '9'))
 
 DESCRIPTION = 'A Django app for DRY thumbnails in admin list views and forms.'
 
 CLASSIFIERS = [
     'Development Status :: 4 - Beta',
     'Environment :: Web Environment',
     'Intended Audience :: Developers',
```

