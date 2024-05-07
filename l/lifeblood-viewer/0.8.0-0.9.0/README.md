# Comparing `tmp/lifeblood-viewer-0.8.0.tar.gz` & `tmp/lifeblood-viewer-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeblood-viewer-0.8.0.tar", last modified: Wed Feb 28 20:25:59 2024, max compression
+gzip compressed data, was "lifeblood-viewer-0.9.0.tar", last modified: Sun Mar 10 23:19:51 2024, max compression
```

## Comparing `lifeblood-viewer-0.8.0.tar` & `lifeblood-viewer-0.9.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:59.395215 lifeblood-viewer-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-02-28 20:25:59.395215 lifeblood-viewer-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-02-28 20:25:59.395215 lifeblood-viewer-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:59.383215 lifeblood-viewer-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:59.391215 lifeblood-viewer-0.8.0/src/lifeblood_viewer/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    86923 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/breeze_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:59.391215 lifeblood-viewer-0.8.0/src/lifeblood_viewer/code_editor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/code_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/code_editor/editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    37591 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/connection_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10233 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/create_task_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/db_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/editor_scene_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    94032 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/graphics_items.py
--rw-r--r--   0 runner    (1001) docker     (127)    79193 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/graphics_scene.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:59.391215 lifeblood-viewer-0.8.0/src/lifeblood_viewer/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/icons/lifeblood.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/imgui_opengl_hotfix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/launch.py
--rw-r--r--   0 runner    (1001) docker     (127)    17408 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/lifeblood_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/long_op.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/menu_entry_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:59.391215 lifeblood-viewer-0.8.0/src/lifeblood_viewer/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/models/multiple_sort_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/node_extra_items.py
--rw-r--r--   0 runner    (1001) docker     (127)    52843 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/nodeeditor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:59.391215 lifeblood-viewer-0.8.0/src/lifeblood_viewer/nodeeditor_overlays/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/nodeeditor_overlays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/nodeeditor_overlays/overlay_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/nodeeditor_overlays/task_history_overlay.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:59.391215 lifeblood-viewer-0.8.0/src/lifeblood_viewer/nodeeditor_windows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/nodeeditor_windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/nodeeditor_windows/ui_create_node_popup.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/nodeeditor_windows/ui_longop_window.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/nodeeditor_windows/ui_parameters_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/nodeeditor_windows/ui_task_list_window.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/nodeeditor_windows/ui_undo_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/save_node_settings_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    16232 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/scene_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/ui_elements_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/ui_scene_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/ui_snippets.py
--rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/undo_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:59.395215 lifeblood-viewer-0.8.0/src/lifeblood_viewer/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/widgets/flashy_label.py
--rw-r--r--   0 runner    (1001) docker     (127)    14871 2024-02-28 20:25:43.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer/widgets/worker_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:59.395215 lifeblood-viewer-0.8.0/src/lifeblood_viewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-02-28 20:25:59.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-02-28 20:25:59.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 20:25:59.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-28 20:25:59.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-28 20:25:59.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-28 20:25:59.000000 lifeblood-viewer-0.8.0/src/lifeblood_viewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:51.079595 lifeblood-viewer-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-03-10 23:19:51.079595 lifeblood-viewer-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-10 23:19:51.079595 lifeblood-viewer-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:51.067595 lifeblood-viewer-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:51.075595 lifeblood-viewer-0.9.0/src/lifeblood_viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86923 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/breeze_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:51.075595 lifeblood-viewer-0.9.0/src/lifeblood_viewer/code_editor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/code_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/code_editor/editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37845 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/connection_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10233 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/create_task_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/db_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/editor_scene_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94032 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/graphics_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79193 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/graphics_scene.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:51.075595 lifeblood-viewer-0.9.0/src/lifeblood_viewer/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/icons/lifeblood.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/imgui_opengl_hotfix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18562 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/lifeblood_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/long_op.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/menu_entry_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:51.079595 lifeblood-viewer-0.9.0/src/lifeblood_viewer/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/models/multiple_sort_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/node_extra_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52843 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/nodeeditor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:51.079595 lifeblood-viewer-0.9.0/src/lifeblood_viewer/nodeeditor_overlays/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/nodeeditor_overlays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/nodeeditor_overlays/overlay_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/nodeeditor_overlays/task_history_overlay.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:51.079595 lifeblood-viewer-0.9.0/src/lifeblood_viewer/nodeeditor_windows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/nodeeditor_windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/nodeeditor_windows/ui_create_node_popup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/nodeeditor_windows/ui_longop_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/nodeeditor_windows/ui_parameters_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/nodeeditor_windows/ui_task_list_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/nodeeditor_windows/ui_undo_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/save_node_settings_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16232 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/scene_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/ui_elements_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/ui_scene_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/ui_snippets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/undo_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:51.079595 lifeblood-viewer-0.9.0/src/lifeblood_viewer/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/widgets/flashy_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14871 2024-03-10 23:19:42.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer/widgets/worker_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:51.079595 lifeblood-viewer-0.9.0/src/lifeblood_viewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-03-10 23:19:51.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-03-10 23:19:51.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-10 23:19:51.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-10 23:19:51.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-10 23:19:51.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-10 23:19:51.000000 lifeblood-viewer-0.9.0/src/lifeblood_viewer.egg-info/top_level.txt
```

### Comparing `lifeblood-viewer-0.8.0/PKG-INFO` & `lifeblood-viewer-0.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeblood-viewer
-Version: 0.8.0
+Version: 0.9.0
 Summary: view the LIFEBLOOD !!
 Home-page: https://github.com/pedohorse/lifeblood
 Author: XAPKOHHEH
 Project-URL: Bug Tracker, https://github.com/pedohorse/lifeblood/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -17,17 +17,17 @@
 Requires-Dist: lz4~=4.0
 Requires-Dist: lifeblood~=0.1
 Requires-Dist: grandalf~=0.7
 Requires-Dist: numpy~=1.21
 
 [Documentation](https://pedohorse.github.io/lifeblood)
 
-|master|dev|
-|---|---|
-|[![Tests](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml/badge.svg?branch=master)](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml)<br>[![Tests windows](https://github.com/pedohorse/lifeblood/actions/workflows/tests-win.yml/badge.svg?branch=master)](https://github.com/pedohorse/lifeblood/actions/workflows/tests-win.yml)|[![Tests](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml/badge.svg?branch=dev)](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml)<br>[![Tests windows](https://github.com/pedohorse/lifeblood/actions/workflows/tests-win.yml/badge.svg?branch=dev)](https://github.com/pedohorse/lifeblood/actions/workflows/tests-win.yml)|
+| dev                                                                                                                                                                         |
+|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| [![Tests](https://github.com/pedohorse/lifeblood/actions/workflows/tests.yml/badge.svg?branch=dev)](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml)|
 
 ![](icon/lifeblood.svg)
 
 ## Lifeblood
 Lifeblood is a task/job management software package  
 currently it aims for smaller teams, farms or even individual setups, but with scaling  always in mind.
 
@@ -42,14 +42,16 @@
 processing graph.
 
 This system overview should be very familiar to anyone who saw at least one renderfarm.
 
 check [documentation here](https://pedohorse.github.io/lifeblood)  
 and also [video tutorials](https://pedohorse.github.io/lifeblood/tutorials.html)
 
+## UNDER DEVELOPMENT
+
 ### Features:
 - instantly and easily deployable
 - easy scaling in mind
 - dynamic slots, worker resources management
 - support for environment wrappers (allow you to integrate with existing packaging systems like rez)
 
 ### Features To Be Done:
@@ -65,9 +67,12 @@
 
 ## Installation
 
 There are multiple ways to get Lifeblood to try it out, refer to [installation section in the docs](https://pedohorse.github.io/lifeblood/installation.html#simplest-lifeblood-manager)
 
 In short - easiest way is to use [Lifeblood-Manager](https://github.com/pedohorse/lifeblood-manager/releases), as described in the docs
 
-## UNDER DEVELOPMENT
+## Links
 
+- [blog + support](https://www.patreon.com/xapkohheh)
+- [telegram support/discussion group](https://t.me/+v9klFGZcKVY2MjYy)
+- [documentation](https://pedohorse.github.io/lifeblood)
```

### Comparing `lifeblood-viewer-0.8.0/README.md` & `lifeblood-viewer-0.9.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [Documentation](https://pedohorse.github.io/lifeblood)
 
-|master|dev|
-|---|---|
-|[![Tests](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml/badge.svg?branch=master)](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml)<br>[![Tests windows](https://github.com/pedohorse/lifeblood/actions/workflows/tests-win.yml/badge.svg?branch=master)](https://github.com/pedohorse/lifeblood/actions/workflows/tests-win.yml)|[![Tests](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml/badge.svg?branch=dev)](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml)<br>[![Tests windows](https://github.com/pedohorse/lifeblood/actions/workflows/tests-win.yml/badge.svg?branch=dev)](https://github.com/pedohorse/lifeblood/actions/workflows/tests-win.yml)|
+| dev                                                                                                                                                                         |
+|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| [![Tests](https://github.com/pedohorse/lifeblood/actions/workflows/tests.yml/badge.svg?branch=dev)](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml)|
 
 ![](icon/lifeblood.svg)
 
 ## Lifeblood
 Lifeblood is a task/job management software package  
 currently it aims for smaller teams, farms or even individual setups, but with scaling  always in mind.
 
@@ -21,14 +21,16 @@
 processing graph.
 
 This system overview should be very familiar to anyone who saw at least one renderfarm.
 
 check [documentation here](https://pedohorse.github.io/lifeblood)  
 and also [video tutorials](https://pedohorse.github.io/lifeblood/tutorials.html)
 
+## UNDER DEVELOPMENT
+
 ### Features:
 - instantly and easily deployable
 - easy scaling in mind
 - dynamic slots, worker resources management
 - support for environment wrappers (allow you to integrate with existing packaging systems like rez)
 
 ### Features To Be Done:
@@ -44,9 +46,12 @@
 
 ## Installation
 
 There are multiple ways to get Lifeblood to try it out, refer to [installation section in the docs](https://pedohorse.github.io/lifeblood/installation.html#simplest-lifeblood-manager)
 
 In short - easiest way is to use [Lifeblood-Manager](https://github.com/pedohorse/lifeblood-manager/releases), as described in the docs
 
-## UNDER DEVELOPMENT
+## Links
 
+- [blog + support](https://www.patreon.com/xapkohheh)
+- [telegram support/discussion group](https://t.me/+v9klFGZcKVY2MjYy)
+- [documentation](https://pedohorse.github.io/lifeblood)
```

### Comparing `lifeblood-viewer-0.8.0/setup.cfg` & `lifeblood-viewer-0.9.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lifeblood-viewer
-version = 0.8.0
+version = 0.9.0
 author = XAPKOHHEH
 description = view the LIFEBLOOD !!
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pedohorse/lifeblood
 project_urls = 
 	Bug Tracker = https://github.com/pedohorse/lifeblood/issues
```

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/breeze_resources.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/breeze_resources.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/code_editor/editor.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/code_editor/editor.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/connection_worker.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/connection_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,16 @@
     full_update = Signal(object)
     db_uid_update = Signal(object)
     graph_full_update = Signal(object)
     tasks_full_update = Signal(object)
     tasks_events_arrived = Signal(object, bool)
     groups_full_update = Signal(object)
     workers_full_update = Signal(object)
+    scheduler_connection_lost = Signal()
+    scheduler_connection_established = Signal()
 
     log_fetched = Signal(int, object, bool, object)
     nodeui_fetched = Signal(int, NodeUi)
     task_attribs_fetched = Signal(int, tuple, object)
     task_invocation_job_fetched = Signal(int, InvocationJob)
     nodetypes_fetched = Signal(dict)
     nodepresets_fetched = Signal(dict)
@@ -222,14 +224,15 @@
         self.__task_group_filter = groups
         self.__event_filter_changed = True
         self.poke_graph_and_tasks_update()
 
     def ensure_connected(self) -> bool:
         if self.__client is not None:
             return True
+        self.scheduler_connection_lost.emit()
 
         async def _interrupt_waiter():
             while True:
                 if self.interruption_requested():
                     return None
                 await asyncio.sleep(0.5)
 
@@ -243,15 +246,15 @@
                 sche_port = int(sche_port)
             if sche_addr is not None:
                 logger.info(f'trying to connect to the last known scheduler\'s address {sche_addr}:{sche_port}')
                 tmp_sock = None
                 try:
                     tmp_sock = socket.create_connection((sche_addr, sche_port), timeout=5)
                     tmp_sock.sendall(b'\0\1\0\0')
-                except ConnectionError:
+                except (ConnectionError, OSError):  # some errors such as "No route to host" are OSErrors
                     logger.info('last known address didn\'t work')
                     sche_addr, sche_port = None, None
                 finally:
                     if tmp_sock is not None:
                         tmp_sock.close()
 
             if sche_addr is None:
@@ -295,14 +298,15 @@
                     if self.interruption_requested():
                         return False
                 timeout = min(timeout * 2, 60)
             else:
                 break
 
         assert self.__client is not None
+        self.scheduler_connection_established.emit()
         config.set_option_noasync('viewer.last_scheduler_address', f'{sche_addr}:{sche_port}')
         return True
 
     def skip_dead(self) -> bool:
         return self.__skip_dead
 
     def skip_archived_groups(self) -> bool:
```

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/create_task_dialog.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/create_task_dialog.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/db_misc.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/db_misc.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/dialogs.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/dialogs.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/editor_scene_integration.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/editor_scene_integration.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/graphics_items.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/graphics_items.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/graphics_scene.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/graphics_scene.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/icons/lifeblood.svg` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/icons/lifeblood.svg`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/imgui_opengl_hotfix.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/imgui_opengl_hotfix.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/launch.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/launch.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/lifeblood_viewer.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/lifeblood_viewer.py`

 * *Files 6% similar despite different names*

```diff
@@ -231,14 +231,18 @@
         self.__central_widget = QSplitter()
         self.setCentralWidget(self.__central_widget)
         self.__workerview_splitter = QSplitter(Qt.Vertical)
         #self.__main_layout = QHBoxLayout(self.centralWidget())
         self.__node_editor = NodeEditor(db_path, self.__ui_connection_worker)
         self.__group_list = GroupsView()
         self.__group_list.setSizePolicy(QSizePolicy.Minimum, QSizePolicy.Minimum)
+        self.__overlay_connection_message = QLabel(self)  # no layout for this one
+        font = self.__overlay_connection_message.font()
+        font.setPixelSize(18)
+        self.__overlay_connection_message.setFont(font)
         # main menu
         mbar: QMenuBar = self.menuBar()
         main_menu = mbar.addMenu('main')
         main_menu.addAction('Quit').triggered.connect(self.close)
         view_menu = mbar.addMenu('view')
         act: QAction = view_menu.addAction('show dead tasks')
         act.setCheckable(True)
@@ -315,27 +319,47 @@
         self.__worker_list.setFocusPolicy(Qt.ClickFocus)
 
         # cOnNeC1
         # TODO: Now that lifeblood_viewer owns connection worker - we may reconnect these in a more straight way...
         scene = self.__node_editor.scene()
         assert isinstance(scene, QGraphicsImguiScene)
         self.__ui_connection_worker.groups_full_update.connect(self.update_groups)
+        self.__ui_connection_worker.scheduler_connection_lost.connect(self._show_connection_message)
+        self.__ui_connection_worker.scheduler_connection_established.connect(self._hide_connection_message)
         self.__group_list.selection_changed.connect(scene.set_task_group_filter)
         self.__group_list.group_pause_state_change_requested.connect(scene.set_tasks_paused)
         self.__group_list.task_group_archived_state_change_requested.connect(scene.set_task_group_archived_state)
 
         if mem_debug:
             self.__tracemalloc_timer = QTimer(self)
             self.__tracemalloc_timer.setInterval(60000)
             self.__tracemalloc_timer.timeout.connect(self._tmlc_print)
             self.__tracemalloc_timer.start()
 
         # start
         self.start()
 
+    def resizeEvent(self, event):
+        self.__layout_overlay_items()
+        return super().resizeEvent(event)
+
+    @Slot()
+    def _show_connection_message(self):
+        self.__overlay_connection_message.setText('disconnected. trying to reconnect...')
+        self.__overlay_connection_message.resize(self.__overlay_connection_message.sizeHint())
+        self.__layout_overlay_items()
+        self.__overlay_connection_message.show()
+
+    def __layout_overlay_items(self):
+        self.__overlay_connection_message.move(self.width() // 2 - self.__overlay_connection_message.width() // 2, self.height() * 1 // 6)
+
+    @Slot()
+    def _hide_connection_message(self):
+        self.__overlay_connection_message.hide()
+
     if mem_debug:
         def _tmlc_print(self):
             snapshot = tracemalloc.take_snapshot()
             top_stats = snapshot.statistics('lineno')
             print('\n\n[ Top 10 MEM USERS]\n{}\n\n'.format("\n".join(str(stat) for stat in top_stats[:10])))
 
     def set_dead_shown(self, show):
```

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/long_op.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/long_op.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/models/multiple_sort_model.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/models/multiple_sort_model.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/node_extra_items.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/node_extra_items.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/nodeeditor.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/nodeeditor.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/nodeeditor_overlays/overlay_base.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/nodeeditor_overlays/overlay_base.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/nodeeditor_overlays/task_history_overlay.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/nodeeditor_overlays/task_history_overlay.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/nodeeditor_windows/ui_create_node_popup.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/nodeeditor_windows/ui_create_node_popup.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/nodeeditor_windows/ui_longop_window.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/nodeeditor_windows/ui_longop_window.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/nodeeditor_windows/ui_parameters_window.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/nodeeditor_windows/ui_parameters_window.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/nodeeditor_windows/ui_task_list_window.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/nodeeditor_windows/ui_task_list_window.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/nodeeditor_windows/ui_undo_window.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/nodeeditor_windows/ui_undo_window.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/save_node_settings_dialog.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/save_node_settings_dialog.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/scene_ops.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/scene_ops.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/ui_elements_base.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/ui_elements_base.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/ui_scene_elements.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/ui_scene_elements.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/ui_snippets.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/ui_snippets.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/undo_stack.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/undo_stack.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/utils.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/utils.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/widgets/flashy_label.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/widgets/flashy_label.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer/widgets/worker_list.py` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer/widgets/worker_list.py`

 * *Files identical despite different names*

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer.egg-info/PKG-INFO` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeblood-viewer
-Version: 0.8.0
+Version: 0.9.0
 Summary: view the LIFEBLOOD !!
 Home-page: https://github.com/pedohorse/lifeblood
 Author: XAPKOHHEH
 Project-URL: Bug Tracker, https://github.com/pedohorse/lifeblood/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -17,17 +17,17 @@
 Requires-Dist: lz4~=4.0
 Requires-Dist: lifeblood~=0.1
 Requires-Dist: grandalf~=0.7
 Requires-Dist: numpy~=1.21
 
 [Documentation](https://pedohorse.github.io/lifeblood)
 
-|master|dev|
-|---|---|
-|[![Tests](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml/badge.svg?branch=master)](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml)<br>[![Tests windows](https://github.com/pedohorse/lifeblood/actions/workflows/tests-win.yml/badge.svg?branch=master)](https://github.com/pedohorse/lifeblood/actions/workflows/tests-win.yml)|[![Tests](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml/badge.svg?branch=dev)](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml)<br>[![Tests windows](https://github.com/pedohorse/lifeblood/actions/workflows/tests-win.yml/badge.svg?branch=dev)](https://github.com/pedohorse/lifeblood/actions/workflows/tests-win.yml)|
+| dev                                                                                                                                                                         |
+|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| [![Tests](https://github.com/pedohorse/lifeblood/actions/workflows/tests.yml/badge.svg?branch=dev)](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml)|
 
 ![](icon/lifeblood.svg)
 
 ## Lifeblood
 Lifeblood is a task/job management software package  
 currently it aims for smaller teams, farms or even individual setups, but with scaling  always in mind.
 
@@ -42,14 +42,16 @@
 processing graph.
 
 This system overview should be very familiar to anyone who saw at least one renderfarm.
 
 check [documentation here](https://pedohorse.github.io/lifeblood)  
 and also [video tutorials](https://pedohorse.github.io/lifeblood/tutorials.html)
 
+## UNDER DEVELOPMENT
+
 ### Features:
 - instantly and easily deployable
 - easy scaling in mind
 - dynamic slots, worker resources management
 - support for environment wrappers (allow you to integrate with existing packaging systems like rez)
 
 ### Features To Be Done:
@@ -65,9 +67,12 @@
 
 ## Installation
 
 There are multiple ways to get Lifeblood to try it out, refer to [installation section in the docs](https://pedohorse.github.io/lifeblood/installation.html#simplest-lifeblood-manager)
 
 In short - easiest way is to use [Lifeblood-Manager](https://github.com/pedohorse/lifeblood-manager/releases), as described in the docs
 
-## UNDER DEVELOPMENT
+## Links
 
+- [blog + support](https://www.patreon.com/xapkohheh)
+- [telegram support/discussion group](https://t.me/+v9klFGZcKVY2MjYy)
+- [documentation](https://pedohorse.github.io/lifeblood)
```

### Comparing `lifeblood-viewer-0.8.0/src/lifeblood_viewer.egg-info/SOURCES.txt` & `lifeblood-viewer-0.9.0/src/lifeblood_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

