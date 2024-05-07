# Comparing `tmp/brigid-0.5.0.tar.gz` & `tmp/brigid-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brigid-0.5.0.tar", max compression
+gzip compressed data, was "brigid-0.6.0.tar", max compression
```

## Comparing `brigid-0.5.0.tar` & `brigid-0.6.0.tar`

### file list

```diff
@@ -1,96 +1,102 @@
--rw-r--r--   0        0        0     1504 2024-03-24 15:55:55.772507 brigid-0.5.0/LICENSE
--rw-r--r--   0        0        0     1509 2024-03-24 15:55:55.772507 brigid-0.5.0/README.md
--rw-r--r--   0        0        0        0 2024-03-24 15:55:55.772507 brigid-0.5.0/brigid/__init__.py
--rw-r--r--   0        0        0        0 2024-03-24 15:55:55.772507 brigid-0.5.0/brigid/api/__init__.py
--rw-r--r--   0        0        0      276 2024-03-24 15:55:55.772507 brigid-0.5.0/brigid/api/default_translations.py
--rw-r--r--   0        0        0     3381 2024-03-24 15:55:55.772507 brigid-0.5.0/brigid/api/http_handlers.py
--rw-r--r--   0        0        0     2042 2024-03-24 15:55:55.772507 brigid-0.5.0/brigid/api/middlewares.py
--rw-r--r--   0        0        0     7127 2024-03-24 15:55:55.772507 brigid-0.5.0/brigid/api/renderers.py
--rw-r--r--   0        0        0      275 2024-03-24 15:55:55.772507 brigid-0.5.0/brigid/api/settings.py
--rw-r--r--   0        0        0     3962 2024-03-24 15:55:55.772507 brigid-0.5.0/brigid/api/sitemaps.py
--rw-r--r--   0        0        0     1828 2024-03-24 15:55:55.772507 brigid-0.5.0/brigid/api/static_cache.py
--rw-r--r--   0        0        0     4990 2024-03-24 15:55:55.772507 brigid-0.5.0/brigid/api/utils.py
--rw-r--r--   0        0        0        0 2024-03-24 15:55:55.772507 brigid-0.5.0/brigid/application/__init__.py
--rw-r--r--   0        0        0     3079 2024-03-24 15:55:55.772507 brigid-0.5.0/brigid/application/application.py
--rw-r--r--   0        0        0      822 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/application/settings.py
--rw-r--r--   0        0        0        0 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/cli/__init__.py
--rw-r--r--   0        0        0      169 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/cli/__main__.py
--rw-r--r--   0        0        0      174 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/cli/application.py
--rw-r--r--   0        0        0        0 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/cli/commands/__init__.py
--rw-r--r--   0        0        0      738 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/cli/commands/configs.py
--rw-r--r--   0        0        0      754 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/cli/commands/validate.py
--rw-r--r--   0        0        0      567 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/conftest.py
--rw-r--r--   0        0        0        0 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/core/__init__.py
--rw-r--r--   0        0        0      633 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/core/api.py
--rw-r--r--   0        0        0      493 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/core/entities.py
--rw-r--r--   0        0        0      165 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/core/errors.py
--rw-r--r--   0        0        0     5444 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/core/logging.py
--rw-r--r--   0        0        0     1331 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/core/sentry.py
--rw-r--r--   0        0        0      347 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/core/settings.py
--rw-r--r--   0        0        0      979 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/core/utils.py
--rw-r--r--   0        0        0        0 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/domain/__init__.py
--rw-r--r--   0        0        0      311 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/domain/html.py
--rw-r--r--   0        0        0        0 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/domain/tests/__init__.py
--rw-r--r--   0        0        0      548 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/domain/tests/test_html.py
--rw-r--r--   0        0        0     6149 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/domain/urls.py
--rw-r--r--   0        0        0        0 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/library/__init__.py
--rw-r--r--   0        0        0     1295 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/library/connectivity.py
--rw-r--r--   0        0        0     5177 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/library/discovering.py
--rw-r--r--   0        0        0     6439 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/library/entities.py
--rw-r--r--   0        0        0      292 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/library/settings.py
--rw-r--r--   0        0        0     2502 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/library/similarity.py
--rw-r--r--   0        0        0     4749 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/library/storage.py
--rw-r--r--   0        0        0        0 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/library/tests/__init__.py
--rw-r--r--   0        0        0     1798 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/library/tests/make.py
--rw-r--r--   0        0        0        0 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/renderer/__init__.py
--rw-r--r--   0        0        0     1336 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/renderer/context.py
--rw-r--r--   0        0        0     3873 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/renderer/markdown_render.py
--rw-r--r--   0        0        0        0 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/renderer/processors/__init__.py
--rw-r--r--   0        0        0      812 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/renderer/processors/collection_block.py
--rw-r--r--   0        0        0     1631 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/renderer/processors/external_links.py
--rw-r--r--   0        0        0     2161 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/renderer/processors/header_anchors.py
--rw-r--r--   0        0        0     3299 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/renderer/processors/images_block.py
--rw-r--r--   0        0        0     6062 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/renderer/processors/internal_links.py
--rw-r--r--   0        0        0      442 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/renderer/processors/old_image_markup_validation.py
--rw-r--r--   0        0        0      680 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/renderer/processors/snippets.py
--rw-r--r--   0        0        0        0 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/renderer/processors/tests/__init__.py
--rw-r--r--   0        0        0     4890 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/renderer/processors/tests/test_images_block.py
--rw-r--r--   0        0        0     1788 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/renderer/processors/toml_block.py
--rw-r--r--   0        0        0      902 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/renderer/processors/youtube_block.py
--rw-r--r--   0        0        0      649 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/renderer/static_files.py
--rw-r--r--   0        0        0        0 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/theme/__init__.py
--rw-r--r--   0        0        0      854 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/theme/default_translations.py
--rw-r--r--   0        0        0      310 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/theme/entities.py
--rw-r--r--   0        0        0     1980 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/theme/jinjaglobals.py
--rw-r--r--   0        0        0      808 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/theme/settings.py
--rw-r--r--   0        0        0   100395 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/theme/static/main.css
--rw-r--r--   0        0        0     1211 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/theme/templates/article.html.j2
--rw-r--r--   0        0        0      521 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/theme/templates/article_footer.html.j2
--rw-r--r--   0        0        0      488 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/theme/templates/article_wide.html.j2
--rw-r--r--   0        0        0     1551 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/theme/templates/base.html.j2
--rw-r--r--   0        0        0      661 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/theme/templates/blocks/collection.html.j2
--rw-r--r--   0        0        0      526 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/theme/templates/blocks/images.html.j2
--rw-r--r--   0        0        0      161 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/theme/templates/blocks/youtube.html.j2
--rw-r--r--   0        0        0     1484 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/theme/templates/blog_index.html.j2
--rw-r--r--   0        0        0      673 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/theme/templates/header.html.j2
--rw-r--r--   0        0        0      907 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/theme/templates/languages_links.html.j2
--rw-r--r--   0        0        0      353 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/theme/templates/last_posts.html.j2
--rw-r--r--   0        0        0     4679 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/theme/templates/meta.html.j2
--rw-r--r--   0        0        0     1727 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/theme/templates/pagination.html.j2
--rw-r--r--   0        0        0      798 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/theme/templates/similar_pages.html.j2
--rw-r--r--   0        0        0     2235 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/theme/templates/tags_filter.html.j2
--rw-r--r--   0        0        0      180 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/theme/templates/utils.html.j2
--rw-r--r--   0        0        0     1545 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/theme/templates.py
--rw-r--r--   0        0        0      126 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/theme/utils.py
--rw-r--r--   0        0        0        0 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/validation/__init__.py
--rw-r--r--   0        0        0      138 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/validation/entities.py
--rw-r--r--   0        0        0      785 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/validation/global_validators.py
--rw-r--r--   0        0        0     1198 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/validation/lists_formatting.py
--rw-r--r--   0        0        0      417 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/validation/page_validators.py
--rw-r--r--   0        0        0        0 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/validation/tests/__init__.py
--rw-r--r--   0        0        0     1061 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/validation/tests/test_global_validators.py
--rw-r--r--   0        0        0     2745 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/validation/tests/test_lists_formatting.py
--rw-r--r--   0        0        0      587 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/validation/tests/test_page_validators.py
--rw-r--r--   0        0        0      731 2024-03-24 15:55:55.776507 brigid-0.5.0/brigid/validation/validators.py
--rw-r--r--   0        0        0     3183 2024-03-24 15:56:03.076496 brigid-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3600 1970-01-01 00:00:00.000000 brigid-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-05-07 14:11:26.087611 brigid-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1509 2024-05-07 14:11:26.087611 brigid-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-07 14:11:26.087611 brigid-0.6.0/brigid/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:11:26.087611 brigid-0.6.0/brigid/api/__init__.py
+-rw-r--r--   0        0        0      276 2024-05-07 14:11:26.087611 brigid-0.6.0/brigid/api/default_translations.py
+-rw-r--r--   0        0        0     3381 2024-05-07 14:11:26.087611 brigid-0.6.0/brigid/api/http_handlers.py
+-rw-r--r--   0        0        0     2042 2024-05-07 14:11:26.087611 brigid-0.6.0/brigid/api/middlewares.py
+-rw-r--r--   0        0        0     7103 2024-05-07 14:11:26.087611 brigid-0.6.0/brigid/api/renderers.py
+-rw-r--r--   0        0        0      275 2024-05-07 14:11:26.087611 brigid-0.6.0/brigid/api/settings.py
+-rw-r--r--   0        0        0     3962 2024-05-07 14:11:26.087611 brigid-0.6.0/brigid/api/sitemaps.py
+-rw-r--r--   0        0        0     1828 2024-05-07 14:11:26.087611 brigid-0.6.0/brigid/api/static_cache.py
+-rw-r--r--   0        0        0     4990 2024-05-07 14:11:26.087611 brigid-0.6.0/brigid/api/utils.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:11:26.087611 brigid-0.6.0/brigid/application/__init__.py
+-rw-r--r--   0        0        0     2930 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/application/application.py
+-rw-r--r--   0        0        0      879 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/application/settings.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/cli/__init__.py
+-rw-r--r--   0        0        0      169 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/cli/__main__.py
+-rw-r--r--   0        0        0      174 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/cli/application.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/cli/commands/__init__.py
+-rw-r--r--   0        0        0      738 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/cli/commands/configs.py
+-rw-r--r--   0        0        0      754 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/cli/commands/validate.py
+-rw-r--r--   0        0        0      700 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/core/__init__.py
+-rw-r--r--   0        0        0      633 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/core/api.py
+-rw-r--r--   0        0        0      589 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/core/entities.py
+-rw-r--r--   0        0        0      165 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/core/errors.py
+-rw-r--r--   0        0        0     5444 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/core/logging.py
+-rw-r--r--   0        0        0     1331 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/core/sentry.py
+-rw-r--r--   0        0        0      347 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/core/settings.py
+-rw-r--r--   0        0        0     1088 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/core/utils.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/domain/__init__.py
+-rw-r--r--   0        0        0       56 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/domain/constants.py
+-rw-r--r--   0        0        0       85 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/domain/entities.py
+-rw-r--r--   0        0        0      311 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/domain/html.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/domain/tests/__init__.py
+-rw-r--r--   0        0        0      548 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/domain/tests/test_html.py
+-rw-r--r--   0        0        0     6149 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/domain/urls.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/library/__init__.py
+-rw-r--r--   0        0        0     1295 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/library/connectivity.py
+-rw-r--r--   0        0        0     5177 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/library/discovering.py
+-rw-r--r--   0        0        0     7070 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/library/entities.py
+-rw-r--r--   0        0        0      292 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/library/settings.py
+-rw-r--r--   0        0        0     2502 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/library/similarity.py
+-rw-r--r--   0        0        0     4749 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/library/storage.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/library/tests/__init__.py
+-rw-r--r--   0        0        0     1834 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/library/tests/make.py
+-rw-r--r--   0        0        0      705 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/library/tests/test_entities.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/renderer/__init__.py
+-rw-r--r--   0        0        0     1336 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/renderer/context.py
+-rw-r--r--   0        0        0     3873 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/renderer/markdown_render.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/renderer/processors/__init__.py
+-rw-r--r--   0        0        0      812 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/renderer/processors/collection_block.py
+-rw-r--r--   0        0        0     1572 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/renderer/processors/external_links.py
+-rw-r--r--   0        0        0     2161 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/renderer/processors/header_anchors.py
+-rw-r--r--   0        0        0     3299 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/renderer/processors/images_block.py
+-rw-r--r--   0        0        0     6062 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/renderer/processors/internal_links.py
+-rw-r--r--   0        0        0      442 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/renderer/processors/old_image_markup_validation.py
+-rw-r--r--   0        0        0      680 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/renderer/processors/snippets.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/renderer/processors/tests/__init__.py
+-rw-r--r--   0        0        0     1405 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/renderer/processors/tests/test_external_links.py
+-rw-r--r--   0        0        0     4890 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/renderer/processors/tests/test_images_block.py
+-rw-r--r--   0        0        0     1788 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/renderer/processors/toml_block.py
+-rw-r--r--   0        0        0      902 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/renderer/processors/youtube_block.py
+-rw-r--r--   0        0        0      649 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/renderer/static_files.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/__init__.py
+-rw-r--r--   0        0        0     1171 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/default_translations.py
+-rw-r--r--   0        0        0      477 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/entities.py
+-rw-r--r--   0        0        0     2376 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/jinjaglobals.py
+-rw-r--r--   0        0        0      809 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/settings.py
+-rw-r--r--   0        0        0   100702 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/static/main.css
+-rw-r--r--   0        0        0     1211 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/templates/article.html.j2
+-rw-r--r--   0        0        0      521 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/templates/article_footer.html.j2
+-rw-r--r--   0        0        0      488 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/templates/article_wide.html.j2
+-rw-r--r--   0        0        0     2624 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/templates/base.html.j2
+-rw-r--r--   0        0        0      661 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/templates/blocks/collection.html.j2
+-rw-r--r--   0        0        0      526 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/templates/blocks/images.html.j2
+-rw-r--r--   0        0        0      161 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/templates/blocks/youtube.html.j2
+-rw-r--r--   0        0        0     1653 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/templates/blog_index.html.j2
+-rw-r--r--   0        0        0      673 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/templates/header.html.j2
+-rw-r--r--   0        0        0      907 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/templates/languages_links.html.j2
+-rw-r--r--   0        0        0      353 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/templates/last_posts.html.j2
+-rw-r--r--   0        0        0     4691 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/templates/meta.html.j2
+-rw-r--r--   0        0        0     1727 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/templates/pagination.html.j2
+-rw-r--r--   0        0        0      798 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/templates/similar_pages.html.j2
+-rw-r--r--   0        0        0     2235 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/templates/tags_filter.html.j2
+-rw-r--r--   0        0        0      180 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/templates/utils.html.j2
+-rw-r--r--   0        0        0     1545 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/templates.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/tests/__init__.py
+-rw-r--r--   0        0        0     5548 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/tests/test_templates.py
+-rw-r--r--   0        0        0      126 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/theme/utils.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/validation/__init__.py
+-rw-r--r--   0        0        0      138 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/validation/entities.py
+-rw-r--r--   0        0        0      785 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/validation/global_validators.py
+-rw-r--r--   0        0        0     1198 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/validation/lists_formatting.py
+-rw-r--r--   0        0        0      417 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/validation/page_validators.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/validation/tests/__init__.py
+-rw-r--r--   0        0        0     1061 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/validation/tests/test_global_validators.py
+-rw-r--r--   0        0        0     2745 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/validation/tests/test_lists_formatting.py
+-rw-r--r--   0        0        0      587 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/validation/tests/test_page_validators.py
+-rw-r--r--   0        0        0      731 2024-05-07 14:11:26.091611 brigid-0.6.0/brigid/validation/validators.py
+-rw-r--r--   0        0        0     3202 2024-05-07 14:11:37.811751 brigid-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3634 1970-01-01 00:00:00.000000 brigid-0.6.0/PKG-INFO
```

### Comparing `brigid-0.5.0/LICENSE` & `brigid-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/README.md` & `brigid-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/api/http_handlers.py` & `brigid-0.6.0/brigid/api/http_handlers.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/api/middlewares.py` & `brigid-0.6.0/brigid/api/middlewares.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/api/renderers.py` & `brigid-0.6.0/brigid/api/renderers.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from feedgenerator import Atom1Feed
 
 from brigid.api.utils import construct_index_description, construct_index_title, to_integer
 from brigid.core import errors
 from brigid.domain.urls import UrlsFeedsAtom, UrlsPost, UrlsTags
 from brigid.library.similarity import get_similar_pages
 from brigid.library.storage import storage
-from brigid.theme.entities import MetaInfo
+from brigid.theme.entities import MetaInfo, Template
 from brigid.theme.jinjaglobals import render_page_intro
 from brigid.theme.templates import render
 
 
 def render_index(language: str, raw_tags: str) -> HTMLResponse:  # noqa: CCR001, CFQ001
     site = storage.get_site()
 
@@ -91,24 +91,23 @@
         language=language,
         # TODO: construct language urls for filters
         #       it is complicated, because
         #       - we need to reset page number to 1 when changing language
         #       - we need to reapply filters to pages to calculate total pages
         allowed_languages=[],
         title=seo_title,
-        description=seo_description,
+        seo_description=seo_description,
         author=site.languages[language].author,
         tags=translated_tags_required,
         published_at=None,
         seo_image_url=None,
     )
 
-    # TODO: template names should have prefixes
     content = render(
-        "./blog_index.html.j2",
+        str(Template.index_page),
         {
             "language": language,
             "meta_info": meta_info,
             "site": site,
             "pages": pages,
             "current_url": filter_state,
             "article": None,
@@ -136,37 +135,37 @@
         raise errors.PageNotFound()
 
     page = storage.get_page(id=article.pages[language])
 
     similar_pages = get_similar_pages(language=language, original_page=page, number=site.posts_in_similar)
 
     # TODO: default template for each page type
-    template = page.template or site.default_page_template
+    template = page.template or Template.article_page
 
     post_url = UrlsPost(language=page.language, slug=article.slug)
 
     seo_image_url = None
 
     if page.seo_image:
         seo_image_url = post_url.file_url(page.seo_image)
 
     meta_info = MetaInfo(
         site_title=site.languages[language].title,
         language=language,
         allowed_languages=[language for language in site.allowed_languages if language in article.pages],
         title=page.title,
-        description=page.description,
+        seo_description=page.seo_description,
         author=site.languages[language].author,
         tags=[site.languages[language].tags_translations[tag] for tag in page.tags],
         published_at=page.published_at,
         seo_image_url=seo_image_url,
     )
 
     content = render(
-        template,
+        str(template),
         {
             "language": language,
             "meta_info": meta_info,
             "site": storage.get_site(),
             "article": article,
             "similar_pages": similar_pages,
             "page": page,
```

### Comparing `brigid-0.5.0/brigid/api/sitemaps.py` & `brigid-0.6.0/brigid/api/sitemaps.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/api/static_cache.py` & `brigid-0.6.0/brigid/api/static_cache.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/api/utils.py` & `brigid-0.6.0/brigid/api/utils.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/application/application.py` & `brigid-0.6.0/brigid/application/application.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,37 +50,28 @@
     logger.info("sentry_initialized")
 
     yield
 
     logger.info("sentry_disabled")
 
 
-def smart_url(domain: str, port: int) -> str:
-    if port == 80:
-        return f"http://{domain}"
-
-    if port == 443:
-        return f"https://{domain}"
-
-    return f"http://{domain}:{port}"
-
-
 def create_app() -> fastapi.FastAPI:  # noqa: CCR001
     logging.initialize(use_sentry=settings.sentry.enabled)
 
     logger.info("create_app")
 
     @contextlib.asynccontextmanager
     async def lifespan(app: fastapi.FastAPI) -> AsyncGenerator[None, None]:
         async with contextlib.AsyncExitStack() as stack:
             if settings.sentry.enabled:
                 await stack.enter_async_context(use_sentry())
 
             await app.router.startup()
 
+            # TODO: must be skipped in tests?
             discovering.load(directory=library_settings.directory)
 
             yield
 
             await app.router.shutdown()
 
     app = fastapi.FastAPI(
```

### Comparing `brigid-0.5.0/brigid/application/settings.py` & `brigid-0.6.0/brigid/application/settings.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import pydantic
 import pydantic_settings
 
 from brigid.core.settings import BaseSettings
+from brigid.domain.entities import Environment
 
 
 class Sentry(pydantic.BaseModel):
     enabled: bool = False
     dsn: str = ""
     sample_rate: float = 1.0
     enable_tracing: bool = False
     traces_sample_rate: float = 1.0
 
 
-_development_origins = ("*",)
+_local_origins = ("*",)
 
 
 class Settings(BaseSettings):
-    environment: str = "local"
+    environment: Environment = Environment.local
 
     sentry: Sentry = Sentry()
 
-    origins: tuple[str, ...] = _development_origins
+    origins: tuple[str, ...] = _local_origins
 
     @pydantic.model_validator(mode="after")
     def origin_must_be_redefined_in_prod(self) -> "Settings":
-        if self.environment == "prod" and self.origins == _development_origins:
+        if self.environment == Environment.prod and self.origins == _local_origins:
             raise ValueError("Origins must be redefined in prod")
 
         return self
 
     model_config = pydantic_settings.SettingsConfigDict(env_prefix="BRIGID_")
```

### Comparing `brigid-0.5.0/brigid/cli/commands/configs.py` & `brigid-0.6.0/brigid/cli/commands/configs.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/cli/commands/validate.py` & `brigid-0.6.0/brigid/cli/commands/validate.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/conftest.py` & `brigid-0.6.0/brigid/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import asyncio
+import os
 from typing import AsyncGenerator, Generator
 
 import fastapi
 import pytest
 import pytest_asyncio
 
 from brigid.application import application
 
 
 @pytest.fixture(scope="session", autouse=True)
+def mark_tests_running():
+    os.environ["BRIGID_TESTS_RUNNING"] = "True"
+
+
+@pytest.fixture(scope="session", autouse=True)
 def event_loop() -> Generator[asyncio.AbstractEventLoop, asyncio.AbstractEventLoop, None]:
     loop = asyncio.get_event_loop_policy().new_event_loop()
     yield loop
     loop.close()
 
 
 @pytest_asyncio.fixture(scope="session", autouse=True)
```

### Comparing `brigid-0.5.0/brigid/core/api.py` & `brigid-0.6.0/brigid/core/api.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/core/logging.py` & `brigid-0.6.0/brigid/core/logging.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/core/sentry.py` & `brigid-0.6.0/brigid/core/sentry.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/core/utils.py` & `brigid-0.6.0/brigid/core/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import importlib
 import pathlib
 import sys
 import types
 
 
 def discover_submodules(parent_module: str) -> list[types.ModuleType]:
@@ -32,7 +33,11 @@
 
         if submodule is None:
             submodule = importlib.import_module(full_module_name)
 
         child_modules.append(submodule)
 
     return child_modules
+
+
+def now() -> datetime.datetime:
+    return datetime.datetime.now(tz=datetime.timezone.utc)
```

### Comparing `brigid-0.5.0/brigid/domain/tests/test_html.py` & `brigid-0.6.0/brigid/domain/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/domain/urls.py` & `brigid-0.6.0/brigid/domain/urls.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/library/connectivity.py` & `brigid-0.6.0/brigid/library/connectivity.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/library/discovering.py` & `brigid-0.6.0/brigid/library/discovering.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/library/entities.py` & `brigid-0.6.0/brigid/library/entities.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from functools import cached_property
 from typing import Literal
 
 import pydantic
 
 from brigid.core.entities import BaseEntity
 from brigid.domain import urls
+from brigid.domain.entities import Environment
 
 MORE_RE = re.compile(r"<!--\s*more\s*-->", re.IGNORECASE)
 
 
 class MenuItemType(enum.StrEnum):
     article = "article"
     feed = "feed"
@@ -86,48 +87,69 @@
     referenced_from_score: int = 100
     referenced_to_score: int = 100
     bonus_per_reference: int = 10
     ignore_similar_tags: set[str] = pydantic.Field(default_factory=set)
     bonus_for_tags: dict[str, int] = pydantic.Field(default_factory=dict)
 
 
+class License(BaseEntity):
+    name: str
+    url: str
+
+
 class SiteLanguage(BaseEntity):
     title: str
     subtitle: str
     author: str
+    license: License | None = None
 
     tags_translations: dict[str, str] = pydantic.Field(default_factory=dict)
     theme_translations: dict[str, str] = pydantic.Field(default_factory=dict)
     seo_translations: dict[str, str] = pydantic.Field(default_factory=dict)
 
     menu: list[MenuItem] = pydantic.Field(default_factory=list)
 
 
 class Site(BaseEntity):
-    url: str  # TODO: pydantic.UrlStr
-
+    prod_url: pydantic.HttpUrl
+    local_url: pydantic.HttpUrl = pydantic.Field("http://0.0.0.0:8000")
     default_language: str
     allowed_languages: set[str] = pydantic.Field(default_factory=set)
     posts_per_page: int = 5
     posts_in_feed: int = 10
     posts_in_latest: int = 20
     posts_in_similar: int = 6
     languages: dict[str, SiteLanguage] = pydantic.Field(default_factory=dict)
-    default_page_template: str = "article.html.j2"
     favicon: str | None = None
 
     path: pathlib.Path
 
     footer_html: str | None = None
     header_html: str | None = None
 
+    content_repository: str | None = None
+
+    show_brigid_link: bool = True
+
     similarity: SimilarityConfig = SimilarityConfig()
 
     model_config = pydantic.ConfigDict(frozen=False)
 
+    @cached_property
+    def url(self) -> str:
+        from brigid.application.settings import settings
+
+        if settings.environment == Environment.prod:
+            return str(self.prod_url).rstrip("/")
+
+        if settings.environment == Environment.local:
+            return str(self.local_url).rstrip("/")
+
+        raise NotImplementedError(f"Unknown environment: {settings.environment}")
+
 
 class Article(BaseEntity):
     path: pathlib.Path
 
     slug: str
 
     type: ArticleType = ArticleType.post
@@ -167,15 +189,15 @@
     language: str
 
     title: str
 
     # Google could show max from 155 to 160 characters from description in the search results
     # Facebook, Twitter could show more characters
     # But we'll stick to minimum from maximum
-    description: str = pydantic.Field(max_length=155)
+    seo_description: str = pydantic.Field(max_length=155)
 
     # could be None, but page should define it explicitly
     seo_image: str | None
 
     body: str
 
     tags: set[str] = pydantic.Field(default_factory=list)
```

### Comparing `brigid-0.5.0/brigid/library/similarity.py` & `brigid-0.6.0/brigid/library/similarity.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/library/storage.py` & `brigid-0.6.0/brigid/library/storage.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/library/tests/make.py` & `brigid-0.6.0/brigid/library/tests/make.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
 import pathlib
 import uuid
 from typing import Iterable
 
+from brigid.core.utils import now
 from brigid.library.entities import Article, ArticleType, Page
 from brigid.library.storage import storage
 
 
 def article(
     path: pathlib.Path | None = None, slug: str | None = None, type: ArticleType = ArticleType.post
 ) -> Article:
@@ -29,15 +30,15 @@
 
 def page(  # noqa: CFQ002
     article: Article | None = None,
     path: pathlib.Path | None = None,
     published_at: datetime.datetime | None = None,
     language: str = "en",
     title: str | None = None,
-    description: str | None = None,
+    seo_description: str | None = None,
     seo_image: str | None = None,
     body: str | None = None,
     tags: Iterable[str] = (),
     template: str | None = None,
 ) -> Page:
 
     if article is None:
@@ -45,30 +46,30 @@
 
     if path is None:
         path = article.path.parent / f"{language}.md"
 
     if title is None:
         title = f"Title: {article.slug} {language}"
 
-    if description is None:
-        description = f"Description: {article.slug} {language}"
+    if seo_description is None:
+        seo_description = f"Description: {article.slug} {language}"
 
     if published_at is None:
-        published_at = datetime.datetime.now()
+        published_at = now()
 
     if body is None:
         body = f"Body: {article.slug} {language}"
 
     page = Page(
         article_id=article.id,
         path=path,
         published_at=published_at,
         language=language,
         title=title,
-        description=description,
+        seo_description=seo_description,
         seo_image=seo_image,
         body=body,
         tags=set(tags),
         template=template,
     )
 
     storage.add_page(page)
```

### Comparing `brigid-0.5.0/brigid/renderer/context.py` & `brigid-0.6.0/brigid/renderer/context.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/renderer/markdown_render.py` & `brigid-0.6.0/brigid/renderer/markdown_render.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/renderer/processors/collection_block.py` & `brigid-0.6.0/brigid/renderer/processors/collection_block.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/renderer/processors/external_links.py` & `brigid-0.6.0/brigid/renderer/processors/external_links.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,22 +30,23 @@
         parsed_site = urlparse(site.url)
 
         # validate external links
 
         # TODO: compare taking into account the default ports, aka example.com:90 = example.com
         # TODO: is this required, link could be to the same domain but in different project
         if parsed_site.netloc == parsed_url.netloc:
-            context.add_error(failed_text=data, message="No need to start local link with domain")
+            context.add_error(
+                failed_text=data, message="Use internal links syntax to specify links to the same domain"
+            )
             return result
 
-        if parsed_url.scheme == "" and parsed_url.netloc != "":
+        if parsed_url.scheme == "":
             context.add_error(failed_text=data, message="Specify schema/protocol for external links")
             return result
 
-        if parsed_url.scheme != "" and parsed_url.netloc == "":
-            context.add_error(failed_text=data, message="Specify domain for external links")
-            return result
+        # all external links must be with target="_blank"
+        result[0].set("target", "_blank")
 
         return result
 
 
 __all__ = ["ExternalLinkInlineProcessor", "EXTERNAL_LINK_RE"]
```

### Comparing `brigid-0.5.0/brigid/renderer/processors/header_anchors.py` & `brigid-0.6.0/brigid/renderer/processors/header_anchors.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/renderer/processors/images_block.py` & `brigid-0.6.0/brigid/renderer/processors/images_block.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/renderer/processors/internal_links.py` & `brigid-0.6.0/brigid/renderer/processors/internal_links.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/renderer/processors/snippets.py` & `brigid-0.6.0/brigid/renderer/processors/snippets.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/renderer/processors/tests/test_images_block.py` & `brigid-0.6.0/brigid/renderer/processors/tests/test_images_block.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/renderer/processors/toml_block.py` & `brigid-0.6.0/brigid/renderer/processors/toml_block.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/renderer/processors/youtube_block.py` & `brigid-0.6.0/brigid/renderer/processors/youtube_block.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/renderer/static_files.py` & `brigid-0.6.0/brigid/renderer/static_files.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/theme/default_translations.py` & `brigid-0.6.0/brigid/theme/default_translations.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,19 +4,25 @@
         "no_posts_found": "Ничего не найдено.",
         "pagination_first_page": "к новым",
         "pagination_last_page": "к старым",
         "tags_filter_header": "Нашли постов:",
         "article_similar_header": "Похожее",
         "last_posts_header": "Последние посты",
         "similarity_score_tooltip": "Уровень похожести",
+        "license": "лицензия",
+        "content_repository": "исходники постов",
+        "site_is_created_with": "сайт создан с помощью",
     },
     "en": {
         "read_more": "Read more",
         "no_posts_found": "Nothing found.",
         "pagination_first_page": "to new",
         "pagination_last_page": "to old",
         "tags_filter_header": "Found posts:",
         "article_similar_header": "Similar",
         "last_posts_header": "Last posts",
         "similarity_score_tooltip": "Similarity score",
+        "license": "license",
+        "content_repository": "content repository",
+        "site_is_created_with": "site is created with",
     },
 }
```

### Comparing `brigid-0.5.0/brigid/theme/jinjaglobals.py` & `brigid-0.6.0/brigid/theme/jinjaglobals.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,31 @@
+import os
 import pathlib
 
 from markupsafe import Markup
 
+from brigid.domain import constants as domain_constants
 from brigid.domain.urls import UrlsRoot
 from brigid.library.entities import Page
 from brigid.library.storage import Storage, storage
 from brigid.renderer.markdown_render import render_page as markdown_render_page
 from brigid.renderer.markdown_render import render_page_intro as markdown_render_page_intro
 from brigid.renderer.markdown_render import render_text as markdown_render_text
 from brigid.renderer.static_files import ImageInfo, files
 from brigid.theme.default_translations import translations
 from brigid.theme.settings import PhotoSwipe, settings
 from brigid.theme.utils import jinjafilter, jinjaglobal
 
 
 @jinjafilter
+def upper_first(text: str) -> str:
+    return text[0].upper() + text[1:]
+
+
+@jinjafilter
 def render_page(page: Page) -> str:
     return Markup(markdown_render_page(page=page).content)
 
 
 @jinjafilter
 def render_page_intro(page: Page) -> str:
     return Markup(markdown_render_page_intro(page=page).content)
@@ -68,7 +75,21 @@
     if language not in translations:
         language = "en"
 
     if text_id in translations[language]:
         return translations[language][text_id]
 
     return text_id
+
+
+@jinjaglobal
+def test_marker(marker: str) -> str:
+
+    if not os.environ.get("BRIGID_TESTS_RUNNING"):
+        return ""
+
+    return Markup(marker)
+
+
+@jinjaglobal
+def brigid_repository() -> str:
+    return domain_constants.brigid_repository
```

### Comparing `brigid-0.5.0/brigid/theme/settings.py` & `brigid-0.6.0/brigid/theme/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     stylesheet: str = "https://cdnjs.cloudflare.com/ajax/libs/photoswipe/5.4.2/photoswipe.min.css"
     lightbox: str = "https://cdnjs.cloudflare.com/ajax/libs/photoswipe/5.4.2/photoswipe-lightbox.esm.min.js"
     pswp: str = "https://cdnjs.cloudflare.com/ajax/libs/photoswipe/5.4.2/photoswipe.esm.min.js"
 
 
 class Templates(pydantic.BaseModel):
     directory: pathlib.Path = pathlib.Path(__file__).parent / "templates"
-    reload: bool = True
+    reload: bool = False
 
 
 class Settings(BaseSettings):
     photoswipe: PhotoSwipe = PhotoSwipe()
 
     templates: Templates = Templates()
```

### Comparing `brigid-0.5.0/brigid/theme/static/main.css` & `brigid-0.6.0/brigid/theme/static/main.css`

 * *Files 0% similar despite different names*

```diff
@@ -1867,15 +1867,15 @@
 }
 
 .brigid-index-navigation :where(.prose > :last-child):not(:where([class~="not-prose"],[class~="not-prose"] *)) {
   margin-bottom: 0;
 }
 
 .brigid-index-navigation {
-  margin-bottom: 1rem;
+  max-width: 42rem;
   border-bottom-width: 4px;
   border-style: double;
   .brigid-index-navigation-item {
     display: inline-block;
   }
 }
 
@@ -1999,14 +1999,35 @@
     .brigid-languages-list-active {
     }
     .brigid-languages-list-link {
       --tw-text-opacity: 1;
       color: rgb(148 163 184 / var(--tw-text-opacity));
     }
   }
+  .brigid-footer {
+    margin-top: 1rem;
+  }
+  .brigid-footer {
+    border-bottom-width: 0px;
+  }
+  .brigid-footer {
+    font-size: 0.875rem;
+    line-height: 1.25rem;
+  }
+  .brigid-footer {
+    ul {
+      margin: 0px;
+    }
+    ul {
+      list-style-type: none;
+    }
+    ul {
+      padding: 0px;
+    }
+  }
 }
 
 .brigid-article {
   color: var(--tw-prose-body);
   max-width: 65ch;
 }
 
@@ -2544,15 +2565,15 @@
   flex-grow: 1;
   border-bottom-width: 4px;
   border-style: double;
   margin-bottom: 2rem;
   padding-bottom: 1rem;
 }
 
-.brigid-article:last-child {
+.brigid-article:last-of-type {
   margin-bottom: 0px;
 }
 
 .brigid-article {
   a {
     text-decoration-color: #ea580c;
   }
```

### Comparing `brigid-0.5.0/brigid/theme/templates/article.html.j2` & `brigid-0.6.0/brigid/theme/templates/article.html.j2`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/theme/templates/article_footer.html.j2` & `brigid-0.6.0/brigid/theme/templates/article_footer.html.j2`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/theme/templates/blocks/collection.html.j2` & `brigid-0.6.0/brigid/theme/templates/blocks/collection.html.j2`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/theme/templates/blocks/images.html.j2` & `brigid-0.6.0/brigid/theme/templates/blocks/images.html.j2`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/theme/templates/blog_index.html.j2` & `brigid-0.6.0/brigid/theme/templates/blog_index.html.j2`

 * *Files 5% similar despite different names*

```diff
@@ -28,66 +28,77 @@
 000001b0: 6574 5f61 7274 6963 6c65 2869 643d 7061  et_article(id=pa
 000001c0: 6765 2e61 7274 6963 6c65 5f69 6429 2025  ge.article_id) %
 000001d0: 7d0a 0a20 2020 2020 2020 2020 2020 203c  }..            <
 000001e0: 6469 7620 636c 6173 733d 2262 7269 6769  div class="brigi
 000001f0: 642d 6172 7469 636c 6522 3e0a 2020 2020  d-article">.    
 00000200: 2020 2020 2020 2020 2020 3c68 313e 0a20            <h1>. 
 00000210: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000220: 6120 6872 6566 3d22 7b7b 726f 6f74 5f75  a href="{{root_u
-00000230: 726c 286c 616e 6775 6167 6529 2e74 6f5f  rl(language).to_
-00000240: 706f 7374 2861 7274 6963 6c65 2e73 6c75  post(article.slu
-00000250: 6729 2e75 726c 2829 7d7d 223e 7b7b 7061  g).url()}}">{{pa
-00000260: 6765 2e74 6974 6c65 7d7d 3c2f 613e 0a20  ge.title}}</a>. 
-00000270: 2020 2020 2020 2020 2020 2020 203c 2f68               </h
-00000280: 313e 0a0a 2020 2020 2020 2020 2020 2020  1>..            
-00000290: 2020 7b7b 7061 6765 7c72 656e 6465 725f    {{page|render_
-000002a0: 7061 6765 5f69 6e74 726f 7d7d 0a0a 2020  page_intro}}..  
-000002b0: 2020 2020 2020 2020 2020 2020 3c70 3e0a              <p>.
-000002c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000002d0: 3c61 2068 7265 663d 227b 7b72 6f6f 745f  <a href="{{root_
-000002e0: 7572 6c28 6c61 6e67 7561 6765 292e 746f  url(language).to
-000002f0: 5f70 6f73 7428 6172 7469 636c 652e 736c  _post(article.sl
-00000300: 7567 292e 7572 6c28 297d 7d22 3e0a 2020  ug).url()}}">.  
-00000310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000320: 7b7b 7472 616e 736c 6174 655f 7468 656d  {{translate_them
-00000330: 6528 6c61 6e67 7561 6765 2c20 2772 6561  e(language, 'rea
-00000340: 645f 6d6f 7265 2729 7d7d 0a20 2020 2020  d_more')}}.     
-00000350: 2020 2020 2020 2020 2020 203c 2f61 3e0a             </a>.
-00000360: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00000370: 703e 0a0a 2020 2020 2020 2020 2020 2020  p>..            
-00000380: 2020 7b7b 2061 7274 6963 6c65 5f66 6f6f    {{ article_foo
-00000390: 7465 7228 7061 6765 2920 7d7d 0a20 2020  ter(page) }}.   
-000003a0: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-000003b0: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
-000003c0: 666f 7220 257d 0a20 2020 2020 2020 203c  for %}.        <
-000003d0: 2f64 6976 3e0a 2020 2020 2020 2020 7b7b  /div>.        {{
-000003e0: 2070 6167 696e 6174 696f 6e28 6375 7272   pagination(curr
-000003f0: 656e 745f 7572 6c3d 6375 7272 656e 745f  ent_url=current_
-00000400: 7572 6c29 207d 7d0a 2020 2020 2020 7b25  url) }}.      {%
-00000410: 2065 6c73 6520 257d 0a20 2020 2020 2020   else %}.       
-00000420: 207b 2320 544f 444f 3a20 6265 7474 6572   {# TODO: better
-00000430: 2073 7479 6c65 7320 237d 0a20 2020 2020   styles #}.     
-00000440: 2020 203c 6469 7620 636c 6173 733d 2262     <div class="b
-00000450: 7269 6769 642d 696e 6465 782d 706f 7374  rigid-index-post
-00000460: 7322 3e0a 2020 2020 2020 2020 2020 3c64  s">.          <d
-00000470: 6976 2063 6c61 7373 3d22 6272 6967 6964  iv class="brigid
-00000480: 2d61 7274 6963 6c65 223e 0a20 2020 2020  -article">.     
-00000490: 2020 2020 2020 203c 703e 0a20 2020 2020         <p>.     
-000004a0: 2020 2020 2020 2020 207b 7b74 7261 6e73           {{trans
-000004b0: 6c61 7465 5f74 6865 6d65 286c 616e 6775  late_theme(langu
-000004c0: 6167 652c 2027 6e6f 5f70 6f73 7473 5f66  age, 'no_posts_f
-000004d0: 6f75 6e64 2729 7d7d 0a20 2020 2020 2020  ound')}}.       
-000004e0: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
-000004f0: 2020 3c2f 6469 763e 0a20 2020 2020 207b    </div>.      {
-00000500: 2520 656e 6469 6620 257d 0a20 2020 203c  % endif %}.    <
-00000510: 2f64 6976 3e0a 0a20 2020 203c 6e61 7620  /div>..    <nav 
-00000520: 636c 6173 733d 2262 7269 6769 642d 7369  class="brigid-si
-00000530: 6465 2d62 6c6f 636b 223e 0a20 2020 2020  de-block">.     
-00000540: 207b 7b20 7461 6773 5f66 696c 7465 7228   {{ tags_filter(
-00000550: 6375 7272 656e 745f 7572 6c3d 6375 7272  current_url=curr
-00000560: 656e 745f 7572 6c2c 2074 6167 735f 636f  ent_url, tags_co
-00000570: 756e 743d 7461 6773 5f63 6f75 6e74 2c20  unt=tags_count, 
-00000580: 7369 7465 3d73 6974 652c 2070 6167 6573  site=site, pages
-00000590: 5f66 6f75 6e64 3d70 6167 6573 5f66 6f75  _found=pages_fou
-000005a0: 6e64 2920 7d7d 0a20 2020 203c 2f6e 6176  nd) }}.    </nav
-000005b0: 3e0a 0a20 203c 2f64 6976 3e0a 0a7b 2520  >..  </div>..{% 
-000005c0: 656e 6462 6c6f 636b 2025 7d0a            endblock %}.
+00000220: 6120 636c 6173 733d 227b 7b74 6573 745f  a class="{{test_
+00000230: 6d61 726b 6572 2827 7465 7374 2d70 6167  marker('test-pag
+00000240: 652d 6865 6164 6572 2d6c 696e 6b27 297d  e-header-link')}
+00000250: 7d22 2068 7265 663d 227b 7b72 6f6f 745f  }" href="{{root_
+00000260: 7572 6c28 6c61 6e67 7561 6765 292e 746f  url(language).to
+00000270: 5f70 6f73 7428 6172 7469 636c 652e 736c  _post(article.sl
+00000280: 7567 292e 7572 6c28 297d 7d22 3e7b 7b70  ug).url()}}">{{p
+00000290: 6167 652e 7469 746c 657d 7d3c 2f61 3e0a  age.title}}</a>.
+000002a0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+000002b0: 6831 3e0a 0a20 2020 2020 2020 2020 2020  h1>..           
+000002c0: 2020 207b 7b70 6167 657c 7265 6e64 6572     {{page|render
+000002d0: 5f70 6167 655f 696e 7472 6f7d 7d0a 0a20  _page_intro}}.. 
+000002e0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+000002f0: 6966 2070 6167 652e 6861 735f 6d6f 7265  if page.has_more
+00000300: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00000310: 2020 2020 3c70 3e0a 2020 2020 2020 2020      <p>.        
+00000320: 2020 2020 2020 2020 2020 3c61 2063 6c61            <a cla
+00000330: 7373 3d22 7b7b 7465 7374 5f6d 6172 6b65  ss="{{test_marke
+00000340: 7228 2774 6573 742d 7061 6765 2d6d 6f72  r('test-page-mor
+00000350: 652d 6c69 6e6b 2729 7d7d 2220 6872 6566  e-link')}}" href
+00000360: 3d22 7b7b 726f 6f74 5f75 726c 286c 616e  ="{{root_url(lan
+00000370: 6775 6167 6529 2e74 6f5f 706f 7374 2861  guage).to_post(a
+00000380: 7274 6963 6c65 2e73 6c75 6729 2e75 726c  rticle.slug).url
+00000390: 2829 7d7d 223e 0a20 2020 2020 2020 2020  ()}}">.         
+000003a0: 2020 2020 2020 2020 2020 207b 7b74 7261             {{tra
+000003b0: 6e73 6c61 7465 5f74 6865 6d65 286c 616e  nslate_theme(lan
+000003c0: 6775 6167 652c 2027 7265 6164 5f6d 6f72  guage, 'read_mor
+000003d0: 6527 297d 7d0a 2020 2020 2020 2020 2020  e')}}.          
+000003e0: 2020 2020 2020 2020 3c2f 613e 0a20 2020          </a>.   
+000003f0: 2020 2020 2020 2020 2020 2020 203c 2f70               </p
+00000400: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000410: 7b25 2065 6e64 6966 2025 7d0a 0a20 2020  {% endif %}..   
+00000420: 2020 2020 2020 2020 2020 207b 7b20 6172             {{ ar
+00000430: 7469 636c 655f 666f 6f74 6572 2870 6167  ticle_footer(pag
+00000440: 6529 207d 7d0a 2020 2020 2020 2020 2020  e) }}.          
+00000450: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00000460: 2020 207b 2520 656e 6466 6f72 2025 7d0a     {% endfor %}.
+00000470: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00000480: 2020 2020 2020 207b 7b20 7061 6769 6e61         {{ pagina
+00000490: 7469 6f6e 2863 7572 7265 6e74 5f75 726c  tion(current_url
+000004a0: 3d63 7572 7265 6e74 5f75 726c 2920 7d7d  =current_url) }}
+000004b0: 0a20 2020 2020 207b 2520 656c 7365 2025  .      {% else %
+000004c0: 7d0a 2020 2020 2020 2020 7b23 2054 4f44  }.        {# TOD
+000004d0: 4f3a 2062 6574 7465 7220 7374 796c 6573  O: better styles
+000004e0: 2023 7d0a 2020 2020 2020 2020 3c64 6976   #}.        <div
+000004f0: 2063 6c61 7373 3d22 6272 6967 6964 2d69   class="brigid-i
+00000500: 6e64 6578 2d70 6f73 7473 223e 0a20 2020  ndex-posts">.   
+00000510: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00000520: 733d 2262 7269 6769 642d 6172 7469 636c  s="brigid-articl
+00000530: 6522 3e0a 2020 2020 2020 2020 2020 2020  e">.            
+00000540: 3c70 3e0a 2020 2020 2020 2020 2020 2020  <p>.            
+00000550: 2020 7b7b 7472 616e 736c 6174 655f 7468    {{translate_th
+00000560: 656d 6528 6c61 6e67 7561 6765 2c20 276e  eme(language, 'n
+00000570: 6f5f 706f 7374 735f 666f 756e 6427 297d  o_posts_found')}
+00000580: 7d0a 2020 2020 2020 2020 2020 3c2f 6469  }.          </di
+00000590: 763e 0a20 2020 2020 2020 203c 2f64 6976  v>.        </div
+000005a0: 3e0a 2020 2020 2020 7b25 2065 6e64 6966  >.      {% endif
+000005b0: 2025 7d0a 2020 2020 3c2f 6469 763e 0a0a   %}.    </div>..
+000005c0: 2020 2020 3c6e 6176 2063 6c61 7373 3d22      <nav class="
+000005d0: 6272 6967 6964 2d73 6964 652d 626c 6f63  brigid-side-bloc
+000005e0: 6b22 3e0a 2020 2020 2020 7b7b 2074 6167  k">.      {{ tag
+000005f0: 735f 6669 6c74 6572 2863 7572 7265 6e74  s_filter(current
+00000600: 5f75 726c 3d63 7572 7265 6e74 5f75 726c  _url=current_url
+00000610: 2c20 7461 6773 5f63 6f75 6e74 3d74 6167  , tags_count=tag
+00000620: 735f 636f 756e 742c 2073 6974 653d 7369  s_count, site=si
+00000630: 7465 2c20 7061 6765 735f 666f 756e 643d  te, pages_found=
+00000640: 7061 6765 735f 666f 756e 6429 207d 7d0a  pages_found) }}.
+00000650: 2020 2020 3c2f 6e61 763e 0a0a 2020 3c2f      </nav>..  </
+00000660: 6469 763e 0a0a 7b25 2065 6e64 626c 6f63  div>..{% endbloc
+00000670: 6b20 257d 0a                             k %}.
```

### Comparing `brigid-0.5.0/brigid/theme/templates/header.html.j2` & `brigid-0.6.0/brigid/theme/templates/header.html.j2`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/theme/templates/languages_links.html.j2` & `brigid-0.6.0/brigid/theme/templates/languages_links.html.j2`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/theme/templates/meta.html.j2` & `brigid-0.6.0/brigid/theme/templates/meta.html.j2`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
       {% continue %}
     {% endif %}
     <link rel="alternate" hreflang="{{language}}" href="{{current_url.to_language(language).url()}}">
   {% endfor %}
 
   <title>{{meta_info.title}}</title>
 
-  <meta name="description" content="{{meta_info.description}}">
+  <meta name="description" content="{{meta_info.seo_description}}">
 
   <meta name="keywords" content="{{', '.join(meta_info.tags|sort)}}">
 
   <meta name="author" content="{{meta_info.author}}">
 
   <meta name="referrer" content="unsafe-URL">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
@@ -94,15 +94,15 @@
 
   {% if meta_info.seo_image_url %}
     <meta property="og:image" content="{{meta_info.seo_image_url}}">
   {% endif %}
 
   <meta property="og:url" content="{{current_url.url()}}">
 
-  <meta property="og:description" content="{{meta_info.description}}">
+  <meta property="og:description" content="{{meta_info.seo_description}}">
 
   {# TODO: do we need to specify territories with langúage codes? #}
   {# og:locale - The locale these tags are marked up in. Of the format language_TERRITORY. Default is en_US. #}
   <meta property="og:locale" content="{{meta_info.language}}">
 
   {% for language in meta_info.allowed_languages %}
     {% if language == meta_info.language %}
@@ -123,15 +123,15 @@
 
   <meta property="article:author" content="{{meta_info.author}}">
 
   <meta property="og:image" content="./favicon.ico">
 
   <meta property="og:url" content="{{current_url.url()}}">
 
-  <meta property="og:description" content="{{meta_info.description}}">
+  <meta property="og:description" content="{{meta_info.seo_description}}">
 
   {# TODO: do we need to specify territories with langúage codes? #}
   {# og:locale - The locale these tags are marked up in. Of the format language_TERRITORY. Default is en_US. #}
   <meta property="og:locale" content="{{meta_info.language}}">
 
   {% for language in meta_info.allowed_languages %}
     {% if language == meta_info.language %}
```

### Comparing `brigid-0.5.0/brigid/theme/templates/pagination.html.j2` & `brigid-0.6.0/brigid/theme/templates/pagination.html.j2`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/theme/templates/similar_pages.html.j2` & `brigid-0.6.0/brigid/theme/templates/similar_pages.html.j2`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/theme/templates/tags_filter.html.j2` & `brigid-0.6.0/brigid/theme/templates/tags_filter.html.j2`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/theme/templates.py` & `brigid-0.6.0/brigid/theme/templates.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/validation/global_validators.py` & `brigid-0.6.0/brigid/validation/global_validators.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/validation/lists_formatting.py` & `brigid-0.6.0/brigid/validation/lists_formatting.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/validation/tests/test_global_validators.py` & `brigid-0.6.0/brigid/validation/tests/test_global_validators.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/validation/tests/test_lists_formatting.py` & `brigid-0.6.0/brigid/validation/tests/test_lists_formatting.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/validation/tests/test_page_validators.py` & `brigid-0.6.0/brigid/validation/tests/test_page_validators.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/brigid/validation/validators.py` & `brigid-0.6.0/brigid/validation/validators.py`

 * *Files identical despite different names*

### Comparing `brigid-0.5.0/pyproject.toml` & `brigid-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brigid"
-version = "0.5.0"
+version = "0.6.0"
 description = "Static site generator."
 readme = "README.md"
 repository = "https://github.com/Tiendil/brigid"
 authors = ["Aliaksei Yaletski (Tiendil) <a.eletsky@gmail.com>"]
 license = "BSD-3-Clause"
 keywords = ["blog", "blog-engine", "site", "markdown", "cms", "content management system", "personal site"]
 classifiers = [
@@ -44,14 +44,15 @@
 
 jinja2 = "3.1.*"
 markdown = "3.5.*"
 pymdown-extensions = "10.7.*"
 python-frontmatter = "1.1.*"
 feedgenerator = "2.1.*"
 beautifulsoup4 = "4.12.*"
+html5lib = "1.1.*"
 
 sentry-sdk = "1.39.*"
 typer = "0.9.*"
 
 [tool.poetry.dev-dependencies]
 uvicorn = {version = "0.27.*", extras = ["standard"]}
```

### Comparing `brigid-0.5.0/PKG-INFO` & `brigid-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brigid
-Version: 0.5.0
+Version: 0.6.0
 Summary: Static site generator.
 Home-page: https://github.com/Tiendil/brigid
 License: BSD-3-Clause
 Keywords: blog,blog-engine,site,markdown,cms,content management system,personal site
 Author: Aliaksei Yaletski (Tiendil)
 Author-email: a.eletsky@gmail.com
 Requires-Python: >=3.12,<4.0
@@ -29,14 +29,15 @@
 Classifier: Topic :: Office/Business :: News/Diary
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Requires-Dist: beautifulsoup4 (==4.12.*)
 Requires-Dist: fastapi (==0.109.*)
 Requires-Dist: feedgenerator (==2.1.*)
+Requires-Dist: html5lib (==1.1.*)
 Requires-Dist: jinja2 (==3.1.*)
 Requires-Dist: markdown (==3.5.*)
 Requires-Dist: pillow (==10.2.*)
 Requires-Dist: pydantic (==2.5.*)
 Requires-Dist: pydantic-settings (==2.1.*)
 Requires-Dist: pymdown-extensions (==10.7.*)
 Requires-Dist: python-frontmatter (==1.1.*)
```

