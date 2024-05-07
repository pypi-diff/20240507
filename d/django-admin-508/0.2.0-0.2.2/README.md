# Comparing `tmp/django-admin-508-0.2.0.tar.gz` & `tmp/django_admin_508-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-508-0.2.0.tar", last modified: Thu Apr 14 17:21:21 2022, max compression
+gzip compressed data, was "django_admin_508-0.2.2.tar", last modified: Tue May  7 21:05:57 2024, max compression
```

## Comparing `django-admin-508-0.2.0.tar` & `django_admin_508-0.2.2.tar`

### file list

```diff
@@ -1,146 +1,151 @@
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.072449 django-admin-508-0.2.0/
--rw-r--r--   0 jorge      (501) staff       (20)     1182 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/LICENSE.txt
--rw-r--r--   0 jorge      (501) staff       (20)      121 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/MANIFEST.in
--rw-r--r--   0 jorge      (501) staff       (20)     4079 2022-04-14 17:21:21.072672 django-admin-508-0.2.0/PKG-INFO
--rw-r--r--   0 jorge      (501) staff       (20)     2328 2022-01-05 18:14:54.000000 django-admin-508-0.2.0/README.md
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.019696 django-admin-508-0.2.0/admin_interface/
--rw-r--r--   0 jorge      (501) staff       (20)       90 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/__init__.py
--rw-r--r--   0 jorge      (501) staff       (20)     3858 2022-04-01 18:11:24.000000 django-admin-508-0.2.0/admin_interface/admin.py
--rw-r--r--   0 jorge      (501) staff       (20)      569 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/apps.py
--rw-r--r--   0 jorge      (501) staff       (20)      471 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/cache.py
--rw-r--r--   0 jorge      (501) staff       (20)      469 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/compat.py
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.019938 django-admin-508-0.2.0/admin_interface/fixtures/
--rw-r--r--   0 jorge      (501) staff       (20)     1592 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/fixtures/admin_interface_theme_uswds.json
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.012560 django-admin-508-0.2.0/admin_interface/locale/
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.011850 django-admin-508-0.2.0/admin_interface/locale/es/
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.020661 django-admin-508-0.2.0/admin_interface/locale/es/LC_MESSAGES/
--rw-r--r--   0 jorge      (501) staff       (20)     2289 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 jorge      (501) staff       (20)     5035 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.012054 django-admin-508-0.2.0/admin_interface/locale/fa/
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.021335 django-admin-508-0.2.0/admin_interface/locale/fa/LC_MESSAGES/
--rw-r--r--   0 jorge      (501) staff       (20)     2994 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 jorge      (501) staff       (20)     5392 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.012246 django-admin-508-0.2.0/admin_interface/locale/fr/
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.021989 django-admin-508-0.2.0/admin_interface/locale/fr/LC_MESSAGES/
--rw-r--r--   0 jorge      (501) staff       (20)     2688 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 jorge      (501) staff       (20)     5143 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.012439 django-admin-508-0.2.0/admin_interface/locale/it/
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.022618 django-admin-508-0.2.0/admin_interface/locale/it/LC_MESSAGES/
--rw-r--r--   0 jorge      (501) staff       (20)     2855 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 jorge      (501) staff       (20)     5171 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.012632 django-admin-508-0.2.0/admin_interface/locale/tr/
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.023251 django-admin-508-0.2.0/admin_interface/locale/tr/LC_MESSAGES/
--rw-r--r--   0 jorge      (501) staff       (20)     2903 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 jorge      (501) staff       (20)     5257 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.023887 django-admin-508-0.2.0/admin_interface/migrations/
--rw-r--r--   0 jorge      (501) staff       (20)     7629 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/migrations/0001_initial.py
--rw-r--r--   0 jorge      (501) staff       (20)        0 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/migrations/__init__.py
--rw-r--r--   0 jorge      (501) staff       (20)    10069 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/models.py
--rw-r--r--   0 jorge      (501) staff       (20)      966 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/settings.py
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.013792 django-admin-508-0.2.0/admin_interface/static/
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.013132 django-admin-508-0.2.0/admin_interface/static/admin/
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.025572 django-admin-508-0.2.0/admin_interface/static/admin/css/
--rw-r--r--   0 jorge      (501) staff       (20)    16522 2022-04-13 15:24:14.000000 django-admin-508-0.2.0/admin_interface/static/admin/css/base.css
--rw-r--r--   0 jorge      (501) staff       (20)     7001 2022-04-13 15:19:41.000000 django-admin-508-0.2.0/admin_interface/static/admin/css/changelists.css
--rw-r--r--   0 jorge      (501) staff       (20)     3392 2022-04-13 15:15:26.000000 django-admin-508-0.2.0/admin_interface/static/admin/css/nav_sidebar.css
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.027992 django-admin-508-0.2.0/admin_interface/static/admin/js/
--rw-r--r--   0 jorge      (501) staff       (20)     7157 2022-04-05 14:05:15.000000 django-admin-508-0.2.0/admin_interface/static/admin/js/actions.js
--rw-r--r--   0 jorge      (501) staff       (20)      728 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/admin/js/cancel.js
--rw-r--r--   0 jorge      (501) staff       (20)     3184 2022-03-29 17:39:33.000000 django-admin-508-0.2.0/admin_interface/static/admin/js/nav_sidebar.js
--rw-r--r--   0 jorge      (501) staff       (20)     1839 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/admin/js/popup_response.js
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.013664 django-admin-508-0.2.0/admin_interface/static/admin_interface/
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.031745 django-admin-508-0.2.0/admin_interface/static/admin_interface/508/
--rw-r--r--   0 jorge      (501) staff       (20)      432 2021-10-19 18:23:52.000000 django-admin-508-0.2.0/admin_interface/static/admin_interface/508/actions.js
--rw-r--r--   0 jorge      (501) staff       (20)      909 2021-09-29 20:34:32.000000 django-admin-508-0.2.0/admin_interface/static/admin_interface/508/dropdown-filter.js
--rw-r--r--   0 jorge      (501) staff       (20)      593 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/admin_interface/508/error-alert.js
--rw-r--r--   0 jorge      (501) staff       (20)      712 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/admin_interface/508/form-labels.js
--rw-r--r--   0 jorge      (501) staff       (20)      847 2022-01-05 19:33:14.000000 django-admin-508-0.2.0/admin_interface/static/admin_interface/508/help-tooltip.js
--rw-r--r--   0 jorge      (501) staff       (20)      798 2022-03-29 17:39:33.000000 django-admin-508-0.2.0/admin_interface/static/admin_interface/508/required-field-error.js
--rw-r--r--   0 jorge      (501) staff       (20)      959 2021-09-01 14:11:29.000000 django-admin-508-0.2.0/admin_interface/static/admin_interface/508/table-checkboxes.js
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.032864 django-admin-508-0.2.0/admin_interface/static/admin_interface/favico/
--rw-r--r--   0 jorge      (501) staff       (20)    30766 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/admin_interface/favico/favico-0.3.10-patched.js
--rw-r--r--   0 jorge      (501) staff       (20)     9302 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/admin_interface/favico/favico-0.3.10-patched.min.js
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.034071 django-admin-508-0.2.0/admin_interface/static/admin_interface/magnific-popup/
--rwxr-xr-x   0 jorge      (501) staff       (20)    60830 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/admin_interface/magnific-popup/jquery.magnific-popup.js
--rwxr-xr-x   0 jorge      (501) staff       (20)     6951 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/admin_interface/magnific-popup/magnific-popup.css
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.034681 django-admin-508-0.2.0/admin_interface/static/admin_interface/related-modal/
--rw-r--r--   0 jorge      (501) staff       (20)     6324 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/admin_interface/related-modal/related-modal.js
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.013864 django-admin-508-0.2.0/admin_interface/static/ckeditor/
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.013937 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.014008 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.040808 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/
--rw-r--r--   0 jorge      (501) staff       (20)     1072 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/LICENSE
--rw-r--r--   0 jorge      (501) staff       (20)       42 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/README.md
--rw-r--r--   0 jorge      (501) staff       (20)      265 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/bower.json
--rw-r--r--   0 jorge      (501) staff       (20)    15856 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/dialog.css
--rw-r--r--   0 jorge      (501) staff       (20)    36243 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/editor.css
--rw-r--r--   0 jorge      (501) staff       (20)    34639 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/editor_gecko.css
--rw-r--r--   0 jorge      (501) staff       (20)    36187 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/editor_ie.css
--rw-r--r--   0 jorge      (501) staff       (20)    38212 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/editor_ie7.css
--rw-r--r--   0 jorge      (501) staff       (20)    36362 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/editor_ie8.css
--rw-r--r--   0 jorge      (501) staff       (20)    22758 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/icons.png
--rw-r--r--   0 jorge      (501) staff       (20)    33069 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/icons_hidpi.png
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.042585 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/images/
--rw-r--r--   0 jorge      (501) staff       (20)      261 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/images/arrow.png
--rw-r--r--   0 jorge      (501) staff       (20)      824 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/images/close.png
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.044215 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/
--rw-r--r--   0 jorge      (501) staff       (20)     1792 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/close.png
--rw-r--r--   0 jorge      (501) staff       (20)     1503 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/lock-open.png
--rw-r--r--   0 jorge      (501) staff       (20)     1616 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/lock.png
--rw-r--r--   0 jorge      (501) staff       (20)     2320 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/refresh.png
--rw-r--r--   0 jorge      (501) staff       (20)      736 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/images/lock-open.png
--rw-r--r--   0 jorge      (501) staff       (20)      728 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/images/lock.png
--rw-r--r--   0 jorge      (501) staff       (20)      953 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/images/refresh.png
--rw-r--r--   0 jorge      (501) staff       (20)    14994 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/skin.js
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.014669 django-admin-508-0.2.0/admin_interface/templates/
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.049516 django-admin-508-0.2.0/admin_interface/templates/admin/
--rw-r--r--   0 jorge      (501) staff       (20)     1313 2022-04-04 15:43:56.000000 django-admin-508-0.2.0/admin_interface/templates/admin/actions.html
--rw-r--r--   0 jorge      (501) staff       (20)     4599 2022-03-14 18:31:11.000000 django-admin-508-0.2.0/admin_interface/templates/admin/base.html
--rw-r--r--   0 jorge      (501) staff       (20)     3657 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/templates/admin/base_site.html
--rw-r--r--   0 jorge      (501) staff       (20)     3278 2022-04-04 15:48:20.000000 django-admin-508-0.2.0/admin_interface/templates/admin/change_form.html
--rw-r--r--   0 jorge      (501) staff       (20)     3457 2022-04-13 14:38:07.000000 django-admin-508-0.2.0/admin_interface/templates/admin/change_list.html
--rw-r--r--   0 jorge      (501) staff       (20)     1899 2021-10-19 18:21:28.000000 django-admin-508-0.2.0/admin_interface/templates/admin/change_list_results.html
--rw-r--r--   0 jorge      (501) staff       (20)      658 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/templates/admin/filter.html
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.050135 django-admin-508-0.2.0/admin_interface/templates/admin/includes/
--rw-r--r--   0 jorge      (501) staff       (20)     1787 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/templates/admin/includes/fieldset.html
--rw-r--r--   0 jorge      (501) staff       (20)      750 2022-04-04 15:48:20.000000 django-admin-508-0.2.0/admin_interface/templates/admin/nav_sidebar.html
--rw-r--r--   0 jorge      (501) staff       (20)      603 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/templates/admin/popup_response.html
--rw-r--r--   0 jorge      (501) staff       (20)     1214 2021-09-29 20:47:34.000000 django-admin-508-0.2.0/admin_interface/templates/admin/search_form.html
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.056902 django-admin-508-0.2.0/admin_interface/templates/admin_interface/
--rw-r--r--   0 jorge      (501) staff       (20)      134 2021-09-29 20:00:07.000000 django-admin-508-0.2.0/admin_interface/templates/admin_interface/actions_fix.html
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.067372 django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/
--rw-r--r--   0 jorge      (501) staff       (20)    14520 2022-04-13 15:01:11.000000 django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/admin-interface-fix.css
--rw-r--r--   0 jorge      (501) staff       (20)    20082 2022-03-14 18:31:11.000000 django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/admin-interface.css
--rw-r--r--   0 jorge      (501) staff       (20)     2719 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/ckeditor.css
--rw-r--r--   0 jorge      (501) staff       (20)     2425 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/form-controls.css
--rw-r--r--   0 jorge      (501) staff       (20)     5289 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/jquery.ui.tabs.css
--rw-r--r--   0 jorge      (501) staff       (20)      940 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/json-widget.css
--rw-r--r--   0 jorge      (501) staff       (20)      215 2022-04-13 14:40:33.000000 django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/list-filter-dropdown.css
--rw-r--r--   0 jorge      (501) staff       (20)      356 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/modeltranslation.css
--rw-r--r--   0 jorge      (501) staff       (20)      215 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/recent-actions.css
--rw-r--r--   0 jorge      (501) staff       (20)     2869 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/related-modal.css
--rw-r--r--   0 jorge      (501) staff       (20)     1016 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/rtl.css
--rw-r--r--   0 jorge      (501) staff       (20)     1451 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/sorl-thumbnail.css
--rw-r--r--   0 jorge      (501) staff       (20)      853 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/tabbed-admin.css
--rw-r--r--   0 jorge      (501) staff       (20)       77 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/tinymce.css
--rw-r--r--   0 jorge      (501) staff       (20)      443 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/templates/admin_interface/dropdown_filter.html
--rw-r--r--   0 jorge      (501) staff       (20)      142 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/templates/admin_interface/dropdown_filter_fix.html
--rw-r--r--   0 jorge      (501) staff       (20)      138 2022-02-02 14:35:14.000000 django-admin-508-0.2.0/admin_interface/templates/admin_interface/error-alert.html
--rw-r--r--   0 jorge      (501) staff       (20)      498 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/templates/admin_interface/favicon.html
--rw-r--r--   0 jorge      (501) staff       (20)      138 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/templates/admin_interface/form-labels.html
--rw-r--r--   0 jorge      (501) staff       (20)      139 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/templates/admin_interface/help-tooltip.html
--rw-r--r--   0 jorge      (501) staff       (20)      982 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/templates/admin_interface/language_chooser.html
--rw-r--r--   0 jorge      (501) staff       (20)      454 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/templates/admin_interface/related-modal.html
--rw-r--r--   0 jorge      (501) staff       (20)      143 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/templates/admin_interface/table-checkboxes.html
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.069394 django-admin-508-0.2.0/admin_interface/templatetags/
--rw-r--r--   0 jorge      (501) staff       (20)        0 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/admin_interface/templatetags/__init__.py
--rw-r--r--   0 jorge      (501) staff       (20)     2965 2022-02-28 14:41:19.000000 django-admin-508-0.2.0/admin_interface/templatetags/admin_interface_tags.py
--rw-r--r--   0 jorge      (501) staff       (20)       47 2022-04-13 15:17:17.000000 django-admin-508-0.2.0/admin_interface/version.py
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2022-04-14 17:21:21.072083 django-admin-508-0.2.0/django_admin_508.egg-info/
--rw-r--r--   0 jorge      (501) staff       (20)     4079 2022-04-14 17:21:20.000000 django-admin-508-0.2.0/django_admin_508.egg-info/PKG-INFO
--rw-r--r--   0 jorge      (501) staff       (20)     5773 2022-04-14 17:21:21.000000 django-admin-508-0.2.0/django_admin_508.egg-info/SOURCES.txt
--rw-r--r--   0 jorge      (501) staff       (20)        1 2022-04-14 17:21:20.000000 django-admin-508-0.2.0/django_admin_508.egg-info/dependency_links.txt
--rw-r--r--   0 jorge      (501) staff       (20)      107 2022-04-14 17:21:20.000000 django-admin-508-0.2.0/django_admin_508.egg-info/requires.txt
--rw-r--r--   0 jorge      (501) staff       (20)       16 2022-04-14 17:21:20.000000 django-admin-508-0.2.0/django_admin_508.egg-info/top_level.txt
--rw-r--r--   0 jorge      (501) staff       (20)       79 2022-04-14 17:21:21.073426 django-admin-508-0.2.0/setup.cfg
--rw-r--r--   0 jorge      (501) staff       (20)     2848 2021-08-31 13:55:10.000000 django-admin-508-0.2.0/setup.py
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.045901 django_admin_508-0.2.2/
+-rw-r--r--   0 msohani    (501) staff       (20)     1182 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/LICENSE.txt
+-rw-r--r--   0 msohani    (501) staff       (20)      121 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/MANIFEST.in
+-rw-r--r--   0 msohani    (501) staff       (20)     4226 2024-05-07 21:05:57.045828 django_admin_508-0.2.2/PKG-INFO
+-rw-r--r--   0 msohani    (501) staff       (20)     2328 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/README.md
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.013171 django_admin_508-0.2.2/admin_interface/
+-rw-r--r--   0 msohani    (501) staff       (20)       90 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/__init__.py
+-rw-r--r--   0 msohani    (501) staff       (20)     3858 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/admin.py
+-rw-r--r--   0 msohani    (501) staff       (20)      569 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/apps.py
+-rw-r--r--   0 msohani    (501) staff       (20)      471 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/cache.py
+-rw-r--r--   0 msohani    (501) staff       (20)      469 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/compat.py
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.013301 django_admin_508-0.2.2/admin_interface/fixtures/
+-rw-r--r--   0 msohani    (501) staff       (20)     1592 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/fixtures/admin_interface_theme_uswds.json
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.009937 django_admin_508-0.2.2/admin_interface/locale/
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.009508 django_admin_508-0.2.2/admin_interface/locale/es/
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.019370 django_admin_508-0.2.2/admin_interface/locale/es/LC_MESSAGES/
+-rw-r--r--   0 msohani    (501) staff       (20)     2289 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 msohani    (501) staff       (20)     5035 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.009630 django_admin_508-0.2.2/admin_interface/locale/fa/
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.019793 django_admin_508-0.2.2/admin_interface/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 msohani    (501) staff       (20)     2994 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 msohani    (501) staff       (20)     5392 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.009752 django_admin_508-0.2.2/admin_interface/locale/fr/
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.020491 django_admin_508-0.2.2/admin_interface/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 msohani    (501) staff       (20)     2688 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 msohani    (501) staff       (20)     5143 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.009871 django_admin_508-0.2.2/admin_interface/locale/it/
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.020790 django_admin_508-0.2.2/admin_interface/locale/it/LC_MESSAGES/
+-rw-r--r--   0 msohani    (501) staff       (20)     2855 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 msohani    (501) staff       (20)     5171 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.009990 django_admin_508-0.2.2/admin_interface/locale/tr/
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.021139 django_admin_508-0.2.2/admin_interface/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 msohani    (501) staff       (20)     2903 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 msohani    (501) staff       (20)     5257 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.021532 django_admin_508-0.2.2/admin_interface/migrations/
+-rw-r--r--   0 msohani    (501) staff       (20)     7629 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/migrations/0001_initial.py
+-rw-r--r--   0 msohani    (501) staff       (20)        0 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/migrations/__init__.py
+-rw-r--r--   0 msohani    (501) staff       (20)    10069 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/models.py
+-rw-r--r--   0 msohani    (501) staff       (20)      966 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/settings.py
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.010676 django_admin_508-0.2.2/admin_interface/static/
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.010304 django_admin_508-0.2.2/admin_interface/static/admin/
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.022194 django_admin_508-0.2.2/admin_interface/static/admin/css/
+-rw-r--r--   0 msohani    (501) staff       (20)    16522 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/admin/css/base.css
+-rw-r--r--   0 msohani    (501) staff       (20)     7001 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/admin/css/changelists.css
+-rw-r--r--   0 msohani    (501) staff       (20)     3392 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/admin/css/nav_sidebar.css
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.022929 django_admin_508-0.2.2/admin_interface/static/admin/js/
+-rw-r--r--   0 msohani    (501) staff       (20)     7157 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/admin/js/actions.js
+-rw-r--r--   0 msohani    (501) staff       (20)      728 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/admin/js/cancel.js
+-rw-r--r--   0 msohani    (501) staff       (20)     3184 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/admin/js/nav_sidebar.js
+-rw-r--r--   0 msohani    (501) staff       (20)     1839 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/admin/js/popup_response.js
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.010609 django_admin_508-0.2.2/admin_interface/static/admin_interface/
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.023893 django_admin_508-0.2.2/admin_interface/static/admin_interface/508/
+-rw-r--r--   0 msohani    (501) staff       (20)      432 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/admin_interface/508/actions.js
+-rw-r--r--   0 msohani    (501) staff       (20)      993 2024-05-07 20:51:09.000000 django_admin_508-0.2.2/admin_interface/static/admin_interface/508/dropdown-filter.js
+-rw-r--r--   0 msohani    (501) staff       (20)      593 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/admin_interface/508/error-alert.js
+-rw-r--r--   0 msohani    (501) staff       (20)      712 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/admin_interface/508/form-labels.js
+-rw-r--r--   0 msohani    (501) staff       (20)      847 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/admin_interface/508/help-tooltip.js
+-rw-r--r--   0 msohani    (501) staff       (20)      798 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/admin_interface/508/required-field-error.js
+-rw-r--r--   0 msohani    (501) staff       (20)      959 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/admin_interface/508/table-checkboxes.js
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.024450 django_admin_508-0.2.2/admin_interface/static/admin_interface/favico/
+-rw-r--r--   0 msohani    (501) staff       (20)    30766 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/admin_interface/favico/favico-0.3.10-patched.js
+-rw-r--r--   0 msohani    (501) staff       (20)     9302 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/admin_interface/favico/favico-0.3.10-patched.min.js
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.024931 django_admin_508-0.2.2/admin_interface/static/admin_interface/magnific-popup/
+-rwxr-xr-x   0 msohani    (501) staff       (20)    60830 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/admin_interface/magnific-popup/jquery.magnific-popup.js
+-rwxr-xr-x   0 msohani    (501) staff       (20)     6951 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/admin_interface/magnific-popup/magnific-popup.css
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.025169 django_admin_508-0.2.2/admin_interface/static/admin_interface/related-modal/
+-rw-r--r--   0 msohani    (501) staff       (20)     6324 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/admin_interface/related-modal/related-modal.js
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.010724 django_admin_508-0.2.2/admin_interface/static/ckeditor/
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.010779 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.010831 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.029792 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/
+-rw-r--r--   0 msohani    (501) staff       (20)     1072 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/LICENSE
+-rw-r--r--   0 msohani    (501) staff       (20)       42 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/README.md
+-rw-r--r--   0 msohani    (501) staff       (20)      265 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/bower.json
+-rw-r--r--   0 msohani    (501) staff       (20)    15856 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/dialog.css
+-rw-r--r--   0 msohani    (501) staff       (20)    36243 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/editor.css
+-rw-r--r--   0 msohani    (501) staff       (20)    34639 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/editor_gecko.css
+-rw-r--r--   0 msohani    (501) staff       (20)    36187 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/editor_ie.css
+-rw-r--r--   0 msohani    (501) staff       (20)    38212 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/editor_ie7.css
+-rw-r--r--   0 msohani    (501) staff       (20)    36362 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/editor_ie8.css
+-rw-r--r--   0 msohani    (501) staff       (20)    22758 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/icons.png
+-rw-r--r--   0 msohani    (501) staff       (20)    33069 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/icons_hidpi.png
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.031348 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/
+-rw-r--r--   0 msohani    (501) staff       (20)      261 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/arrow.png
+-rw-r--r--   0 msohani    (501) staff       (20)      824 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/close.png
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.032052 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/
+-rw-r--r--   0 msohani    (501) staff       (20)     1792 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/close.png
+-rw-r--r--   0 msohani    (501) staff       (20)     1503 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/lock-open.png
+-rw-r--r--   0 msohani    (501) staff       (20)     1616 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/lock.png
+-rw-r--r--   0 msohani    (501) staff       (20)     2320 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/refresh.png
+-rw-r--r--   0 msohani    (501) staff       (20)      736 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/lock-open.png
+-rw-r--r--   0 msohani    (501) staff       (20)      728 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/lock.png
+-rw-r--r--   0 msohani    (501) staff       (20)      953 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/refresh.png
+-rw-r--r--   0 msohani    (501) staff       (20)    14994 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/skin.js
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.011196 django_admin_508-0.2.2/admin_interface/templates/
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.034004 django_admin_508-0.2.2/admin_interface/templates/admin/
+-rw-r--r--   0 msohani    (501) staff       (20)     1313 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin/actions.html
+-rw-r--r--   0 msohani    (501) staff       (20)     4599 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin/base.html
+-rw-r--r--   0 msohani    (501) staff       (20)     3657 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin/base_site.html
+-rw-r--r--   0 msohani    (501) staff       (20)     3278 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin/change_form.html
+-rw-r--r--   0 msohani    (501) staff       (20)     3457 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin/change_list.html
+-rw-r--r--   0 msohani    (501) staff       (20)     1899 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin/change_list_results.html
+-rw-r--r--   0 msohani    (501) staff       (20)      658 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin/filter.html
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.034167 django_admin_508-0.2.2/admin_interface/templates/admin/includes/
+-rw-r--r--   0 msohani    (501) staff       (20)     1787 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin/includes/fieldset.html
+-rw-r--r--   0 msohani    (501) staff       (20)      750 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin/nav_sidebar.html
+-rw-r--r--   0 msohani    (501) staff       (20)      603 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin/popup_response.html
+-rw-r--r--   0 msohani    (501) staff       (20)     1214 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin/search_form.html
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.040905 django_admin_508-0.2.2/admin_interface/templates/admin_interface/
+-rw-r--r--   0 msohani    (501) staff       (20)      134 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin_interface/actions_fix.html
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.043430 django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/
+-rw-r--r--   0 msohani    (501) staff       (20)    14520 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/admin-interface-fix.css
+-rw-r--r--   0 msohani    (501) staff       (20)    20082 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/admin-interface.css
+-rw-r--r--   0 msohani    (501) staff       (20)     2719 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/ckeditor.css
+-rw-r--r--   0 msohani    (501) staff       (20)     2425 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/form-controls.css
+-rw-r--r--   0 msohani    (501) staff       (20)     5289 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/jquery.ui.tabs.css
+-rw-r--r--   0 msohani    (501) staff       (20)      940 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/json-widget.css
+-rw-r--r--   0 msohani    (501) staff       (20)      215 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/list-filter-dropdown.css
+-rw-r--r--   0 msohani    (501) staff       (20)      356 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/modeltranslation.css
+-rw-r--r--   0 msohani    (501) staff       (20)      215 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/recent-actions.css
+-rw-r--r--   0 msohani    (501) staff       (20)     2869 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/related-modal.css
+-rw-r--r--   0 msohani    (501) staff       (20)     1016 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/rtl.css
+-rw-r--r--   0 msohani    (501) staff       (20)     1451 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/sorl-thumbnail.css
+-rw-r--r--   0 msohani    (501) staff       (20)      853 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/tabbed-admin.css
+-rw-r--r--   0 msohani    (501) staff       (20)       77 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/tinymce.css
+-rw-r--r--   0 msohani    (501) staff       (20)      443 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin_interface/dropdown_filter.html
+-rw-r--r--   0 msohani    (501) staff       (20)      142 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin_interface/dropdown_filter_fix.html
+-rw-r--r--   0 msohani    (501) staff       (20)      138 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin_interface/error-alert.html
+-rw-r--r--   0 msohani    (501) staff       (20)      498 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin_interface/favicon.html
+-rw-r--r--   0 msohani    (501) staff       (20)      138 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin_interface/form-labels.html
+-rw-r--r--   0 msohani    (501) staff       (20)      139 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin_interface/help-tooltip.html
+-rw-r--r--   0 msohani    (501) staff       (20)      982 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin_interface/language_chooser.html
+-rw-r--r--   0 msohani    (501) staff       (20)      454 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin_interface/related-modal.html
+-rw-r--r--   0 msohani    (501) staff       (20)      143 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templates/admin_interface/table-checkboxes.html
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.043694 django_admin_508-0.2.2/admin_interface/templatetags/
+-rw-r--r--   0 msohani    (501) staff       (20)        0 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templatetags/__init__.py
+-rw-r--r--   0 msohani    (501) staff       (20)     2965 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/admin_interface/templatetags/admin_interface_tags.py
+-rw-r--r--   0 msohani    (501) staff       (20)       47 2024-05-07 20:59:27.000000 django_admin_508-0.2.2/admin_interface/version.py
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.045292 django_admin_508-0.2.2/django_admin_508.egg-info/
+-rw-r--r--   0 msohani    (501) staff       (20)     4226 2024-05-07 21:05:57.000000 django_admin_508-0.2.2/django_admin_508.egg-info/PKG-INFO
+-rw-r--r--   0 msohani    (501) staff       (20)     5867 2024-05-07 21:05:57.000000 django_admin_508-0.2.2/django_admin_508.egg-info/SOURCES.txt
+-rw-r--r--   0 msohani    (501) staff       (20)        1 2024-05-07 21:05:57.000000 django_admin_508-0.2.2/django_admin_508.egg-info/dependency_links.txt
+-rw-r--r--   0 msohani    (501) staff       (20)      107 2024-05-07 21:05:57.000000 django_admin_508-0.2.2/django_admin_508.egg-info/requires.txt
+-rw-r--r--   0 msohani    (501) staff       (20)       16 2024-05-07 21:05:57.000000 django_admin_508-0.2.2/django_admin_508.egg-info/top_level.txt
+-rw-r--r--   0 msohani    (501) staff       (20)       79 2024-05-07 21:05:57.046172 django_admin_508-0.2.2/setup.cfg
+-rw-r--r--   0 msohani    (501) staff       (20)     2848 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/setup.py
+drwxr-xr-x   0 msohani    (501) staff       (20)        0 2024-05-07 21:05:57.044925 django_admin_508-0.2.2/tests/
+-rw-r--r--   0 msohani    (501) staff       (20)     1556 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/tests/test_fixtures.py
+-rw-r--r--   0 msohani    (501) staff       (20)     3477 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/tests/test_models.py
+-rw-r--r--   0 msohani    (501) staff       (20)     2581 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/tests/test_settings.py
+-rw-r--r--   0 msohani    (501) staff       (20)     4323 2024-05-07 16:25:54.000000 django_admin_508-0.2.2/tests/test_templatetags.py
```

### Comparing `django-admin-508-0.2.0/LICENSE.txt` & `django_admin_508-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/PKG-INFO` & `django_admin_508-0.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: django-admin-508
-Version: 0.2.0
+Version: 0.2.2
 Summary: django-admin-508 is a modern responsive django admin interface.
 Home-page: https://github.com/raft-tech/django-admin-508
-Download-URL: https://github.com/raft-tech/django-admin-508/archive/0.2.0.tar.gz
+Download-URL: https://github.com/raft-tech/django-admin-508/archive/0.2.2.tar.gz
 Author: Raft
 Author-email: info@goraft.tech
 License: MIT
 Keywords: django,admin,interface,responsive,flat,theme,custom,ui
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.7
 Classifier: Framework :: Django :: 1.8
 Classifier: Framework :: Django :: 1.9
 Classifier: Framework :: Django :: 1.10
@@ -36,14 +35,18 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Build Tools
 Requires: django(>=1.7)
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: django-colorfield<1.0,>=0.2
+Requires-Dist: django-flat-theme<2.0,>=1.0
+Requires-Dist: django-flat-responsive<3.0,>=1.0
+Requires-Dist: six<2.0.0,>=1.9.0
 
 
 [![](https://img.shields.io/pypi/pyversions/django-admin-508.svg?color=3776AB&logo=python&logoColor=white)](https://www.python.org/)
 [![](https://img.shields.io/pypi/djversions/django-admin-508?color=0C4B33&logo=django&logoColor=white&label=django)](https://www.djangoproject.com/)
 
 [![](https://img.shields.io/pypi/v/django-admin-508.svg?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/django-admin-508/)
 [![](https://img.shields.io/pypi/l/django-admin-508.svg?color=blue)](https://github.com/raft-tech/django-admin-508/blob/main/LICENSE.txt)
@@ -128,9 +131,7 @@
 
 ## License
 Released under [MIT License](LICENSE.txt).
 
 ## See also
 
 This project started out as a fork of the excellent [Django Admin Interface](https://github.com/fabiocaccamo/django-admin-interface).
-
-
```

### Comparing `django-admin-508-0.2.0/README.md` & `django_admin_508-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/admin.py` & `django_admin_508-0.2.2/admin_interface/admin.py`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/apps.py` & `django_admin_508-0.2.2/admin_interface/apps.py`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/fixtures/admin_interface_theme_uswds.json` & `django_admin_508-0.2.2/admin_interface/fixtures/admin_interface_theme_uswds.json`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/locale/es/LC_MESSAGES/django.mo` & `django_admin_508-0.2.2/admin_interface/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/locale/es/LC_MESSAGES/django.po` & `django_admin_508-0.2.2/admin_interface/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/locale/fa/LC_MESSAGES/django.mo` & `django_admin_508-0.2.2/admin_interface/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/locale/fa/LC_MESSAGES/django.po` & `django_admin_508-0.2.2/admin_interface/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/locale/fr/LC_MESSAGES/django.mo` & `django_admin_508-0.2.2/admin_interface/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/locale/fr/LC_MESSAGES/django.po` & `django_admin_508-0.2.2/admin_interface/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/locale/it/LC_MESSAGES/django.mo` & `django_admin_508-0.2.2/admin_interface/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/locale/it/LC_MESSAGES/django.po` & `django_admin_508-0.2.2/admin_interface/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/locale/tr/LC_MESSAGES/django.mo` & `django_admin_508-0.2.2/admin_interface/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/locale/tr/LC_MESSAGES/django.po` & `django_admin_508-0.2.2/admin_interface/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/migrations/0001_initial.py` & `django_admin_508-0.2.2/admin_interface/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/models.py` & `django_admin_508-0.2.2/admin_interface/models.py`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/settings.py` & `django_admin_508-0.2.2/admin_interface/settings.py`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/admin/css/base.css` & `django_admin_508-0.2.2/admin_interface/static/admin/css/base.css`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/admin/css/changelists.css` & `django_admin_508-0.2.2/admin_interface/static/admin/css/changelists.css`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/admin/css/nav_sidebar.css` & `django_admin_508-0.2.2/admin_interface/static/admin/css/nav_sidebar.css`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/admin/js/actions.js` & `django_admin_508-0.2.2/admin_interface/static/admin/js/actions.js`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/admin/js/cancel.js` & `django_admin_508-0.2.2/admin_interface/static/admin/js/cancel.js`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/admin/js/nav_sidebar.js` & `django_admin_508-0.2.2/admin_interface/static/admin/js/nav_sidebar.js`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/admin/js/popup_response.js` & `django_admin_508-0.2.2/admin_interface/static/admin/js/popup_response.js`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/admin_interface/508/dropdown-filter.js` & `django_admin_508-0.2.2/admin_interface/static/admin_interface/508/dropdown-filter.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,18 @@
         $(document).ready(function() {
             const filters = document.querySelectorAll('#changelist-filter .list-filter-dropdown select')
             let options = ''
             // Override the default onchange handler of each filter
             for (const filter of filters) {
                 // This needs to be a function expression so `this` references the filter elements themselves
                 filter.onchange = function() {
-                    const value = this.options[this.selectedIndex].value
+                    let value = this.options[this.selectedIndex].value
+                    if (options !== '') {
+                        value = value.replace('?', '&')
+                    }
                     options = options.concat(value)
                 };
             }
 
             const applyFiltersButton = document.querySelector('#submit-filters');
             if (applyFiltersButton) {
                 applyFiltersButton.onclick = function() {
```

### Comparing `django-admin-508-0.2.0/admin_interface/static/admin_interface/508/error-alert.js` & `django_admin_508-0.2.2/admin_interface/static/admin_interface/508/error-alert.js`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/admin_interface/508/form-labels.js` & `django_admin_508-0.2.2/admin_interface/static/admin_interface/508/form-labels.js`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/admin_interface/508/help-tooltip.js` & `django_admin_508-0.2.2/admin_interface/static/admin_interface/508/help-tooltip.js`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/admin_interface/508/required-field-error.js` & `django_admin_508-0.2.2/admin_interface/static/admin_interface/508/required-field-error.js`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/admin_interface/508/table-checkboxes.js` & `django_admin_508-0.2.2/admin_interface/static/admin_interface/508/table-checkboxes.js`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/admin_interface/favico/favico-0.3.10-patched.js` & `django_admin_508-0.2.2/admin_interface/static/admin_interface/favico/favico-0.3.10-patched.js`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/admin_interface/favico/favico-0.3.10-patched.min.js` & `django_admin_508-0.2.2/admin_interface/static/admin_interface/favico/favico-0.3.10-patched.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/admin_interface/magnific-popup/jquery.magnific-popup.js` & `django_admin_508-0.2.2/admin_interface/static/admin_interface/magnific-popup/jquery.magnific-popup.js`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/admin_interface/magnific-popup/magnific-popup.css` & `django_admin_508-0.2.2/admin_interface/static/admin_interface/magnific-popup/magnific-popup.css`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/admin_interface/related-modal/related-modal.js` & `django_admin_508-0.2.2/admin_interface/static/admin_interface/related-modal/related-modal.js`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/LICENSE` & `django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/dialog.css` & `django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/dialog.css`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/editor.css` & `django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/editor.css`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/editor_gecko.css` & `django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/editor_gecko.css`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/editor_ie.css` & `django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/editor_ie.css`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/editor_ie7.css` & `django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/editor_ie7.css`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/editor_ie8.css` & `django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/editor_ie8.css`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/icons.png` & `django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/icons.png`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/icons_hidpi.png` & `django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/icons_hidpi.png`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/images/close.png` & `django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/close.png`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/close.png` & `django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/close.png`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/lock-open.png` & `django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/lock-open.png`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/lock.png` & `django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/lock.png`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/refresh.png` & `django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/hidpi/refresh.png`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/images/lock-open.png` & `django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/lock-open.png`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/images/lock.png` & `django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/lock.png`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/images/refresh.png` & `django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/images/refresh.png`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/static/ckeditor/ckeditor/skins/light/skin.js` & `django_admin_508-0.2.2/admin_interface/static/ckeditor/ckeditor/skins/light/skin.js`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/templates/admin/actions.html` & `django_admin_508-0.2.2/admin_interface/templates/admin/actions.html`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/templates/admin/base.html` & `django_admin_508-0.2.2/admin_interface/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/templates/admin/base_site.html` & `django_admin_508-0.2.2/admin_interface/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/templates/admin/change_form.html` & `django_admin_508-0.2.2/admin_interface/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/templates/admin/change_list.html` & `django_admin_508-0.2.2/admin_interface/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/templates/admin/change_list_results.html` & `django_admin_508-0.2.2/admin_interface/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/templates/admin/filter.html` & `django_admin_508-0.2.2/admin_interface/templates/admin/filter.html`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/templates/admin/includes/fieldset.html` & `django_admin_508-0.2.2/admin_interface/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/templates/admin/nav_sidebar.html` & `django_admin_508-0.2.2/admin_interface/templates/admin/nav_sidebar.html`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/templates/admin/popup_response.html` & `django_admin_508-0.2.2/admin_interface/templates/admin/popup_response.html`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/templates/admin/search_form.html` & `django_admin_508-0.2.2/admin_interface/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/admin-interface-fix.css` & `django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/admin-interface-fix.css`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/admin-interface.css` & `django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/admin-interface.css`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/ckeditor.css` & `django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/ckeditor.css`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/form-controls.css` & `django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/form-controls.css`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/jquery.ui.tabs.css` & `django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/jquery.ui.tabs.css`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/json-widget.css` & `django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/json-widget.css`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/related-modal.css` & `django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/related-modal.css`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/rtl.css` & `django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/rtl.css`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/sorl-thumbnail.css` & `django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/sorl-thumbnail.css`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/templates/admin_interface/css/tabbed-admin.css` & `django_admin_508-0.2.2/admin_interface/templates/admin_interface/css/tabbed-admin.css`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/templates/admin_interface/language_chooser.html` & `django_admin_508-0.2.2/admin_interface/templates/admin_interface/language_chooser.html`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/admin_interface/templatetags/admin_interface_tags.py` & `django_admin_508-0.2.2/admin_interface/templatetags/admin_interface_tags.py`

 * *Files identical despite different names*

### Comparing `django-admin-508-0.2.0/django_admin_508.egg-info/PKG-INFO` & `django_admin_508-0.2.2/django_admin_508.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: django-admin-508
-Version: 0.2.0
+Version: 0.2.2
 Summary: django-admin-508 is a modern responsive django admin interface.
 Home-page: https://github.com/raft-tech/django-admin-508
-Download-URL: https://github.com/raft-tech/django-admin-508/archive/0.2.0.tar.gz
+Download-URL: https://github.com/raft-tech/django-admin-508/archive/0.2.2.tar.gz
 Author: Raft
 Author-email: info@goraft.tech
 License: MIT
 Keywords: django,admin,interface,responsive,flat,theme,custom,ui
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.7
 Classifier: Framework :: Django :: 1.8
 Classifier: Framework :: Django :: 1.9
 Classifier: Framework :: Django :: 1.10
@@ -36,14 +35,18 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Build Tools
 Requires: django(>=1.7)
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: django-colorfield<1.0,>=0.2
+Requires-Dist: django-flat-theme<2.0,>=1.0
+Requires-Dist: django-flat-responsive<3.0,>=1.0
+Requires-Dist: six<2.0.0,>=1.9.0
 
 
 [![](https://img.shields.io/pypi/pyversions/django-admin-508.svg?color=3776AB&logo=python&logoColor=white)](https://www.python.org/)
 [![](https://img.shields.io/pypi/djversions/django-admin-508?color=0C4B33&logo=django&logoColor=white&label=django)](https://www.djangoproject.com/)
 
 [![](https://img.shields.io/pypi/v/django-admin-508.svg?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/django-admin-508/)
 [![](https://img.shields.io/pypi/l/django-admin-508.svg?color=blue)](https://github.com/raft-tech/django-admin-508/blob/main/LICENSE.txt)
@@ -128,9 +131,7 @@
 
 ## License
 Released under [MIT License](LICENSE.txt).
 
 ## See also
 
 This project started out as a fork of the excellent [Django Admin Interface](https://github.com/fabiocaccamo/django-admin-interface).
-
-
```

### Comparing `django-admin-508-0.2.0/django_admin_508.egg-info/SOURCES.txt` & `django_admin_508-0.2.2/django_admin_508.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -101,8 +101,12 @@
 admin_interface/templates/admin_interface/css/tinymce.css
 admin_interface/templatetags/__init__.py
 admin_interface/templatetags/admin_interface_tags.py
 django_admin_508.egg-info/PKG-INFO
 django_admin_508.egg-info/SOURCES.txt
 django_admin_508.egg-info/dependency_links.txt
 django_admin_508.egg-info/requires.txt
-django_admin_508.egg-info/top_level.txt
+django_admin_508.egg-info/top_level.txt
+tests/test_fixtures.py
+tests/test_models.py
+tests/test_settings.py
+tests/test_templatetags.py
```

### Comparing `django-admin-508-0.2.0/setup.py` & `django_admin_508-0.2.2/setup.py`

 * *Files identical despite different names*

