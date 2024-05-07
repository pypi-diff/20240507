# Comparing `tmp/django_cms_articles-2.0.3.tar.gz` & `tmp/django_cms_articles-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_cms_articles-2.0.3.tar", max compression
+gzip compressed data, was "django_cms_articles-2.1.0.tar", max compression
```

## Comparing `django_cms_articles-2.0.3.tar` & `django_cms_articles-2.1.0.tar`

### file list

```diff
@@ -1,83 +1,84 @@
--rw-r--r--   0        0        0     1507 2022-09-20 10:23:53.365187 django_cms_articles-2.0.3/LICENSE
--rw-r--r--   0        0        0     1189 2022-09-20 10:23:53.365187 django_cms_articles-2.0.3/README.md
--rw-r--r--   0        0        0       59 2022-09-20 11:07:46.821205 django_cms_articles-2.0.3/cms_articles/__init__.py
--rw-r--r--   0        0        0       93 2022-09-20 10:23:53.365187 django_cms_articles-2.0.3/cms_articles/admin/__init__.py
--rw-r--r--   0        0        0    19135 2022-12-30 15:26:17.765974 django_cms_articles-2.0.3/cms_articles/admin/article.py
--rw-r--r--   0        0        0      277 2022-09-20 10:23:53.365187 django_cms_articles-2.0.3/cms_articles/admin/attribute.py
--rw-r--r--   0        0        0      224 2022-09-20 11:07:46.825205 django_cms_articles-2.0.3/cms_articles/admin/category.py
--rw-r--r--   0        0        0     3029 2022-12-30 15:25:49.465921 django_cms_articles-2.0.3/cms_articles/admin/forms.py
--rw-r--r--   0        0        0     5230 2022-09-22 22:13:29.570734 django_cms_articles-2.0.3/cms_articles/api.py
--rw-r--r--   0        0        0      281 2022-09-22 21:48:17.595607 django_cms_articles-2.0.3/cms_articles/apps.py
--rw-r--r--   0        0        0     4409 2022-09-20 11:07:47.037209 django_cms_articles-2.0.3/cms_articles/archive.py
--rw-r--r--   0        0        0     1526 2022-09-20 11:07:46.993208 django_cms_articles-2.0.3/cms_articles/article_rendering.py
--rw-r--r--   0        0        0      359 2022-09-22 21:48:17.595607 django_cms_articles-2.0.3/cms_articles/cms_apps.py
--rw-r--r--   0        0        0     2628 2022-09-22 21:56:11.181288 django_cms_articles-2.0.3/cms_articles/cms_plugins.py
--rw-r--r--   0        0        0     2724 2022-09-22 21:48:17.595607 django_cms_articles-2.0.3/cms_articles/cms_toolbars.py
--rw-r--r--   0        0        0      485 2022-09-20 11:07:47.053209 django_cms_articles-2.0.3/cms_articles/conf/__init__.py
--rw-r--r--   0        0        0      830 2022-09-22 21:48:17.595607 django_cms_articles-2.0.3/cms_articles/conf/default_settings.py
--rw-r--r--   0        0        0       91 2022-09-20 11:07:47.077209 django_cms_articles-2.0.3/cms_articles/import_wordpress/__init__.py
--rw-r--r--   0        0        0     9644 2022-12-30 15:25:23.225873 django_cms_articles-2.0.3/cms_articles/import_wordpress/admin.py
--rw-r--r--   0        0        0      253 2022-09-22 21:48:17.595607 django_cms_articles-2.0.3/cms_articles/import_wordpress/apps.py
--rw-r--r--   0        0        0      655 2022-09-22 21:48:17.595607 django_cms_articles-2.0.3/cms_articles/import_wordpress/forms.py
--rw-r--r--   0        0        0        0 2022-09-20 10:23:53.369187 django_cms_articles-2.0.3/cms_articles/import_wordpress/management/__init__.py
--rw-r--r--   0        0        0        0 2022-09-20 10:23:53.369187 django_cms_articles-2.0.3/cms_articles/import_wordpress/management/commands/__init__.py
--rw-r--r--   0        0        0      943 2022-09-20 11:11:49.856420 django_cms_articles-2.0.3/cms_articles/import_wordpress/management/commands/cms_import_wordpress.py
--rw-r--r--   0        0        0    13535 2022-09-22 23:04:36.720295 django_cms_articles-2.0.3/cms_articles/import_wordpress/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-09-20 10:23:53.369187 django_cms_articles-2.0.3/cms_articles/import_wordpress/migrations/__init__.py
--rw-r--r--   0        0        0    14429 2022-09-22 23:06:50.591246 django_cms_articles-2.0.3/cms_articles/import_wordpress/models.py
--rw-r--r--   0        0        0     2194 2022-09-20 10:23:53.369187 django_cms_articles-2.0.3/cms_articles/import_wordpress/templates/cms_articles/import_wordpress/cms_import.html
--rw-r--r--   0        0        0     1098 2022-09-20 10:23:53.369187 django_cms_articles-2.0.3/cms_articles/import_wordpress/templates/cms_articles/import_wordpress/form.html
--rwxr-xr-x   0        0        0     7009 2022-09-20 11:07:47.345213 django_cms_articles-2.0.3/cms_articles/import_wordpress/utils.py
--rw-r--r--   0        0        0    11767 2022-09-20 10:23:53.373187 django_cms_articles-2.0.3/cms_articles/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18344 2022-09-20 10:23:53.373187 django_cms_articles-2.0.3/cms_articles/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    10495 2022-09-22 22:40:46.906000 django_cms_articles-2.0.3/cms_articles/migrations/0001_initial.py
--rw-r--r--   0        0        0      386 2022-09-22 22:40:46.605981 django_cms_articles-2.0.3/cms_articles/migrations/0002_remove_title_excerpt.py
--rw-r--r--   0        0        0     2254 2022-09-22 22:40:21.876400 django_cms_articles-2.0.3/cms_articles/migrations/0003_description_image.py
--rw-r--r--   0        0        0     4742 2022-09-22 22:40:46.821994 django_cms_articles-2.0.3/cms_articles/migrations/0004_categories.py
--rw-r--r--   0        0        0     1712 2022-09-22 22:40:46.693987 django_cms_articles-2.0.3/cms_articles/migrations/0005_attributes.py
--rw-r--r--   0        0        0     1282 2022-09-22 22:40:46.657984 django_cms_articles-2.0.3/cms_articles/migrations/0006_order_date.py
--rw-r--r--   0        0        0      971 2022-09-22 22:40:46.705987 django_cms_articles-2.0.3/cms_articles/migrations/0007_plugins.py
--rw-r--r--   0        0        0     2765 2022-09-22 22:40:46.817994 django_cms_articles-2.0.3/cms_articles/migrations/0008_cms_3_4.py
--rw-r--r--   0        0        0      997 2022-09-22 22:40:46.769991 django_cms_articles-2.0.3/cms_articles/migrations/0009_number_min_value.py
--rw-r--r--   0        0        0      402 2022-09-22 22:40:46.789992 django_cms_articles-2.0.3/cms_articles/migrations/0010_remove_article_revision_id.py
--rw-r--r--   0        0        0     1085 2022-09-22 22:40:46.833995 django_cms_articles-2.0.3/cms_articles/migrations/0011_attribute_site.py
--rw-r--r--   0        0        0     1327 2022-09-22 22:40:46.865997 django_cms_articles-2.0.3/cms_articles/migrations/0012_protect_keys.py
--rw-r--r--   0        0        0        0 2022-09-20 10:23:53.373187 django_cms_articles-2.0.3/cms_articles/migrations/__init__.py
--rw-r--r--   0        0        0      287 2022-09-20 10:23:53.373187 django_cms_articles-2.0.3/cms_articles/models/__init__.py
--rw-r--r--   0        0        0    23967 2022-12-30 15:26:47.710033 django_cms_articles-2.0.3/cms_articles/models/article.py
--rw-r--r--   0        0        0      619 2022-09-22 23:03:54.335412 django_cms_articles-2.0.3/cms_articles/models/attribute.py
--rw-r--r--   0        0        0      843 2023-11-25 22:48:33.472751 django_cms_articles-2.0.3/cms_articles/models/category.py
--rw-r--r--   0        0        0     4220 2022-09-20 11:07:47.569217 django_cms_articles-2.0.3/cms_articles/models/managers.py
--rw-r--r--   0        0        0     4540 2022-12-30 15:24:29.529780 django_cms_articles-2.0.3/cms_articles/models/plugins.py
--rw-r--r--   0        0        0      276 2022-09-20 11:07:47.581217 django_cms_articles-2.0.3/cms_articles/models/query.py
--rw-r--r--   0        0        0     4212 2022-12-30 15:23:52.297721 django_cms_articles-2.0.3/cms_articles/models/title.py
--rw-r--r--   0        0        0     4609 2022-12-30 13:29:58.468309 django_cms_articles-2.0.3/cms_articles/search_indexes.py
--rw-r--r--   0        0        0     1252 2022-09-22 22:28:00.384915 django_cms_articles-2.0.3/cms_articles/signals/__init__.py
--rw-r--r--   0        0        0      816 2022-09-20 11:07:47.813220 django_cms_articles-2.0.3/cms_articles/signals/article.py
--rw-r--r--   0        0        0     1939 2022-09-20 11:07:47.865221 django_cms_articles-2.0.3/cms_articles/signals/plugins.py
--rw-r--r--   0        0        0      892 2022-09-20 11:07:47.845221 django_cms_articles-2.0.3/cms_articles/signals/title.py
--rw-r--r--   0        0        0      717 2022-09-20 10:23:53.377187 django_cms_articles-2.0.3/cms_articles/static/cms_articles/css/changelist.css
--rw-r--r--   0        0        0     2262 2022-09-20 10:23:53.377187 django_cms_articles-2.0.3/cms_articles/static/cms_articles/js/changelist.js
--rw-r--r--   0        0        0      378 2022-12-29 16:48:51.328113 django_cms_articles-2.0.3/cms_articles/templates/admin/cms_articles/article/change_form.html
--rw-r--r--   0        0        0     3619 2022-09-20 10:23:53.377187 django_cms_articles-2.0.3/cms_articles/templates/admin/cms_articles/article/change_list_lang.html
--rw-r--r--   0        0        0      661 2022-09-20 10:23:53.377187 django_cms_articles-2.0.3/cms_articles/templates/admin/cms_articles/article/change_list_preview.html
--rw-r--r--   0        0        0      757 2022-12-29 16:48:51.328113 django_cms_articles-2.0.3/cms_articles/templates/admin/cms_articles/article_changelist.html
--rw-r--r--   0        0        0       77 2022-09-20 10:23:53.377187 django_cms_articles-2.0.3/cms_articles/templates/cms_articles/article/default.html
--rw-r--r--   0        0        0      558 2022-09-20 10:23:53.377187 django_cms_articles-2.0.3/cms_articles/templates/cms_articles/article_preview.html
--rw-r--r--   0        0        0     1144 2022-09-20 10:23:53.377187 django_cms_articles-2.0.3/cms_articles/templates/cms_articles/articles/default.html
--rw-r--r--   0        0        0     1219 2022-09-22 22:44:45.738639 django_cms_articles-2.0.3/cms_articles/templates/cms_articles/base.html
--rw-r--r--   0        0        0      730 2022-09-20 10:23:53.381187 django_cms_articles-2.0.3/cms_articles/templates/cms_articles/default.html
--rw-r--r--   0        0        0        0 2022-09-20 10:23:53.381187 django_cms_articles-2.0.3/cms_articles/templatetags/__init__.py
--rw-r--r--   0        0        0     8972 2022-12-30 15:23:35.569696 django_cms_articles-2.0.3/cms_articles/templatetags/cms_articles.py
--rw-r--r--   0        0        0        0 2022-09-22 22:29:38.096301 django_cms_articles-2.0.3/cms_articles/tests/__init__.py
--rw-r--r--   0        0        0      924 2022-09-22 21:32:42.470486 django_cms_articles-2.0.3/cms_articles/tests/fixtures.py
--rw-r--r--   0        0        0     3054 2022-09-22 23:26:09.567216 django_cms_articles-2.0.3/cms_articles/tests/settings.py
--rw-r--r--   0        0        0      417 2022-09-22 23:17:26.339321 django_cms_articles-2.0.3/cms_articles/tests/templates/default.html
--rw-r--r--   0        0        0      514 2022-12-29 16:48:51.332113 django_cms_articles-2.0.3/cms_articles/tests/test_api.py
--rw-r--r--   0        0        0      328 2022-09-20 11:07:47.885222 django_cms_articles-2.0.3/cms_articles/urls.py
--rw-r--r--   0        0        0      435 2022-09-20 11:07:47.897222 django_cms_articles-2.0.3/cms_articles/utils/__init__.py
--rw-r--r--   0        0        0      941 2022-09-20 11:07:47.933222 django_cms_articles-2.0.3/cms_articles/utils/article.py
--rw-r--r--   0        0        0     1016 2022-09-20 11:17:31.723767 django_cms_articles-2.0.3/cms_articles/utils/placeholder.py
--rw-r--r--   0        0        0     4694 2022-09-20 11:07:48.037224 django_cms_articles-2.0.3/cms_articles/views.py
--rw-r--r--   0        0        0     1608 2023-11-25 22:56:24.810970 django_cms_articles-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     2701 1970-01-01 00:00:00.000000 django_cms_articles-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1507 2022-09-20 10:23:53.365187 django_cms_articles-2.1.0/LICENSE
+-rw-r--r--   0        0        0     1189 2022-09-20 10:23:53.365187 django_cms_articles-2.1.0/README.md
+-rw-r--r--   0        0        0       59 2022-09-20 11:07:46.821205 django_cms_articles-2.1.0/cms_articles/__init__.py
+-rw-r--r--   0        0        0       93 2022-09-20 10:23:53.365187 django_cms_articles-2.1.0/cms_articles/admin/__init__.py
+-rw-r--r--   0        0        0    19135 2022-12-30 15:26:17.765974 django_cms_articles-2.1.0/cms_articles/admin/article.py
+-rw-r--r--   0        0        0      277 2022-09-20 10:23:53.365187 django_cms_articles-2.1.0/cms_articles/admin/attribute.py
+-rw-r--r--   0        0        0      224 2022-09-20 11:07:46.825205 django_cms_articles-2.1.0/cms_articles/admin/category.py
+-rw-r--r--   0        0        0     3029 2022-12-30 15:25:49.465921 django_cms_articles-2.1.0/cms_articles/admin/forms.py
+-rw-r--r--   0        0        0     5230 2022-09-22 22:13:29.570734 django_cms_articles-2.1.0/cms_articles/api.py
+-rw-r--r--   0        0        0      281 2022-09-22 21:48:17.595607 django_cms_articles-2.1.0/cms_articles/apps.py
+-rw-r--r--   0        0        0     4409 2022-09-20 11:07:47.037209 django_cms_articles-2.1.0/cms_articles/archive.py
+-rw-r--r--   0        0        0     1526 2022-09-20 11:07:46.993208 django_cms_articles-2.1.0/cms_articles/article_rendering.py
+-rw-r--r--   0        0        0      359 2022-09-22 21:48:17.595607 django_cms_articles-2.1.0/cms_articles/cms_apps.py
+-rw-r--r--   0        0        0     2628 2022-09-22 21:56:11.181288 django_cms_articles-2.1.0/cms_articles/cms_plugins.py
+-rw-r--r--   0        0        0     2724 2022-09-22 21:48:17.595607 django_cms_articles-2.1.0/cms_articles/cms_toolbars.py
+-rw-r--r--   0        0        0      485 2022-09-20 11:07:47.053209 django_cms_articles-2.1.0/cms_articles/conf/__init__.py
+-rw-r--r--   0        0        0      830 2022-09-22 21:48:17.595607 django_cms_articles-2.1.0/cms_articles/conf/default_settings.py
+-rw-r--r--   0        0        0       91 2022-09-20 11:07:47.077209 django_cms_articles-2.1.0/cms_articles/import_wordpress/__init__.py
+-rw-r--r--   0        0        0     9759 2024-05-06 23:19:01.606972 django_cms_articles-2.1.0/cms_articles/import_wordpress/admin.py
+-rw-r--r--   0        0        0      253 2022-09-22 21:48:17.595607 django_cms_articles-2.1.0/cms_articles/import_wordpress/apps.py
+-rw-r--r--   0        0        0      655 2022-09-22 21:48:17.595607 django_cms_articles-2.1.0/cms_articles/import_wordpress/forms.py
+-rw-r--r--   0        0        0        0 2022-09-20 10:23:53.369187 django_cms_articles-2.1.0/cms_articles/import_wordpress/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-20 10:23:53.369187 django_cms_articles-2.1.0/cms_articles/import_wordpress/management/commands/__init__.py
+-rw-r--r--   0        0        0     1087 2024-05-06 21:26:07.209560 django_cms_articles-2.1.0/cms_articles/import_wordpress/management/commands/cms_import_wordpress.py
+-rw-r--r--   0        0        0    13873 2024-05-06 20:46:46.623419 django_cms_articles-2.1.0/cms_articles/import_wordpress/migrations/0001_initial.py
+-rw-r--r--   0        0        0      995 2024-05-06 23:19:01.523971 django_cms_articles-2.1.0/cms_articles/import_wordpress/migrations/0002_update.py
+-rw-r--r--   0        0        0        0 2022-09-20 10:23:53.369187 django_cms_articles-2.1.0/cms_articles/import_wordpress/migrations/__init__.py
+-rw-r--r--   0        0        0    14646 2024-05-07 09:29:02.671056 django_cms_articles-2.1.0/cms_articles/import_wordpress/models.py
+-rw-r--r--   0        0        0     2194 2022-09-20 10:23:53.369187 django_cms_articles-2.1.0/cms_articles/import_wordpress/templates/cms_articles/import_wordpress/cms_import.html
+-rw-r--r--   0        0        0     1098 2022-09-20 10:23:53.369187 django_cms_articles-2.1.0/cms_articles/import_wordpress/templates/cms_articles/import_wordpress/form.html
+-rwxr-xr-x   0        0        0     7109 2024-05-06 21:26:07.270560 django_cms_articles-2.1.0/cms_articles/import_wordpress/utils.py
+-rw-r--r--   0        0        0    11767 2022-09-20 10:23:53.373187 django_cms_articles-2.1.0/cms_articles/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18344 2022-09-20 10:23:53.373187 django_cms_articles-2.1.0/cms_articles/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10495 2022-09-22 22:40:46.906000 django_cms_articles-2.1.0/cms_articles/migrations/0001_initial.py
+-rw-r--r--   0        0        0      386 2022-09-22 22:40:46.605981 django_cms_articles-2.1.0/cms_articles/migrations/0002_remove_title_excerpt.py
+-rw-r--r--   0        0        0     2254 2022-09-22 22:40:21.876400 django_cms_articles-2.1.0/cms_articles/migrations/0003_description_image.py
+-rw-r--r--   0        0        0     4742 2022-09-22 22:40:46.821994 django_cms_articles-2.1.0/cms_articles/migrations/0004_categories.py
+-rw-r--r--   0        0        0     1712 2022-09-22 22:40:46.693987 django_cms_articles-2.1.0/cms_articles/migrations/0005_attributes.py
+-rw-r--r--   0        0        0     1282 2022-09-22 22:40:46.657984 django_cms_articles-2.1.0/cms_articles/migrations/0006_order_date.py
+-rw-r--r--   0        0        0      971 2022-09-22 22:40:46.705987 django_cms_articles-2.1.0/cms_articles/migrations/0007_plugins.py
+-rw-r--r--   0        0        0     2765 2022-09-22 22:40:46.817994 django_cms_articles-2.1.0/cms_articles/migrations/0008_cms_3_4.py
+-rw-r--r--   0        0        0      997 2022-09-22 22:40:46.769991 django_cms_articles-2.1.0/cms_articles/migrations/0009_number_min_value.py
+-rw-r--r--   0        0        0      402 2022-09-22 22:40:46.789992 django_cms_articles-2.1.0/cms_articles/migrations/0010_remove_article_revision_id.py
+-rw-r--r--   0        0        0     1085 2022-09-22 22:40:46.833995 django_cms_articles-2.1.0/cms_articles/migrations/0011_attribute_site.py
+-rw-r--r--   0        0        0     1327 2022-09-22 22:40:46.865997 django_cms_articles-2.1.0/cms_articles/migrations/0012_protect_keys.py
+-rw-r--r--   0        0        0        0 2022-09-20 10:23:53.373187 django_cms_articles-2.1.0/cms_articles/migrations/__init__.py
+-rw-r--r--   0        0        0      287 2022-09-20 10:23:53.373187 django_cms_articles-2.1.0/cms_articles/models/__init__.py
+-rw-r--r--   0        0        0    23967 2022-12-30 15:26:47.710033 django_cms_articles-2.1.0/cms_articles/models/article.py
+-rw-r--r--   0        0        0      619 2022-09-22 23:03:54.335412 django_cms_articles-2.1.0/cms_articles/models/attribute.py
+-rw-r--r--   0        0        0      843 2023-11-25 22:48:33.472751 django_cms_articles-2.1.0/cms_articles/models/category.py
+-rw-r--r--   0        0        0     4220 2022-09-20 11:07:47.569217 django_cms_articles-2.1.0/cms_articles/models/managers.py
+-rw-r--r--   0        0        0     4540 2022-12-30 15:24:29.529780 django_cms_articles-2.1.0/cms_articles/models/plugins.py
+-rw-r--r--   0        0        0      276 2022-09-20 11:07:47.581217 django_cms_articles-2.1.0/cms_articles/models/query.py
+-rw-r--r--   0        0        0     4212 2022-12-30 15:23:52.297721 django_cms_articles-2.1.0/cms_articles/models/title.py
+-rw-r--r--   0        0        0     4609 2022-12-30 13:29:58.468309 django_cms_articles-2.1.0/cms_articles/search_indexes.py
+-rw-r--r--   0        0        0     1252 2022-09-22 22:28:00.384915 django_cms_articles-2.1.0/cms_articles/signals/__init__.py
+-rw-r--r--   0        0        0      816 2022-09-20 11:07:47.813220 django_cms_articles-2.1.0/cms_articles/signals/article.py
+-rw-r--r--   0        0        0     1939 2022-09-20 11:07:47.865221 django_cms_articles-2.1.0/cms_articles/signals/plugins.py
+-rw-r--r--   0        0        0      892 2022-09-20 11:07:47.845221 django_cms_articles-2.1.0/cms_articles/signals/title.py
+-rw-r--r--   0        0        0      717 2022-09-20 10:23:53.377187 django_cms_articles-2.1.0/cms_articles/static/cms_articles/css/changelist.css
+-rw-r--r--   0        0        0     2262 2022-09-20 10:23:53.377187 django_cms_articles-2.1.0/cms_articles/static/cms_articles/js/changelist.js
+-rw-r--r--   0        0        0      378 2022-12-29 16:48:51.328113 django_cms_articles-2.1.0/cms_articles/templates/admin/cms_articles/article/change_form.html
+-rw-r--r--   0        0        0     3619 2022-09-20 10:23:53.377187 django_cms_articles-2.1.0/cms_articles/templates/admin/cms_articles/article/change_list_lang.html
+-rw-r--r--   0        0        0      661 2022-09-20 10:23:53.377187 django_cms_articles-2.1.0/cms_articles/templates/admin/cms_articles/article/change_list_preview.html
+-rw-r--r--   0        0        0      757 2022-12-29 16:48:51.328113 django_cms_articles-2.1.0/cms_articles/templates/admin/cms_articles/article_changelist.html
+-rw-r--r--   0        0        0       77 2022-09-20 10:23:53.377187 django_cms_articles-2.1.0/cms_articles/templates/cms_articles/article/default.html
+-rw-r--r--   0        0        0      558 2022-09-20 10:23:53.377187 django_cms_articles-2.1.0/cms_articles/templates/cms_articles/article_preview.html
+-rw-r--r--   0        0        0     1144 2022-09-20 10:23:53.377187 django_cms_articles-2.1.0/cms_articles/templates/cms_articles/articles/default.html
+-rw-r--r--   0        0        0     1219 2022-09-22 22:44:45.738639 django_cms_articles-2.1.0/cms_articles/templates/cms_articles/base.html
+-rw-r--r--   0        0        0      730 2022-09-20 10:23:53.381187 django_cms_articles-2.1.0/cms_articles/templates/cms_articles/default.html
+-rw-r--r--   0        0        0        0 2022-09-20 10:23:53.381187 django_cms_articles-2.1.0/cms_articles/templatetags/__init__.py
+-rw-r--r--   0        0        0     8972 2022-12-30 15:23:35.569696 django_cms_articles-2.1.0/cms_articles/templatetags/cms_articles.py
+-rw-r--r--   0        0        0        0 2022-09-22 22:29:38.096301 django_cms_articles-2.1.0/cms_articles/tests/__init__.py
+-rw-r--r--   0        0        0      924 2022-09-22 21:32:42.470486 django_cms_articles-2.1.0/cms_articles/tests/fixtures.py
+-rw-r--r--   0        0        0     3054 2022-09-22 23:26:09.567216 django_cms_articles-2.1.0/cms_articles/tests/settings.py
+-rw-r--r--   0        0        0      417 2022-09-22 23:17:26.339321 django_cms_articles-2.1.0/cms_articles/tests/templates/default.html
+-rw-r--r--   0        0        0      514 2022-12-29 16:48:51.332113 django_cms_articles-2.1.0/cms_articles/tests/test_api.py
+-rw-r--r--   0        0        0      328 2022-09-20 11:07:47.885222 django_cms_articles-2.1.0/cms_articles/urls.py
+-rw-r--r--   0        0        0      435 2022-09-20 11:07:47.897222 django_cms_articles-2.1.0/cms_articles/utils/__init__.py
+-rw-r--r--   0        0        0      941 2022-09-20 11:07:47.933222 django_cms_articles-2.1.0/cms_articles/utils/article.py
+-rw-r--r--   0        0        0     1016 2022-09-20 11:17:31.723767 django_cms_articles-2.1.0/cms_articles/utils/placeholder.py
+-rw-r--r--   0        0        0     4694 2022-09-20 11:07:48.037224 django_cms_articles-2.1.0/cms_articles/views.py
+-rw-r--r--   0        0        0     1608 2024-05-07 09:32:11.459083 django_cms_articles-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2701 1970-01-01 00:00:00.000000 django_cms_articles-2.1.0/PKG-INFO
```

### Comparing `django_cms_articles-2.0.3/LICENSE` & `django_cms_articles-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/README.md` & `django_cms_articles-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/admin/article.py` & `django_cms_articles-2.1.0/cms_articles/admin/article.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/admin/forms.py` & `django_cms_articles-2.1.0/cms_articles/admin/forms.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/api.py` & `django_cms_articles-2.1.0/cms_articles/api.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/archive.py` & `django_cms_articles-2.1.0/cms_articles/archive.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/article_rendering.py` & `django_cms_articles-2.1.0/cms_articles/article_rendering.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/cms_plugins.py` & `django_cms_articles-2.1.0/cms_articles/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/cms_toolbars.py` & `django_cms_articles-2.1.0/cms_articles/cms_toolbars.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/conf/default_settings.py` & `django_cms_articles-2.1.0/cms_articles/conf/default_settings.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/import_wordpress/admin.py` & `django_cms_articles-2.1.0/cms_articles/import_wordpress/admin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-# -*- coding: utf-8 -*-
 from django.conf.urls import url
 from django.contrib import admin, messages
 from django.contrib.admin import helpers
 from django.contrib.auth import get_user_model
-from django.core.urlresolvers import reverse
+from django.urls import reverse
 from django.db import transaction
 from django.http import HttpResponse, HttpResponseBadRequest
-from django.shortcuts import get_object_or_404, render_to_response
-from django.template import RequestContext
+from django.shortcuts import get_object_or_404, render
+
+# from django.template import RequestContext
+from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
 
 from .forms import CMSImportForm, XMLImportForm
 from .models import Author, Category, Item, Options
 
 User = get_user_model()
 
@@ -135,112 +136,111 @@
         return self.response_post_save_add(request, obj)
 
     def get_form(self, request, obj=None, **kwargs):
         if not obj:
             kwargs["form"] = XMLImportForm
         return super().get_form(request, obj, **kwargs)
 
+    @admin.display(description=_("post parent"), ordering="post_parent")
     def parent_link(self, obj):
         if obj.post_parent:
-            return '<a href="{url}">{label}</a>'.format(
-                url=reverse(
-                    "admin:{}_{}_changelist".format(
-                        Item._meta.app_label,
-                        Item._meta.model_name,
+            return mark_safe(
+                '<a href="{url}">{label}</a>'.format(
+                    url=reverse(
+                        "admin:{}_{}_changelist".format(
+                            Item._meta.app_label,
+                            Item._meta.model_name,
+                        )
                     )
+                    + "?post_id__exact={}".format(obj.post_parent),
+                    label=obj.post_parent,
                 )
-                + "?post_id__exact={}".format(obj.post_parent),
-                label=obj.post_parent,
             )
         else:
             return ""
 
-    parent_link.short_description = _("post parent")
-    parent_link.admin_order_field = "post_parent"
-    parent_link.allow_tags = True
-
+    @admin.display(description=_("post children"))
     def children_link(self, obj):
         count = obj.children.count()
         if count:
-            return '<a href="{url}">{label}</a>'.format(
-                url=reverse(
-                    "admin:{}_{}_changelist".format(
-                        Item._meta.app_label,
-                        Item._meta.model_name,
+            return mark_safe(
+                '<a href="{url}">{label}</a>'.format(
+                    url=reverse(
+                        "admin:{}_{}_changelist".format(
+                            Item._meta.app_label,
+                            Item._meta.model_name,
+                        )
                     )
+                    + "?post_parent__exact={}".format(obj.post_id),
+                    label=count,
                 )
-                + "?post_parent__exact={}".format(obj.post_id),
-                label=count,
             )
         else:
             return ""
 
-    children_link.short_description = _("post children")
-    children_link.allow_tags = True
-
+    @admin.display(description=_("title"), ordering="title")
     def title_link(self, obj):
-        return '<a href="{url}" title="{url}" target="_blank">{title}</a>'.format(
-            url=obj.guid,
-            title=obj.title,
+        return mark_safe(
+            '<a href="{url}" title="{url}" target="_blank">{title}</a>'.format(
+                url=obj.guid,
+                title=obj.title,
+            )
         )
 
-    title_link.short_description = _("title")
-    title_link.admin_order_field = "title"
-    title_link.allow_tags = True
-
+    @admin.display(description=_("imported as"))
     def imported_link(self, obj):
         url = None
         if obj.article or obj.page:
             url = (obj.article or obj.page).get_absolute_url()
         elif obj.file:
             url = obj.file.file.url
         elif obj.folder:
             url = obj.folder.get_admin_directory_listing_url_path()
         if url:
-            return '<a href="{url}" target="_blank">{obj}</a>'.format(
-                obj=obj.article or obj.page or obj.file or obj.folder,
-                url=url,
+            return mark_safe(
+                '<a href="{url}" target="_blank">{obj}</a>'.format(
+                    obj=obj.article or obj.page or obj.file or obj.folder,
+                    url=url,
+                )
             )
         else:
             return ""
 
-    imported_link.short_description = _("imported as")
-    imported_link.allow_tags = True
-
+    @admin.action(description=_("Import selected items into CMS"))
     def cms_import(self, request, queryset):
         if request.POST.get("post", "no") == "yes":
             form = CMSImportForm(request.POST)
             if form.is_valid():
-                return render_to_response(
+                return render(
+                    request,
                     "cms_articles/import_wordpress/cms_import.html",
                     {
                         "title": _("Running import"),
                         "items": queryset,
                         "options": form.cleaned_data["options"],
                         "media": self.media,
                         "opts": self.model._meta,
                     },
-                    context_instance=RequestContext(request),
+                    # context_instance=RequestContext(request), # TODO: delete this line
                 )
         else:
             form = CMSImportForm()
-        return render_to_response(
+        return render(
+            request,
             "cms_articles/import_wordpress/form.html",
             {
                 "title": _("Select predefined import options"),
                 "queryset": queryset,
                 "opts": self.model._meta,
                 "form": form,
                 "action_checkbox_name": helpers.ACTION_CHECKBOX_NAME,
             },
-            context_instance=RequestContext(request),
+            # context_instance=RequestContext(request),  # TODO: delete this line
         )
 
-    cms_import.short_description = _("Import selected items into CMS")
-
     @transaction.atomic
     def import_item(self, request):
         try:
             item_id = int(request.GET["item_id"])
             options_id = int(request.GET["options_id"])
         except (KeyError, ValueError):
             return HttpResponseBadRequest()
```

### Comparing `django_cms_articles-2.0.3/cms_articles/import_wordpress/forms.py` & `django_cms_articles-2.1.0/cms_articles/import_wordpress/forms.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/import_wordpress/management/commands/cms_import_wordpress.py` & `django_cms_articles-2.1.0/cms_articles/import_wordpress/management/commands/cms_import_wordpress.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,16 +8,20 @@
 
     def add_arguments(self, parser):
         parser.add_argument("wordpress_xml", nargs="+", type=str)
 
     def handle(self, *args, **options):
         for wordpress_xml in options["wordpress_xml"]:
             try:
-                imported, errors = import_wordpress(wordpress_xml)
+                result = import_wordpress(wordpress_xml)
             except Exception as e:
                 self.stderr.write(self.style.ERROR('Failed to import "{}": {}.'.format(wordpress_xml, e)))
                 raise CommandError(e)
-            if errors:
+            if result["errors"]:
                 self.stderr.write(self.style.ERROR("Failed to import {} items.".format(wordpress_xml)))
             self.stdout.write(
-                self.style.SUCCESS('Successfully imported {} items from "{}".'.format(imported, wordpress_xml))
+                self.style.SUCCESS(
+                    'Successfully imported {authors} authors, {categories} categories, and {items} items from "{xml}".'.format(
+                        **result, xml=wordpress_xml
+                    )
+                )
             )
```

### Comparing `django_cms_articles-2.0.3/cms_articles/import_wordpress/migrations/0001_initial.py` & `django_cms_articles-2.1.0/cms_articles/import_wordpress/migrations/0001_initial.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-# -*- coding: utf-8 -*-
-# Generated by Django 1.9.5 on 2016-05-20 20:00
-from __future__ import unicode_literals
+# Generated by Django 3.2.25 on 2024-05-06 20:46
 
 import cms.models.fields
-from cms.models import Page
-from cms_articles.conf import settings
+from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 import filer.fields.folder
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
-        ("filer", "0002_auto_20150606_2003"),
+        ("cms", "0022_auto_20180620_1551"),
+        ("filer", "0017_image__transparent"),
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
-        ("cms_articles", "0004_categories"),
-        ("cms", "0013_urlconfrevision"),
+        ("cms_articles", "0012_protect_keys"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="Author",
             fields=[
                 ("id", models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name="ID")),
@@ -60,128 +56,48 @@
                 (
                     "category",
                     models.ForeignKey(
                         blank=True,
                         null=True,
                         on_delete=django.db.models.deletion.SET_NULL,
                         related_name="+",
-                        to="cms_articles.Category",
+                        to="cms_articles.category",
                         verbose_name="articles category",
                     ),
                 ),
             ],
             options={
                 "verbose_name": "category",
                 "verbose_name_plural": "categories",
             },
         ),
         migrations.CreateModel(
-            name="Item",
-            fields=[
-                ("id", models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name="ID")),
-                ("title", models.TextField(default="", verbose_name="title")),
-                ("link", models.CharField(max_length=255, verbose_name="link")),
-                ("pub_date", models.DateTimeField(verbose_name="publication date")),
-                ("guid", models.CharField(max_length=255, verbose_name="url")),
-                ("description", models.TextField(verbose_name="description")),
-                ("content", models.TextField(verbose_name="content")),
-                ("excerpt", models.TextField(verbose_name="excerpt")),
-                ("post_id", models.IntegerField(unique=True, verbose_name="post id")),
-                ("post_date", models.DateTimeField(verbose_name="post date")),
-                ("post_name", models.CharField(max_length=255, verbose_name="post name")),
-                ("status", models.CharField(max_length=20, verbose_name="status")),
-                ("post_parent", models.IntegerField(verbose_name="parent post id")),
-                ("post_type", models.CharField(max_length=20, verbose_name="type")),
-                ("postmeta", models.TextField(verbose_name="metadata")),
-                (
-                    "article",
-                    models.OneToOneField(
-                        blank=True,
-                        null=True,
-                        on_delete=django.db.models.deletion.SET_NULL,
-                        related_name="+",
-                        to="cms_articles.Article",
-                        verbose_name="imported article",
-                    ),
-                ),
-                (
-                    "categories",
-                    models.ManyToManyField(blank=True, related_name="kategorie", to="import_wordpress.Category"),
-                ),
-                (
-                    "created_by",
-                    models.ForeignKey(
-                        on_delete=django.db.models.deletion.CASCADE,
-                        to="import_wordpress.Author",
-                        verbose_name="created by",
-                    ),
-                ),
-                (
-                    "file",
-                    models.OneToOneField(
-                        blank=True,
-                        null=True,
-                        on_delete=django.db.models.deletion.SET_NULL,
-                        related_name="+",
-                        to="filer.File",
-                        verbose_name="imported file",
-                    ),
-                ),
-                (
-                    "folder",
-                    models.ForeignKey(
-                        blank=True,
-                        null=True,
-                        on_delete=django.db.models.deletion.SET_NULL,
-                        related_name="+",
-                        to="filer.Folder",
-                        verbose_name="attachments folder",
-                    ),
-                ),
-                (
-                    "page",
-                    models.OneToOneField(
-                        blank=True,
-                        null=True,
-                        on_delete=django.db.models.deletion.SET_NULL,
-                        related_name="+",
-                        to="cms.Page",
-                        verbose_name="imported page",
-                    ),
-                ),
-            ],
-            options={
-                "verbose_name": "item",
-                "verbose_name_plural": "items",
-            },
-        ),
-        migrations.CreateModel(
             name="Options",
             fields=[
                 ("id", models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name="ID")),
                 ("name", models.CharField(max_length=255, unique=True, verbose_name="name")),
                 (
                     "language",
                     models.CharField(
                         help_text="The language of the content fields.", max_length=15, verbose_name="language"
                     ),
                 ),
                 (
                     "article_template",
                     models.CharField(
-                        choices=settings.CMS_ARTICLES_TEMPLATES,
-                        default=settings.CMS_ARTICLES_TEMPLATES[0][0],
+                        choices=[("cms_articles/default.html", "Default")],
+                        default="cms_articles/default.html",
                         max_length=100,
                         verbose_name="template",
                     ),
                 ),
                 (
                     "article_slot",
                     models.CharField(
-                        default=settings.CMS_ARTICLES_SLOT,
+                        default="content",
                         help_text="The name of placeholder used to create content plugins in.",
                         max_length=255,
                         verbose_name="slot",
                     ),
                 ),
                 (
                     "article_redirects",
@@ -194,16 +110,20 @@
                 (
                     "article_publish",
                     models.BooleanField(default=False, help_text="Publish imported articles.", verbose_name="publish"),
                 ),
                 (
                     "page_template",
                     models.CharField(
-                        choices=Page.template_choices,
-                        default=Page.TEMPLATE_DEFAULT,
+                        choices=[
+                            ("default.html", "Výchozí"),
+                            ("home.html", "Titulní stránka"),
+                            ("INHERIT", "Inherit the template of the nearest ancestor"),
+                        ],
+                        default="INHERIT",
                         max_length=100,
                         verbose_name="template",
                     ),
                 ),
                 (
                     "page_slot",
                     models.CharField(
@@ -229,88 +149,173 @@
                     "article_folder",
                     filer.fields.folder.FilerFolderField(
                         blank=True,
                         help_text="Select folder for articles. Subfolder will be created for each article with attachments.",
                         null=True,
                         on_delete=django.db.models.deletion.SET_NULL,
                         related_name="+",
-                        to="filer.Folder",
+                        to="filer.folder",
                         verbose_name="attachments folder",
                     ),
                 ),
                 (
                     "article_tree",
                     models.ForeignKey(
                         help_text="All posts will be imported as articles in this tree.",
-                        on_delete=django.db.models.deletion.CASCADE,
+                        limit_choices_to={
+                            "application_urls": "CMSArticlesApp",
+                            "node__site_id": 1,
+                            "publisher_is_draft": False,
+                        },
+                        on_delete=django.db.models.deletion.PROTECT,
                         related_name="+",
-                        to="cms.Page",
+                        to="cms.page",
                         verbose_name="tree",
                     ),
                 ),
                 (
                     "file_folder",
                     filer.fields.folder.FilerFolderField(
                         blank=True,
                         help_text="Select folder for other attachments.",
                         null=True,
                         on_delete=django.db.models.deletion.SET_NULL,
                         related_name="+",
-                        to="filer.Folder",
+                        to="filer.folder",
                         verbose_name="folder",
                     ),
                 ),
                 (
                     "gallery_folder",
                     filer.fields.folder.FilerFolderField(
                         blank=True,
                         help_text="Select folder for galleries. Subfolder will be created for each gallery.",
                         null=True,
                         on_delete=django.db.models.deletion.SET_NULL,
                         related_name="+",
-                        to="filer.Folder",
+                        to="filer.folder",
                         verbose_name="folder",
                     ),
                 ),
                 (
                     "page_folder",
                     filer.fields.folder.FilerFolderField(
                         blank=True,
                         help_text="Select folder for pages. Subfolder will be created for each page with attachments.",
                         null=True,
                         on_delete=django.db.models.deletion.SET_NULL,
                         related_name="+",
-                        to="filer.Folder",
+                        to="filer.folder",
                         verbose_name="attachments folder",
                     ),
                 ),
                 (
                     "page_root",
                     cms.models.fields.PageField(
                         blank=True,
                         help_text="All pages will be imported as sub-pages of this page.",
                         null=True,
                         on_delete=django.db.models.deletion.SET_NULL,
                         related_name="+",
-                        to="cms.Page",
+                        to="cms.page",
                         verbose_name="root",
                     ),
                 ),
                 (
                     "slide_folder",
                     filer.fields.folder.FilerFolderField(
                         blank=True,
                         help_text="Select folder for slides.",
                         null=True,
                         on_delete=django.db.models.deletion.SET_NULL,
                         related_name="+",
-                        to="filer.Folder",
+                        to="filer.folder",
                         verbose_name="folder",
                     ),
                 ),
             ],
             options={
                 "verbose_name": "options",
                 "verbose_name_plural": "options",
             },
         ),
+        migrations.CreateModel(
+            name="Item",
+            fields=[
+                ("id", models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name="ID")),
+                ("title", models.TextField(default="", verbose_name="title")),
+                ("link", models.CharField(max_length=255, verbose_name="link")),
+                ("pub_date", models.DateTimeField(verbose_name="publication date")),
+                ("guid", models.CharField(max_length=255, verbose_name="url")),
+                ("description", models.TextField(verbose_name="description")),
+                ("content", models.TextField(verbose_name="content")),
+                ("excerpt", models.TextField(verbose_name="excerpt")),
+                ("post_id", models.IntegerField(unique=True, verbose_name="post id")),
+                ("post_date", models.DateTimeField(verbose_name="post date")),
+                ("post_name", models.CharField(max_length=255, verbose_name="post name")),
+                ("status", models.CharField(max_length=20, verbose_name="status")),
+                ("post_parent", models.IntegerField(verbose_name="parent post id")),
+                ("post_type", models.CharField(max_length=20, verbose_name="type")),
+                ("postmeta", models.TextField(verbose_name="metadata")),
+                (
+                    "article",
+                    models.OneToOneField(
+                        blank=True,
+                        null=True,
+                        on_delete=django.db.models.deletion.SET_NULL,
+                        related_name="+",
+                        to="cms_articles.article",
+                        verbose_name="imported article",
+                    ),
+                ),
+                (
+                    "categories",
+                    models.ManyToManyField(blank=True, related_name="kategorie", to="import_wordpress.Category"),
+                ),
+                (
+                    "created_by",
+                    models.ForeignKey(
+                        on_delete=django.db.models.deletion.PROTECT,
+                        to="import_wordpress.author",
+                        verbose_name="created by",
+                    ),
+                ),
+                (
+                    "file",
+                    models.OneToOneField(
+                        blank=True,
+                        null=True,
+                        on_delete=django.db.models.deletion.SET_NULL,
+                        related_name="+",
+                        to="filer.file",
+                        verbose_name="imported file",
+                    ),
+                ),
+                (
+                    "folder",
+                    models.ForeignKey(
+                        blank=True,
+                        null=True,
+                        on_delete=django.db.models.deletion.SET_NULL,
+                        related_name="+",
+                        to="filer.folder",
+                        verbose_name="attachments folder",
+                    ),
+                ),
+                (
+                    "page",
+                    models.OneToOneField(
+                        blank=True,
+                        null=True,
+                        on_delete=django.db.models.deletion.SET_NULL,
+                        related_name="+",
+                        to="cms.page",
+                        verbose_name="imported page",
+                    ),
+                ),
+            ],
+            options={
+                "verbose_name": "item",
+                "verbose_name_plural": "items",
+            },
+        ),
     ]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django_cms_articles-2.0.3/cms_articles/import_wordpress/models.py` & `django_cms_articles-2.1.0/cms_articles/import_wordpress/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,30 +2,27 @@
 
 from cms.api import create_page
 from cms.models import Page
 from cms.models.fields import PageField
 from django.core.files import File as DjangoFile
 from django.core.files.temp import NamedTemporaryFile
 from django.db import models
-from django.utils.encoding import force_bytes
 from django.utils.functional import cached_property
 from django.utils.text import slugify
 from django.utils.translation import gettext_lazy as _
 from filer.fields.folder import FilerFolderField
 from filer.models import File, Folder
 
 from cms_articles.api import add_content, create_article, publish_article
 from cms_articles.conf import settings
 
 from .utils import create_redirect
 
-try:
-    from urllib.request import urlopen
-except ImportError:
-    from urllib2 import urlopen
+from urllib.request import urlopen
+from urllib.parse import quote, urlparse
 
 
 class Author(models.Model):
     author_id = models.IntegerField(_("author id"), unique=True)
     login = models.CharField(_("login name"), max_length=255)
     email = models.EmailField(_("email"), blank=True, null=True)
     first_name = models.CharField(_("first name"), max_length=255, blank=True, null=True)
@@ -79,17 +76,19 @@
     class Meta:
         verbose_name = _("category")
         verbose_name_plural = _("categories")
 
 
 class Item(models.Model):
     title = models.TextField(_("title"), default="")
-    link = models.CharField(_("link"), max_length=255)
-    pub_date = models.DateTimeField(_("publication date"))
-    created_by = models.ForeignKey(Author, verbose_name=_("created by"))
+    link = models.CharField(_("link"), max_length=512)
+    pub_date = models.DateTimeField(_("publication date"), blank=True, null=True)
+    created_by = models.ForeignKey(
+        Author, verbose_name=_("created by"), on_delete=models.SET_NULL, blank=True, null=True
+    )
     guid = models.CharField(_("url"), max_length=255)
     description = models.TextField(_("description"))
     content = models.TextField(_("content"))
     excerpt = models.TextField(_("excerpt"))
     post_id = models.IntegerField(_("post id"), unique=True)
     post_date = models.DateTimeField(_("post date"))
     post_name = models.CharField(_("post name"), max_length=255)
@@ -166,19 +165,20 @@
             tree=options.article_tree,
             template=options.article_template,
             title=self.title,
             language=options.language,
             description=self.excerpt,
             created_by=self.created_by.user or self.created_by.login,
             image=image,
-            publicationdate=self.pub_date,
+            publication_date=self.pub_date,
             categories=[c.category for c in self.categories.exclude(category=None)],
         )
-        self.article.creation_date = self.post_date
-        self.article.save()
+        if self.post_date:
+            self.article.creation_date = self.post_date
+            self.article.save()
         content = "\n".join("<p>{}</p>".format(p) for p in self.content.split("\n\n"))
         add_content(self.article, language=options.language, slot=options.article_slot, content=content)
         if options.article_publish:
             self.article = publish_article(
                 article=self.article,
                 language=options.language,
                 changed_by=self.created_by.user or self.created_by.login,
@@ -236,16 +236,19 @@
     def get_or_import_file(self, options):
         from filer.management.commands.import_files import FileImporter
 
         assert self.post_type == "attachment"
         if self.file:
             return self.file
         # download content into deleted temp_file
+        parsed_url = urlparse(self.guid)
+        parsed_url = parsed_url._replace(path=quote(parsed_url.path))
+        url = parsed_url.geturl()
         temp_file = NamedTemporaryFile(delete=True)
-        temp_file.write(urlopen(force_bytes(self.guid)).read())
+        temp_file.write(urlopen(url).read())
         temp_file.flush()
         # create DjangoFile object
         django_file = DjangoFile(temp_file, name=self.guid.split("/")[-1])
         # choose folder
         if self.parent:
             folder = self.parent.get_or_create_folder(options)
         else:
@@ -284,14 +287,15 @@
 
     # global options
     language = models.CharField(_("language"), max_length=15, help_text=_("The language of the content fields."))
 
     # article specific options
     article_tree = models.ForeignKey(
         Page,
+        on_delete=models.PROTECT,
         verbose_name=_("tree"),
         related_name="+",
         help_text=_("All posts will be imported as articles in this tree."),
         limit_choices_to={
             "publisher_is_draft": False,
             "application_urls": "CMSArticlesApp",
             "node__site_id": settings.SITE_ID,
```

### Comparing `django_cms_articles-2.0.3/cms_articles/import_wordpress/templates/cms_articles/import_wordpress/cms_import.html` & `django_cms_articles-2.1.0/cms_articles/import_wordpress/templates/cms_articles/import_wordpress/cms_import.html`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/import_wordpress/templates/cms_articles/import_wordpress/form.html` & `django_cms_articles-2.1.0/cms_articles/import_wordpress/templates/cms_articles/import_wordpress/form.html`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/import_wordpress/utils.py` & `django_cms_articles-2.1.0/cms_articles/import_wordpress/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,21 +5,17 @@
 from cms.utils.compat.dj import is_installed
 from dateutil.parser import parse
 from django.utils.timezone import make_aware
 
 from ..conf import settings
 
 if is_installed("django.contrib.redirects"):
+    from urllib.parse import urlparse
     from django.contrib.redirects.models import Redirect
 
-    try:
-        from urllib.parse import urlparse
-    except ImportError:
-        from urlparse import urlparse
-
     def create_redirect(old_url, new_url):
         old_path = urlparse(old_url).path
         new_path = urlparse(new_url).path
         if old_path != "/" and new_path != old_path:
             redirect = Redirect.objects.get_or_create(
                 site_id=settings.SITE_ID,
                 old_path=urlparse(old_path).path,
@@ -111,15 +107,15 @@
     for item in rss.findall("*/item"):
         post_id = "unknown"
         try:
             # first of all try to parse post_id for use in potential error messages
             post_id = int(item.find("{http://wordpress.org/export/1.2/}post_id").text)
             title = item.find("title").text or ""
             link = item.find("link").text or ""
-            pub_date = parse(item.find("pubDate").text)
+            pub_date = item.find("pubDate").text
             created_by = item.find("{http://purl.org/dc/elements/1.1/}creator").text
             guid = item.find("guid").text
             description = item.find("description").text or ""
             content = item.find("{http://purl.org/rss/1.0/modules/content/}encoded").text or ""
             excerpt = item.find("{http://wordpress.org/export/1.2/excerpt/}encoded").text or ""
             post_date = make_aware(parse(item.find("{http://wordpress.org/export/1.2/}post_date").text))
             post_name = item.find("{http://wordpress.org/export/1.2/}post_name").text or ""
@@ -142,32 +138,35 @@
             ]
         except Exception as e:
             error = "Failed to parse item with post_id {}: {}".format(post_id, e)
             logging.warning(error)
             errors.append(error)
             continue
         try:
-            item = Item.objects.create(
-                title=title,
-                link=link,
-                pub_date=pub_date,
-                created_by=authors[created_by],
-                guid=guid,
-                description=description,
-                content=content,
-                excerpt=excerpt,
+            item = Item.objects.update_or_create(
                 post_id=post_id,
-                post_date=post_date,
-                post_name=post_name,
-                status=status,
-                post_parent=post_parent,
-                post_type=post_type,
-                postmeta=postmeta,
-            )
-            item.categories = cats
+                defaults=dict(
+                    title=title,
+                    link=link,
+                    pub_date=pub_date and parse(pub_date),
+                    created_by=authors.get(created_by),
+                    guid=guid,
+                    description=description,
+                    content=content,
+                    excerpt=excerpt,
+                    post_id=post_id,
+                    post_date=post_date,
+                    post_name=post_name,
+                    status=status,
+                    post_parent=post_parent,
+                    post_type=post_type,
+                    postmeta=postmeta,
+                ),
+            )[0]
+            item.categories.set(cats)
         except Exception as e:
             error = "Failed to save item with post_id {}: {}".format(post_id, e)
             logging.warning(error)
             errors.append(error)
             continue
         imported_items += 1
     return {
```

### Comparing `django_cms_articles-2.0.3/cms_articles/locale/cs/LC_MESSAGES/django.mo` & `django_cms_articles-2.1.0/cms_articles/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/locale/cs/LC_MESSAGES/django.po` & `django_cms_articles-2.1.0/cms_articles/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/migrations/0001_initial.py` & `django_cms_articles-2.1.0/cms_articles/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/migrations/0003_description_image.py` & `django_cms_articles-2.1.0/cms_articles/migrations/0003_description_image.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/migrations/0004_categories.py` & `django_cms_articles-2.1.0/cms_articles/migrations/0004_categories.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/migrations/0005_attributes.py` & `django_cms_articles-2.1.0/cms_articles/migrations/0005_attributes.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/migrations/0006_order_date.py` & `django_cms_articles-2.1.0/cms_articles/migrations/0006_order_date.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/migrations/0007_plugins.py` & `django_cms_articles-2.1.0/cms_articles/migrations/0007_plugins.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/migrations/0008_cms_3_4.py` & `django_cms_articles-2.1.0/cms_articles/migrations/0008_cms_3_4.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/migrations/0009_number_min_value.py` & `django_cms_articles-2.1.0/cms_articles/migrations/0009_number_min_value.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/migrations/0011_attribute_site.py` & `django_cms_articles-2.1.0/cms_articles/migrations/0011_attribute_site.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/migrations/0012_protect_keys.py` & `django_cms_articles-2.1.0/cms_articles/migrations/0012_protect_keys.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/models/article.py` & `django_cms_articles-2.1.0/cms_articles/models/article.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/models/attribute.py` & `django_cms_articles-2.1.0/cms_articles/models/attribute.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/models/category.py` & `django_cms_articles-2.1.0/cms_articles/models/category.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/models/managers.py` & `django_cms_articles-2.1.0/cms_articles/models/managers.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/models/plugins.py` & `django_cms_articles-2.1.0/cms_articles/models/plugins.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/models/title.py` & `django_cms_articles-2.1.0/cms_articles/models/title.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/search_indexes.py` & `django_cms_articles-2.1.0/cms_articles/search_indexes.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/signals/__init__.py` & `django_cms_articles-2.1.0/cms_articles/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/signals/article.py` & `django_cms_articles-2.1.0/cms_articles/signals/article.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/signals/plugins.py` & `django_cms_articles-2.1.0/cms_articles/signals/plugins.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/signals/title.py` & `django_cms_articles-2.1.0/cms_articles/signals/title.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/static/cms_articles/css/changelist.css` & `django_cms_articles-2.1.0/cms_articles/static/cms_articles/css/changelist.css`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/static/cms_articles/js/changelist.js` & `django_cms_articles-2.1.0/cms_articles/static/cms_articles/js/changelist.js`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/templates/admin/cms_articles/article/change_list_lang.html` & `django_cms_articles-2.1.0/cms_articles/templates/admin/cms_articles/article/change_list_lang.html`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/templates/admin/cms_articles/article/change_list_preview.html` & `django_cms_articles-2.1.0/cms_articles/templates/admin/cms_articles/article/change_list_preview.html`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/templates/admin/cms_articles/article_changelist.html` & `django_cms_articles-2.1.0/cms_articles/templates/admin/cms_articles/article_changelist.html`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/templates/cms_articles/article_preview.html` & `django_cms_articles-2.1.0/cms_articles/templates/cms_articles/article_preview.html`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/templates/cms_articles/articles/default.html` & `django_cms_articles-2.1.0/cms_articles/templates/cms_articles/articles/default.html`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/templates/cms_articles/base.html` & `django_cms_articles-2.1.0/cms_articles/templates/cms_articles/base.html`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/templates/cms_articles/default.html` & `django_cms_articles-2.1.0/cms_articles/templates/cms_articles/default.html`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/templatetags/cms_articles.py` & `django_cms_articles-2.1.0/cms_articles/templatetags/cms_articles.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/tests/fixtures.py` & `django_cms_articles-2.1.0/cms_articles/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/tests/settings.py` & `django_cms_articles-2.1.0/cms_articles/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/tests/test_api.py` & `django_cms_articles-2.1.0/cms_articles/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/utils/article.py` & `django_cms_articles-2.1.0/cms_articles/utils/article.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/utils/placeholder.py` & `django_cms_articles-2.1.0/cms_articles/utils/placeholder.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/cms_articles/views.py` & `django_cms_articles-2.1.0/cms_articles/views.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.0.3/pyproject.toml` & `django_cms_articles-2.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 multi_line_output = 3
 profile = "black"
 skip_glob = "*migrations*"
 use_parentheses = true
 
 [tool.poetry]
 name = "django-cms-articles"
-version = "2.0.3"
+version = "2.1.0"
 description = "django CMS application for managing articles"
 authors = ["Jakub Dorňák <jakub.dornak@qbsoftware.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 packages = [{include = "cms_articles"}]
 repository = "https://github.com/misli/django-cms-articles"
 classifiers = [
```

### Comparing `django_cms_articles-2.0.3/PKG-INFO` & `django_cms_articles-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cms-articles
-Version: 2.0.3
+Version: 2.1.0
 Summary: django CMS application for managing articles
 Home-page: https://github.com/misli/django-cms-articles
 License: BSD-3-Clause
 Author: Jakub Dorňák
 Author-email: jakub.dornak@qbsoftware.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

