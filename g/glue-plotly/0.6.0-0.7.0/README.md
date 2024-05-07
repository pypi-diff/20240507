# Comparing `tmp/glue-plotly-0.6.0.tar.gz` & `tmp/glue_plotly-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue-plotly-0.6.0.tar", last modified: Wed Apr 10 21:04:37 2024, max compression
+gzip compressed data, was "glue_plotly-0.7.0.tar", last modified: Tue May  7 20:46:24 2024, max compression
```

## Comparing `glue-plotly-0.6.0.tar` & `glue_plotly-0.7.0.tar`

### file list

```diff
@@ -1,123 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.035477 glue-plotly-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.019477 glue-plotly-0.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.019477 glue-plotly-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/.github/workflows/ci_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/.github/workflows/update-changelog.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-10 21:04:37.035477 glue-plotly-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/RELEASE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.019477 glue-plotly-0.6.0/doc/
--rw-r--r--   0 runner    (1001) docker     (127)    14339 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/doc/BqplotToolbarHighlighted.png
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/doc/PlotlyViewerExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   151377 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/doc/QtChartStudioExport.gif
--rw-r--r--   0 runner    (1001) docker     (127)   221318 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/doc/QtToolbarExport.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.023477 glue-plotly-0.6.0/glue_plotly/
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.023477 glue-plotly-0.6.0/glue_plotly/common/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    14894 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    12901 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/scatter2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/scatter3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.027477 glue-plotly-0.6.0/glue_plotly/common/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/tests/test_dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/tests/test_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/tests/test_scatter2d.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/common/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/export_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.027477 glue-plotly-0.6.0/glue_plotly/html_exporters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.027477 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/scatter2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.027477 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/tests/test_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/tests/test_scatter2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.027477 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/scatter2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/scatter3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.031477 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_scatter2d.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_scatter3d.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/save_hover.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/save_hover.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/sort_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/sort_components.ui
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.031477 glue-plotly-0.6.0/glue_plotly/viewers/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.031477 glue-plotly-0.6.0/glue_plotly/viewers/common/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.031477 glue-plotly-0.6.0/glue_plotly/viewers/common/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/common/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/common/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/common/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/common/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/common/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.031477 glue-plotly-0.6.0/glue_plotly/viewers/histogram/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/histogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/histogram/layer_artist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/histogram/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.031477 glue-plotly-0.6.0/glue_plotly/viewers/scatter/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/scatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/scatter/layer_artist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/viewers/scatter/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.031477 glue-plotly-0.6.0/glue_plotly/web/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/web/export_plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.031477 glue-plotly-0.6.0/glue_plotly/web/qt/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/web/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/web/qt/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/web/qt/exporter.ui
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.035477 glue-plotly-0.6.0/glue_plotly/web/qt/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/web/qt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/web/qt/tests/test_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/web/qt/tests/test_plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.035477 glue-plotly-0.6.0/glue_plotly/web/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/glue_plotly/web/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:04:37.035477 glue-plotly-0.6.0/glue_plotly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-10 21:04:36.000000 glue-plotly-0.6.0/glue_plotly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-10 21:04:37.000000 glue-plotly-0.6.0/glue_plotly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:04:36.000000 glue-plotly-0.6.0/glue_plotly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-10 21:04:36.000000 glue-plotly-0.6.0/glue_plotly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:04:36.000000 glue-plotly-0.6.0/glue_plotly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-10 21:04:36.000000 glue-plotly-0.6.0/glue_plotly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 21:04:36.000000 glue-plotly-0.6.0/glue_plotly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-10 21:04:37.035477 glue-plotly-0.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      432 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-10 21:04:06.000000 glue-plotly-0.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.698685 glue_plotly-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.678685 glue_plotly-0.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.678685 glue_plotly-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/.github/workflows/update-changelog.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-07 20:46:24.698685 glue_plotly-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/RELEASE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.682685 glue_plotly-0.7.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)    14339 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/doc/BqplotToolbarHighlighted.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/doc/PlotlyViewerExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   151377 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/doc/QtChartStudioExport.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   221318 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/doc/QtToolbarExport.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.682685 glue_plotly-0.7.0/glue_plotly/
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.686685 glue_plotly-0.7.0/glue_plotly/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/dotplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14894 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/scatter2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/scatter3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.686685 glue_plotly-0.7.0/glue_plotly/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/tests/test_dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/tests/test_dotplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/tests/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/tests/test_scatter2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/export_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.686685 glue_plotly-0.7.0/glue_plotly/html_exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.686685 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/scatter2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.690685 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/tests/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/tests/test_scatter2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.690685 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/scatter2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/scatter3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.694685 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_scatter2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_scatter3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/save_hover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/save_hover.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/sort_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/sort_components.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.694685 glue_plotly-0.7.0/glue_plotly/viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.694685 glue_plotly-0.7.0/glue_plotly/viewers/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.694685 glue_plotly-0.7.0/glue_plotly/viewers/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/common/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/common/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/common/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/common/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/common/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.694685 glue_plotly-0.7.0/glue_plotly/viewers/histogram/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/histogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/histogram/dotplot_layer_artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/histogram/layer_artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/histogram/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.694685 glue_plotly-0.7.0/glue_plotly/viewers/scatter/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/scatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/scatter/layer_artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/scatter/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.694685 glue_plotly-0.7.0/glue_plotly/web/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/web/export_plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.694685 glue_plotly-0.7.0/glue_plotly/web/qt/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/web/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/web/qt/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/web/qt/exporter.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.698685 glue_plotly-0.7.0/glue_plotly/web/qt/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/web/qt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/web/qt/tests/test_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/web/qt/tests/test_plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.698685 glue_plotly-0.7.0/glue_plotly/web/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/web/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.698685 glue_plotly-0.7.0/glue_plotly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-07 20:46:24.000000 glue_plotly-0.7.0/glue_plotly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-07 20:46:24.000000 glue_plotly-0.7.0/glue_plotly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:46:24.000000 glue_plotly-0.7.0/glue_plotly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-07 20:46:24.000000 glue_plotly-0.7.0/glue_plotly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:46:24.000000 glue_plotly-0.7.0/glue_plotly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-07 20:46:24.000000 glue_plotly-0.7.0/glue_plotly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 20:46:24.000000 glue_plotly-0.7.0/glue_plotly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-07 20:46:24.698685 glue_plotly-0.7.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      432 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/tox.ini
```

### Comparing `glue-plotly-0.6.0/.github/workflows/ci_workflows.yml` & `glue_plotly-0.7.0/.github/workflows/ci_workflows.yml`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/.github/workflows/update-changelog.yaml` & `glue_plotly-0.7.0/.github/workflows/update-changelog.yaml`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/CHANGES.md` & `glue_plotly-0.7.0/CHANGES.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,38 @@
 # Full changelog
 
+## v0.7.0 - 2024-05-07
+
+<!-- Release notes generated using configuration in .github/release.yml at main -->
+### What's Changed
+
+#### New Features
+
+* Add dotplot layer artist for histogram by @Carifio24 in https://github.com/glue-viz/glue-plotly/pull/58
+
+**Full Changelog**: https://github.com/glue-viz/glue-plotly/compare/v0.6.0...v0.7.0
+
+## v0.6.0 - 2024-04-10
+
+<!-- Release notes generated using configuration in .github/release.yml at main -->
+### What's Changed
+
+#### New Features
+
+* Update image export for layer-specific stretch customizations by @Carifio24 in https://github.com/glue-viz/glue-plotly/pull/52
+* Add hover and horizontal/vertical zoom tools by @Carifio24 in https://github.com/glue-viz/glue-plotly/pull/56
+
+#### Documentation
+
+* Add information to README by @Carifio24 in https://github.com/glue-viz/glue-plotly/pull/48
+* Add image and GIF showing where to access export tools by @Carifio24 in https://github.com/glue-viz/glue-plotly/pull/49
+* More README updates by @Carifio24 in https://github.com/glue-viz/glue-plotly/pull/50
+
+**Full Changelog**: https://github.com/glue-viz/glue-plotly/compare/v0.5.1...v0.6.0
+
 ## v0.5.1 - 2023-10-04
 
 <!-- Release notes generated using configuration in .github/release.yml at main -->
 ### What's Changed
 
 #### Bug Fixes
```

### Comparing `glue-plotly-0.6.0/LICENSE` & `glue_plotly-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/PKG-INFO` & `glue_plotly-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-plotly
-Version: 0.6.0
+Version: 0.7.0
 Summary: Experimental plot.ly exporters for glue
 Home-page: https://github.com/glue-viz/glue-plotly
 Author: Thomas Robitaille and Catherine Zucker
 Author-email: glue.viz@gmail.com
 License: BSD 3-Clause License
 Provides: glue_plotly
 Requires-Python: >=3.8
```

### Comparing `glue-plotly-0.6.0/README.rst` & `glue_plotly-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/doc/BqplotToolbarHighlighted.png` & `glue_plotly-0.7.0/doc/BqplotToolbarHighlighted.png`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/doc/PlotlyViewerExample.ipynb` & `glue_plotly-0.7.0/doc/PlotlyViewerExample.ipynb`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/doc/QtChartStudioExport.gif` & `glue_plotly-0.7.0/doc/QtChartStudioExport.gif`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/doc/QtToolbarExport.gif` & `glue_plotly-0.7.0/doc/QtToolbarExport.gif`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/__init__.py` & `glue_plotly-0.7.0/glue_plotly/__init__.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/common/common.py` & `glue_plotly-0.7.0/glue_plotly/common/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,11 +133,11 @@
     rgba_strs = [f'rgba({r},{g},{b},{opacity_value_string(a)})' for r, g, b, a in rgba_list]
     return rgba_strs
 
 
 def color_info(layer_state, mask=None,
                mode_att="cmap_mode",
                cmap_att="cmap_att"):
-    if getattr(layer_state, mode_att) == "Fixed":
+    if getattr(layer_state, mode_att, "Fixed") == "Fixed":
         return fixed_color(layer_state)
     else:
         return rgb_colors(layer_state, mask, cmap_att)
```

### Comparing `glue-plotly-0.6.0/glue_plotly/common/dendrogram.py` & `glue_plotly-0.7.0/glue_plotly/common/dendrogram.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/common/histogram.py` & `glue_plotly-0.7.0/glue_plotly/common/histogram.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/common/image.py` & `glue_plotly-0.7.0/glue_plotly/common/image.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/common/profile.py` & `glue_plotly-0.7.0/glue_plotly/common/profile.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/common/scatter2d.py` & `glue_plotly-0.7.0/glue_plotly/common/scatter2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
         s *= 0.95
         s += 0.05
         s *= (45 * layer_state.size_scaling)
         s[np.isnan(s)] = 0
         return s
 
 
-def base_marker(layer_state, mask):
+def base_marker(layer_state, mask=None):
     color = color_info(layer_state, mask)
     marker = dict(size=size_info(layer_state, mask),
                   color=color,
                   opacity=layer_state.alpha)
 
     if layer_state.fill:
         marker['line'] = dict(width=0)
```

### Comparing `glue-plotly-0.6.0/glue_plotly/common/scatter3d.py` & `glue_plotly-0.7.0/glue_plotly/common/scatter3d.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/common/tests/test_dendrogram.py` & `glue_plotly-0.7.0/glue_plotly/common/tests/test_dendrogram.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/common/tests/test_histogram.py` & `glue_plotly-0.7.0/glue_plotly/common/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/common/tests/test_profile.py` & `glue_plotly-0.7.0/glue_plotly/common/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/common/tests/test_scatter2d.py` & `glue_plotly-0.7.0/glue_plotly/common/tests/test_scatter2d.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/common/tests/utils.py` & `glue_plotly-0.7.0/glue_plotly/common/tests/utils.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/export_dialog.py` & `glue_plotly-0.7.0/glue_plotly/export_dialog.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/base.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/base.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/histogram.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/histogram.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/image.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/image.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/profile.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/profile.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/scatter2d.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/scatter2d.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/tests/test_base.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/tests/test_histogram.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/tests/test_image.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/tests/test_profile.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/bqplot/tests/test_scatter2d.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/tests/test_scatter2d.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/dendrogram.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/dendrogram.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/histogram.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/histogram.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/image.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/image.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/profile.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/profile.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/scatter2d.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/scatter2d.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/scatter3d.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/scatter3d.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/table.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/table.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_base.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_dendrogram.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_dendrogram.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_histogram.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_image.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_profile.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_scatter2d.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_scatter2d.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_scatter3d.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_scatter3d.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/html_exporters/qt/tests/test_table.py` & `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/logo.png` & `glue_plotly-0.7.0/glue_plotly/logo.png`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/logo.svg` & `glue_plotly-0.7.0/glue_plotly/logo.svg`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/save_hover.py` & `glue_plotly-0.7.0/glue_plotly/save_hover.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/save_hover.ui` & `glue_plotly-0.7.0/glue_plotly/save_hover.ui`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/sort_components.py` & `glue_plotly-0.7.0/glue_plotly/sort_components.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/sort_components.ui` & `glue_plotly-0.7.0/glue_plotly/sort_components.ui`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/utils.py` & `glue_plotly-0.7.0/glue_plotly/utils.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/viewers/common/tests/test_tools.py` & `glue_plotly-0.7.0/glue_plotly/viewers/common/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/viewers/common/tests/utils.py` & `glue_plotly-0.7.0/glue_plotly/viewers/common/tests/utils.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/viewers/common/tools.py` & `glue_plotly-0.7.0/glue_plotly/viewers/common/tools.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/viewers/common/viewer.py` & `glue_plotly-0.7.0/glue_plotly/viewers/common/viewer.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/viewers/histogram/layer_artist.py` & `glue_plotly-0.7.0/glue_plotly/viewers/histogram/layer_artist.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/viewers/histogram/viewer.py` & `glue_plotly-0.7.0/glue_plotly/viewers/histogram/viewer.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/viewers/scatter/layer_artist.py` & `glue_plotly-0.7.0/glue_plotly/viewers/scatter/layer_artist.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/viewers/scatter/viewer.py` & `glue_plotly-0.7.0/glue_plotly/viewers/scatter/viewer.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/web/export_plotly.py` & `glue_plotly-0.7.0/glue_plotly/web/export_plotly.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/web/qt/__init__.py` & `glue_plotly-0.7.0/glue_plotly/web/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/web/qt/exporter.py` & `glue_plotly-0.7.0/glue_plotly/web/qt/exporter.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/web/qt/exporter.ui` & `glue_plotly-0.7.0/glue_plotly/web/qt/exporter.ui`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/web/qt/tests/test_exporter.py` & `glue_plotly-0.7.0/glue_plotly/web/qt/tests/test_exporter.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly/web/qt/tests/test_plotly.py` & `glue_plotly-0.7.0/glue_plotly/web/qt/tests/test_plotly.py`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/glue_plotly.egg-info/PKG-INFO` & `glue_plotly-0.7.0/glue_plotly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-plotly
-Version: 0.6.0
+Version: 0.7.0
 Summary: Experimental plot.ly exporters for glue
 Home-page: https://github.com/glue-viz/glue-plotly
 Author: Thomas Robitaille and Catherine Zucker
 Author-email: glue.viz@gmail.com
 License: BSD 3-Clause License
 Provides: glue_plotly
 Requires-Python: >=3.8
```

### Comparing `glue-plotly-0.6.0/glue_plotly.egg-info/SOURCES.txt` & `glue_plotly-0.7.0/glue_plotly.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,21 +31,23 @@
 glue_plotly.egg-info/entry_points.txt
 glue_plotly.egg-info/not-zip-safe
 glue_plotly.egg-info/requires.txt
 glue_plotly.egg-info/top_level.txt
 glue_plotly/common/__init__.py
 glue_plotly/common/common.py
 glue_plotly/common/dendrogram.py
+glue_plotly/common/dotplot.py
 glue_plotly/common/histogram.py
 glue_plotly/common/image.py
 glue_plotly/common/profile.py
 glue_plotly/common/scatter2d.py
 glue_plotly/common/scatter3d.py
 glue_plotly/common/tests/__init__.py
 glue_plotly/common/tests/test_dendrogram.py
+glue_plotly/common/tests/test_dotplot.py
 glue_plotly/common/tests/test_histogram.py
 glue_plotly/common/tests/test_profile.py
 glue_plotly/common/tests/test_scatter2d.py
 glue_plotly/common/tests/utils.py
 glue_plotly/html_exporters/__init__.py
 glue_plotly/html_exporters/bqplot/__init__.py
 glue_plotly/html_exporters/bqplot/base.py
@@ -80,14 +82,15 @@
 glue_plotly/viewers/common/__init__.py
 glue_plotly/viewers/common/tools.py
 glue_plotly/viewers/common/viewer.py
 glue_plotly/viewers/common/tests/__init__.py
 glue_plotly/viewers/common/tests/test_tools.py
 glue_plotly/viewers/common/tests/utils.py
 glue_plotly/viewers/histogram/__init__.py
+glue_plotly/viewers/histogram/dotplot_layer_artist.py
 glue_plotly/viewers/histogram/layer_artist.py
 glue_plotly/viewers/histogram/viewer.py
 glue_plotly/viewers/scatter/__init__.py
 glue_plotly/viewers/scatter/layer_artist.py
 glue_plotly/viewers/scatter/viewer.py
 glue_plotly/web/__init__.py
 glue_plotly/web/export_plotly.py
```

### Comparing `glue-plotly-0.6.0/setup.cfg` & `glue_plotly-0.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `glue-plotly-0.6.0/tox.ini` & `glue_plotly-0.7.0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 extras =
     test: test,qt,jupyter
 commands =
     glue113: pip install glue-core==1.13.* glue-jupyter<=0.19
     glue114: pip install glue-core==1.14.* glue-jupyter<=0.19
     glue115: pip install glue-core==1.15.* glue-jupyter<=0.19
     glue116: pip install glue-core==1.16.* glue-jupyter<=0.19
-    glue117: pip install glue-core==1.17.*
+    glue117: pip install glue-core==1.17.* glue-jupyter<=0.20
     test: pip freeze
     test: pytest --pyargs glue_plotly --cov glue_plotly {posargs}
 
 [testenv:codestyle]
 deps = flake8
 skipsdist = true
 skip_install = true
```

