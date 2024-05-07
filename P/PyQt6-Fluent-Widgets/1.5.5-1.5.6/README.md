# Comparing `tmp/PyQt6-Fluent-Widgets-1.5.5.tar.gz` & `tmp/PyQt6-Fluent-Widgets-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyQt6-Fluent-Widgets-1.5.5.tar", last modified: Sat Apr 13 07:06:06 2024, max compression
+gzip compressed data, was "dist\PyQt6-Fluent-Widgets-1.5.6.tar", last modified: Tue May  7 03:50:30 2024, max compression
```

## Comparing `PyQt6-Fluent-Widgets-1.5.5.tar` & `PyQt6-Fluent-Widgets-1.5.6.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 07:06:06.362288 PyQt6-Fluent-Widgets-1.5.5/
--rw-rw-rw-   0        0        0    35825 2024-04-13 06:56:15.000000 PyQt6-Fluent-Widgets-1.5.5/LICENSE
--rw-rw-rw-   0        0        0     5053 2024-04-13 07:06:06.361278 PyQt6-Fluent-Widgets-1.5.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-13 07:06:06.162294 PyQt6-Fluent-Widgets-1.5.5/PyQt6_Fluent_Widgets.egg-info/
--rw-rw-rw-   0        0        0     5053 2024-04-13 07:06:06.000000 PyQt6-Fluent-Widgets-1.5.5/PyQt6_Fluent_Widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4919 2024-04-13 07:06:06.000000 PyQt6-Fluent-Widgets-1.5.5/PyQt6_Fluent_Widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 07:06:06.000000 PyQt6-Fluent-Widgets-1.5.5/PyQt6_Fluent_Widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2024-04-13 07:06:06.000000 PyQt6-Fluent-Widgets-1.5.5/PyQt6_Fluent_Widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-13 07:06:06.000000 PyQt6-Fluent-Widgets-1.5.5/PyQt6_Fluent_Widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4277 2024-04-13 06:56:15.000000 PyQt6-Fluent-Widgets-1.5.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-13 07:06:06.163809 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/
--rw-rw-rw-   0        0        0      550 2024-04-13 06:56:28.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:06:06.167956 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/_rc/
--rw-rw-rw-   0        0        0        0 2023-10-15 01:50:42.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/_rc/__init__.py
--rw-rw-rw-   0        0        0  3307374 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:06:06.202752 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/
--rw-rw-rw-   0        0        0      664 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/__init__.py
--rw-rw-rw-   0        0        0    22679 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/animation.py
--rw-rw-rw-   0        0        0     4742 2023-12-29 09:55:21.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/auto_wrap.py
--rw-rw-rw-   0        0        0     1587 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/color.py
--rw-rw-rw-   0        0        0    11167 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/config.py
--rw-rw-rw-   0        0        0      675 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/exception_handler.py
--rw-rw-rw-   0        0        0      817 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/font.py
--rw-rw-rw-   0        0        0    13818 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/icon.py
--rw-rw-rw-   0        0        0     5549 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/image_utils.py
--rw-rw-rw-   0        0        0     1635 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/overload.py
--rw-rw-rw-   0        0        0     3866 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/router.py
--rw-rw-rw-   0        0        0      658 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/screen.py
--rw-rw-rw-   0        0        0     4847 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/smooth_scroll.py
--rw-rw-rw-   0        0        0    14425 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/style_sheet.py
--rw-rw-rw-   0        0        0      452 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/translator.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:06:06.205194 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/
--rw-rw-rw-   0        0        0      150 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:06:06.216091 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/
--rw-rw-rw-   0        0        0      234 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/__init__.py
--rw-rw-rw-   0        0        0     2354 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/calendar_picker.py
--rw-rw-rw-   0        0        0    22447 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/calendar_view.py
--rw-rw-rw-   0        0        0     7658 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/date_picker.py
--rw-rw-rw-   0        0        0    19774 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/picker_base.py
--rw-rw-rw-   0        0        0     6439 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/time_picker.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:06:06.230586 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/
--rw-rw-rw-   0        0        0      216 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/__init__.py
--rw-rw-rw-   0        0        0    15056 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/color_dialog.py
--rw-rw-rw-   0        0        0     6001 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/dialog.py
--rw-rw-rw-   0        0        0    11791 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/folder_list_dialog.py
--rw-rw-rw-   0        0        0     3157 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/mask_dialog_base.py
--rw-rw-rw-   0        0        0     2967 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/message_box_base.py
--rw-rw-rw-   0        0        0     2424 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/message_dialog.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:06:06.238120 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/
--rw-rw-rw-   0        0        0      114 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/__init__.py
--rw-rw-rw-   0        0        0     2727 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/expand_layout.py
--rw-rw-rw-   0        0        0     7110 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/flow_layout.py
--rw-rw-rw-   0        0        0     1262 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/v_box_layout.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:06:06.250457 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/
--rw-rw-rw-   0        0        0      538 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/__init__.py
--rw-rw-rw-   0        0        0     3032 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_combo_box.py
--rw-rw-rw-   0        0        0     3580 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_flyout.py
--rw-rw-rw-   0        0        0      763 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_line_edit.py
--rw-rw-rw-   0        0        0     6314 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_menu.py
--rw-rw-rw-   0        0        0     1181 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_tool_tip.py
--rw-rw-rw-   0        0        0     1453 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:06:06.266147 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/
--rw-rw-rw-   0        0        0      716 2023-11-24 09:36:26.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/__init__.py
--rw-rw-rw-   0        0        0    10070 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/breadcrumb.py
--rw-rw-rw-   0        0        0    13248 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_bar.py
--rw-rw-rw-   0        0        0     8745 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_interface.py
--rw-rw-rw-   0        0        0    24728 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_panel.py
--rw-rw-rw-   0        0        0    19994 2024-04-13 06:57:06.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_widget.py
--rw-rw-rw-   0        0        0     6888 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/pivot.py
--rw-rw-rw-   0        0        0     5254 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/segmented_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:06:06.279918 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/
--rw-rw-rw-   0        0        0      550 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/__init__.py
--rw-rw-rw-   0        0        0     5354 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/custom_color_setting_card.py
--rw-rw-rw-   0        0        0    11296 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/expand_setting_card.py
--rw-rw-rw-   0        0        0     4697 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/folder_list_setting_card.py
--rw-rw-rw-   0        0        0     2843 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/options_setting_card.py
--rw-rw-rw-   0        0        0    14288 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/setting_card.py
--rw-rw-rw-   0        0        0     1544 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/setting_card_group.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:06:06.343420 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/
--rw-rw-rw-   0        0        0     3328 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/__init__.py
--rw-rw-rw-   0        0        0     8098 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/acrylic_label.py
--rw-rw-rw-   0        0        0    30220 2024-04-13 06:56:28.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/button.py
--rw-rw-rw-   0        0        0     7755 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/card_widget.py
--rw-rw-rw-   0        0        0     5835 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/check_box.py
--rw-rw-rw-   0        0        0    15886 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/combo_box.py
--rw-rw-rw-   0        0        0    19946 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/command_bar.py
--rw-rw-rw-   0        0        0     8072 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/cycle_list_widget.py
--rw-rw-rw-   0        0        0    13322 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/flip_view.py
--rw-rw-rw-   0        0        0    17277 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/flyout.py
--rw-rw-rw-   0        0        0     2318 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/frameless_window.py
--rw-rw-rw-   0        0        0     1552 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/icon_widget.py
--rw-rw-rw-   0        0        0    16747 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/info_badge.py
--rw-rw-rw-   0        0        0    19320 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/info_bar.py
--rw-rw-rw-   0        0        0    14940 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/label.py
--rw-rw-rw-   0        0        0    14414 2024-04-13 06:56:28.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/line_edit.py
--rw-rw-rw-   0        0        0     4750 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/list_view.py
--rw-rw-rw-   0        0        0    40909 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/menu.py
--rw-rw-rw-   0        0        0    11379 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/pips_pager.py
--rw-rw-rw-   0        0        0     9269 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     7143 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/progress_ring.py
--rw-rw-rw-   0        0        0     2758 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/scroll_area.py
--rw-rw-rw-   0        0        0    18352 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/scroll_bar.py
--rw-rw-rw-   0        0        0     1226 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/separator.py
--rw-rw-rw-   0        0        0    10206 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/slider.py
--rw-rw-rw-   0        0        0     8776 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/spin_box.py
--rw-rw-rw-   0        0        0     6564 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0     5923 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/state_tool_tip.py
--rw-rw-rw-   0        0        0     8768 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/switch_button.py
--rw-rw-rw-   0        0        0    26737 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/tab_view.py
--rw-rw-rw-   0        0        0    11626 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/table_view.py
--rw-rw-rw-   0        0        0    23075 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/teaching_tip.py
--rw-rw-rw-   0        0        0    10674 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/tool_tip.py
--rw-rw-rw-   0        0        0     4671 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/tree_view.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:06:06.351421 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/
--rw-rw-rw-   0        0        0      183 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/__init__.py
--rw-rw-rw-   0        0        0    11775 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/media_play_bar.py
--rw-rw-rw-   0        0        0     3943 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/media_player.py
--rw-rw-rw-   0        0        0     2947 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/video_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:06:06.359406 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/window/
--rw-rw-rw-   0        0        0      187 2024-04-13 06:56:28.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/window/__init__.py
--rw-rw-rw-   0        0        0    13085 2024-04-13 06:56:28.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/window/fluent_window.py
--rw-rw-rw-   0        0        0     2840 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/window/splash_screen.py
--rw-rw-rw-   0        0        0     1685 2024-04-13 06:56:16.000000 PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/window/stacked_widget.py
--rw-rw-rw-   0        0        0       42 2024-04-13 07:06:06.362288 PyQt6-Fluent-Widgets-1.5.5/setup.cfg
--rw-rw-rw-   0        0        0     1205 2024-04-13 06:56:38.000000 PyQt6-Fluent-Widgets-1.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.692561 PyQt6-Fluent-Widgets-1.5.6/
+-rw-rw-rw-   0        0        0    35825 2024-05-07 03:47:53.000000 PyQt6-Fluent-Widgets-1.5.6/LICENSE
+-rw-rw-rw-   0        0        0     5230 2024-05-07 03:50:30.691563 PyQt6-Fluent-Widgets-1.5.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.501443 PyQt6-Fluent-Widgets-1.5.6/PyQt6_Fluent_Widgets.egg-info/
+-rw-rw-rw-   0        0        0     5230 2024-05-07 03:50:30.000000 PyQt6-Fluent-Widgets-1.5.6/PyQt6_Fluent_Widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4919 2024-05-07 03:50:30.000000 PyQt6-Fluent-Widgets-1.5.6/PyQt6_Fluent_Widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 03:50:30.000000 PyQt6-Fluent-Widgets-1.5.6/PyQt6_Fluent_Widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2024-05-07 03:50:30.000000 PyQt6-Fluent-Widgets-1.5.6/PyQt6_Fluent_Widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-07 03:50:30.000000 PyQt6-Fluent-Widgets-1.5.6/PyQt6_Fluent_Widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4454 2024-05-07 03:48:38.000000 PyQt6-Fluent-Widgets-1.5.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.502543 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/
+-rw-rw-rw-   0        0        0      550 2024-05-07 03:48:16.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.506112 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/_rc/
+-rw-rw-rw-   0        0        0        0 2023-10-15 01:50:42.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/_rc/__init__.py
+-rw-rw-rw-   0        0        0  6502800 2024-05-07 03:49:15.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.544397 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/
+-rw-rw-rw-   0        0        0      664 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/__init__.py
+-rw-rw-rw-   0        0        0    22679 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/animation.py
+-rw-rw-rw-   0        0        0     4742 2023-12-29 09:55:21.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/auto_wrap.py
+-rw-rw-rw-   0        0        0     1587 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/color.py
+-rw-rw-rw-   0        0        0    11167 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/config.py
+-rw-rw-rw-   0        0        0      675 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/exception_handler.py
+-rw-rw-rw-   0        0        0      817 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/font.py
+-rw-rw-rw-   0        0        0    13818 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/icon.py
+-rw-rw-rw-   0        0        0     5549 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/image_utils.py
+-rw-rw-rw-   0        0        0     1635 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/overload.py
+-rw-rw-rw-   0        0        0     3866 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/router.py
+-rw-rw-rw-   0        0        0      658 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/screen.py
+-rw-rw-rw-   0        0        0     4847 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/smooth_scroll.py
+-rw-rw-rw-   0        0        0    14425 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/style_sheet.py
+-rw-rw-rw-   0        0        0      452 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/translator.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.546397 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/
+-rw-rw-rw-   0        0        0      150 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.556107 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/
+-rw-rw-rw-   0        0        0      234 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/__init__.py
+-rw-rw-rw-   0        0        0     2594 2024-05-07 03:48:16.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/calendar_picker.py
+-rw-rw-rw-   0        0        0    22447 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/calendar_view.py
+-rw-rw-rw-   0        0        0     7658 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/date_picker.py
+-rw-rw-rw-   0        0        0    19774 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/picker_base.py
+-rw-rw-rw-   0        0        0     6439 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/time_picker.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.568013 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/
+-rw-rw-rw-   0        0        0      216 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/__init__.py
+-rw-rw-rw-   0        0        0    15056 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/color_dialog.py
+-rw-rw-rw-   0        0        0     6001 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/dialog.py
+-rw-rw-rw-   0        0        0    11791 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/folder_list_dialog.py
+-rw-rw-rw-   0        0        0     3157 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/mask_dialog_base.py
+-rw-rw-rw-   0        0        0     2967 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/message_box_base.py
+-rw-rw-rw-   0        0        0     2424 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/message_dialog.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.574296 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/
+-rw-rw-rw-   0        0        0      114 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/__init__.py
+-rw-rw-rw-   0        0        0     2727 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/expand_layout.py
+-rw-rw-rw-   0        0        0     7110 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/flow_layout.py
+-rw-rw-rw-   0        0        0     1262 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/v_box_layout.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.586181 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/
+-rw-rw-rw-   0        0        0      538 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/__init__.py
+-rw-rw-rw-   0        0        0     3032 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_combo_box.py
+-rw-rw-rw-   0        0        0     3580 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_flyout.py
+-rw-rw-rw-   0        0        0      763 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_line_edit.py
+-rw-rw-rw-   0        0        0     6314 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_menu.py
+-rw-rw-rw-   0        0        0     1181 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_tool_tip.py
+-rw-rw-rw-   0        0        0     1453 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.600454 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/
+-rw-rw-rw-   0        0        0      716 2023-11-24 09:36:26.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/__init__.py
+-rw-rw-rw-   0        0        0    10126 2024-05-07 03:48:16.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/breadcrumb.py
+-rw-rw-rw-   0        0        0    13248 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_bar.py
+-rw-rw-rw-   0        0        0     8745 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_interface.py
+-rw-rw-rw-   0        0        0    24728 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_panel.py
+-rw-rw-rw-   0        0        0    19994 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_widget.py
+-rw-rw-rw-   0        0        0     6888 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/pivot.py
+-rw-rw-rw-   0        0        0     5254 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/segmented_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.613788 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/
+-rw-rw-rw-   0        0        0      550 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/__init__.py
+-rw-rw-rw-   0        0        0     5354 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/custom_color_setting_card.py
+-rw-rw-rw-   0        0        0    11296 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/expand_setting_card.py
+-rw-rw-rw-   0        0        0     4697 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/folder_list_setting_card.py
+-rw-rw-rw-   0        0        0     2843 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/options_setting_card.py
+-rw-rw-rw-   0        0        0    14288 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/setting_card.py
+-rw-rw-rw-   0        0        0     1544 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/setting_card_group.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.675267 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/
+-rw-rw-rw-   0        0        0     3328 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/__init__.py
+-rw-rw-rw-   0        0        0     8188 2024-05-07 03:48:16.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/acrylic_label.py
+-rw-rw-rw-   0        0        0    30220 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/button.py
+-rw-rw-rw-   0        0        0     7755 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/card_widget.py
+-rw-rw-rw-   0        0        0     5835 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/check_box.py
+-rw-rw-rw-   0        0        0    15886 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/combo_box.py
+-rw-rw-rw-   0        0        0    19946 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/command_bar.py
+-rw-rw-rw-   0        0        0     8072 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/cycle_list_widget.py
+-rw-rw-rw-   0        0        0    13322 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/flip_view.py
+-rw-rw-rw-   0        0        0    17277 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/flyout.py
+-rw-rw-rw-   0        0        0     2318 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/frameless_window.py
+-rw-rw-rw-   0        0        0     1552 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0    16747 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/info_badge.py
+-rw-rw-rw-   0        0        0    19320 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/info_bar.py
+-rw-rw-rw-   0        0        0    14940 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/label.py
+-rw-rw-rw-   0        0        0    14414 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     4750 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/list_view.py
+-rw-rw-rw-   0        0        0    40909 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/menu.py
+-rw-rw-rw-   0        0        0    11379 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/pips_pager.py
+-rw-rw-rw-   0        0        0     9269 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     7143 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/progress_ring.py
+-rw-rw-rw-   0        0        0     2758 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0    18352 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/scroll_bar.py
+-rw-rw-rw-   0        0        0     1226 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/separator.py
+-rw-rw-rw-   0        0        0    10206 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/slider.py
+-rw-rw-rw-   0        0        0     8850 2024-05-07 03:48:16.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     6564 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0     5923 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/state_tool_tip.py
+-rw-rw-rw-   0        0        0     8768 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/switch_button.py
+-rw-rw-rw-   0        0        0    26737 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tab_view.py
+-rw-rw-rw-   0        0        0    11626 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/table_view.py
+-rw-rw-rw-   0        0        0    23075 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/teaching_tip.py
+-rw-rw-rw-   0        0        0    10674 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tool_tip.py
+-rw-rw-rw-   0        0        0     4671 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tree_view.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.682143 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/
+-rw-rw-rw-   0        0        0      183 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/__init__.py
+-rw-rw-rw-   0        0        0    11775 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/media_play_bar.py
+-rw-rw-rw-   0        0        0     3943 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/media_player.py
+-rw-rw-rw-   0        0        0     2947 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/video_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.689561 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/window/
+-rw-rw-rw-   0        0        0      187 2024-04-13 06:56:28.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/window/__init__.py
+-rw-rw-rw-   0        0        0    13085 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/window/fluent_window.py
+-rw-rw-rw-   0        0        0     2840 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/window/splash_screen.py
+-rw-rw-rw-   0        0        0     1685 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/window/stacked_widget.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 03:50:30.692861 PyQt6-Fluent-Widgets-1.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     1205 2024-05-07 03:48:44.000000 PyQt6-Fluent-Widgets-1.5.6/setup.py
```

### Comparing `PyQt6-Fluent-Widgets-1.5.5/LICENSE` & `PyQt6-Fluent-Widgets-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/PKG-INFO` & `PyQt6-Fluent-Widgets-1.5.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-Fluent-Widgets
-Version: 1.5.5
+Version: 1.5.6
 Summary: A fluent design widgets library based on PyQt6
 Home-page: https://qfluentwidgets.com
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://qfluentwidgets.com/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PyQt6
@@ -89,17 +89,19 @@
 
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
 * [**zhiyiYo/QMaterialWidgets**: A material design widgets library based on PyQt/PySide](https://qmaterialwidgets.vercel.app)
 * [**zhiyiYo/Groove**: A cross-platform music player based on PyQt5](https://github.com/zhiyiYo/Groove)
 * [**zhiyiYo/Alpha-Gobang-Zero**: A gobang robot based on reinforcement learning](https://github.com/zhiyiYo/Alpha-Gobang-Zero)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyQt6-Fluent-Widgets Version: 1.5.5 Summary: A
+Metadata-Version: 2.1 Name: PyQt6-Fluent-Widgets Version: 1.5.6 Summary: A
 fluent design widgets library based on PyQt6 Home-page: https://
 qfluentwidgets.com Author: zhiyiYo Author-email: shokokawaii@outlook.com
 License: GPLv3 Project-URL: Documentation, https://qfluentwidgets.com/ Project-
 URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PyQt6
 Project-URL: Bug Tracker, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues
 Keywords: pyqt6 fluent widgets Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
@@ -36,21 +36,23 @@
 //pypi.org/simple and reinstall again. ## Documentation Want to know more about
 PyQt-Fluent-Widgets? Please read the [help document](https://
 qfluentwidgets.com) ð ## License PyQt6-Fluent-Widgets is licensed under
 [GPLv3](./LICENSE) for non-commercial project. For commercial use, please
 purchase a [commercial license](https://qfluentwidgets.com/price). Copyright Â©
 2021 by zhiyiYo. ## Video Demonstration Check out this [â¶ example video]
 (https://www.bilibili.com/video/BV12c411L73q) that shows off what PyQt-Fluent-
-Widgets are capable of ð ## Support If this project helps you a lot and you
-want to support the development and maintenance of this project, feel free to
-sponsor me via [ç±åçµ](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-
-fi.com/zhiyiYo). Your support is highly appreciated ð¥° ## See Also Here are
-some projects based on PyQt-Fluent-Widgets: * [**zhiyiYo/QMaterialWidgets**: A
-material design widgets library based on PyQt/PySide](https://
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
+library based on PyQt/PySide](https://qmaterialwidgets.vercel.app) *
+[**zhiyiYo/Groove**: A cross-platform music player based on PyQt5](https://
+github.com/zhiyiYo/Groove) * [**zhiyiYo/Alpha-Gobang-Zero**: A gobang robot
+based on reinforcement learning](https://github.com/zhiyiYo/Alpha-Gobang-Zero)
+## Reference * [**Windows design**: Design guidelines and toolkits for creating
+native app experiences](https://learn.microsoft.com/zh-cn/windows/apps/design/
+) * [**Microsoft/WinUI-Gallery**: An app demonstrates the controls available in
+WinUI and the Fluent Design System](https://github.com/microsoft/WinUI-Gallery)
```

### Comparing `PyQt6-Fluent-Widgets-1.5.5/PyQt6_Fluent_Widgets.egg-info/PKG-INFO` & `PyQt6-Fluent-Widgets-1.5.6/PyQt6_Fluent_Widgets.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-Fluent-Widgets
-Version: 1.5.5
+Version: 1.5.6
 Summary: A fluent design widgets library based on PyQt6
 Home-page: https://qfluentwidgets.com
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://qfluentwidgets.com/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PyQt6
@@ -89,17 +89,19 @@
 
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
 * [**zhiyiYo/QMaterialWidgets**: A material design widgets library based on PyQt/PySide](https://qmaterialwidgets.vercel.app)
 * [**zhiyiYo/Groove**: A cross-platform music player based on PyQt5](https://github.com/zhiyiYo/Groove)
 * [**zhiyiYo/Alpha-Gobang-Zero**: A gobang robot based on reinforcement learning](https://github.com/zhiyiYo/Alpha-Gobang-Zero)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyQt6-Fluent-Widgets Version: 1.5.5 Summary: A
+Metadata-Version: 2.1 Name: PyQt6-Fluent-Widgets Version: 1.5.6 Summary: A
 fluent design widgets library based on PyQt6 Home-page: https://
 qfluentwidgets.com Author: zhiyiYo Author-email: shokokawaii@outlook.com
 License: GPLv3 Project-URL: Documentation, https://qfluentwidgets.com/ Project-
 URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PyQt6
 Project-URL: Bug Tracker, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues
 Keywords: pyqt6 fluent widgets Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
@@ -36,21 +36,23 @@
 //pypi.org/simple and reinstall again. ## Documentation Want to know more about
 PyQt-Fluent-Widgets? Please read the [help document](https://
 qfluentwidgets.com) ð ## License PyQt6-Fluent-Widgets is licensed under
 [GPLv3](./LICENSE) for non-commercial project. For commercial use, please
 purchase a [commercial license](https://qfluentwidgets.com/price). Copyright Â©
 2021 by zhiyiYo. ## Video Demonstration Check out this [â¶ example video]
 (https://www.bilibili.com/video/BV12c411L73q) that shows off what PyQt-Fluent-
-Widgets are capable of ð ## Support If this project helps you a lot and you
-want to support the development and maintenance of this project, feel free to
-sponsor me via [ç±åçµ](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-
-fi.com/zhiyiYo). Your support is highly appreciated ð¥° ## See Also Here are
-some projects based on PyQt-Fluent-Widgets: * [**zhiyiYo/QMaterialWidgets**: A
-material design widgets library based on PyQt/PySide](https://
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
+library based on PyQt/PySide](https://qmaterialwidgets.vercel.app) *
+[**zhiyiYo/Groove**: A cross-platform music player based on PyQt5](https://
+github.com/zhiyiYo/Groove) * [**zhiyiYo/Alpha-Gobang-Zero**: A gobang robot
+based on reinforcement learning](https://github.com/zhiyiYo/Alpha-Gobang-Zero)
+## Reference * [**Windows design**: Design guidelines and toolkits for creating
+native app experiences](https://learn.microsoft.com/zh-cn/windows/apps/design/
+) * [**Microsoft/WinUI-Gallery**: An app demonstrates the controls available in
+WinUI and the Fluent Design System](https://github.com/microsoft/WinUI-Gallery)
```

### Comparing `PyQt6-Fluent-Widgets-1.5.5/PyQt6_Fluent_Widgets.egg-info/SOURCES.txt` & `PyQt6-Fluent-Widgets-1.5.6/PyQt6_Fluent_Widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/README.md` & `PyQt6-Fluent-Widgets-1.5.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -69,17 +69,19 @@
 
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
 * [**zhiyiYo/QMaterialWidgets**: A material design widgets library based on PyQt/PySide](https://qmaterialwidgets.vercel.app)
 * [**zhiyiYo/Groove**: A cross-platform music player based on PyQt5](https://github.com/zhiyiYo/Groove)
 * [**zhiyiYo/Alpha-Gobang-Zero**: A gobang robot based on reinforcement learning](https://github.com/zhiyiYo/Alpha-Gobang-Zero)
```

#### html2text {}

```diff
@@ -25,21 +25,23 @@
 //pypi.org/simple and reinstall again. ## Documentation Want to know more about
 PyQt-Fluent-Widgets? Please read the [help document](https://
 qfluentwidgets.com) ð ## License PyQt6-Fluent-Widgets is licensed under
 [GPLv3](./LICENSE) for non-commercial project. For commercial use, please
 purchase a [commercial license](https://qfluentwidgets.com/price). Copyright Â©
 2021 by zhiyiYo. ## Video Demonstration Check out this [â¶ example video]
 (https://www.bilibili.com/video/BV12c411L73q) that shows off what PyQt-Fluent-
-Widgets are capable of ð ## Support If this project helps you a lot and you
-want to support the development and maintenance of this project, feel free to
-sponsor me via [ç±åçµ](https://afdian.net/a/zhiyiYo) or [ko-fi](https://ko-
-fi.com/zhiyiYo). Your support is highly appreciated ð¥° ## See Also Here are
-some projects based on PyQt-Fluent-Widgets: * [**zhiyiYo/QMaterialWidgets**: A
-material design widgets library based on PyQt/PySide](https://
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
+library based on PyQt/PySide](https://qmaterialwidgets.vercel.app) *
+[**zhiyiYo/Groove**: A cross-platform music player based on PyQt5](https://
+github.com/zhiyiYo/Groove) * [**zhiyiYo/Alpha-Gobang-Zero**: A gobang robot
+based on reinforcement learning](https://github.com/zhiyiYo/Alpha-Gobang-Zero)
+## Reference * [**Windows design**: Design guidelines and toolkits for creating
+native app experiences](https://learn.microsoft.com/zh-cn/windows/apps/design/
+) * [**Microsoft/WinUI-Gallery**: An app demonstrates the controls available in
+WinUI and the Fluent Design System](https://github.com/microsoft/WinUI-Gallery)
```

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/__init__.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,14 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PyQt6/examples.
 
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

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/__init__.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/animation.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/animation.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/auto_wrap.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/auto_wrap.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/color.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/color.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/config.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/config.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/exception_handler.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/exception_handler.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/font.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/font.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/icon.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/icon.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/image_utils.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/image_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/overload.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/overload.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/router.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/router.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/screen.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/screen.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/smooth_scroll.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/smooth_scroll.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/common/style_sheet.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/style_sheet.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/calendar_picker.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/calendar_picker.py`

 * *Files 7% similar despite different names*

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

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/calendar_view.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/calendar_view.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/date_picker.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/date_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/picker_base.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/picker_base.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/date_time/time_picker.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/time_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/color_dialog.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/color_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/dialog.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/folder_list_dialog.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/folder_list_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/mask_dialog_base.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/mask_dialog_base.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/message_box_base.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/message_box_base.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/dialog_box/message_dialog.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/message_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/expand_layout.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/expand_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/flow_layout.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/layout/v_box_layout.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/v_box_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/__init__.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_combo_box.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_combo_box.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_flyout.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_flyout.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_line_edit.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_menu.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_menu.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_tool_tip.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/material/acrylic_widget.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/__init__.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/breadcrumb.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/breadcrumb.py`

 * *Files 8% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 
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
@@ -241,22 +241,25 @@
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

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_bar.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_interface.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_interface.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_panel.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_panel.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/navigation_widget.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/pivot.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/pivot.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/navigation/segmented_widget.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/segmented_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/__init__.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/custom_color_setting_card.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/custom_color_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/expand_setting_card.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/expand_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/folder_list_setting_card.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/folder_list_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/options_setting_card.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/options_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/setting_card.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/settings/setting_card_group.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/setting_card_group.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/__init__.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/acrylic_label.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/acrylic_label.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import warnings
 from  typing import Union
 
 from PyQt6.QtCore import Qt, QThread, pyqtSignal, QRect
 from PyQt6.QtGui import QBrush, QColor, QImage, QPainter, QPixmap, QPainterPath
 from PyQt6.QtWidgets import QLabel, QApplication, QWidget
 
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

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/button.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/card_widget.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/card_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/check_box.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/check_box.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/combo_box.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/command_bar.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/command_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/cycle_list_widget.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/cycle_list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/flip_view.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/flip_view.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/flyout.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/flyout.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/frameless_window.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/frameless_window.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/icon_widget.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/info_badge.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/info_badge.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/info_bar.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/info_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/label.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/line_edit.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/list_view.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/list_view.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/menu.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/pips_pager.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/pips_pager.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/progress_bar.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/progress_ring.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/progress_ring.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/scroll_area.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/scroll_bar.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/scroll_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/separator.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/slider.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/spin_box.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/spin_box.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,17 @@
 
     def paintEvent(self, e):
         super().paintEvent(e)
         painter = QPainter(self)
         painter.setRenderHints(QPainter.RenderHint.Antialiasing |
                                QPainter.RenderHint.SmoothPixmapTransform)
 
-        if self.isPressed:
+        if not self.isEnabled():
+            painter.setOpacity(0.36)
+        elif self.isPressed:
             painter.setOpacity(0.7)
 
         self._icon.render(painter, QRectF(10, 6.5, 11, 11))
 
 
 class CompactSpinButton(QToolButton):
     """ Compact spin button """
```

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/stacked_widget.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/state_tool_tip.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/state_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/switch_button.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/switch_button.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/tab_view.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tab_view.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/table_view.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/table_view.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/teaching_tip.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/teaching_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/tool_tip.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tool_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/components/widgets/tree_view.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tree_view.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/media_play_bar.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/media_play_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/media_player.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/media_player.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/multimedia/video_widget.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/video_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/window/fluent_window.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/window/fluent_window.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/window/splash_screen.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/window/splash_screen.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/qfluentwidgets/window/stacked_widget.py` & `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/window/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.5/setup.py` & `PyQt6-Fluent-Widgets-1.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PyQt6-Fluent-Widgets",
-    version="1.5.5",
+    version="1.5.6",
     keywords="pyqt6 fluent widgets",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A fluent design widgets library based on PyQt6",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

