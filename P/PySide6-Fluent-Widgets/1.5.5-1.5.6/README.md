# Comparing `tmp/PySide6-Fluent-Widgets-1.5.5.tar.gz` & `tmp/PySide6-Fluent-Widgets-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySide6-Fluent-Widgets-1.5.5.tar", last modified: Sat Apr 13 06:40:11 2024, max compression
+gzip compressed data, was "dist\PySide6-Fluent-Widgets-1.5.6.tar", last modified: Tue May  7 03:43:54 2024, max compression
```

## Comparing `PySide6-Fluent-Widgets-1.5.5.tar` & `PySide6-Fluent-Widgets-1.5.6.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.391186 PySide6-Fluent-Widgets-1.5.5/
--rw-rw-rw-   0        0        0    35823 2024-04-13 06:31:05.000000 PySide6-Fluent-Widgets-1.5.5/LICENSE
--rw-rw-rw-   0        0        0     5183 2024-04-13 06:40:11.390162 PySide6-Fluent-Widgets-1.5.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.188526 PySide6-Fluent-Widgets-1.5.5/PySide6_Fluent_Widgets.egg-info/
--rw-rw-rw-   0        0        0     5183 2024-04-13 06:40:11.000000 PySide6-Fluent-Widgets-1.5.5/PySide6_Fluent_Widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4929 2024-04-13 06:40:11.000000 PySide6-Fluent-Widgets-1.5.5/PySide6_Fluent_Widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 06:40:11.000000 PySide6-Fluent-Widgets-1.5.5/PySide6_Fluent_Widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2024-04-13 06:40:11.000000 PySide6-Fluent-Widgets-1.5.5/PySide6_Fluent_Widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-13 06:40:11.000000 PySide6-Fluent-Widgets-1.5.5/PySide6_Fluent_Widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4399 2024-04-13 06:31:05.000000 PySide6-Fluent-Widgets-1.5.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.190908 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/
--rw-rw-rw-   0        0        0      566 2024-04-13 06:31:18.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.194044 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/_rc/
--rw-rw-rw-   0        0        0        0 2023-10-15 01:50:42.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/_rc/__init__.py
--rw-rw-rw-   0        0        0  3307370 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.230411 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/
--rw-rw-rw-   0        0        0      664 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/__init__.py
--rw-rw-rw-   0        0        0    15208 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/animation.py
--rw-rw-rw-   0        0        0     4742 2023-12-29 09:55:21.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/auto_wrap.py
--rw-rw-rw-   0        0        0     1589 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/color.py
--rw-rw-rw-   0        0        0    11172 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/config.py
--rw-rw-rw-   0        0        0      675 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/exception_handler.py
--rw-rw-rw-   0        0        0      807 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/font.py
--rw-rw-rw-   0        0        0    13725 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/icon.py
--rw-rw-rw-   0        0        0     5554 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/image_utils.py
--rw-rw-rw-   0        0        0     1635 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/overload.py
--rw-rw-rw-   0        0        0     3862 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/router.py
--rw-rw-rw-   0        0        0      664 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/screen.py
--rw-rw-rw-   0        0        0     4862 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/smooth_scroll.py
--rw-rw-rw-   0        0        0    14471 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/style_sheet.py
--rw-rw-rw-   0        0        0      454 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/translator.py
-drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.232893 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/
--rw-rw-rw-   0        0        0      150 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.242789 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/
--rw-rw-rw-   0        0        0      234 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/__init__.py
--rw-rw-rw-   0        0        0     2329 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/calendar_picker.py
--rw-rw-rw-   0        0        0    21813 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/calendar_view.py
--rw-rw-rw-   0        0        0     7630 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/date_picker.py
--rw-rw-rw-   0        0        0    19331 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/picker_base.py
--rw-rw-rw-   0        0        0     6406 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/time_picker.py
-drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.256229 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/
--rw-rw-rw-   0        0        0      216 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/__init__.py
--rw-rw-rw-   0        0        0    14892 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/color_dialog.py
--rw-rw-rw-   0        0        0     5896 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/dialog.py
--rw-rw-rw-   0        0        0    11413 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/folder_list_dialog.py
--rw-rw-rw-   0        0        0     3179 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/mask_dialog_base.py
--rw-rw-rw-   0        0        0     2873 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/message_box_base.py
--rw-rw-rw-   0        0        0     2425 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/message_dialog.py
-drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.263592 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/
--rw-rw-rw-   0        0        0      114 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/__init__.py
--rw-rw-rw-   0        0        0     2716 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/expand_layout.py
--rw-rw-rw-   0        0        0     7104 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/flow_layout.py
--rw-rw-rw-   0        0        0     1305 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/v_box_layout.py
-drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.276958 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/
--rw-rw-rw-   0        0        0      538 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/__init__.py
--rw-rw-rw-   0        0        0     3129 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_combo_box.py
--rw-rw-rw-   0        0        0     3542 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_flyout.py
--rw-rw-rw-   0        0        0      763 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_line_edit.py
--rw-rw-rw-   0        0        0     6778 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_menu.py
--rw-rw-rw-   0        0        0     1187 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_tool_tip.py
--rw-rw-rw-   0        0        0     1310 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.293112 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/
--rw-rw-rw-   0        0        0      716 2023-11-24 09:36:26.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/__init__.py
--rw-rw-rw-   0        0        0     9884 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/breadcrumb.py
--rw-rw-rw-   0        0        0    12954 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_bar.py
--rw-rw-rw-   0        0        0     8771 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_interface.py
--rw-rw-rw-   0        0        0    24105 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_panel.py
--rw-rw-rw-   0        0        0    19679 2024-04-13 06:32:17.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_widget.py
--rw-rw-rw-   0        0        0     6823 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/pivot.py
--rw-rw-rw-   0        0        0     5205 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/segmented_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.306148 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/
--rw-rw-rw-   0        0        0      550 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/__init__.py
--rw-rw-rw-   0        0        0     5280 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/custom_color_setting_card.py
--rw-rw-rw-   0        0        0    11031 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/expand_setting_card.py
--rw-rw-rw-   0        0        0     4644 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/folder_list_setting_card.py
--rw-rw-rw-   0        0        0     2841 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/options_setting_card.py
--rw-rw-rw-   0        0        0    14031 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/setting_card.py
--rw-rw-rw-   0        0        0     1590 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/setting_card_group.py
-drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.372345 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/
--rw-rw-rw-   0        0        0     3316 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/__init__.py
--rw-rw-rw-   0        0        0     7971 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/acrylic_label.py
--rw-rw-rw-   0        0        0    29986 2024-04-13 06:31:18.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/button.py
--rw-rw-rw-   0        0        0     7688 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/card_widget.py
--rw-rw-rw-   0        0        0     5808 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/check_box.py
--rw-rw-rw-   0        0        0    16342 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/combo_box.py
--rw-rw-rw-   0        0        0    19812 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/command_bar.py
--rw-rw-rw-   0        0        0     7934 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/cycle_list_widget.py
--rw-rw-rw-   0        0        0    13111 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/flip_view.py
--rw-rw-rw-   0        0        0    17080 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/flyout.py
--rw-rw-rw-   0        0        0     2229 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/frameless_window.py
--rw-rw-rw-   0        0        0     1496 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/icon_widget.py
--rw-rw-rw-   0        0        0    16653 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/info_badge.py
--rw-rw-rw-   0        0        0    18932 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/info_bar.py
--rw-rw-rw-   0        0        0    14700 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/label.py
--rw-rw-rw-   0        0        0    14221 2024-04-13 06:32:27.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/line_edit.py
--rw-rw-rw-   0        0        0     4579 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/list_view.py
--rw-rw-rw-   0        0        0    40995 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/menu.py
--rw-rw-rw-   0        0        0    11197 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/pips_pager.py
--rw-rw-rw-   0        0        0     9173 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     7029 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/progress_ring.py
--rw-rw-rw-   0        0        0     2720 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/scroll_area.py
--rw-rw-rw-   0        0        0    17861 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/scroll_bar.py
--rw-rw-rw-   0        0        0     1167 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/separator.py
--rw-rw-rw-   0        0        0    10310 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/slider.py
--rw-rw-rw-   0        0        0     8563 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/spin_box.py
--rw-rw-rw-   0        0        0     6535 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0     5854 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/state_tool_tip.py
--rw-rw-rw-   0        0        0     8597 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/switch_button.py
--rw-rw-rw-   0        0        0    26330 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/tab_view.py
--rw-rw-rw-   0        0        0    11774 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/table_view.py
--rw-rw-rw-   0        0        0    22912 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/teaching_tip.py
--rw-rw-rw-   0        0        0    10581 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/tool_tip.py
--rw-rw-rw-   0        0        0     4555 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/tree_view.py
-drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.379368 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/
--rw-rw-rw-   0        0        0      183 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/__init__.py
--rw-rw-rw-   0        0        0    11597 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/media_play_bar.py
--rw-rw-rw-   0        0        0     3887 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/media_player.py
--rw-rw-rw-   0        0        0     2849 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/video_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-13 06:40:11.386859 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/window/
--rw-rw-rw-   0        0        0      187 2024-04-13 06:31:18.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/window/__init__.py
--rw-rw-rw-   0        0        0    12940 2024-04-13 06:31:18.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/window/fluent_window.py
--rw-rw-rw-   0        0        0     2827 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/window/splash_screen.py
--rw-rw-rw-   0        0        0     1660 2024-04-13 06:31:06.000000 PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/window/stacked_widget.py
--rw-rw-rw-   0        0        0       42 2024-04-13 06:40:11.391186 PySide6-Fluent-Widgets-1.5.5/setup.cfg
--rw-rw-rw-   0        0        0     1219 2024-04-13 06:31:33.000000 PySide6-Fluent-Widgets-1.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.214608 PySide6-Fluent-Widgets-1.5.6/
+-rw-rw-rw-   0        0        0    35823 2024-05-07 03:40:07.000000 PySide6-Fluent-Widgets-1.5.6/LICENSE
+-rw-rw-rw-   0        0        0     5360 2024-05-07 03:43:54.214095 PySide6-Fluent-Widgets-1.5.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.022369 PySide6-Fluent-Widgets-1.5.6/PySide6_Fluent_Widgets.egg-info/
+-rw-rw-rw-   0        0        0     5360 2024-05-07 03:43:53.000000 PySide6-Fluent-Widgets-1.5.6/PySide6_Fluent_Widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4929 2024-05-07 03:43:53.000000 PySide6-Fluent-Widgets-1.5.6/PySide6_Fluent_Widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 03:43:53.000000 PySide6-Fluent-Widgets-1.5.6/PySide6_Fluent_Widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2024-05-07 03:43:53.000000 PySide6-Fluent-Widgets-1.5.6/PySide6_Fluent_Widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-07 03:43:53.000000 PySide6-Fluent-Widgets-1.5.6/PySide6_Fluent_Widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4576 2024-05-07 03:40:41.000000 PySide6-Fluent-Widgets-1.5.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.023535 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/
+-rw-rw-rw-   0        0        0      566 2024-05-07 03:40:18.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.029018 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/_rc/
+-rw-rw-rw-   0        0        0        0 2023-10-15 01:50:42.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/_rc/__init__.py
+-rw-rw-rw-   0        0        0  3307368 2024-05-07 03:41:23.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.058560 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/
+-rw-rw-rw-   0        0        0      664 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/__init__.py
+-rw-rw-rw-   0        0        0    15208 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/animation.py
+-rw-rw-rw-   0        0        0     4742 2023-12-29 09:55:21.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/auto_wrap.py
+-rw-rw-rw-   0        0        0     1589 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/color.py
+-rw-rw-rw-   0        0        0    11172 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/config.py
+-rw-rw-rw-   0        0        0      675 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/exception_handler.py
+-rw-rw-rw-   0        0        0      807 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/font.py
+-rw-rw-rw-   0        0        0    13725 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/icon.py
+-rw-rw-rw-   0        0        0     5554 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/image_utils.py
+-rw-rw-rw-   0        0        0     1635 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/overload.py
+-rw-rw-rw-   0        0        0     3862 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/router.py
+-rw-rw-rw-   0        0        0      664 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/screen.py
+-rw-rw-rw-   0        0        0     4862 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/smooth_scroll.py
+-rw-rw-rw-   0        0        0    14471 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/style_sheet.py
+-rw-rw-rw-   0        0        0      454 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/translator.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.065571 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/
+-rw-rw-rw-   0        0        0      150 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.076755 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/
+-rw-rw-rw-   0        0        0      234 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/__init__.py
+-rw-rw-rw-   0        0        0     2569 2024-05-07 03:40:18.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/calendar_picker.py
+-rw-rw-rw-   0        0        0    21813 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/calendar_view.py
+-rw-rw-rw-   0        0        0     7630 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/date_picker.py
+-rw-rw-rw-   0        0        0    19331 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/picker_base.py
+-rw-rw-rw-   0        0        0     6406 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/time_picker.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.088949 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/
+-rw-rw-rw-   0        0        0      216 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/__init__.py
+-rw-rw-rw-   0        0        0    14892 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/color_dialog.py
+-rw-rw-rw-   0        0        0     5896 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/dialog.py
+-rw-rw-rw-   0        0        0    11413 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/folder_list_dialog.py
+-rw-rw-rw-   0        0        0     3179 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/mask_dialog_base.py
+-rw-rw-rw-   0        0        0     2873 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/message_box_base.py
+-rw-rw-rw-   0        0        0     2425 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/message_dialog.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.095022 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/
+-rw-rw-rw-   0        0        0      114 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/__init__.py
+-rw-rw-rw-   0        0        0     2716 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/expand_layout.py
+-rw-rw-rw-   0        0        0     7104 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/flow_layout.py
+-rw-rw-rw-   0        0        0     1305 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/v_box_layout.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.107119 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/
+-rw-rw-rw-   0        0        0      538 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/__init__.py
+-rw-rw-rw-   0        0        0     3129 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_combo_box.py
+-rw-rw-rw-   0        0        0     3542 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_flyout.py
+-rw-rw-rw-   0        0        0      763 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_line_edit.py
+-rw-rw-rw-   0        0        0     6778 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_menu.py
+-rw-rw-rw-   0        0        0     1187 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_tool_tip.py
+-rw-rw-rw-   0        0        0     1310 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.123019 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/
+-rw-rw-rw-   0        0        0      716 2023-11-24 09:36:26.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/__init__.py
+-rw-rw-rw-   0        0        0     9940 2024-05-07 03:40:18.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/breadcrumb.py
+-rw-rw-rw-   0        0        0    12954 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_bar.py
+-rw-rw-rw-   0        0        0     8771 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_interface.py
+-rw-rw-rw-   0        0        0    24105 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_panel.py
+-rw-rw-rw-   0        0        0    19679 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_widget.py
+-rw-rw-rw-   0        0        0     6823 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/pivot.py
+-rw-rw-rw-   0        0        0     5205 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/segmented_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.136873 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/
+-rw-rw-rw-   0        0        0      550 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/__init__.py
+-rw-rw-rw-   0        0        0     5280 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/custom_color_setting_card.py
+-rw-rw-rw-   0        0        0    11031 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/expand_setting_card.py
+-rw-rw-rw-   0        0        0     4644 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/folder_list_setting_card.py
+-rw-rw-rw-   0        0        0     2841 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/options_setting_card.py
+-rw-rw-rw-   0        0        0    14031 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/setting_card.py
+-rw-rw-rw-   0        0        0     1590 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/setting_card_group.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.197817 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/
+-rw-rw-rw-   0        0        0     3316 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/__init__.py
+-rw-rw-rw-   0        0        0     8061 2024-05-07 03:40:18.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/acrylic_label.py
+-rw-rw-rw-   0        0        0    29986 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/button.py
+-rw-rw-rw-   0        0        0     7688 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/card_widget.py
+-rw-rw-rw-   0        0        0     5808 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/check_box.py
+-rw-rw-rw-   0        0        0    16342 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/combo_box.py
+-rw-rw-rw-   0        0        0    19812 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/command_bar.py
+-rw-rw-rw-   0        0        0     7934 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/cycle_list_widget.py
+-rw-rw-rw-   0        0        0    13111 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/flip_view.py
+-rw-rw-rw-   0        0        0    17080 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/flyout.py
+-rw-rw-rw-   0        0        0     2229 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/frameless_window.py
+-rw-rw-rw-   0        0        0     1496 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0    16653 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/info_badge.py
+-rw-rw-rw-   0        0        0    18932 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/info_bar.py
+-rw-rw-rw-   0        0        0    14700 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/label.py
+-rw-rw-rw-   0        0        0    14221 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     4579 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/list_view.py
+-rw-rw-rw-   0        0        0    40995 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/menu.py
+-rw-rw-rw-   0        0        0    11197 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/pips_pager.py
+-rw-rw-rw-   0        0        0     9173 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     7029 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/progress_ring.py
+-rw-rw-rw-   0        0        0     2720 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0    17861 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/scroll_bar.py
+-rw-rw-rw-   0        0        0     1167 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/separator.py
+-rw-rw-rw-   0        0        0    10310 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/slider.py
+-rw-rw-rw-   0        0        0     8637 2024-05-07 03:40:18.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     6535 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0     5854 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/state_tool_tip.py
+-rw-rw-rw-   0        0        0     8597 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/switch_button.py
+-rw-rw-rw-   0        0        0    26330 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tab_view.py
+-rw-rw-rw-   0        0        0    11774 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/table_view.py
+-rw-rw-rw-   0        0        0    22912 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/teaching_tip.py
+-rw-rw-rw-   0        0        0    10581 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tool_tip.py
+-rw-rw-rw-   0        0        0     4555 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tree_view.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.204023 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/
+-rw-rw-rw-   0        0        0      183 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/__init__.py
+-rw-rw-rw-   0        0        0    11597 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/media_play_bar.py
+-rw-rw-rw-   0        0        0     3887 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/media_player.py
+-rw-rw-rw-   0        0        0     2849 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/video_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.208601 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/window/
+-rw-rw-rw-   0        0        0      187 2024-04-13 06:56:28.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/window/__init__.py
+-rw-rw-rw-   0        0        0    12940 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/window/fluent_window.py
+-rw-rw-rw-   0        0        0     2827 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/window/splash_screen.py
+-rw-rw-rw-   0        0        0     1660 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/window/stacked_widget.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 03:43:54.214608 PySide6-Fluent-Widgets-1.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2024-05-07 03:40:52.000000 PySide6-Fluent-Widgets-1.5.6/setup.py
```

### Comparing `PySide6-Fluent-Widgets-1.5.5/LICENSE` & `PySide6-Fluent-Widgets-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/PKG-INFO` & `PySide6-Fluent-Widgets-1.5.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide6-Fluent-Widgets
-Version: 1.5.5
+Version: 1.5.6
 Summary: A fluent design widgets library based on PySide6
 Home-page: https://qfluentwidgets.com
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://qfluentwidgets.com/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6
@@ -90,17 +90,19 @@
 
 Copyright © 2021 by zhiyiYo.
 
 
 ## Video Demonstration
 Check out this [▶ example video](https://www.bilibili.com/video/BV12c411L73q) that shows off what PyQt-Fluent-Widgets are capable of 🎉
 
+## Work with Designer
+[Fluent Client](https://www.youtube.com/watch?v=7UCmcsOlhTk) integrates designer plugins, supporting direct drag-and-drop usage of QFluentWidgets components in Designer. You can purchase the client from [Afadian](https://afdian.net/item/62cc7298cd9411eeb14d52540025c377) or [TaoBao](https://item.taobao.com/item.htm?ft=t&id=767961666600).
+
+![Fluent Designer](https://img.fastmirror.net/s/2024/02/18/65d22363d4a73.jpg)
 
-## Support
-If this project helps you a lot and you want to support the development and maintenance of this project, feel free to sponsor me via [爱发电](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-fi.com/zhiyiYo). Your support is highly appreciated 🥰
 
 ## See Also
 Here are some projects based on PyQt-Fluent-Widgets:
 * [**zhiyiYo/QMaterialWidgets**: A material design widgets library based on PySide](https://qmaterialwidgets.vercel.app)
 * [**zhiyiYo/Groove**: A cross-platform music player based on PyQt5](https://github.com/zhiyiYo/Groove)
 * [**zhiyiYo/Alpha-Gobang-Zero**: A gobang robot based on reinforcement learning](https://github.com/zhiyiYo/Alpha-Gobang-Zero)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PySide6-Fluent-Widgets Version: 1.5.5 Summary: A
+Metadata-Version: 2.1 Name: PySide6-Fluent-Widgets Version: 1.5.6 Summary: A
 fluent design widgets library based on PySide6 Home-page: https://
 qfluentwidgets.com Author: zhiyiYo Author-email: shokokawaii@outlook.com
 License: GPLv3 Project-URL: Documentation, https://qfluentwidgets.com/ Project-
 URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6
 Project-URL: Bug Tracker, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues
 Keywords: pyside6 fluent widgets Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
@@ -37,21 +37,23 @@
 PySide6-Fluent-Widgets? Please read the [help document](https://
 qfluentwidgets.com) ð ## License PySide6-Fluent-Widgets adopts dual
 licenses. Non-commercial usage is licensed under [GPLv3](./LICENSE). For
 commercial purposes, please purchase [commercial license](https://
 qfluentwidgets.com/price) to support the development of this project. Copyright
 Â© 2021 by zhiyiYo. ## Video Demonstration Check out this [â¶ example video]
 (https://www.bilibili.com/video/BV12c411L73q) that shows off what PyQt-Fluent-
-Widgets are capable of ð ## Support If this project helps you a lot and you
-want to support the development and maintenance of this project, feel free to
-sponsor me via [ç±åçµ](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-
-fi.com/zhiyiYo). Your support is highly appreciated ð¥° ## See Also Here are
-some projects based on PyQt-Fluent-Widgets: * [**zhiyiYo/QMaterialWidgets**: A
-material design widgets library based on PySide](https://
-qmaterialwidgets.vercel.app) * [**zhiyiYo/Groove**: A cross-platform music
-player based on PyQt5](https://github.com/zhiyiYo/Groove) * [**zhiyiYo/Alpha-
-Gobang-Zero**: A gobang robot based on reinforcement learning](https://
-github.com/zhiyiYo/Alpha-Gobang-Zero) ## Reference * [**Windows design**:
-Design guidelines and toolkits for creating native app experiences](https://
-learn.microsoft.com/zh-cn/windows/apps/design/) * [**Microsoft/WinUI-Gallery**:
-An app demonstrates the controls available in WinUI and the Fluent Design
-System](https://github.com/microsoft/WinUI-Gallery)
+Widgets are capable of ð ## Work with Designer [Fluent Client](https://
+www.youtube.com/watch?v=7UCmcsOlhTk) integrates designer plugins, supporting
+direct drag-and-drop usage of QFluentWidgets components in Designer. You can
+purchase the client from [Afadian](https://afdian.net/item/
+62cc7298cd9411eeb14d52540025c377) or [TaoBao](https://item.taobao.com/
+item.htm?ft=t&id=767961666600). ![Fluent Designer](https://img.fastmirror.net/
+s/2024/02/18/65d22363d4a73.jpg) ## See Also Here are some projects based on
+PyQt-Fluent-Widgets: * [**zhiyiYo/QMaterialWidgets**: A material design widgets
+library based on PySide](https://qmaterialwidgets.vercel.app) * [**zhiyiYo/
+Groove**: A cross-platform music player based on PyQt5](https://github.com/
+zhiyiYo/Groove) * [**zhiyiYo/Alpha-Gobang-Zero**: A gobang robot based on
+reinforcement learning](https://github.com/zhiyiYo/Alpha-Gobang-Zero) ##
+Reference * [**Windows design**: Design guidelines and toolkits for creating
+native app experiences](https://learn.microsoft.com/zh-cn/windows/apps/design/
+) * [**Microsoft/WinUI-Gallery**: An app demonstrates the controls available in
+WinUI and the Fluent Design System](https://github.com/microsoft/WinUI-Gallery)
```

### Comparing `PySide6-Fluent-Widgets-1.5.5/PySide6_Fluent_Widgets.egg-info/PKG-INFO` & `PySide6-Fluent-Widgets-1.5.6/PySide6_Fluent_Widgets.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide6-Fluent-Widgets
-Version: 1.5.5
+Version: 1.5.6
 Summary: A fluent design widgets library based on PySide6
 Home-page: https://qfluentwidgets.com
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://qfluentwidgets.com/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6
@@ -90,17 +90,19 @@
 
 Copyright © 2021 by zhiyiYo.
 
 
 ## Video Demonstration
 Check out this [▶ example video](https://www.bilibili.com/video/BV12c411L73q) that shows off what PyQt-Fluent-Widgets are capable of 🎉
 
+## Work with Designer
+[Fluent Client](https://www.youtube.com/watch?v=7UCmcsOlhTk) integrates designer plugins, supporting direct drag-and-drop usage of QFluentWidgets components in Designer. You can purchase the client from [Afadian](https://afdian.net/item/62cc7298cd9411eeb14d52540025c377) or [TaoBao](https://item.taobao.com/item.htm?ft=t&id=767961666600).
+
+![Fluent Designer](https://img.fastmirror.net/s/2024/02/18/65d22363d4a73.jpg)
 
-## Support
-If this project helps you a lot and you want to support the development and maintenance of this project, feel free to sponsor me via [爱发电](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-fi.com/zhiyiYo). Your support is highly appreciated 🥰
 
 ## See Also
 Here are some projects based on PyQt-Fluent-Widgets:
 * [**zhiyiYo/QMaterialWidgets**: A material design widgets library based on PySide](https://qmaterialwidgets.vercel.app)
 * [**zhiyiYo/Groove**: A cross-platform music player based on PyQt5](https://github.com/zhiyiYo/Groove)
 * [**zhiyiYo/Alpha-Gobang-Zero**: A gobang robot based on reinforcement learning](https://github.com/zhiyiYo/Alpha-Gobang-Zero)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PySide6-Fluent-Widgets Version: 1.5.5 Summary: A
+Metadata-Version: 2.1 Name: PySide6-Fluent-Widgets Version: 1.5.6 Summary: A
 fluent design widgets library based on PySide6 Home-page: https://
 qfluentwidgets.com Author: zhiyiYo Author-email: shokokawaii@outlook.com
 License: GPLv3 Project-URL: Documentation, https://qfluentwidgets.com/ Project-
 URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6
 Project-URL: Bug Tracker, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues
 Keywords: pyside6 fluent widgets Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
@@ -37,21 +37,23 @@
 PySide6-Fluent-Widgets? Please read the [help document](https://
 qfluentwidgets.com) ð ## License PySide6-Fluent-Widgets adopts dual
 licenses. Non-commercial usage is licensed under [GPLv3](./LICENSE). For
 commercial purposes, please purchase [commercial license](https://
 qfluentwidgets.com/price) to support the development of this project. Copyright
 Â© 2021 by zhiyiYo. ## Video Demonstration Check out this [â¶ example video]
 (https://www.bilibili.com/video/BV12c411L73q) that shows off what PyQt-Fluent-
-Widgets are capable of ð ## Support If this project helps you a lot and you
-want to support the development and maintenance of this project, feel free to
-sponsor me via [ç±åçµ](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-
-fi.com/zhiyiYo). Your support is highly appreciated ð¥° ## See Also Here are
-some projects based on PyQt-Fluent-Widgets: * [**zhiyiYo/QMaterialWidgets**: A
-material design widgets library based on PySide](https://
-qmaterialwidgets.vercel.app) * [**zhiyiYo/Groove**: A cross-platform music
-player based on PyQt5](https://github.com/zhiyiYo/Groove) * [**zhiyiYo/Alpha-
-Gobang-Zero**: A gobang robot based on reinforcement learning](https://
-github.com/zhiyiYo/Alpha-Gobang-Zero) ## Reference * [**Windows design**:
-Design guidelines and toolkits for creating native app experiences](https://
-learn.microsoft.com/zh-cn/windows/apps/design/) * [**Microsoft/WinUI-Gallery**:
-An app demonstrates the controls available in WinUI and the Fluent Design
-System](https://github.com/microsoft/WinUI-Gallery)
+Widgets are capable of ð ## Work with Designer [Fluent Client](https://
+www.youtube.com/watch?v=7UCmcsOlhTk) integrates designer plugins, supporting
+direct drag-and-drop usage of QFluentWidgets components in Designer. You can
+purchase the client from [Afadian](https://afdian.net/item/
+62cc7298cd9411eeb14d52540025c377) or [TaoBao](https://item.taobao.com/
+item.htm?ft=t&id=767961666600). ![Fluent Designer](https://img.fastmirror.net/
+s/2024/02/18/65d22363d4a73.jpg) ## See Also Here are some projects based on
+PyQt-Fluent-Widgets: * [**zhiyiYo/QMaterialWidgets**: A material design widgets
+library based on PySide](https://qmaterialwidgets.vercel.app) * [**zhiyiYo/
+Groove**: A cross-platform music player based on PyQt5](https://github.com/
+zhiyiYo/Groove) * [**zhiyiYo/Alpha-Gobang-Zero**: A gobang robot based on
+reinforcement learning](https://github.com/zhiyiYo/Alpha-Gobang-Zero) ##
+Reference * [**Windows design**: Design guidelines and toolkits for creating
+native app experiences](https://learn.microsoft.com/zh-cn/windows/apps/design/
+) * [**Microsoft/WinUI-Gallery**: An app demonstrates the controls available in
+WinUI and the Fluent Design System](https://github.com/microsoft/WinUI-Gallery)
```

### Comparing `PySide6-Fluent-Widgets-1.5.5/PySide6_Fluent_Widgets.egg-info/SOURCES.txt` & `PySide6-Fluent-Widgets-1.5.6/PySide6_Fluent_Widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/README.md` & `PySide6-Fluent-Widgets-1.5.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -70,17 +70,19 @@
 
 Copyright © 2021 by zhiyiYo.
 
 
 ## Video Demonstration
 Check out this [▶ example video](https://www.bilibili.com/video/BV12c411L73q) that shows off what PyQt-Fluent-Widgets are capable of 🎉
 
+## Work with Designer
+[Fluent Client](https://www.youtube.com/watch?v=7UCmcsOlhTk) integrates designer plugins, supporting direct drag-and-drop usage of QFluentWidgets components in Designer. You can purchase the client from [Afadian](https://afdian.net/item/62cc7298cd9411eeb14d52540025c377) or [TaoBao](https://item.taobao.com/item.htm?ft=t&id=767961666600).
+
+![Fluent Designer](https://img.fastmirror.net/s/2024/02/18/65d22363d4a73.jpg)
 
-## Support
-If this project helps you a lot and you want to support the development and maintenance of this project, feel free to sponsor me via [爱发电](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-fi.com/zhiyiYo). Your support is highly appreciated 🥰
 
 ## See Also
 Here are some projects based on PyQt-Fluent-Widgets:
 * [**zhiyiYo/QMaterialWidgets**: A material design widgets library based on PySide](https://qmaterialwidgets.vercel.app)
 * [**zhiyiYo/Groove**: A cross-platform music player based on PyQt5](https://github.com/zhiyiYo/Groove)
 * [**zhiyiYo/Alpha-Gobang-Zero**: A gobang robot based on reinforcement learning](https://github.com/zhiyiYo/Alpha-Gobang-Zero)
```

#### html2text {}

```diff
@@ -26,21 +26,23 @@
 PySide6-Fluent-Widgets? Please read the [help document](https://
 qfluentwidgets.com) ð ## License PySide6-Fluent-Widgets adopts dual
 licenses. Non-commercial usage is licensed under [GPLv3](./LICENSE). For
 commercial purposes, please purchase [commercial license](https://
 qfluentwidgets.com/price) to support the development of this project. Copyright
 Â© 2021 by zhiyiYo. ## Video Demonstration Check out this [â¶ example video]
 (https://www.bilibili.com/video/BV12c411L73q) that shows off what PyQt-Fluent-
-Widgets are capable of ð ## Support If this project helps you a lot and you
-want to support the development and maintenance of this project, feel free to
-sponsor me via [ç±åçµ](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-
-fi.com/zhiyiYo). Your support is highly appreciated ð¥° ## See Also Here are
-some projects based on PyQt-Fluent-Widgets: * [**zhiyiYo/QMaterialWidgets**: A
-material design widgets library based on PySide](https://
-qmaterialwidgets.vercel.app) * [**zhiyiYo/Groove**: A cross-platform music
-player based on PyQt5](https://github.com/zhiyiYo/Groove) * [**zhiyiYo/Alpha-
-Gobang-Zero**: A gobang robot based on reinforcement learning](https://
-github.com/zhiyiYo/Alpha-Gobang-Zero) ## Reference * [**Windows design**:
-Design guidelines and toolkits for creating native app experiences](https://
-learn.microsoft.com/zh-cn/windows/apps/design/) * [**Microsoft/WinUI-Gallery**:
-An app demonstrates the controls available in WinUI and the Fluent Design
-System](https://github.com/microsoft/WinUI-Gallery)
+Widgets are capable of ð ## Work with Designer [Fluent Client](https://
+www.youtube.com/watch?v=7UCmcsOlhTk) integrates designer plugins, supporting
+direct drag-and-drop usage of QFluentWidgets components in Designer. You can
+purchase the client from [Afadian](https://afdian.net/item/
+62cc7298cd9411eeb14d52540025c377) or [TaoBao](https://item.taobao.com/
+item.htm?ft=t&id=767961666600). ![Fluent Designer](https://img.fastmirror.net/
+s/2024/02/18/65d22363d4a73.jpg) ## See Also Here are some projects based on
+PyQt-Fluent-Widgets: * [**zhiyiYo/QMaterialWidgets**: A material design widgets
+library based on PySide](https://qmaterialwidgets.vercel.app) * [**zhiyiYo/
+Groove**: A cross-platform music player based on PyQt5](https://github.com/
+zhiyiYo/Groove) * [**zhiyiYo/Alpha-Gobang-Zero**: A gobang robot based on
+reinforcement learning](https://github.com/zhiyiYo/Alpha-Gobang-Zero) ##
+Reference * [**Windows design**: Design guidelines and toolkits for creating
+native app experiences](https://learn.microsoft.com/zh-cn/windows/apps/design/
+) * [**Microsoft/WinUI-Gallery**: An app demonstrates the controls available in
+WinUI and the Fluent Design System](https://github.com/microsoft/WinUI-Gallery)
```

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/__init__.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,14 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: GPLv3 for non-commercial project, see README for more details.
 """
 
-__version__ = "1.5.5"
+__version__ = "1.5.6"
 __author__ = "zhiyiYo"
 
 from .components import *
 from .common import *
 from .window import *
 from ._rc import resource
```

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/_rc/resource.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/_rc/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Resource object code (Python 3)
 # Created by: object code
-# Created by: The Resource Compiler for Qt version 6.6.2
+# Created by: The Resource Compiler for Qt version 6.4.2
 # WARNING! All changes made in this file will be lost!
 
 from PySide6 import QtCore
 
 qt_resource_data = b"\
 \x00\x00\x1d\xac\
 \x89\
@@ -93335,15 +93335,15 @@
 und-color: rgba(\
 0, 0, 0, 9);\x0d\x0a}\x0d\
 \x0a\x0d\x0aInfoBarCloseB\
 utton:pressed {\x0d\
 \x0a    background-\
 color: rgba(0, 0\
 , 0, 6);\x0d\x0a}\
-\x00\x00\x057\
+\x00\x00\x056\
 L\
 ineEdit, TextEdi\
 t, PlainTextEdit\
  {\x0d\x0a    color: b\
 lack;\x0d\x0a    backg\
 round-color: rgb\
 a(255, 255, 255,\
@@ -93395,40 +93395,40 @@
   background-col\
 or: white;\x0d\x0a}\x0d\x0a\x0d\
 \x0aLineEdit:disabl\
 ed, TextEdit:dis\
 abled,\x0d\x0aPlainTex\
 tEdit:disabled {\
 \x0d\x0a    color: rgb\
-a(0, 0, 0, 150);\
-\x0d\x0a    background\
--color: rgba(249\
-, 249, 249, 0.3)\
-;\x0d\x0a    border: 1\
-px solid rgba(0,\
- 0, 0, 13);\x0d\x0a   \
- border-bottom: \
-1px solid rgba(0\
-, 0, 0, 13);\x0d\x0a}\x0d\
-\x0a\x0d\x0a#lineEditButt\
-on {\x0d\x0a    backgr\
-ound-color: tran\
-sparent;\x0d\x0a    bo\
-rder-radius: 4px\
-;\x0d\x0a    margin: 0\
-;\x0d\x0a}\x0d\x0a\x0d\x0a#lineEdi\
-tButton:hover {\x0d\
+a(0, 0, 0, 92);\x0d\
 \x0a    background-\
-color: rgba(0, 0\
-, 0, 9);\x0d\x0a}\x0d\x0a\x0d\x0a#\
-lineEditButton:p\
-ressed {\x0d\x0a    ba\
-ckground-color: \
-rgba(0, 0, 0, 6)\
-;\x0d\x0a}\x0d\x0a\
+color: rgba(249,\
+ 249, 249, 0.3);\
+\x0d\x0a    border: 1p\
+x solid rgba(0, \
+0, 0, 13);\x0d\x0a    \
+border-bottom: 1\
+px solid rgba(0,\
+ 0, 0, 13);\x0d\x0a}\x0d\x0a\
+\x0d\x0a#lineEditButto\
+n {\x0d\x0a    backgro\
+und-color: trans\
+parent;\x0d\x0a    bor\
+der-radius: 4px;\
+\x0d\x0a    margin: 0;\
+\x0d\x0a}\x0d\x0a\x0d\x0a#lineEdit\
+Button:hover {\x0d\x0a\
+    background-c\
+olor: rgba(0, 0,\
+ 0, 9);\x0d\x0a}\x0d\x0a\x0d\x0a#l\
+ineEditButton:pr\
+essed {\x0d\x0a    bac\
+kground-color: r\
+gba(0, 0, 0, 6);\
+\x0d\x0a}\x0d\x0a\
 \x00\x00\x01q\
 S\
 tateToolTip,\x0d\x0aTo\
 astToolTip {\x0d\x0a  \
   background-col\
 or: --ThemeColor\
 Dark1;\x0d\x0a    bord\
@@ -93748,51 +93748,51 @@
 gba(0, 0, 0, 0.0\
 6);\x0d\x0a}\x0d\x0a\x0d\x0aComboB\
 ox[isPlaceholder\
 Text=true] {\x0d\x0a  \
   color: rgba(0,\
  0, 0, 0.6063);\x0d\
 \x0a}\
-\x00\x00\x02/\
+\x00\x00\x02.\
 \x00\
-\x00\x0a>x\xda\xcdV]o\x9b0\x14}\x8f\x94\xff\
-`\xe5i\xadBK\xda\xd0\xadD{Y7i\x93\xb6\
-\xa7t\x93\xaaj\x0f\x06;\xc4\x1a\xd8\xc8v\xb6TS\
-\xff\xfb\xdc\x04\x03\xfe\x22\xbclZ\x14!8\xe7\xde{\
-\xae\x0f\x17\xc3\xba&\xf4\x1d\xdb\xcf\xa7\x93\xf7l\x97\x95\
-x\xdd]C\x89? \x22\x9b\xd3{R\xe9\xcb\xde\xe9\
-\x1d\xabj\x98\xcb.\xab\x01\xecb\x1a\xeej\xf6\x10\xb7\
-\x9eF\xc0\xef\xe9\x04\xa8_\xceJ\xc6S\x90\x950\xff\
-\xb1:B\x99:-8\xdbQ\x145,/2\xf8\xea\
-*I\xe6\xa0;\xc4\x17\xaf\xcft\x02\xe3\x08\xab\xb0E\
-\xbd\x07\x82\x95\x04\x1d\x13b\x15t\xf8/\xae\xcd\xc8(\
-cR\xb2j !\x8e\xad\x0c\x0e\x11\xd9\x89\x14$\xf5\
-\xbe!.\xcf\xc1\x86Q\xa9\x8a,U\x95\xd9\x1a\x17\x0c\
-\x83\xaf\x9ffs0\xfbBr\xce\x04\xdbH\xf0\x00?\
-b2[\x81\xf3\xcbcR\x0d\x11\x22\xb4HA\xacr\
-\xde\xbc\x1cb%\xd6\xd6\x14\xb8\xc4\xb9$\x8cF\xae\x07\
-Qt\xbf\xc5\x15\xbe{\xb9\xfaL\x8a\xad\x5c\xa8\xa4\xe7\
-\xe9\xe4\x9f\xdd)\xa3\xf7\xab\x9b~\xef\x876\x1a\xa1\x94\
-c\x88\x22F\xcb'{\xf2L\xa6\xe9\xc2\x01\xb5\xacA\
-xAs\xdd>*,oy\x11\xe2\x86t\xbd\x5c\xa3\
-\xf5(\x9e\xaa\x8c\x95\xdf\x88 \xaa\x81\xb7\x1bX\x0a\xfc\
-\xdd\xf6#\x18\xd445\xc4k\xf1P\xcc)\xde\xf4\xee\
-D\xd4\xa8\xae-GG\x84\x8d\xecq0\xcc;\x9c\x8b\
-88\x9c[\xf6\x13sg0[T\x8fC\x1fh\xef\
-\xb3\x06\x1d\xc0\x1aD\x0b\xf6K\xd9\x03\xe8\xc1C:&\
-\xae\x1d\x08\xed\x9a\xcb[\xb5a\xb6\x87\xf8\x22\xf9\xdb\xbb\
-\xa6\xe1\xf7\x86\xe5;\xe1\xf8\xdd\xa2z\xf5}\xa0]\x9e\
-\x06\x1d\xc0\xf2\xdb\x82\xfdR\xb6\xdf\x1e<\xa4c\xe2\xad\
-\xdf#M\xe9\x5ctn\xd0\xaf-\x91\xd8v\x0c\x11\x01\
-U\xff\xc81\xadO\xe8UXX\xdbi\x0f\xf7a\x96\
-\x81.\x13T\xb6m\xf4S\x03\x9a\x0ee}\x08X\xee\
-%\xf1\xd9\xea\xbf\x99\xefks\xbcw*\x9c\x86\x1f?\
-\xc9!\x155\xe4\x98J\xff\xb7\xc4\xb2}\xefW\x90\x17\
-\x84\xaa\xcd\xcb\xad?\xea!o[\xbc\xf5t\x98\xd6\x1c\
-\x0b\xd1\x19}\xaa\xc6\xcd\xa1\xc6\x1f\xfc\xafN.\
+\x00\x0a=x\xda\xcdV]o\xd30\x14}\xaf\xd4\xff\
+`\xf5\x89M\xcd\x96v\xed`\xa9xa \x81\x04O\
+\x1dH\x08\xf1\xe0\xc4nj\x91\xd8\x91\xed@'\xb4\xff\
+\x8e\xd7\xc6I\xfc\x95\xe6\x05DUE\xc99\xf7\xdes\
+}r\xe3d[\x11\xfa\x86\x1d\xe6\xd3\xc9[V\xa7\x05\
+\xdev\xd7P\xe2w\x88\xc8\xe6\xf4\x81\x94\xfa\xb2wz\
+\xcf\xca\x0af\xb2\xcbj\x00\xbb\x98\x86\xbb\x9a=\xc4\xad\
+\xa7\x11\xf0{:\x01\xea\x97\xb1\x82\xf1\x04\xa4\x05\xcc~\
+lNP\xaaNs\xcej\x8a\xa2\x86\xe5y\x0a_,\
+\xd7\xeb9\xe8\x0e\xf1\xd5\xcb\x0b\x9d\xc08\xc2*lQ\
+\x1d\x80`\x05A\xa7\x84X\x05\x1d\xff\x8b\x1b32J\
+\x99\x94\xac\x1cH\x88c+\x83CDj\x91\x80uu\
+h\x88\xebK\xb0cT\xaa\x22+Ue\xb6\xc59\xc3\
+\xe0\xf3\x87\xd9\x1c\xcc>\x91\x8c3\xc1v\x12|\x85\xef\
+1\x99m\xc0\xe5\xf5)\xa9\x82\x08\x11\x9a' V9\
+\xaf\x9e\x0f\xb1\x12kk\x0a\x5c\xe0L\x12F#\xd7\x83\
+(z\xd8\xe3\x12\xdf?_}$\xf9^.T\xd2\xd3\
+t\xf2\xcf\xee\x94\xd1\xfb\xf2\xb6\xdf\xfb\xb1\x8dF(\xe1\
+\x18\xa2\x88\xd1\xe2\xd1\x9e<\x93i\xbap@-k\x10\
+^\xd0\x5c\xb7\x8f\x0a\xcb[^\x84\xb8!]/\xd7h\
+}\x13\x8fe\xca\x8a/D\x10\xd5\xc0\xeb\x1d,\x04\xfe\
+n\xfb\x11\x0cj\x9a\x1a\xe2\xb5x(\xe6\x1cozw\
+&jT\xd7\x96\xa3#\xc2F\xf68\x18\xe6\x1d\xceE\
+\x1c\x1c\xce=\xfb\x89\xb93\x98-\xaa\xc7\xa1\x0f\xb4\xf7\
+Y\x83\x0e`\x0d\xa2\x05\xfb\xa5\xec\x01\xf4\xe0!\x1d\x13\
+\xd7\x0e\x84v\xcd\xd5\x9d\xda0\xdbC|\xb5\xfe\xdb\xbb\
+\xa6\xe1\xf7\x8ee\xb5p\xfcnQ\xbd\xfa>\xd0.O\
+\x83\x0e`\xf9m\xc1~)\xdbo\x0f\x1e\xd21\xf1\xd6\
+\xef\x91\xa6t.:7\xe8\xd7\x9eHl;\x86\x88\x80\
+\xaa\x7f\xe4\x98\xd6'\xf4*,\xac\xed\xb4\x87\xfb0\xcb\
+@\x97\x09*\xdb6\xfa\xa9\x01M\x87\xb2>\x04L\xf7\
+\xee\x96\x17\x9b\xfff\xbco\xcc\xe9\xaeU8\x0d?}\
+\x92C**\xc81\x95\xfeO\x89U\xfb\xda/!\xcf\
+\x09U{\x97[\x7f\xd43\xde\xd9\xe5\xe90\xa98\x16\
+\xa2\xf3\xf9\x5c\x8d\xdbc\x8d?\xd9\xd1N\x03\
 \x00\x00\x00\x9b\
 H\
 eaderCardWidget \
 #headerLabel {\x0d\x0a\
     color: black\
 ;\x0d\x0a}\x0d\x0a\x0d\x0aHeaderCa\
 rdWidget > #head\
@@ -94509,15 +94509,15 @@
 5, 255, 255, 9);\
 \x0d\x0a}\x0d\x0a\x0d\x0aInfoBarCl\
 oseButton:presse\
 d {\x0d\x0a    backgro\
 und-color: rgba(\
 255, 255, 255, 6\
 );\x0d\x0a}\
-\x00\x00\x05v\
+\x00\x00\x05u\
 L\
 ineEdit, TextEdi\
 t, PlainTextEdit\
  {\x0d\x0a    backgrou\
 nd-color: rgba(2\
 55, 255, 255, 0.\
 0605);\x0d\x0a    bord\
@@ -94575,38 +94575,38 @@
 0, 30, 0.7);\x0d\x0a}\x0d\
 \x0a\x0d\x0aLineEdit:disa\
 bled, TextEdit:d\
 isabled, PlainTe\
 xtEdit:disabled \
 {\x0d\x0a    color: rg\
 ba(255, 255, 255\
-, 150);\x0d\x0a    bac\
-kground-color: r\
-gba(255, 255, 25\
-5, 0.0419);\x0d\x0a   \
- border: 1px sol\
-id rgba(255, 255\
-, 255, 0.0698);\x0d\
-\x0a}\x0d\x0a\x0d\x0a#lineEditB\
-utton {\x0d\x0a    bac\
-kground-color: t\
-ransparent;\x0d\x0a   \
- border-radius: \
-4px;\x0d\x0a    margin\
-: 0;\x0d\x0a}\x0d\x0a\x0d\x0a#line\
-EditButton:hover\
- {\x0d\x0a    backgrou\
-nd-color: rgba(2\
-55, 255, 255, 9)\
-;\x0d\x0a}\x0d\x0a\x0d\x0a#lineEdi\
-tButton:pressed \
+, 92);\x0d\x0a    back\
+ground-color: rg\
+ba(255, 255, 255\
+, 0.0419);\x0d\x0a    \
+border: 1px soli\
+d rgba(255, 255,\
+ 255, 0.0698);\x0d\x0a\
+}\x0d\x0a\x0d\x0a#lineEditBu\
+tton {\x0d\x0a    back\
+ground-color: tr\
+ansparent;\x0d\x0a    \
+border-radius: 4\
+px;\x0d\x0a    margin:\
+ 0;\x0d\x0a}\x0d\x0a\x0d\x0a#lineE\
+ditButton:hover \
 {\x0d\x0a    backgroun\
 d-color: rgba(25\
-5, 255, 255, 6);\
-\x0d\x0a}\x0d\x0a\
+5, 255, 255, 9);\
+\x0d\x0a}\x0d\x0a\x0d\x0a#lineEdit\
+Button:pressed {\
+\x0d\x0a    background\
+-color: rgba(255\
+, 255, 255, 6);\x0d\
+\x0a}\x0d\x0a\
 \x00\x00\x01r\
 S\
 tateToolTip,\x0d\x0aTo\
 astToolTip {\x0d\x0a  \
   background-col\
 or: --ThemeColor\
 Dark1;\x0d\x0a    bord\
@@ -94928,56 +94928,56 @@
 , 255, 255, 0.05\
 3);\x0d\x0a}\x0d\x0a\x0d\x0aComboB\
 ox[isPlaceholder\
 Text=true] {\x0d\x0a  \
   color: rgba(25\
 5, 255, 255, 0.6\
 063);\x0d\x0a}\
-\x00\x00\x02x\
+\x00\x00\x02v\
 \x00\
-\x00\x0c\x93x\xda\xbdV[k\xdb0\x14~\x0f\xe4?\
-\x88<\xb5%n\x9d\x8b\xb3\xd4\xa5/\xeb\x06\xdb\xc3`\
-\x90n0J\x1fd[I\xc4l\xcbH\xf2\x960\xfa\
-\xdf\xa7\xa6\x92/\xba\xd8\xce\x1e\x16H\x88\xbf\xf3\x9d\x8b\
-\x8e\xbe#kS\xe0\xfc=9L\xc7\xa3\x0f\xa4\x8cR\
-\xb4\xa9\x9f!G\x1f\x13\xcc\xe5\xdfG\x9c\xa9\xc7\xc6\xdf\
-\x07\x92\x150\xe6\xb5\x97\x04\xf4`\x0a\xaec6\x103\
-\x9eB\xc0\x9f\xf1\x08\x88O\x04\xe3\x9f;J\xca<\xf1\
-b\x92\x12\x1a\x02\xba\x8b\xe0\xc5<\x08\xa6\xa0\xfe\xf1\xaf\
-\xfd\x95\x1f\x5c\xdeI\x1fB\x13$\x98\xb3\xe2\x00\x18I\
-q\xe2\xf2Y\xb7=\xbc\x88pN\xb2~\xc7`\xb9\x9c\
-k\xae\x14&\xb8d!\x08\x8a\x834\xdc\x5c\x81-\xc9\
-\xb9\x88\xb6\x14\xe1&\x1b\xb4#\x08|\xfb<\x99\x82\xc9\
-\x17\x1cS\xc2\xc8\x96\x83\x1f\xf0\x13\xc2\x93;pu\xf3\
-\xe6T\xc0$\xc1\xf9.\x04\xbe\xf0Y\xbf\xfe\xf8`\xe6\
-W1e\x0b~\xef1G\x12b(E1\xc7$\xf7\
-\xccVy\xde\xe3\x1ee\xe8\xe1\xf5\xe9+\xc5\x19\xa4G\
-\xc3KR\xa3Tx\x0b\xe3\xcbx\xf4\xdf\xf6\xb6\xb5\xd8\
-\xf9\xaa\xb9\xd8S\x192QH\x11L<\x92\xa7G]\
-\xabm\x8b\xac\xc2\x00U\xda\x96\xc1\x0a\xb6\xd7m3\xb9\
-\xd3k\xbdp\xd9\xba\xf2Zm2\xd7\x13;f\x11I\
-\xbfc\x86E\x01\xf7[\x982\xf4\xac\xf7\xc3I\x92E\
-u\xd9Ur\x17\xa7\xcf\xde\xee]\x0fkP\xd5ZG\
-\x07\xd0\x06\xd6\xd8I\xb3\x8as\xe6;\xc5\xb9'\xbf\x10\
-5\x84Y\xa1J\x0eM\xa0\xdag\x05\x1a\x80&D\x0d\
-\xb6\xa7\xd2\x05h\xc1]y\xda\xf8\xd9G\xefz\xf1\xee\
-Rk\xcb\x13\xa70g\x05\xa4(\xe7\xf7\x9c\x96\xe89\
-\xdc\x92\xb8d\x86b;xj\xdf\xbb)\xd5f\xbai\
-\x03(\x9az{\x89C\x17\xa1kx\x10sx\xbd}\
-\xccj+\xcf{\xbf5^\x8cv\x0d,\xfc)P_\
-\xff\xda\xd8\xfd0\xc1\x0c\x8a\xfe$\xc6\x5c4\x0dJ\xa8\
-\x1aV\x89\xb1\x81\xdb0mFL\x8b3\xb3>)v\
-SGN\xc3\xa4\xfa\xdc1'\xb3\xc0\xefi\xaas\xb0\
-\xecw\x1a\xc75\xe8v\xdd9\x8bo\x87\xdc\x80a\xd4\
-\x896\x05[8VEj\xbc!\x9c\x8e\x81\xb43\x07\
-\xaf\xa4k$\xdd\xd43j\xee\xa5\x9a\x07\xecI\x01\x17\
-\x8b\x99\x98\xa8\xd3\xb7\xbd\x85\xa5\x98\xda\xdc}*7\xd2\
-\xd8\xef\xa4\xcb\xea\xfe(n\x80;\x9c\x8bw\x9a\x19\xff\
-_\xce\xfe[K\x9daA\x11c\xf5H\x0c\x8b\xb4:\
-E\xfa\x0b\xeea.\x91\
+\x00\x0c\x93x\xda\xbdV]k\xdb0\x14}\x0f\xe4?\
+\x88<\xb5%n\x9d4\xc9\x12\x97\xbe\xac\x1bl\x0f\x83\
+A\xba\xc1(}\x90m%\x11\xb3-#\xc9[\xc2\xe8\
+\x7f\x9f\x9aJ\x8e\xad\x0f[\xd9\xc3\x02\x0e\xf6\xb9\xe7~\
+\xe8\xea\x5c\xd9\xeb\x12\x17\xef\xc9~<\x1c| U\x9c\
+\xa1\xf5\xe9\x19r\xf41\xc5\x5c\xde>\xe2\x5c=6n\
+\x1fH^\xc2\x84\x9f\xbc$\xa0\x07S\xf0)f\x031\
+\xe3)\x04\xfc\x19\x0e\x80\xf8\xc50\xf9\xb9\xa5\xa4*\xd2\
+ !\x19\xa1\x11\xa0\xdb\x18^L\xe7\xf318\xfd\x85\
+\xd7\xe1\x22\x9c_\xdeI\x1fBS$\x98\x93r\x0f\x18\
+\xc9p\xea\xf2Y\xb6=\x82\x98pN\xf2~\xc7\xf9l\
+6\xd5\x5c)Lq\xc5\x220/\xf7\xd2ps\x056\
+\xa4\xe0\x22\xdaL\x84\x1b\xad\xd1\x96 \xf0\xed\xf3h\x0c\
+F_pB\x09#\x1b\x0e~\xc0O\x08\x8f\xee\xc0\xd5\
+\xcd\x9bS\x09\xd3\x14\x17\xdb\x08\x84\xc2g\xf9\xfa\x17\x82\
+IX\xc7\x94-\xf8\xbd\xc3\x1cI\x88\xa1\x0c%\x1c\x93\
+\x220[\x15\x04\x8f;\x94\xa3\x87\xd7\xa7\xaf\x14\xe7\x90\
+\x1e\x0c/I\x8d3\xe1-\x8c/\xc3\xc1\x7f\xdb\xdb\xd6\
+b\xa7\x8b\xe6b\x8fe\xc8D\x11E0\x0dH\x91\x1d\
+t\xad\xb6-\xb2\x0a\x03Ti[\x06+\xd8^\xb7\xcd\
+\xe4N\xaf\xf5\xc2e\xeb\xcak\xb5\xc9\x5cO\xec\x90\xc7\
+$\xfb\x8e\x19\x16\x05\xdco`\xc6\xd0\xb3\xde\x0f'I\
+\x16\xd5eW\xc9]\x9c>{\xbbw=,\xaf\xaa\xb5\
+\x8ez\xd0<k\xec\xa4Y\xc59\x09\x9d\xe2\xdc\x91_\
+\x88\x1a\xc2\xacQ%\x87&P\xef\xb3\x02\x0d@\x13\xa2\
+\x06\xdbS\xe9\x02\xb4\xe0\xae<m\xfc\xec\xa3wy\xfb\
+\xeeRk\xcb\x13\xa7\xb0`%\xa4\xa8\xe0\xf7\x9cV\xe8\
+9\xda\x90\xa4b\x86b;xj\xdf\xbb)\xf5f\xba\
+i\x1e\x14M\xbd\xbdD\xdfE\xe8\x1a\xf6b\xfa\xd7\xdb\
+\xc7\xac\xb7\xf2\xbc\xf7[\xe3\xc5h\xd7\xc0m8\x06\xea\
+\x0a\xaf\x8d\xdd\x8fR\xcc\xa0\xe8Oj\xccE\xd3\xa0\x84\
+\xaaa\xb5\x18\x1b\xb8\x0d\xd3f\xc4\xb483\xeb\x93b\
+7u\xe44L\xaa\xcf\x1ds\xb2\x9a\xf6\xf4\xd49W\
+g}\xd2,V\xcb\xceY|;\xe4<\x86Q'\xda\
+\x14l\xe1X\x15\xa9\xf1|8\x1d\x03igz\xaf\xa4\
+k$\xdd\xd43j\xee\xa5\x9a\x07\xecQ\x02\x17\xb7\x13\
+1Q\xc7\xab\xbd\x85\x95\x98\xda\xc2}*7\xd2\xd8\xbf\
+Ig\xf5\xf7\xa3\xf8\x02\xdc\xe2B\xbc\xd3\xcc\xf8\xffr\
+\xf6\xaf,uF%E\x8c\x9dF\xc2/\xd2\xe2\x18\xe9\
+/\xbe\xe3.\xd8\
 \x00\x00\x00\x9b\
 H\
 eaderCardWidget \
 #headerLabel {\x0d\x0a\
     color: white\
 ;\x0d\x0a}\x0d\x0a\x0d\x0aHeaderCa\
 rdWidget > #head\
@@ -98889,150 +98889,150 @@
 \x00\x00\x01\x8d\xa6\xd33\xb3\
 \x00\x00F\xb8\x00\x00\x00\x00\x00\x01\x00\x16?\xfa\
 \x00\x00\x01\x8b1\x07F\x91\
 \x00\x00G\x88\x00\x02\x00\x00\x00\x22\x00\x00\x01\xfe\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00G\x96\x00\x02\x00\x00\x00\x22\x00\x00\x01\xdc\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00J\xf0\x00\x00\x00\x00\x00\x01\x00\x16\xb6\x9c\
+\x00\x00J\xf0\x00\x00\x00\x00\x00\x01\x00\x16\xb6\x9a\
 \x00\x00\x01\x8b1\x07Mz\
-\x00\x00J\x22\x00\x01\x00\x00\x00\x01\x00\x16\xab\xd1\
+\x00\x00J\x22\x00\x01\x00\x00\x00\x01\x00\x16\xab\xcf\
 \x00\x00\x01\x8d\xa5\x92\xa6D\
-\x00\x00Ib\x00\x00\x00\x00\x00\x01\x00\x16\xa4\xc8\
+\x00\x00Ib\x00\x00\x00\x00\x00\x01\x00\x16\xa4\xc6\
 \x00\x00\x01\x8b1\x07MG\
-\x00\x00K\x8c\x00\x01\x00\x00\x00\x01\x00\x16\xbe\xbc\
+\x00\x00K\x8c\x00\x01\x00\x00\x00\x01\x00\x16\xbe\xba\
 \x00\x00\x01\x8c\x01\x8b~\xfe\
-\x00\x00I\xa8\x00\x01\x00\x00\x00\x01\x00\x16\xa5~\
+\x00\x00I\xa8\x00\x01\x00\x00\x00\x01\x00\x16\xa5|\
 \x00\x00\x01\x8d\xa6\xd33\xdd\
-\x00\x00I\xdc\x00\x00\x00\x00\x00\x01\x00\x16\xa96\
+\x00\x00I\xdc\x00\x00\x00\x00\x00\x01\x00\x16\xa94\
 \x00\x00\x01\x8b1\x07M2\
-\x00\x00H\xac\x00\x00\x00\x00\x00\x01\x00\x16\x9a\x95\
+\x00\x00H\xac\x00\x00\x00\x00\x00\x01\x00\x16\x9a\x94\
 \x00\x00\x01\x8b1\x07M\x97\
-\x00\x00K\x0e\x00\x00\x00\x00\x00\x01\x00\x16\xb7\x14\
+\x00\x00K\x0e\x00\x00\x00\x00\x00\x01\x00\x16\xb7\x12\
 \x00\x00\x01\x8b1\x07MW\
-\x00\x00I\x88\x00\x00\x00\x00\x00\x01\x00\x16\xa56\
+\x00\x00I\x88\x00\x00\x00\x00\x00\x01\x00\x16\xa54\
 \x00\x00\x01\x8b1\x07M\x1d\
-\x00\x00I \x00\x01\x00\x00\x00\x01\x00\x16\xa1\xf6\
-\x00\x00\x01\x8ei\xdb\xe2R\
+\x00\x00I \x00\x01\x00\x00\x00\x01\x00\x16\xa1\xf5\
+\x00\x00\x01\x8fQ#I\xf6\
 \x00\x00G\xa6\x00\x00\x00\x00\x00\x01\x00\x16\x85\xe5\
 \x00\x00\x01\x8b1\x07M:\
-\x00\x00I\xfe\x00\x01\x00\x00\x00\x01\x00\x16\xa9z\
+\x00\x00I\xfe\x00\x01\x00\x00\x00\x01\x00\x16\xa9x\
 \x00\x00\x01\x8b1\x07M\x8f\
-\x00\x00K\xec\x00\x01\x00\x00\x00\x01\x00\x16\xc3\xeb\
+\x00\x00K\xec\x00\x01\x00\x00\x00\x01\x00\x16\xc3\xe9\
 \x00\x00\x01\x8b1\x07L\xf6\
-\x00\x00K\xb4\x00\x00\x00\x00\x00\x01\x00\x16\xc0f\
+\x00\x00K\xb4\x00\x00\x00\x00\x00\x01\x00\x16\xc0d\
 \x00\x00\x01\x8c\x00\xb0\x09\x84\
-\x00\x00Hp\x00\x00\x00\x00\x00\x01\x00\x16\x97\x81\
+\x00\x00Hp\x00\x00\x00\x00\x00\x01\x00\x16\x97\x80\
 \x00\x00\x01\x8b1\x07M\x87\
-\x00\x00G\xe4\x00\x00\x00\x00\x00\x01\x00\x16\x8e\xe0\
+\x00\x00G\xe4\x00\x00\x00\x00\x00\x01\x00\x16\x8e\xdf\
 \x00\x00\x01\x8b1\x07Ms\
-\x00\x00K8\x00\x01\x00\x00\x00\x01\x00\x16\xbaX\
+\x00\x00K8\x00\x01\x00\x00\x00\x01\x00\x16\xbaV\
 \x00\x00\x01\x8c\xb4\xff\xf1\xb5\
-\x00\x00JD\x00\x00\x00\x00\x00\x01\x00\x16\xad\xeb\
+\x00\x00JD\x00\x00\x00\x00\x00\x01\x00\x16\xad\xe9\
 \x00\x00\x01\x8c\xb4\xff\xf1\xaf\
-\x00\x00J\x96\x00\x00\x00\x00\x00\x01\x00\x16\xb4\x84\
+\x00\x00J\x96\x00\x00\x00\x00\x00\x01\x00\x16\xb4\x82\
 \x00\x00\x01\x8b1\x07My\
-\x00\x00K\xcc\x00\x00\x00\x00\x00\x01\x00\x16\xc2?\
+\x00\x00K\xcc\x00\x00\x00\x00\x00\x01\x00\x16\xc2=\
 \x00\x00\x01\x8c\xb4\xff\xf1\xa9\
-\x00\x00I\xc2\x00\x01\x00\x00\x00\x01\x00\x16\xa7\x7f\
+\x00\x00I\xc2\x00\x01\x00\x00\x00\x01\x00\x16\xa7}\
 \x00\x00\x01\x8b1\x07Mf\
-\x00\x00H0\x00\x01\x00\x00\x00\x01\x00\x16\x90\x9e\
+\x00\x00H0\x00\x01\x00\x00\x00\x01\x00\x16\x90\x9d\
 \x00\x00\x01\x8d\xb652e\
-\x00\x00J\xbe\x00\x00\x00\x00\x00\x01\x00\x16\xb5\xf5\
+\x00\x00J\xbe\x00\x00\x00\x00\x00\x01\x00\x16\xb5\xf3\
 \x00\x00\x01\x8b1\x07Mf\
-\x00\x00H\x96\x00\x01\x00\x00\x00\x01\x00\x16\x98\xad\
+\x00\x00H\x96\x00\x01\x00\x00\x00\x01\x00\x16\x98\xac\
 \x00\x00\x01\x8bf\xa8\x0a\xf2\
-\x00\x00I>\x00\x00\x00\x00\x00\x01\x00\x16\xa4)\
+\x00\x00I>\x00\x00\x00\x00\x00\x01\x00\x16\xa4'\
 \x00\x00\x01\x8b1\x07L\xfc\
-\x00\x00KX\x00\x01\x00\x00\x00\x01\x00\x16\xbc\xdd\
+\x00\x00KX\x00\x01\x00\x00\x00\x01\x00\x16\xbc\xdb\
 \x00\x00\x01\x8d\xa6\xd33\xe2\
 \x00\x00G\xc4\x00\x00\x00\x00\x00\x01\x00\x16\x89\xa5\
-\x00\x00\x01\x8b1\x07MA\
-\x00\x00Jd\x00\x00\x00\x00\x00\x01\x00\x16\xb0w\
+\x00\x00\x01\x8fQ#I\xf4\
+\x00\x00Jd\x00\x00\x00\x00\x00\x01\x00\x16\xb0u\
 \x00\x00\x01\x8b1\x07M,\
-\x00\x00H\x0e\x00\x00\x00\x00\x00\x01\x00\x16\x90U\
+\x00\x00H\x0e\x00\x00\x00\x00\x00\x01\x00\x16\x90T\
 \x00\x00\x01\x8b1\x07M^\
-\x00\x00L>\x00\x01\x00\x00\x00\x01\x00\x16\xc8\xe1\
+\x00\x00L>\x00\x01\x00\x00\x00\x01\x00\x16\xc8\xdf\
 \x00\x00\x01\x8c\x00\xb0\x09\x8d\
-\x00\x00I\x00\x00\x00\x00\x00\x00\x01\x00\x16\x9e\x9f\
+\x00\x00I\x00\x00\x00\x00\x00\x00\x01\x00\x16\x9e\x9e\
 \x00\x00\x01\x8c\xb4\xff\xf1\xa9\
-\x00\x00H\xca\x00\x00\x00\x00\x00\x01\x00\x16\x9c3\
+\x00\x00H\xca\x00\x00\x00\x00\x00\x01\x00\x16\x9c2\
 \x00\x00\x01\x8b1\x07M^\
-\x00\x00L\x18\x00\x01\x00\x00\x00\x01\x00\x16\xc5\xef\
+\x00\x00L\x18\x00\x01\x00\x00\x00\x01\x00\x16\xc5\xed\
 \x00\x00\x01\x8b1\x07M\x08\
-\x00\x00HJ\x00\x01\x00\x00\x00\x01\x00\x16\x95\x89\
+\x00\x00HJ\x00\x01\x00\x00\x00\x01\x00\x16\x95\x88\
 \x00\x00\x01\x8d\xa6\xd33\xe7\
-\x00\x00J\xf0\x00\x00\x00\x00\x00\x01\x00\x17\x00\xc0\
+\x00\x00J\xf0\x00\x00\x00\x00\x00\x01\x00\x17\x00\xbb\
 \x00\x00\x01\x8b1\x07L\xca\
-\x00\x00J\x22\x00\x01\x00\x00\x00\x01\x00\x16\xf5\xa1\
+\x00\x00J\x22\x00\x01\x00\x00\x00\x01\x00\x16\xf5\x9c\
 \x00\x00\x01\x8c\xb4\xff\xf1\xa3\
-\x00\x00Ib\x00\x00\x00\x00\x00\x01\x00\x16\xea\x14\
+\x00\x00Ib\x00\x00\x00\x00\x00\x01\x00\x16\xea\x0f\
 \x00\x00\x01\x8b1\x07L\x8e\
-\x00\x00K\x8c\x00\x01\x00\x00\x00\x01\x00\x17\x08\xea\
+\x00\x00K\x8c\x00\x01\x00\x00\x00\x01\x00\x17\x08\xe5\
 \x00\x00\x01\x8c\x01\x8b~\xfb\
-\x00\x00I\xa8\x00\x00\x00\x00\x00\x01\x00\x16\xea\xca\
+\x00\x00I\xa8\x00\x00\x00\x00\x00\x01\x00\x16\xea\xc5\
 \x00\x00\x01\x8d\xa6\xd33\xcc\
-\x00\x00I\xdc\x00\x00\x00\x00\x00\x01\x00\x16\xf3\x0e\
+\x00\x00I\xdc\x00\x00\x00\x00\x00\x01\x00\x16\xf3\x09\
 \x00\x00\x01\x8b1\x07Lt\
-\x00\x00H\xac\x00\x00\x00\x00\x00\x01\x00\x16\xdfE\
+\x00\x00H\xac\x00\x00\x00\x00\x00\x01\x00\x16\xdfB\
 \x00\x00\x01\x8b1\x07L\xe3\
-\x00\x00K\x0e\x00\x00\x00\x00\x00\x01\x00\x17\x018\
+\x00\x00K\x0e\x00\x00\x00\x00\x00\x01\x00\x17\x013\
 \x00\x00\x01\x8b1\x07L\x9b\
-\x00\x00I\x88\x00\x00\x00\x00\x00\x01\x00\x16\xea\x82\
+\x00\x00I\x88\x00\x00\x00\x00\x00\x01\x00\x16\xea}\
 \x00\x00\x01\x8b1\x07L\x5c\
-\x00\x00I \x00\x01\x00\x00\x00\x01\x00\x16\xe6\xf9\
-\x00\x00\x01\x8ei\xdb\xe2R\
-\x00\x00G\xa6\x00\x00\x00\x00\x00\x01\x00\x16\xca\x83\
+\x00\x00I \x00\x01\x00\x00\x00\x01\x00\x16\xe6\xf6\
+\x00\x00\x01\x8fQ#I\xf4\
+\x00\x00G\xa6\x00\x00\x00\x00\x00\x01\x00\x16\xca\x81\
 \x00\x00\x01\x8b1\x07L{\
-\x00\x00I\xfe\x00\x01\x00\x00\x00\x01\x00\x16\xf3R\
+\x00\x00I\xfe\x00\x01\x00\x00\x00\x01\x00\x16\xf3M\
 \x00\x00\x01\x8b1\x07L\xdc\
-\x00\x00K\xec\x00\x01\x00\x00\x00\x01\x00\x17\x0e*\
+\x00\x00K\xec\x00\x01\x00\x00\x00\x01\x00\x17\x0e%\
 \x00\x00\x01\x8b1\x07L+\
-\x00\x00K\xb4\x00\x00\x00\x00\x00\x01\x00\x17\x0a\x9f\
+\x00\x00K\xb4\x00\x00\x00\x00\x00\x01\x00\x17\x0a\x9a\
 \x00\x00\x01\x8c\x00\xb0\x09_\
-\x00\x00Hp\x00\x00\x00\x00\x00\x01\x00\x16\xdcC\
+\x00\x00Hp\x00\x00\x00\x00\x00\x01\x00\x16\xdc@\
 \x00\x00\x01\x8b1\x07L\xd6\
-\x00\x00G\xe4\x00\x00\x00\x00\x00\x01\x00\x16\xd3\xb7\
+\x00\x00G\xe4\x00\x00\x00\x00\x00\x01\x00\x16\xd3\xb4\
 \x00\x00\x01\x8b1\x07L\xbc\
-\x00\x00K8\x00\x01\x00\x00\x00\x01\x00\x17\x04\x87\
+\x00\x00K8\x00\x01\x00\x00\x00\x01\x00\x17\x04\x82\
 \x00\x00\x01\x8c\xb4\xff\xf1\xa3\
-\x00\x00JD\x00\x00\x00\x00\x00\x01\x00\x16\xf7\xbe\
+\x00\x00JD\x00\x00\x00\x00\x00\x01\x00\x16\xf7\xb9\
 \x00\x00\x01\x8c\xb4\xff\xf1\xa2\
-\x00\x00J\x96\x00\x00\x00\x00\x00\x01\x00\x16\xfe\x9a\
+\x00\x00J\x96\x00\x00\x00\x00\x00\x01\x00\x16\xfe\x95\
 \x00\x00\x01\x8b1\x07L\xc4\
-\x00\x00K\xcc\x00\x00\x00\x00\x00\x01\x00\x17\x0cx\
+\x00\x00K\xcc\x00\x00\x00\x00\x00\x01\x00\x17\x0cs\
 \x00\x00\x01\x8c\xb4\xff\xf1\x9c\
-\x00\x00I\xc2\x00\x01\x00\x00\x00\x01\x00\x16\xf1o\
+\x00\x00I\xc2\x00\x01\x00\x00\x00\x01\x00\x16\xf1j\
 \x00\x00\x01\x8b1\x07L\xb0\
-\x00\x00H0\x00\x01\x00\x00\x00\x01\x00\x16\xd5v\
+\x00\x00H0\x00\x01\x00\x00\x00\x01\x00\x16\xd5s\
 \x00\x00\x01\x8d\xb652d\
-\x00\x00J\xbe\x00\x00\x00\x00\x00\x01\x00\x17\x00\x17\
+\x00\x00J\xbe\x00\x00\x00\x00\x00\x01\x00\x17\x00\x12\
 \x00\x00\x01\x8b1\x07L\xaf\
-\x00\x00H\x96\x00\x01\x00\x00\x00\x01\x00\x16\xddo\
+\x00\x00H\x96\x00\x01\x00\x00\x00\x01\x00\x16\xddl\
 \x00\x00\x01\x8b1\x07L\x94\
-\x00\x00I>\x00\x00\x00\x00\x00\x01\x00\x16\xe9u\
+\x00\x00I>\x00\x00\x00\x00\x00\x01\x00\x16\xe9p\
 \x00\x00\x01\x8b1\x07L1\
-\x00\x00KX\x00\x01\x00\x00\x00\x01\x00\x17\x07\x1b\
+\x00\x00KX\x00\x01\x00\x00\x00\x01\x00\x17\x07\x16\
 \x00\x00\x01\x8d\xa6\xd33\xd1\
-\x00\x00G\xc4\x00\x00\x00\x00\x00\x01\x00\x16\xce=\
-\x00\x00\x01\x8b1\x07L\x88\
-\x00\x00Jd\x00\x00\x00\x00\x00\x01\x00\x16\xfaF\
+\x00\x00G\xc4\x00\x00\x00\x00\x00\x01\x00\x16\xce;\
+\x00\x00\x01\x8fQ#I\xf3\
+\x00\x00Jd\x00\x00\x00\x00\x00\x01\x00\x16\xfaA\
 \x00\x00\x01\x8b1\x07Ll\
-\x00\x00H\x0e\x00\x00\x00\x00\x00\x01\x00\x16\xd5-\
+\x00\x00H\x0e\x00\x00\x00\x00\x00\x01\x00\x16\xd5*\
 \x00\x00\x01\x8b1\x07L\xa7\
-\x00\x00L>\x00\x01\x00\x00\x00\x01\x00\x17\x13\x1a\
+\x00\x00L>\x00\x01\x00\x00\x00\x01\x00\x17\x13\x15\
 \x00\x00\x01\x8c\x00\xb0\x09f\
-\x00\x00I\x00\x00\x00\x00\x00\x00\x01\x00\x16\xe3l\
+\x00\x00I\x00\x00\x00\x00\x00\x00\x01\x00\x16\xe3i\
 \x00\x00\x01\x8c\xb4\xff\xf1\x9c\
-\x00\x00H\xca\x00\x00\x00\x00\x00\x01\x00\x16\xe1\x08\
+\x00\x00H\xca\x00\x00\x00\x00\x00\x01\x00\x16\xe1\x05\
 \x00\x00\x01\x8b1\x07L\xa1\
-\x00\x00L\x18\x00\x01\x00\x00\x00\x01\x00\x17\x10.\
+\x00\x00L\x18\x00\x01\x00\x00\x00\x01\x00\x17\x10)\
 \x00\x00\x01\x8b1\x07LB\
-\x00\x00HJ\x00\x01\x00\x00\x00\x01\x00\x16\xdaM\
-\x00\x00\x01\x8ei\xd5U\x8e\
+\x00\x00HJ\x00\x01\x00\x00\x00\x01\x00\x16\xdaJ\
+\x00\x00\x01\x8f\x00b\x17\xca\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
     QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
```

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/__init__.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/animation.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/animation.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/auto_wrap.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/auto_wrap.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/color.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/color.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/config.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/config.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/exception_handler.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/exception_handler.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/font.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/font.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/icon.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/icon.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/image_utils.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/image_utils.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/overload.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/overload.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/router.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/router.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/screen.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/screen.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/smooth_scroll.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/smooth_scroll.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/common/style_sheet.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/style_sheet.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/calendar_picker.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/calendar_picker.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,22 @@
     def getDate(self):
         return self._date
 
     def setDate(self, date: QDate):
         """ set the selected date """
         self._onDateChanged(date)
 
+    def reset(self):
+        """ reset date """
+        self._date = QDate()
+        self.setText(self.tr('Pick a date'))
+        self.setProperty('hasDate', False)
+        self.setStyle(QApplication.style())
+        self.update()
+
     def getDateFormat(self):
         return self._dateFormat
 
     def setDateFormat(self, format: Union[Qt.DateFormat, str]):
         self._dateFormat = format
         if self.date.isValid():
             self.setText(self.date.toString(self.dateFormat))
```

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/calendar_view.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/calendar_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/date_picker.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/date_picker.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/picker_base.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/picker_base.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/time_picker.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/time_picker.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/color_dialog.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/color_dialog.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/dialog.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/dialog.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/folder_list_dialog.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/folder_list_dialog.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/mask_dialog_base.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/mask_dialog_base.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/message_box_base.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/message_box_base.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/message_dialog.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/message_dialog.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/expand_layout.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/expand_layout.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/flow_layout.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/v_box_layout.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/v_box_layout.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/__init__.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_combo_box.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_combo_box.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_flyout.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_flyout.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_line_edit.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_line_edit.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_menu.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_menu.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_tool_tip.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_widget.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/__init__.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/breadcrumb.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/breadcrumb.py`

 * *Files 8% similar despite different names*

```diff
@@ -190,15 +190,15 @@
 
         self.updateGeometry()
 
     def setCurrentIndex(self, index: int):
         if not 0 <= index < len(self.items) or index == self.currentIndex():
             return
 
-        if self.currentIndex() >= 0:
+        if 0<= self.currentIndex() < len(self.items):
             self.currentItem().setSelected(False)
 
         self._currentIndex = index
         self.currentItem().setSelected(True)
 
         # remove trailing items
         for item in self.items[-1:index:-1]:
@@ -240,22 +240,25 @@
             item.deleteLater()
 
         self.elideButton.hide()
         self._currentIndex = -1
 
     def popItem(self):
         """ pop trailing item """
-        item = self.items.pop()
-        self.itemMap.pop(item.routeKey)
-        item.deleteLater()
+        if not self.items:
+            return
 
-        if self.currentIndex() >= item.index:
+        if self.count() >= 2:
             self.setCurrentIndex(self.currentIndex() - 1)
+        else:
+            self.clear()
 
-        self.updateGeometry()
+    def count(self):
+        """ Returns the number of items """
+        return len(self.items)
 
     def updateGeometry(self):
         if not self.items:
             return
 
         x = 0
         self.elideButton.hide()
```

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_bar.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_interface.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_interface.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_panel.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_panel.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_widget.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/pivot.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/pivot.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/segmented_widget.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/segmented_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/__init__.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/custom_color_setting_card.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/custom_color_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/expand_setting_card.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/expand_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/folder_list_setting_card.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/folder_list_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/options_setting_card.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/options_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/setting_card.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/setting_card_group.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/setting_card_group.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/__init__.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/acrylic_label.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/acrylic_label.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import warnings
 from  typing import Union
 
 from PySide6.QtCore import Qt, QThread, Signal, QRect
 from PySide6.QtGui import QBrush, QColor, QImage, QPainter, QPixmap, QPainterPath
 from PySide6.QtWidgets import QLabel, QApplication, QWidget
 
+from ...common.screen import getCurrentScreen
+
 try:
     from ...common.image_utils import gaussianBlur
 
     isAcrylicAvailable = True
 except ImportError as e:
     isAcrylicAvailable = False
 
@@ -196,19 +198,21 @@
         """ grab image from screen
 
         Parameters
         ----------
         rect: QRect
             grabbed region
         """
-        screen = QApplication.screenAt(self.device.window().pos())
+        screen = getCurrentScreen()
         if not screen:
             screen = QApplication.screens()[0]
 
         x, y, w, h = rect.x(), rect.y(), rect.width(), rect.height()
+        x -= screen.geometry().x()
+        y -= screen.geometry().y()
         self.setImage(screen.grabWindow(0, x, y, w, h))
 
     def setImage(self, image: Union[str, QImage, QPixmap]):
         """ set blurred image """
         if isinstance(image, str):
             image = QPixmap(image)
         elif isinstance(image, QImage):
```

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/button.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/card_widget.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/card_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/check_box.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/check_box.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/combo_box.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/command_bar.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/command_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/cycle_list_widget.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/cycle_list_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/flip_view.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/flip_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/flyout.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/flyout.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/frameless_window.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/frameless_window.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/icon_widget.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/info_badge.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/info_badge.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/info_bar.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/info_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/label.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/line_edit.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/list_view.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/list_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/menu.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/pips_pager.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/pips_pager.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/progress_bar.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/progress_ring.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/progress_ring.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/scroll_area.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/scroll_bar.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/scroll_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/separator.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/slider.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/spin_box.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/spin_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,17 @@
 
     def paintEvent(self, e):
         super().paintEvent(e)
         painter = QPainter(self)
         painter.setRenderHints(QPainter.Antialiasing |
                                QPainter.SmoothPixmapTransform)
 
-        if self.isPressed:
+        if not self.isEnabled():
+            painter.setOpacity(0.36)
+        elif self.isPressed:
             painter.setOpacity(0.7)
 
         self._icon.render(painter, QRectF(10, 6.5, 11, 11))
 
 
 class CompactSpinButton(QToolButton):
     """ Compact spin button """
```

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/stacked_widget.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/state_tool_tip.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/state_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/switch_button.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/switch_button.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/tab_view.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tab_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/table_view.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/table_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/teaching_tip.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/teaching_tip.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/tool_tip.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tool_tip.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/tree_view.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tree_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/media_play_bar.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/media_play_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/media_player.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/media_player.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/video_widget.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/video_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/window/fluent_window.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/window/fluent_window.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/window/splash_screen.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/window/splash_screen.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/qfluentwidgets/window/stacked_widget.py` & `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/window/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.5/setup.py` & `PySide6-Fluent-Widgets-1.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PySide6-Fluent-Widgets",
-    version="1.5.5",
+    version="1.5.6",
     keywords="pyside6 fluent widgets",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A fluent design widgets library based on PySide6",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

