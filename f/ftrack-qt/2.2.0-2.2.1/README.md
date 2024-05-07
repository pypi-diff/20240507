# Comparing `tmp/ftrack_qt-2.2.0.tar.gz` & `tmp/ftrack_qt-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftrack_qt-2.2.0.tar", max compression
+gzip compressed data, was "ftrack_qt-2.2.1.tar", max compression
```

## Comparing `ftrack_qt-2.2.0.tar` & `ftrack_qt-2.2.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0    10176 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/LICENSE.txt
--rw-r--r--   0        0        0      168 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/README.md
--rw-r--r--   0        0        0     1136 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      895 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/__init__.py
--rw-r--r--   0        0        0       57 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/utils/__init__.py
--rw-r--r--   0        0        0       74 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/utils/decorators/__init__.py
--rw-r--r--   0        0        0      369 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/utils/decorators/threading.py
--rw-r--r--   0        0        0      988 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/utils/layout/__init__.py
--rw-r--r--   0        0        0     1149 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/utils/theme/__init__.py
--rw-r--r--   0        0        0     1251 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/utils/threading/__init__.py
--rw-r--r--   0        0        0     4519 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/utils/widget/__init__.py
--rw-r--r--   0        0        0       57 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/__init__.py
--rw-r--r--   0        0        0       77 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/accordion/__init__.py
--rw-r--r--   0        0        0     9497 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/accordion/accordion_widget.py
--rw-r--r--   0        0        0      267 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/asset/__init__.py
--rw-r--r--   0        0        0     3723 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/asset/asset_version_creation_widget.py
--rw-r--r--   0        0        0     4100 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/asset/asset_version_selection_widget.py
--rw-r--r--   0        0        0     4230 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/asset/new_asset_input_widget.py
--rw-r--r--   0        0        0      132 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/browsers/__init__.py
--rw-r--r--   0        0        0    30840 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/browsers/entity_browser.py
--rw-r--r--   0        0        0     2040 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/browsers/file_browser.py
--rw-r--r--   0        0        0      257 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/buttons/__init__.py
--rw-r--r--   0        0        0     1595 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/buttons/circular_button.py
--rw-r--r--   0        0        0     4099 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/buttons/options_button.py
--rw-r--r--   0        0        0     7300 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/buttons/progress_button.py
--rw-r--r--   0        0        0      168 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/delegate/__init__.py
--rw-r--r--   0        0        0     1716 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/delegate/asset_version_combo_box_delegate.py
--rw-r--r--   0        0        0      346 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/dialogs/__init__.py
--rw-r--r--   0        0        0     1003 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/dialogs/file_dialog.py
--rw-r--r--   0        0        0     4997 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/dialogs/modal_dialog.py
--rw-r--r--   0        0        0     6485 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/dialogs/scroll_tool_configs_dialog.py
--rw-r--r--   0        0        0     3199 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/dialogs/styled_dialog.py
--rw-r--r--   0        0        0     3525 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/dialogs/tab_dialog.py
--rw-r--r--   0        0        0      167 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/headers/__init__.py
--rw-r--r--   0        0        0     6079 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/headers/accordion_header_widget.py
--rw-r--r--   0        0        0     3013 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/headers/session_header_widget.py
--rw-r--r--   0        0        0      207 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/icons/__init__.py
--rw-r--r--   0        0        0      723 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/icons/arrow_icon.py
--rw-r--r--   0        0        0     2461 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/icons/material_icon.py
--rw-r--r--   0        0        0     2869 2024-05-02 08:05:12.046416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/icons/status_icon.py
--rw-r--r--   0        0        0       58 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/info/__init__.py
--rw-r--r--   0        0        0     2687 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/info/entity_info.py
--rw-r--r--   0        0        0       59 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/lines/__init__.py
--rw-r--r--   0        0        0     1255 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/lines/line_widget.py
--rw-r--r--   0        0        0       57 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/lists/__init__.py
--rw-r--r--   0        0        0     5474 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/lists/asset_list.py
--rw-r--r--   0        0        0       59 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/logos/__init__.py
--rw-r--r--   0        0        0     1191 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/logos/ftrack_logo.py
--rw-r--r--   0        0        0      118 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/models/__init__.py
--rw-r--r--   0        0        0     3766 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/models/table_model.py
--rw-r--r--   0        0        0      264 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/overlay/__init__.py
--rw-r--r--   0        0        0     3221 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/overlay/busy_indicator_widget.py
--rw-r--r--   0        0        0     1684 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/overlay/overlay_widget.py
--rw-r--r--   0        0        0     1074 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/overlay/shaded_widget.py
--rw-r--r--   0        0        0      128 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/progress/__init__.py
--rw-r--r--   0        0        0    12979 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/progress/progress_widget.py
--rw-r--r--   0        0        0       70 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/search/__init__.py
--rw-r--r--   0        0        0     3684 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/search/collapsable_search_box.py
--rw-r--r--   0        0        0      392 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/selectors/__init__.py
--rw-r--r--   0        0        0     8949 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/selectors/asset_selector.py
--rw-r--r--   0        0        0     8032 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/selectors/context_selector.py
--rw-r--r--   0        0        0     3526 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/selectors/list_selector.py
--rw-r--r--   0        0        0     1712 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/selectors/status_selector.py
--rw-r--r--   0        0        0     1571 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/selectors/version_selector.py
--rw-r--r--   0        0        0      486 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/__init__.py
--rw-r--r--   0        0        0      920 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/asset_version_thumbnail.py
--rw-r--r--   0        0        0     5714 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/base_thumbnail.py
--rw-r--r--   0        0        0     1950 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/context_thumbnail.py
--rw-r--r--   0        0        0     1007 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/ellipse_thumbnail.py
--rw-r--r--   0        0        0     5783 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/session_base_thumbnail.py
--rw-r--r--   0        0        0     1149 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/user_thumbnail.py
--rw-r--r--   0        0        0      116 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/user/__init__.py
--rw-r--r--   0        0        0     2453 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/user/ftrack_user.py
--rw-r--r--   0        0        0      115 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/views/__init__.py
--rw-r--r--   0        0        0     1676 2024-05-02 08:05:12.050416 ftrack_qt-2.2.0/source/ftrack_qt/widgets/views/table_view.py
--rw-r--r--   0        0        0     1301 1970-01-01 00:00:00.000000 ftrack_qt-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10176 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/LICENSE.txt
+-rw-r--r--   0        0        0      168 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/README.md
+-rw-r--r--   0        0        0     1136 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0      895 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/__init__.py
+-rw-r--r--   0        0        0       57 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/utils/__init__.py
+-rw-r--r--   0        0        0       74 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/utils/decorators/__init__.py
+-rw-r--r--   0        0        0      369 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/utils/decorators/threading.py
+-rw-r--r--   0        0        0      988 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/utils/layout/__init__.py
+-rw-r--r--   0        0        0     1149 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/utils/theme/__init__.py
+-rw-r--r--   0        0        0     1251 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/utils/threading/__init__.py
+-rw-r--r--   0        0        0     4518 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/utils/widget/__init__.py
+-rw-r--r--   0        0        0       57 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/__init__.py
+-rw-r--r--   0        0        0       77 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/accordion/__init__.py
+-rw-r--r--   0        0        0     9497 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/accordion/accordion_widget.py
+-rw-r--r--   0        0        0      267 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/asset/__init__.py
+-rw-r--r--   0        0        0     3723 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/asset/asset_version_creation_widget.py
+-rw-r--r--   0        0        0     4100 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/asset/asset_version_selection_widget.py
+-rw-r--r--   0        0        0     4230 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/asset/new_asset_input_widget.py
+-rw-r--r--   0        0        0      132 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/browsers/__init__.py
+-rw-r--r--   0        0        0    30840 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/browsers/entity_browser.py
+-rw-r--r--   0        0        0     2040 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/browsers/file_browser.py
+-rw-r--r--   0        0        0      257 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/buttons/__init__.py
+-rw-r--r--   0        0        0     1595 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/buttons/circular_button.py
+-rw-r--r--   0        0        0     4099 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/buttons/options_button.py
+-rw-r--r--   0        0        0     7300 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/buttons/progress_button.py
+-rw-r--r--   0        0        0      168 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/delegate/__init__.py
+-rw-r--r--   0        0        0     1716 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/delegate/asset_version_combo_box_delegate.py
+-rw-r--r--   0        0        0      346 2024-05-07 10:30:32.750489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/dialogs/__init__.py
+-rw-r--r--   0        0        0     1003 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/dialogs/file_dialog.py
+-rw-r--r--   0        0        0     4997 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/dialogs/modal_dialog.py
+-rw-r--r--   0        0        0     6485 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/dialogs/scroll_tool_configs_dialog.py
+-rw-r--r--   0        0        0     3199 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/dialogs/styled_dialog.py
+-rw-r--r--   0        0        0     3525 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/dialogs/tab_dialog.py
+-rw-r--r--   0        0        0      167 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/headers/__init__.py
+-rw-r--r--   0        0        0     6079 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/headers/accordion_header_widget.py
+-rw-r--r--   0        0        0     3013 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/headers/session_header_widget.py
+-rw-r--r--   0        0        0      207 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/icons/__init__.py
+-rw-r--r--   0        0        0      723 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/icons/arrow_icon.py
+-rw-r--r--   0        0        0     2461 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/icons/material_icon.py
+-rw-r--r--   0        0        0     2869 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/icons/status_icon.py
+-rw-r--r--   0        0        0       58 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/info/__init__.py
+-rw-r--r--   0        0        0     2687 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/info/entity_info.py
+-rw-r--r--   0        0        0       59 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/lines/__init__.py
+-rw-r--r--   0        0        0     1255 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/lines/line_widget.py
+-rw-r--r--   0        0        0       57 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/lists/__init__.py
+-rw-r--r--   0        0        0     5474 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/lists/asset_list.py
+-rw-r--r--   0        0        0       59 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/logos/__init__.py
+-rw-r--r--   0        0        0     1191 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/logos/ftrack_logo.py
+-rw-r--r--   0        0        0      118 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/models/__init__.py
+-rw-r--r--   0        0        0     3766 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/models/table_model.py
+-rw-r--r--   0        0        0      264 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/overlay/__init__.py
+-rw-r--r--   0        0        0     3221 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/overlay/busy_indicator_widget.py
+-rw-r--r--   0        0        0     1684 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/overlay/overlay_widget.py
+-rw-r--r--   0        0        0     1074 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/overlay/shaded_widget.py
+-rw-r--r--   0        0        0      128 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/progress/__init__.py
+-rw-r--r--   0        0        0    12979 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/progress/progress_widget.py
+-rw-r--r--   0        0        0       70 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/search/__init__.py
+-rw-r--r--   0        0        0     3684 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/search/collapsable_search_box.py
+-rw-r--r--   0        0        0      392 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/selectors/__init__.py
+-rw-r--r--   0        0        0     8949 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/selectors/asset_selector.py
+-rw-r--r--   0        0        0     8032 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/selectors/context_selector.py
+-rw-r--r--   0        0        0     3526 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/selectors/list_selector.py
+-rw-r--r--   0        0        0     1712 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/selectors/status_selector.py
+-rw-r--r--   0        0        0     1571 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/selectors/version_selector.py
+-rw-r--r--   0        0        0      486 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/thumbnails/__init__.py
+-rw-r--r--   0        0        0      920 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/thumbnails/asset_version_thumbnail.py
+-rw-r--r--   0        0        0     5714 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/thumbnails/base_thumbnail.py
+-rw-r--r--   0        0        0     1950 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/thumbnails/context_thumbnail.py
+-rw-r--r--   0        0        0     1007 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/thumbnails/ellipse_thumbnail.py
+-rw-r--r--   0        0        0     5783 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/thumbnails/session_base_thumbnail.py
+-rw-r--r--   0        0        0     1149 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/thumbnails/user_thumbnail.py
+-rw-r--r--   0        0        0      116 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/user/__init__.py
+-rw-r--r--   0        0        0     2453 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/user/ftrack_user.py
+-rw-r--r--   0        0        0      115 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/views/__init__.py
+-rw-r--r--   0        0        0     1676 2024-05-07 10:30:32.754489 ftrack_qt-2.2.1/source/ftrack_qt/widgets/views/table_view.py
+-rw-r--r--   0        0        0     1301 1970-01-01 00:00:00.000000 ftrack_qt-2.2.1/PKG-INFO
```

### Comparing `ftrack_qt-2.2.0/LICENSE.txt` & `ftrack_qt-2.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/pyproject.toml` & `ftrack_qt-2.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ftrack-qt"
-version = "2.2.0"
+version = "2.2.1"
 description='ftrack qt library'
 authors = ["ftrack Integrations Team <integrations@backlight.co>"]
 readme = "README.md"
 packages = [{include = "ftrack_qt", from = "source"}]
 license = "Apache-2.0"
 homepage = "https://ftrack.com"
 repository = "https://github.com/ftrackhq/integrations/tree/main/libs/qt"
```

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/__init__.py` & `ftrack_qt-2.2.1/source/ftrack_qt/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/utils/layout/__init__.py` & `ftrack_qt-2.2.1/source/ftrack_qt/utils/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/utils/theme/__init__.py` & `ftrack_qt-2.2.1/source/ftrack_qt/utils/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/utils/threading/__init__.py` & `ftrack_qt-2.2.1/source/ftrack_qt/utils/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/utils/widget/__init__.py` & `ftrack_qt-2.2.1/source/ftrack_qt/utils/widget/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     Args:
         widget (QWidget): The widget on which to set the properties.
         properties (dict): A dictionary of property names and values.
     """
     for name, value in properties.items():
         widget.setProperty(name, value)
-        if widget.style() is not None and shiboken2.isValid(
+        if widget.style() is not None and shiboken.isValid(
             widget.style()
         ):  # Only update style if applied and valid
             widget.style().unpolish(widget)
             widget.style().polish(widget)
         widget.update()
```

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/accordion/accordion_widget.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/accordion/accordion_widget.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/asset/asset_version_creation_widget.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/asset/asset_version_creation_widget.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/asset/asset_version_selection_widget.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/asset/asset_version_selection_widget.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/asset/new_asset_input_widget.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/asset/new_asset_input_widget.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/browsers/entity_browser.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/browsers/entity_browser.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/browsers/file_browser.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/browsers/file_browser.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/buttons/circular_button.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/buttons/circular_button.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/buttons/options_button.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/buttons/options_button.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/buttons/progress_button.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/buttons/progress_button.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/delegate/asset_version_combo_box_delegate.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/delegate/asset_version_combo_box_delegate.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/dialogs/file_dialog.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/dialogs/file_dialog.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/dialogs/modal_dialog.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/dialogs/modal_dialog.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/dialogs/scroll_tool_configs_dialog.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/dialogs/scroll_tool_configs_dialog.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/dialogs/styled_dialog.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/dialogs/styled_dialog.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/dialogs/tab_dialog.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/dialogs/tab_dialog.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/headers/accordion_header_widget.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/headers/accordion_header_widget.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/headers/session_header_widget.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/headers/session_header_widget.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/icons/arrow_icon.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/icons/arrow_icon.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/icons/material_icon.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/icons/material_icon.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/icons/status_icon.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/icons/status_icon.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/info/entity_info.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/info/entity_info.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/lines/line_widget.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/lines/line_widget.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/lists/asset_list.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/lists/asset_list.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/logos/ftrack_logo.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/logos/ftrack_logo.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/models/table_model.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/models/table_model.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/overlay/busy_indicator_widget.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/overlay/busy_indicator_widget.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/overlay/overlay_widget.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/overlay/overlay_widget.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/overlay/shaded_widget.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/overlay/shaded_widget.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/progress/progress_widget.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/progress/progress_widget.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/search/collapsable_search_box.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/search/collapsable_search_box.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/selectors/asset_selector.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/selectors/asset_selector.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/selectors/context_selector.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/selectors/context_selector.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/selectors/list_selector.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/selectors/list_selector.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/selectors/status_selector.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/selectors/status_selector.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/selectors/version_selector.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/selectors/version_selector.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/asset_version_thumbnail.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/thumbnails/asset_version_thumbnail.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/base_thumbnail.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/thumbnails/base_thumbnail.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/context_thumbnail.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/thumbnails/context_thumbnail.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/ellipse_thumbnail.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/thumbnails/ellipse_thumbnail.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/session_base_thumbnail.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/thumbnails/session_base_thumbnail.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/thumbnails/user_thumbnail.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/thumbnails/user_thumbnail.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/user/ftrack_user.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/user/ftrack_user.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/source/ftrack_qt/widgets/views/table_view.py` & `ftrack_qt-2.2.1/source/ftrack_qt/widgets/views/table_view.py`

 * *Files identical despite different names*

### Comparing `ftrack_qt-2.2.0/PKG-INFO` & `ftrack_qt-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftrack-qt
-Version: 2.2.0
+Version: 2.2.1
 Summary: ftrack qt library
 Home-page: https://ftrack.com
 License: Apache-2.0
 Author: ftrack Integrations Team
 Author-email: integrations@backlight.co
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```

